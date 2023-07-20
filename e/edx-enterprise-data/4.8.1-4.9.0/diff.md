# Comparing `tmp/edx-enterprise-data-4.8.1.tar.gz` & `tmp/edx-enterprise-data-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-4.8.1.tar", last modified: Mon Jul 17 06:50:45 2023, max compression
+gzip compressed data, was "edx-enterprise-data-4.9.0.tar", last modified: Thu Jul 20 08:24:09 2023, max compression
```

## Comparing `edx-enterprise-data-4.8.1.tar` & `edx-enterprise-data-4.9.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:45.003344 edx-enterprise-data-4.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)    17331 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-17 06:50:45.003344 edx-enterprise-data-4.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.983343 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6857 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-17 06:50:44.000000 edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.983343 edx-enterprise-data-4.8.1/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.983343 edx-enterprise-data-4.8.1/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    18646 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.987343 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0030_auto_20230609_1353.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0031_auto_20230615_0705.py
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/0032_auto_20230704_0818.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12280 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    12241 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.995344 edx-enterprise-data-4.8.1/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.999344 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.999344 edx-enterprise-data-4.8.1/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.999344 edx-enterprise-data-4.8.1/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.999344 edx-enterprise-data-4.8.1/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:44.999344 edx-enterprise-data-4.8.1/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:45.003344 edx-enterprise-data-4.8.1/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     9493 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13860 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:50:45.003344 edx-enterprise-data-4.8.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 06:50:45.003344 edx-enterprise-data-4.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-07-17 06:50:39.000000 edx-enterprise-data-4.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    17409 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.426658 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6857 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-20 08:24:09.000000 edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.426658 edx-enterprise-data-4.9.0/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.426658 edx-enterprise-data-4.9.0/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.426658 edx-enterprise-data-4.9.0/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.430658 edx-enterprise-data-4.9.0/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18646 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.430658 edx-enterprise-data-4.9.0/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.430658 edx-enterprise-data-4.9.0/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.430658 edx-enterprise-data-4.9.0/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.430658 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.434658 edx-enterprise-data-4.9.0/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0030_auto_20230609_1353.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0031_auto_20230615_0705.py
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/0032_auto_20230704_0818.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12280 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.434658 edx-enterprise-data-4.9.0/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.434658 edx-enterprise-data-4.9.0/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.434658 edx-enterprise-data-4.9.0/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12241 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.438658 edx-enterprise-data-4.9.0/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9493 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13860 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8571 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9390 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5997 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 08:24:09.442658 edx-enterprise-data-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4927 2023-07-20 08:24:05.000000 edx-enterprise-data-4.9.0/setup.py
```

### Comparing `edx-enterprise-data-4.8.1/CHANGELOG.rst` & `edx-enterprise-data-4.9.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
+[4.9.0] - 2023-07-20
+---------------------
+  * Support added for Django 4.2
+
+
 [4.8.1] - 2023-07-14
 ---------------------
   *  Sort enterprise enrollments by default on last_activity_date.
 
 
 [4.8.0] - 2023-07-4
 ---------------------
```

### Comparing `edx-enterprise-data-4.8.1/LICENSE` & `edx-enterprise-data-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/MANIFEST.in` & `edx-enterprise-data-4.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/PKG-INFO` & `edx-enterprise-data-4.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.8.1
+Version: 4.9.0
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: reporting
 License-File: LICENSE
 
 Tools and products related to providing access to Enterprise data.
```

### Comparing `edx-enterprise-data-4.8.1/README.md` & `edx-enterprise-data-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/PKG-INFO` & `edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.8.1
+Version: 4.9.0
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: reporting
 License-File: LICENSE
 
 Tools and products related to providing access to Enterprise data.
```

### Comparing `edx-enterprise-data-4.8.1/edx_enterprise_data.egg-info/SOURCES.txt` & `edx-enterprise-data-4.9.0/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v0/serializers.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v0/urls.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v0/views.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v1/serializers.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v1/urls.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/api/v1/views.py` & `edx-enterprise-data-4.9.0/enterprise_data/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/clients.py` & `edx-enterprise-data-4.9.0/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/filters.py` & `edx-enterprise-data-4.9.0/enterprise_data/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/fixtures/enterprise_enrollment.json` & `edx-enterprise-data-4.9.0/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/fixtures/enterprise_user.json` & `edx-enterprise-data-4.9.0/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_dummy_data.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_offer.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/create_enterprise_user.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx-enterprise-data-4.9.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0001_initial.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0011_enterpriseuser.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0030_auto_20230609_1353.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0030_auto_20230609_1353.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0031_auto_20230615_0705.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0031_auto_20230615_0705.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/migrations/0032_auto_20230704_0818.py` & `edx-enterprise-data-4.9.0/enterprise_data/migrations/0032_auto_20230704_0818.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/models.py` & `edx-enterprise-data-4.9.0/enterprise_data/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/settings/test.py` & `edx-enterprise-data-4.9.0/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/signals.py` & `edx-enterprise-data-4.9.0/enterprise_data/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/api/v0/test_serializers.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/test_serializers.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/api/v1/test_views.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/api/v1/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/mixins.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/test_clients.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/test_filters.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/test_models.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/test_utils.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/tests/test_views.py` & `edx-enterprise-data-4.9.0/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data/utils.py` & `edx-enterprise-data-4.9.0/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/admin.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0001_initial.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/models.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/rules.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/tests/factories.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_data_roles/tests/test_models.py` & `edx-enterprise-data-4.9.0/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/clients/__init__.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/clients/enterprise.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/clients/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/clients/s3.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/clients/snowflake.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/clients/vertica.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/delivery_method.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/external_resource_link_report.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx-enterprise-data-4.9.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/reporter.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/send_enterprise_reports.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_clients.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_delivery_method.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_enterprise_client.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_external_link_report.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_reporter.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/test_utils.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/tests/utils.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/enterprise_reporting/utils.py` & `edx-enterprise-data-4.9.0/enterprise_reporting/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/requirements/base.txt` & `edx-enterprise-data-4.9.0/requirements/base.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
@@ -50,15 +50,15 @@
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
-django==3.2.19
+django==3.2.20
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -106,15 +106,15 @@
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.2
     # via -r requirements/base.in
 factory-boy==3.2.1
     # via -r requirements/base.in
-faker==18.10.1
+faker==18.11.2
     # via factory-boy
 filelock==3.12.2
     # via snowflake-connector-python
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
@@ -124,15 +124,15 @@
     # via
     #   boto3
     #   botocore
 kombu==4.6.11
     # via celery
 monotonic==1.6
     # via py2neo
-newrelic==8.8.0
+newrelic==8.8.1
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
 packaging==23.1
     # via
     #   py2neo
     #   snowflake-connector-python
@@ -223,15 +223,15 @@
     # via snowflake-connector-python
 sqlparse==0.4.4
     # via django
 stevedore==5.1.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   asgiref
     #   snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
 urllib3==1.26.16
     # via
```

### Comparing `edx-enterprise-data-4.8.1/requirements/ci.txt` & `edx-enterprise-data-4.9.0/requirements/ci.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     # via virtualenv
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via tox
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via tox
 py==1.11.0
     # via tox
 six==1.16.0
     # via tox
 tomli==2.0.1
     # via tox
```

### Comparing `edx-enterprise-data-4.8.1/requirements/constraints.txt` & `edx-enterprise-data-4.9.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/requirements/dev.txt` & `edx-enterprise-data-4.9.0/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
 bleach==6.0.0
     # via readme-renderer
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 build==0.10.0
     # via pip-tools
 celery==4.4.7
@@ -68,23 +68,22 @@
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
-    #   secretstorage
     #   snowflake-connector-python
 diff-cover==7.6.0
     # via -r requirements/dev-enterprise_data.in
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
-django==3.2.19
+django==3.2.20
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -141,15 +140,15 @@
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.2
     # via -r requirements/base.in
 factory-boy==3.2.1
     # via -r requirements/base.in
-faker==18.10.1
+faker==18.11.2
     # via factory-boy
 filelock==3.12.2
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 idna==3.4
@@ -166,27 +165,23 @@
     # via py2neo
 isort==5.12.0
     # via
     #   -r requirements/quality.in
     #   pylint
 jaraco-classes==3.2.3
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
 jinja2==3.1.2
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==23.13.1
+keyring==24.2.0
     # via twine
 kombu==4.6.11
     # via celery
 lazy-object-proxy==1.9.0
     # via astroid
 markdown-it-py==3.0.0
     # via rich
@@ -196,15 +191,15 @@
     # via pylint
 mdurl==0.1.2
     # via markdown-it-py
 monotonic==1.6
     # via py2neo
 more-itertools==9.1.0
     # via jaraco-classes
-newrelic==8.8.0
+newrelic==8.8.1
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
 packaging==23.1
     # via
     #   build
     #   py2neo
@@ -216,23 +211,23 @@
     # via -r requirements/reporting.in
 path==16.6.0
     # via edx-i18n-tools
 pbr==5.11.1
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   pylint
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   diff-cover
     #   tox
 polib==1.2.0
     # via edx-i18n-tools
 psutil==5.9.5
     # via edx-django-utils
@@ -331,16 +326,14 @@
     # via awscli
 rules==3.3
     # via -r requirements/base.in
 s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
-secretstorage==3.3.3
-    # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   bleach
     #   edx-drf-extensions
     #   edx-lint
@@ -369,29 +362,30 @@
 testfixtures==7.1.0
     # via -r requirements/quality.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
+    #   pip-tools
     #   pylint
     #   pyproject-hooks
     #   tox
 tomlkit==0.11.8
     # via pylint
 tox==3.28.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/dev-enterprise_data.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/dev-enterprise_data.in
 twine==4.0.2
     # via -r requirements/dev-enterprise_data.in
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   asgiref
     #   astroid
     #   pylint
     #   rich
     #   snowflake-connector-python
 unicodecsv==0.14.1
```

### Comparing `edx-enterprise-data-4.8.1/requirements/quality.txt` & `edx-enterprise-data-4.9.0/requirements/quality.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
 bleach==6.0.0
     # via readme-renderer
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 build==0.10.0
     # via pip-tools
 celery==4.4.7
@@ -70,25 +70,24 @@
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
-    #   secretstorage
     #   snowflake-connector-python
 ddt==1.6.0
     # via -r requirements/test.in
 diff-cover==7.6.0
     # via -r requirements/dev-enterprise_data.in
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
-django==3.2.19
+django==3.2.20
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -144,21 +143,21 @@
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.2
     # via -r requirements/base.in
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==18.10.1
+faker==18.11.2
     # via factory-boy
 filelock==3.12.2
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 flaky==3.7.0
@@ -181,27 +180,23 @@
     # via py2neo
 isort==5.12.0
     # via
     #   -r requirements/quality.in
     #   pylint
 jaraco-classes==3.2.3
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
 jinja2==3.1.2
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==23.13.1
+keyring==24.2.0
     # via twine
 kombu==4.6.11
     # via celery
 lazy-object-proxy==1.9.0
     # via astroid
 markdown-it-py==3.0.0
     # via rich
@@ -213,15 +208,15 @@
     # via markdown-it-py
 mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
 more-itertools==9.1.0
     # via jaraco-classes
-newrelic==8.8.0
+newrelic==8.8.1
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
 packaging==23.1
     # via
     #   build
     #   py2neo
@@ -234,23 +229,23 @@
     # via -r requirements/reporting.in
 path==16.6.0
     # via edx-i18n-tools
 pbr==5.11.1
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   pylint
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   diff-cover
     #   pytest
     #   tox
 polib==1.2.0
     # via edx-i18n-tools
 psutil==5.9.5
@@ -305,15 +300,15 @@
     # via
     #   edx-django-utils
     #   paramiko
 pyopenssl==23.2.0
     # via snowflake-connector-python
 pyproject-hooks==1.0.0
     # via build
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   pytest-cov
     #   pytest-django
 pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
@@ -363,16 +358,14 @@
     # via awscli
 rules==3.3
     # via -r requirements/base.in
 s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
-secretstorage==3.3.3
-    # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   bleach
     #   edx-drf-extensions
     #   edx-lint
@@ -404,14 +397,15 @@
     #   -r requirements/test.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
     #   coverage
+    #   pip-tools
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   tox
 tomlkit==0.11.8
     # via pylint
 tox==3.28.0
@@ -421,15 +415,15 @@
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/dev-enterprise_data.in
 twine==4.0.2
     # via -r requirements/dev-enterprise_data.in
 types-pyyaml==6.0.12.10
     # via responses
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   asgiref
     #   astroid
     #   pylint
     #   rich
     #   snowflake-connector-python
 unicodecsv==0.14.1
```

### Comparing `edx-enterprise-data-4.8.1/requirements/reporting.in` & `edx-enterprise-data-4.9.0/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.8.1/requirements/test-master.txt` & `edx-enterprise-data-4.9.0/requirements/test-master.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
@@ -54,27 +54,14 @@
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.6.0
     # via -r requirements/test.in
-    # via
-    #   -c requirements/constraints.txt
-    #   -r requirements/base.in
-    #   -r requirements/test-master.in
-    #   django-crum
-    #   django-fernet-fields
-    #   django-filter
-    #   django-model-utils
-    #   djangorestframework
-    #   drf-jwt
-    #   edx-django-utils
-    #   edx-drf-extensions
-    #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
 django-filter==23.2
@@ -111,21 +98,21 @@
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.2
     # via -r requirements/base.in
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==18.10.1
+faker==18.11.2
     # via factory-boy
 filelock==3.12.2
     # via snowflake-connector-python
 flaky==3.7.0
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
@@ -143,15 +130,15 @@
     #   botocore
 kombu==4.6.11
     # via celery
 mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==8.8.0
+newrelic==8.8.1
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
 packaging==23.1
     # via
     #   py2neo
     #   pytest
@@ -160,15 +147,15 @@
     # via py2neo
 paramiko==3.2.0
     # via -r requirements/reporting.in
 pbr==5.11.1
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 psutil==5.9.5
     # via edx-django-utils
 py2neo==2021.2.3
     # via -r requirements/reporting.in
 pyasn1==0.5.0
     # via
@@ -192,15 +179,15 @@
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
 pyopenssl==23.2.0
     # via snowflake-connector-python
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   pytest-cov
     #   pytest-django
 pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
@@ -267,15 +254,15 @@
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 types-pyyaml==6.0.12.10
     # via responses
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   asgiref
     #   snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
 urllib3==1.26.16
     # via
```

### Comparing `edx-enterprise-data-4.8.1/requirements/test-reporting.txt` & `edx-enterprise-data-4.9.0/requirements/test-reporting.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 atomicwrites==1.4.1
     # via pytest
 attrs==23.1.0
     # via pytest
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
@@ -94,17 +94,17 @@
     # via py2neo
 paramiko==3.2.0
     # via -r requirements/reporting.in
 pbr==5.11.1
     # via mock
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
 py==1.11.0
     # via
     #   pytest
     #   tox
@@ -180,15 +180,15 @@
     #   -c requirements/constraints.txt
     #   -r requirements/test-reporting.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/test-reporting.in
 types-pyyaml==6.0.12.10
     # via responses
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
 urllib3==1.26.16
     # via
     #   botocore
     #   py2neo
```

### Comparing `edx-enterprise-data-4.8.1/requirements/test.txt` & `edx-enterprise-data-4.9.0/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.156
+awscli==1.28.0
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.156
+boto3==1.27.0
     # via -r requirements/reporting.in
-botocore==1.29.156
+botocore==1.30.0
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
@@ -54,15 +54,15 @@
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.6.0
     # via -r requirements/test.in
-django==3.2.19
+django==3.2.20
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -109,21 +109,21 @@
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.2
     # via -r requirements/base.in
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==18.10.1
+faker==18.11.2
     # via factory-boy
 filelock==3.12.2
     # via snowflake-connector-python
 flaky==3.7.0
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
@@ -141,15 +141,15 @@
     #   botocore
 kombu==4.6.11
     # via celery
 mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==8.8.0
+newrelic==8.8.1
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
 packaging==23.1
     # via
     #   py2neo
     #   pytest
@@ -158,15 +158,15 @@
     # via py2neo
 paramiko==3.2.0
     # via -r requirements/reporting.in
 pbr==5.11.1
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 psutil==5.9.5
     # via edx-django-utils
 py2neo==2021.2.3
     # via -r requirements/reporting.in
 pyasn1==0.5.0
     # via
@@ -190,15 +190,15 @@
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
 pyopenssl==23.2.0
     # via snowflake-connector-python
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   pytest-cov
     #   pytest-django
 pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
@@ -265,15 +265,15 @@
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 types-pyyaml==6.0.12.10
     # via responses
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   asgiref
     #   snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
 urllib3==1.26.16
     # via
```

### Comparing `edx-enterprise-data-4.8.1/setup.py` & `edx-enterprise-data-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 setup(
     name="edx-enterprise-data",
     version=VERSION,
     classifiers=[
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     description="""Enterprise Reporting""",
     long_description="Tools and products related to providing access to Enterprise data.",
     author="edX",
     author_email="oscm@edx.org",
```

