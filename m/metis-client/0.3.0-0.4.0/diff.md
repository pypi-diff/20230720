# Comparing `tmp/metis_client-0.3.0.tar.gz` & `tmp/metis_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metis_client-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metis_client-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metis_client-0.3.0.tar` & `metis_client-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0      372 2023-05-19 14:20:57.706607 metis_client-0.3.0/.flake8
--rw-r--r--   0        0        0      212 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1396 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/linter.yml
--rw-r--r--   0        0        0      792 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1852 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/push.yml
--rw-r--r--   0        0        0      867 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1338 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1869 2023-05-19 14:20:57.706607 metis_client-0.3.0/.gitignore
--rw-r--r--   0        0        0      275 2023-05-19 14:20:57.706607 metis_client-0.3.0/.whitesource
--rw-r--r--   0        0        0      820 2023-05-19 14:20:57.706607 metis_client-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      492 2023-05-19 14:20:57.706607 metis_client-0.3.0/CITATION.cff
--rw-r--r--   0        0        0     2819 2023-05-19 14:20:57.706607 metis_client-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1452 2023-05-19 14:20:57.706607 metis_client-0.3.0/LICENSE
--rw-r--r--   0        0        0     1746 2023-05-19 14:20:57.706607 metis_client-0.3.0/README.md
--rw-r--r--   0        0        0      156 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/data/user_object_one.dat
--rw-r--r--   0        0        0     2818 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/example_async.py
--rw-r--r--   0        0        0     2601 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/example_sync.py
--rw-r--r--   0        0        0      241 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/__init__.py
--rw-r--r--   0        0        0    10756 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/client.py
--rw-r--r--   0        0        0      625 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/const.py
--rw-r--r--   0        0        0      691 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/__init__.py
--rw-r--r--   0        0        0      314 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/auth.py
--rw-r--r--   0        0        0      386 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/base.py
--rw-r--r--   0        0        0      625 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/calculation.py
--rw-r--r--   0        0        0     1355 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/collection.py
--rw-r--r--   0        0        0     1002 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/datasource.py
--rw-r--r--   0        0        0      405 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/error.py
--rw-r--r--   0        0        0     2183 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/event.py
--rw-r--r--   0        0        0      282 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/resp.py
--rw-r--r--   0        0        0      683 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/user.py
--rw-r--r--   0        0        0     1474 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/exc.py
--rw-r--r--   0        0        0     4342 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/helpers.py
--rw-r--r--   0        0        0     8599 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/metis.py
--rw-r--r--   0        0        0     3736 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/metis_async.py
--rw-r--r--   0        0        0      266 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/__init__.py
--rw-r--r--   0        0        0     2915 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/auth.py
--rw-r--r--   0        0        0      230 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/base.py
--rw-r--r--   0        0        0     2410 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/event.py
--rw-r--r--   0        0        0     1751 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/hub.py
--rw-r--r--   0        0        0     2839 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/subscription.py
--rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/__init__.py
--rw-r--r--   0        0        0      940 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/auth.py
--rw-r--r--   0        0        0      934 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/base.py
--rw-r--r--   0        0        0     7250 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/calculations.py
--rw-r--r--   0        0        0     3554 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/collections.py
--rw-r--r--   0        0        0     3847 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/datasources.py
--rw-r--r--   0        0        0     1064 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/root.py
--rw-r--r--   0        0        0     2293 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/stream.py
--rw-r--r--   0        0        0     1675 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/v0.py
--rw-r--r--   0        0        0     3447 2023-05-19 14:20:57.710607 metis_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      217 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/__init__.py
--rw-r--r--   0        0        0      824 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_no_auth.py
--rw-r--r--   0        0        0     3139 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_password.py
--rw-r--r--   0        0        0     1175 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_token.py
--rw-r--r--   0        0        0      484 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_event.py
--rw-r--r--   0        0        0      211 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_hub.py
--rw-r--r--   0        0        0      821 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_subscription.py
--rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/__init__.py
--rw-r--r--   0        0        0     3761 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_auth.py
--rw-r--r--   0        0        0    12339 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_calculations.py
--rw-r--r--   0        0        0     7952 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_collections.py
--rw-r--r--   0        0        0    10776 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_datasources.py
--rw-r--r--   0        0        0    11730 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_client.py
--rw-r--r--   0        0        0      332 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_exc.py
--rw-r--r--   0        0        0     1023 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_helpers_convert_dict_items_to_datetime.py
--rw-r--r--   0        0        0      976 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_helpers_rfc3339.py
--rw-r--r--   0        0        0      236 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_metis_async.py
--rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 metis_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-07-20 13:46:16.071964 metis_client-0.4.0/.flake8
+-rw-r--r--   0        0        0      212 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1396 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      792 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1968 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/push.yml
+-rw-r--r--   0        0        0      867 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1338 2023-07-20 13:46:16.071964 metis_client-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1869 2023-07-20 13:46:16.071964 metis_client-0.4.0/.gitignore
+-rw-r--r--   0        0        0      275 2023-07-20 13:46:16.071964 metis_client-0.4.0/.whitesource
+-rw-r--r--   0        0        0     1019 2023-07-20 13:46:16.071964 metis_client-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      492 2023-07-20 13:46:16.071964 metis_client-0.4.0/CITATION.cff
+-rw-r--r--   0        0        0     2819 2023-07-20 13:46:16.071964 metis_client-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1452 2023-07-20 13:46:16.071964 metis_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1764 2023-07-20 13:46:16.071964 metis_client-0.4.0/README.md
+-rw-r--r--   0        0        0      156 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/data/user_object_one.dat
+-rw-r--r--   0        0        0     3517 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/example_async.py
+-rw-r--r--   0        0        0     3240 2023-07-20 13:46:16.071964 metis_client-0.4.0/examples/example_sync.py
+-rw-r--r--   0        0        0      241 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/__init__.py
+-rw-r--r--   0        0        0    10738 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/client.py
+-rw-r--r--   0        0        0      625 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/const.py
+-rw-r--r--   0        0        0      691 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/auth.py
+-rw-r--r--   0        0        0      386 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/base.py
+-rw-r--r--   0        0        0      625 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/calculation.py
+-rw-r--r--   0        0        0     1355 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/collection.py
+-rw-r--r--   0        0        0     1002 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/datasource.py
+-rw-r--r--   0        0        0      405 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/error.py
+-rw-r--r--   0        0        0     2214 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/event.py
+-rw-r--r--   0        0        0      282 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/resp.py
+-rw-r--r--   0        0        0      683 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/dtos/user.py
+-rw-r--r--   0        0        0     1474 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/exc.py
+-rw-r--r--   0        0        0     4342 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/helpers.py
+-rw-r--r--   0        0        0    11184 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/metis.py
+-rw-r--r--   0        0        0     4105 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/metis_async.py
+-rw-r--r--   0        0        0      266 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/__init__.py
+-rw-r--r--   0        0        0     2915 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/auth.py
+-rw-r--r--   0        0        0      230 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/base.py
+-rw-r--r--   0        0        0     2410 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/event.py
+-rw-r--r--   0        0        0     1751 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/hub.py
+-rw-r--r--   0        0        0     2770 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/models/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/__init__.py
+-rw-r--r--   0        0        0      934 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/base.py
+-rw-r--r--   0        0        0      697 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/calculations.py
+-rw-r--r--   0        0        0     1439 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/root.py
+-rw-r--r--   0        0        0     2370 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/stream.py
+-rw-r--r--   0        0        0     1711 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0.py
+-rw-r--r--   0        0        0      942 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_auth.py
+-rw-r--r--   0        0        0     7540 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_calculations.py
+-rw-r--r--   0        0        0     3558 2023-07-20 13:46:16.071964 metis_client-0.4.0/metis_client/namespaces/v0_collections.py
+-rw-r--r--   0        0        0     3849 2023-07-20 13:46:16.075964 metis_client-0.4.0/metis_client/namespaces/v0_datasources.py
+-rw-r--r--   0        0        0     3447 2023-07-20 13:46:16.075964 metis_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      217 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/__init__.py
+-rw-r--r--   0        0        0      824 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_no_auth.py
+-rw-r--r--   0        0        0     3139 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_password.py
+-rw-r--r--   0        0        0     1175 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_auth_token.py
+-rw-r--r--   0        0        0      484 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_event.py
+-rw-r--r--   0        0        0      211 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_hub.py
+-rw-r--r--   0        0        0      821 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/models/test_subscription.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_calculations.py
+-rw-r--r--   0        0        0     3763 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_auth.py
+-rw-r--r--   0        0        0    12310 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_calculations.py
+-rw-r--r--   0        0        0     7954 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_collections.py
+-rw-r--r--   0        0        0    11277 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/namespaces/test_v0_datasources.py
+-rw-r--r--   0        0        0    11235 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_client.py
+-rw-r--r--   0        0        0      332 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_exc.py
+-rw-r--r--   0        0        0     1023 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_helpers_convert_dict_items_to_datetime.py
+-rw-r--r--   0        0        0      976 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_helpers_rfc3339.py
+-rw-r--r--   0        0        0      655 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_metis.py
+-rw-r--r--   0        0        0      236 2023-07-20 13:46:16.075964 metis_client-0.4.0/tests/test_metis_async.py
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 metis_client-0.4.0/PKG-INFO
```

### Comparing `metis_client-0.3.0/.github/workflows/linter.yml` & `metis_client-0.4.0/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/.github/workflows/pr.yml` & `metis_client-0.4.0/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/.github/workflows/push.yml` & `metis_client-0.4.0/.github/workflows/push.yml`

 * *Files 7% similar despite different names*

```diff
@@ -35,22 +35,24 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .[release]
 
       - name: Create bump and changelog
         id: cz
+        if: github.repository == 'tilde-lab/metis-client'
         uses: commitizen-tools/commitizen-action@e41bf7f2029bc8175af362badd6fd0860a329b0f
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           changelog_increment_filename: .CHANGELOG-CURRENT.md
           push: true
           commit: true
 
       - name: Print new version
+        if: github.repository == 'tilde-lab/metis-client'
         run: echo "Bumped to version ${{ steps.cz.outputs.version }}"
 
       - name: Build
         run: flit build
 
       - name: Stop if no bump
         id: no-bump
```

### Comparing `metis_client-0.3.0/.github/workflows/release.yml` & `metis_client-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/.github/workflows/test.yml` & `metis_client-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/.gitignore` & `metis_client-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/CHANGELOG.md` & `metis_client-0.4.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## v0.4.0 (2023-06-25)
+
+### Feat
+
+- **namespaces**: implements /calculations namespace, deprecate get_engines()
+- **MetisAPI**: timeouts
+
+### Refactor
+
+- **namespaces**: scope v0 namespaces into v0
+
 ## v0.3.0 (2023-05-19)
 
 ### Feat
 
 - *input* calculation parameter support
 
 ## v0.2.0 (2023-05-02)
```

### Comparing `metis_client-0.3.0/CONTRIBUTING.md` & `metis_client-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/LICENSE` & `metis_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/README.md` & `metis_client-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,24 +36,23 @@
 ### Synchronous client
 
 A synchronous client is `MetisAPI`. Example of usage:
 
 ```python
 from metis_client import MetisAPI, MetisTokenAuth
 
-client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"))
+client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"), timeout=5)
 data = client.v0.datasources.create(content)
-results = client.v0.calculations.create_get_results(data["id"])
+results = client.v0.calculations.create_get_results(data["id"], timeout=False)
 print(results)
 ```
 
 NB in development one can replace a `VERY_SECRET_TOKEN` string with the development user email, e.g.
 `admin@test.com` (refer to **users_emails** BFF table).
 
 ## License
 
 Author Sergey Korolev, Tilde Materials Informatics
 
 Copyright 2023 BASF SE
 
 BSD 3-Clause
-  * [ ]
```

### Comparing `metis_client-0.3.0/examples/example_async.py` & `metis_client-0.4.0/examples/example_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,22 +75,46 @@
         calc["id"], on_progress=stop_watching_on_half
     )
     assert results is None
     await client.v0.calculations.cancel(calc["id"])
     print("=" * 50 + "Test passed")
 
 
+async def create_calc_timeout_cancel(client: MetisAPIAsync):
+    """
+    Create data source. Run calculation.
+    Cancel calculation on timeout.
+    """
+
+    data = await client.v0.datasources.create(CONTENT)
+    assert data
+
+    calc = await client.v0.calculations.create(data.get("id"), engine=TEST_ENGINE)
+    assert calc
+
+    try:
+        results = await asyncio.wait_for(
+            client.v0.calculations.get_results(calc["id"]), timeout=0.1
+        )
+        assert results is None
+    except asyncio.TimeoutError:
+        print("Timeouted as planned")
+        await client.v0.calculations.cancel(calc["id"])
+    print("=" * 50 + "Test passed")
+
+
 async def main():
     "Run all examples"
     async with MetisAPIAsync(API_URL, auth=MetisTokenAuth("admin@test.com")) as client:
         print(await client.v0.auth.whoami())
         print(
             "The following engines are available:",
-            await client.v0.calculations.get_engines(),
+            await client.calculations.supported(),
         )
 
         await create_calc_then_get_results(client)
         await create_calc_and_get_results(client)
         await create_calc_then_cancel(client)
+        await create_calc_timeout_cancel(client)
 
 
 asyncio.run(main())
```

### Comparing `metis_client-0.3.0/examples/example_sync.py` & `metis_client-0.4.0/examples/example_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """Example of usage of synchronous client"""
 # pylint: disable=no-value-for-parameter
 
+import asyncio
 import sys
 
 from metis_client import MetisAPI, MetisTokenAuth
 from metis_client.dtos import MetisCalculationDTO
 
 API_URL = "http://localhost:3000"
 TEST_ENGINE = "dummy"
@@ -75,21 +76,43 @@
         calc["id"], on_progress=stop_watching_on_half
     )
     assert results is None
     client.v0.calculations.cancel(calc["id"])
     print("=" * 50 + "Test passed")
 
 
+def create_calc_timeout_cancel(client: MetisAPI):
+    """
+    Create data source. Run calculation.
+    Cancel calculation on timeout.
+    """
+
+    data = client.v0.datasources.create(CONTENT)
+    assert data
+
+    calc = client.v0.calculations.create(data.get("id"), engine=TEST_ENGINE)
+    assert calc
+
+    try:
+        results = client.v0.calculations.get_results(calc["id"], timeout=1)
+        assert results is None
+    except asyncio.TimeoutError:
+        print("Timeouted as planned")
+        client.v0.calculations.cancel(calc["id"])
+    print("=" * 50 + "Test passed")
+
+
 def main():
     "Run all examples"
 
-    client = MetisAPI(API_URL, auth=MetisTokenAuth("admin@test.com"))
+    client = MetisAPI(API_URL, auth=MetisTokenAuth("admin@test.com"), timeout=60)
 
     print(client.v0.auth.whoami())
-    print("The following engines are available:", client.v0.calculations.get_engines())
+    print("The following engines are available:", client.calculations.supported())
 
     create_calc_then_get_results(client)
     create_calc_and_get_results(client)
     create_calc_then_cancel(client)
+    create_calc_timeout_cancel(client)
 
 
 main()
```

### Comparing `metis_client-0.3.0/metis_client/client.py` & `metis_client-0.4.0/metis_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                 result = await self._session.request(method, url, **aio_opts)
             # rate limit - redo all
             if result.status == HTTPTooManyRequests.status_code:
                 await sleep(10)
                 result.close()
                 return await self._request(url, **opts)
 
-        except (CancelledError, ClientConnectionError) as exc:
+        except ClientConnectionError as exc:
             raise MetisConnectionException(
                 f"Request exception for {str(url)!r} with - {exc}"
             ) from exc
 
         except (TimeoutError, AsyncioTimeoutError, FuturesTimeoutError):
             raise MetisConnectionException(
                 f"Timeout of {opts.get('timeout')} reached while waiting for {str(url)}"
```

### Comparing `metis_client-0.3.0/metis_client/const.py` & `metis_client-0.4.0/metis_client/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants for metis_client."""
 
 from __future__ import annotations
 
 from logging import Logger, getLogger
 from typing import Literal, Union
 
-PROJECT_VERSION = "0.3.0"
+PROJECT_VERSION = "0.4.0"
 PROJECT_NAME = "metis_client"
 
 # This is the default user agent,
 # but it is adviced to use your own when building out your application
 DEFAULT_USER_AGENT = f"metis_client/{PROJECT_VERSION}"
```

### Comparing `metis_client-0.3.0/metis_client/dtos/__init__.py` & `metis_client-0.4.0/metis_client/dtos/__init__.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/dtos/calculation.py` & `metis_client-0.4.0/metis_client/dtos/calculation.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/dtos/collection.py` & `metis_client-0.4.0/metis_client/dtos/collection.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/dtos/datasource.py` & `metis_client-0.4.0/metis_client/dtos/datasource.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/dtos/event.py` & `metis_client-0.4.0/metis_client/dtos/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
 class MetisCollectionsEventDTO(TypedDict):
     "Collections event DTO"
     type: Literal["collections"]
     data: MetisCollectionsEventDataDTO
 
 
+# pylint: disable=invalid-name
 MetisEventDTO = Union[
     MetisCalculationsEventDTO,
     MetisCollectionsEventDTO,
     MetisDataSourcesEventDTO,
     MetisErrorEventDTO,
     MetisPongEventDTO,
 ]
```

### Comparing `metis_client-0.3.0/metis_client/dtos/user.py` & `metis_client-0.4.0/metis_client/dtos/user.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/exc.py` & `metis_client-0.4.0/metis_client/exc.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/helpers.py` & `metis_client-0.4.0/metis_client/helpers.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/metis.py` & `metis_client-0.4.0/metis_client/metis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 """Metis API synchronous client"""
 
+import asyncio
 import sys
 from functools import partial
-from typing import Any, Optional, Sequence, TypeVar, cast
+from typing import Any, Literal, Optional, Sequence, TypeVar, Union, cast
 
 from aiohttp.typedefs import StrOrURL
 from asgiref.sync import async_to_sync
 
 from metis_client.dtos.datasource import MetisDataSourceDTO
 
 from .metis_async import MetisAPIAsync, MetisAPIKwargs
 from .models.base import MetisBase
-from .namespaces.calculations import MetisCalculationOnProgressT
-from .namespaces.collections import MetisCollectionsCreateKwargs
+from .namespaces.v0_calculations import MetisCalculationOnProgressT
+from .namespaces.v0_collections import MetisCollectionsCreateKwargs
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Awaitable, Callable
 else:  # pragma: no cover
     from collections.abc import Awaitable, Callable
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import Concatenate, ParamSpec, Unpack
 else:  # pragma: no cover
     from typing import Concatenate, ParamSpec, Unpack
 
-
 AsyncClientGetter = Callable[[], MetisAPIAsync]
 ReturnT_co = TypeVar("ReturnT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
+TimeoutType = Union[float, Literal[False], None]
 
 
 # pylint: disable=too-few-public-methods
 class MetisNamespaceSyncBase:
     "Base for synchronous namespaces"
     _client_getter: AsyncClientGetter
+    _default_timeout: TimeoutType
 
-    def __init__(self, client_getter: AsyncClientGetter):
+    def __init__(
+        self, client_getter: AsyncClientGetter, default_timeout: TimeoutType = False
+    ):
         self._client_getter = client_getter
+        self._default_timeout = default_timeout
+
+    def _get_timeout(self, timeout: TimeoutType) -> Optional[float]:
+        "Normalize timeout value"
+        if timeout is False:
+            return None
+        if timeout is not None:
+            return timeout
+        if not self._default_timeout:
+            return None
+        return self._default_timeout
 
 
 def to_sync_with_metis_client(
     func: Callable[Concatenate[Any, MetisAPIAsync, ParamT], Awaitable[ReturnT_co]]
 ) -> Callable[Concatenate[Any, ParamT], ReturnT_co]:
     """
     Wraps async MetisNamespaceSync's method.
@@ -50,205 +65,269 @@
     - wrap all with async_to_sync converter
     """
 
     async def inner(
         self: MetisNamespaceSyncBase, *args: ParamT.args, **kwargs: ParamT.kwargs
     ) -> ReturnT_co:
         # pylint: disable=protected-access
+        timeout = self._get_timeout(cast(TimeoutType, kwargs.get("timeout", None)))
+        # pylint: disable=protected-access
         async with self._client_getter() as client:
-            return await func(self, client, *args, **kwargs)
+            return await asyncio.wait_for(func(self, client, *args, **kwargs), timeout)
 
     return cast(Any, async_to_sync(inner))
 
 
-class MetisAuthNamespaceSync(MetisNamespaceSyncBase):
+class MetisCalculationsNamespaceSync(MetisNamespaceSyncBase):
+    """Calculations endpoints namespace"""
+
+    @to_sync_with_metis_client
+    async def supported(self, client: MetisAPIAsync):
+        "Get supported calculation engines"
+        return await client.calculations.supported()
+
+
+class MetisV0AuthNamespaceSync(MetisNamespaceSyncBase):
     """Authentication endpoints namespace"""
 
+    # pylint: disable=unused-argument
+
     @to_sync_with_metis_client
-    async def login(self, client: MetisAPIAsync, email: str, password: str):
+    async def login(
+        self,
+        client: MetisAPIAsync,
+        email: str,
+        password: str,
+        timeout: TimeoutType = None,
+    ):
         "Login"
         return await client.v0.auth.login(email, password)
 
     @to_sync_with_metis_client
-    async def whoami(self, client: MetisAPIAsync):
+    async def whoami(self, client: MetisAPIAsync, timeout: TimeoutType = None):
         "Get self info"
         return await client.v0.auth.whoami()
 
 
-class MetisDatasourcesNamespaceSync(MetisNamespaceSyncBase):
+class MetisV0DatasourcesNamespaceSync(MetisNamespaceSyncBase):
     """Datasources endpoints namespace"""
 
+    # pylint: disable=unused-argument
+
     @to_sync_with_metis_client
     async def create(
         self,
         client: MetisAPIAsync,
         content: str,
         fmt: Optional[str] = None,
         name: Optional[str] = None,
+        timeout: TimeoutType = None,
     ):
         "Create data source and wait for the result"
         return await client.v0.datasources.create(content, fmt, name)
 
     @to_sync_with_metis_client
-    async def delete(self, client: MetisAPIAsync, data_id: int):
+    async def delete(
+        self, client: MetisAPIAsync, data_id: int, timeout: TimeoutType = None
+    ):
         "Delete data source by id and wait for the result"
         return await client.v0.datasources.delete(data_id)
 
     @to_sync_with_metis_client
-    async def list(self, client: MetisAPIAsync):
+    async def list(self, client: MetisAPIAsync, timeout: TimeoutType = None):
         "List data sources and wait for the result"
         return await client.v0.datasources.list()
 
     @to_sync_with_metis_client
     async def get(
-        self, client: MetisAPIAsync, data_id: int
+        self, client: MetisAPIAsync, data_id: int, timeout: TimeoutType = None
     ) -> Optional[MetisDataSourceDTO]:
         "Get data source by id"
         return await client.v0.datasources.get(data_id)
 
     @to_sync_with_metis_client
     async def get_parents(
-        self, client: MetisAPIAsync, data_id: int
+        self, client: MetisAPIAsync, data_id: int, timeout: TimeoutType = None
     ) -> Sequence[MetisDataSourceDTO]:
         "Get parent data sources by id"
         return await client.v0.datasources.get_parents(data_id)
 
     @to_sync_with_metis_client
     async def get_children(
-        self, client: MetisAPIAsync, data_id: int
+        self, client: MetisAPIAsync, data_id: int, timeout: TimeoutType = None
     ) -> Sequence[MetisDataSourceDTO]:
         "Get children data sources by id"
         return await client.v0.datasources.get_children(data_id)
 
     @to_sync_with_metis_client
-    async def get_content(self, client: MetisAPIAsync, data_id: int):
+    async def get_content(
+        self, client: MetisAPIAsync, data_id: int, timeout: TimeoutType = None
+    ):
         "Get data source by id"
         return await client.v0.datasources.get_content(data_id)
 
 
-class MetisCalculationsNamespaceSync(MetisNamespaceSyncBase):
+class MetisV0CalculationsNamespaceSync(MetisNamespaceSyncBase):
     """Calculations endpoints namespace"""
 
+    # pylint: disable=unused-argument
+
     @to_sync_with_metis_client
-    async def cancel(self, client: MetisAPIAsync, calc_id: int):
+    async def cancel(
+        self, client: MetisAPIAsync, calc_id: int, timeout: TimeoutType = None
+    ):
         "Cancel calculation and wait for the result"
         return await client.v0.calculations.cancel(calc_id)
 
     @to_sync_with_metis_client
     async def create(
         self,
         client: MetisAPIAsync,
         data_id: int,
         engine: str = "dummy",
         input: Optional[str] = None,  # pylint: disable=redefined-builtin
+        timeout: TimeoutType = None,
     ):
         "Create calculation and wait for the result"
         return await client.v0.calculations.create(data_id, engine, input)
 
     @to_sync_with_metis_client
     async def get_results(
         self,
         client: MetisAPIAsync,
         calc_id: int,
         on_progress: Optional[MetisCalculationOnProgressT] = None,
+        timeout: TimeoutType = None,
     ):
         "Waits for the end of the calculation and returns the results"
         return await client.v0.calculations.get_results(calc_id, on_progress)
 
     @to_sync_with_metis_client
     async def create_get_results(
         self,
         client: MetisAPIAsync,
         data_id: int,
         engine: str = "dummy",
         input: Optional[str] = None,  # pylint: disable=redefined-builtin
         on_progress: Optional[MetisCalculationOnProgressT] = None,
+        timeout: TimeoutType = None,
     ):
         "Create calculation, wait done and get results"
         return await client.v0.calculations.create_get_results(
             data_id, engine, input, on_progress
         )
 
     @to_sync_with_metis_client
-    async def get_engines(self, client: MetisAPIAsync):
+    async def get_engines(self, client: MetisAPIAsync, timeout: TimeoutType = None):
         "Get supported calculation engines"
         return await client.v0.calculations.get_engines()
 
     @to_sync_with_metis_client
-    async def list(self, client: MetisAPIAsync):
+    async def list(self, client: MetisAPIAsync, timeout: TimeoutType = None):
         "List all user's calculations and wait for the result"
         return await client.v0.calculations.list()
 
     @to_sync_with_metis_client
-    async def get(self, client: MetisAPIAsync, calc_id: int):
+    async def get(
+        self, client: MetisAPIAsync, calc_id: int, timeout: TimeoutType = None
+    ):
         "Get calculation by id"
         return await client.v0.calculations.get(calc_id)
 
 
-class MetisCollectionsNamespaceSync(MetisNamespaceSyncBase):
+class MetisV0CollectionsNamespaceSync(MetisNamespaceSyncBase):
     """Collections endpoints namespace"""
 
+    # pylint: disable=unused-argument
+
     @to_sync_with_metis_client
     async def create(
         self,
         client: MetisAPIAsync,
         type_id: int,
         title: str,
+        timeout: TimeoutType = None,
         **opts: Unpack[MetisCollectionsCreateKwargs],
     ):
         "Create collection and wait for the result"
         return await client.v0.collections.create(type_id, title, **opts)
 
     @to_sync_with_metis_client
-    async def list(self, client: MetisAPIAsync):
+    async def list(self, client: MetisAPIAsync, timeout: TimeoutType = None):
         "List user's collections by criteria and wait for the result"
         return await client.v0.collections.list()
 
     @to_sync_with_metis_client
-    async def delete(self, client: MetisAPIAsync, collection_id: int):
+    async def delete(
+        self, client: MetisAPIAsync, collection_id: int, timeout: TimeoutType = None
+    ):
         "Remove a collection by id and wait for the result"
         return await client.v0.collections.delete(collection_id)
 
 
 # pylint: disable=too-few-public-methods
 class MetisV0NamespaceSync(MetisNamespaceSyncBase):
     """v0 namespace"""
 
-    def __init__(self, client_getter: AsyncClientGetter):
-        super().__init__(client_getter)
-        self.auth = MetisAuthNamespaceSync(client_getter)
-        self.calculations = MetisCalculationsNamespaceSync(client_getter)
-        self.collections = MetisCollectionsNamespaceSync(client_getter)
-        self.datasources = MetisDatasourcesNamespaceSync(client_getter)
+    def __init__(
+        self, client_getter: AsyncClientGetter, default_timeout: Optional[float] = False
+    ):
+        super().__init__(client_getter, default_timeout)
+        self.auth = MetisV0AuthNamespaceSync(client_getter, default_timeout)
+        self.calculations = MetisV0CalculationsNamespaceSync(
+            client_getter, default_timeout
+        )
+        self.collections = MetisV0CollectionsNamespaceSync(
+            client_getter, default_timeout
+        )
+        self.datasources = MetisV0DatasourcesNamespaceSync(
+            client_getter, default_timeout
+        )
 
 
 class MetisAPI(MetisBase):
     """Metis API synchronous client"""
 
     def __init__(
-        self, base_url: StrOrURL, **opts: Unpack[MetisAPIKwargs]
+        self,
+        base_url: StrOrURL,
+        **opts: Unpack[MetisAPIKwargs],
     ):  # pylint: disable=too-many-arguments
         """
         Initialize sync Metis client.
         Sync client is a tiny wrapper over full async client.
 
         **Arguments**:
 
         `bese_url`
         URL of Metis BFF server. `str` or `yarl.URL`.
 
         `headers` (Optional)
         Optional dictionary of always sent headers. Used if `session` is omitted.
 
         `timeout` (Optional)
-        Optional integer of global timeout in seconds or `aiohttp.ClientTimeout`.
-        Used if `session` is omitted.
+        Optional float timeout in seconds. None if no timeout. False if not set.
+        Used as `aiohttp` timeout if `session` is omitted.
+        Used as global timeout for SSE responses.
 
         `client_name` (Optional)
         Optional string for user agent.
         """
-        self._ns_v0 = MetisV0NamespaceSync(partial(MetisAPIAsync, base_url, **opts))
+        timeout = opts.get("timeout", None)
+        self._ns_calculations = MetisCalculationsNamespaceSync(
+            partial(MetisAPIAsync, base_url, **opts), timeout
+        )
+        self._ns_v0 = MetisV0NamespaceSync(
+            partial(MetisAPIAsync, base_url, **opts), timeout
+        )
+
+    @property
+    def calculations(
+        self,
+    ) -> MetisCalculationsNamespaceSync:  # pylint: disable=invalid-name
+        """Property to access the calculations namespace."""
+        return self._ns_calculations
 
     @property
     def v0(self) -> MetisV0NamespaceSync:  # pylint: disable=invalid-name
         """Property to access the v0 namespace."""
         return self._ns_v0
```

### Comparing `metis_client-0.3.0/metis_client/metis_async.py` & `metis_client-0.4.0/metis_client/metis_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Main Metis API async client"""
 
 import sys
 from types import TracebackType
-from typing import Optional, Type
+from typing import Literal, Optional, Type, Union
 
 import aiohttp
 from aiohttp import ClientSession, ClientTimeout, TraceConfig
 from aiohttp.hdrs import USER_AGENT
 from aiohttp.typedefs import LooseHeaders, StrOrURL
 from yarl import URL
 
 from .client import MetisClient
 from .const import DEFAULT_USER_AGENT
 from .models import BaseAuthenticator, MetisBase
+from .namespaces.calculations import MetisCalculationsNamespace
 from .namespaces.root import MetisRootNamespace
 from .namespaces.stream import MetisStreamNamespace
 from .namespaces.v0 import MetisV0Namespace
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import List
 else:  # pragma: no cover
@@ -28,15 +29,15 @@
     from typing import NotRequired, TypedDict, Unpack
 
 
 class MetisAPIKwargs(TypedDict):
     "MetisAPI init kwargs"
     auth: BaseAuthenticator
     headers: NotRequired[LooseHeaders]
-    timeout: NotRequired[int]
+    timeout: NotRequired[Union[float, Literal[False], None]]
     client_name: NotRequired[str]
     trace_configs: NotRequired[List[TraceConfig]]
 
 
 class MetisAPIAsync(MetisBase):
     """Main Metis API async client"""
 
@@ -61,42 +62,49 @@
         `aiohttp.ClientSession` to be used by this package.
         If you do not pass one, one will be created for you.
 
         `headers` (Optional)
         Optional dictionary of always sent headers. Used if `session` is omitted.
 
         `timeout` (Optional)
-        Optional integer of global timeout in seconds or `aiohttp.ClientTimeout`.
-        Used if `session` is omitted.
+        Optional float timeout in seconds. None if not timeout. False if not set.
+        Used as `aiohttp` timeout if `session` is omitted.
 
         `client_name` (Optional)
         Optional string for user agent.
         Used if `session` is omitted.
         """
         headers = opts.get("headers")
         if session is None:
-            timeout = opts.get("timeout")
+            timeout = opts.get("timeout", None)
             session = aiohttp.ClientSession(
                 timeout=timeout
                 if isinstance(timeout, ClientTimeout)
-                else ClientTimeout(total=timeout),
+                else ClientTimeout(total=timeout or None),
                 headers=headers,
                 trace_configs=opts.get("trace_configs"),
             )
             session.headers[USER_AGENT] = opts.get("client_name", DEFAULT_USER_AGENT)
             self._close_session = True
         self._session = session
 
         base_url = URL(base_url)
         if not base_url.is_absolute():
             raise TypeError("Base URL should be absolute")
         client = MetisClient(session, base_url, opts["auth"])
         self._ns_root = MetisRootNamespace(client, base_url)
 
     @property
+    def calculations(
+        self,
+    ) -> MetisCalculationsNamespace:  # pylint: disable=invalid-name
+        """Property to access the calculations namespace."""
+        return self._ns_root.calculations
+
+    @property
     def v0(self) -> MetisV0Namespace:  # pylint: disable=invalid-name
         """Property to access the v0 namespace."""
         return self._ns_root.v0
 
     @property
     def stream(self) -> MetisStreamNamespace:
         """Property to access the stream namespace."""
```

### Comparing `metis_client-0.3.0/metis_client/models/auth.py` & `metis_client-0.4.0/metis_client/models/auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/models/event.py` & `metis_client-0.4.0/metis_client/models/event.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/models/hub.py` & `metis_client-0.4.0/metis_client/models/hub.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/models/subscription.py` & `metis_client-0.4.0/metis_client/models/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,12 @@
         self.hub.unsubscribe(self)
 
     def __aiter__(self) -> "MetisSubscription":
         return self
 
     @asynccontextmanager
     async def _cm(self):
-        try:
-            yield await self.queue.get()
-        finally:
-            self.queue.task_done()
+        yield await self.queue.get()
 
     async def __anext__(self) -> MetisEventDTO:
         async with self._cm() as msg:
             return msg
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/auth.py` & `metis_client-0.4.0/metis_client/namespaces/v0_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Authentication endpoints namespace"""
 
 from ..dtos import MetisAuthCredentialsRequestDTO, MetisUserDTO
 from ..helpers import dict_dt_from_dt_str, raise_on_metis_error
 from .base import BaseNamespace
 
 
-class MetisAuthNamespace(BaseNamespace):
+class MetisV0AuthNamespace(BaseNamespace):
     """Authentication endpoints namespace"""
 
     @raise_on_metis_error
     async def login(self, email: str, password: str) -> bool:
         "Login"
         payload = MetisAuthCredentialsRequestDTO(email=email, password=password)
         async with self._client.request(
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/base.py` & `metis_client-0.4.0/metis_client/namespaces/base.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/metis_client/namespaces/calculations.py` & `metis_client-0.4.0/metis_client/namespaces/v0_calculations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Calculations endpoints namespace"""
 import sys
 from datetime import datetime
 from functools import partial
 from inspect import iscoroutinefunction
 from typing import Awaitable, Callable, Optional, Union, cast
+from warnings import warn
 
 from ..dtos import (
     DataSourceType,
     MetisCalculationDTO,
     MetisDataSourceDTO,
     MetisRequestIdDTO,
 )
+from ..exc import MetisPayloadException
 from ..helpers import raise_on_metis_error
 from ..models import act_and_get_result_from_stream
 from .base import BaseNamespace
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Sequence
 else:  # pragma: no cover
@@ -24,15 +26,15 @@
 DATA_SOURCE_CALC_RESULT_TYPES = [DataSourceType.PROPERTY, DataSourceType.PATTERN]
 
 MetisCalculationOnProgressT = Callable[
     [MetisCalculationDTO], Union[Optional[bool], Awaitable[Optional[bool]]]
 ]
 
 
-class MetisCalculationsNamespace(BaseNamespace):
+class MetisV0CalculationsNamespace(BaseNamespace):
     """Calculations endpoints namespace"""
 
     async def cancel_event(self, calc_id: int) -> MetisRequestIdDTO:
         "Cancel calculation"
         async with await self._client.request(
             method="DELETE",
             url=self._base_url / str(calc_id),
@@ -64,14 +66,17 @@
     async def create(
         self,
         data_id: int,
         engine: str = "dummy",
         input: Optional[str] = None,  # pylint: disable=redefined-builtin
     ) -> Optional[MetisCalculationDTO]:
         "Create calculation and wait for result"
+        valid_engines = await self._root.calculations.supported()
+        if engine not in valid_engines:
+            raise MetisPayloadException(message="unsupported engine", status=400)
         evt = await act_and_get_result_from_stream(
             self._root.stream.subscribe,
             partial(self.create_event, data_id, engine, input),
         )
         if evt["type"] == "calculations":
             data = sorted(
                 evt.get("data", {}).get("data", []),
@@ -163,20 +168,20 @@
             return await self.create(data_id, engine, input)
 
         return await self._get_results(get_calc, on_progress)
 
     @raise_on_metis_error
     async def get_engines(self) -> Sequence[str]:
         "Get supported calculation engines"
-        async with await self._client.request(
-            method="GET",
-            url=self._base_url / "engines",
-            auth_required=False,
-        ) as resp:
-            return await resp.json()
+        msg = (
+            "v0.calculations.get_engines() is deprecated; "
+            "please, use calculations.supported() instead"
+        )
+        warn(DeprecationWarning(msg))
+        return await self._root.calculations.supported()
 
     async def list_event(self) -> MetisRequestIdDTO:
         "List all user's calculations"
         async with await self._client.request(
             method="GET",
             url=self._base_url,
             auth_required=True,
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/collections.py` & `metis_client-0.4.0/metis_client/namespaces/v0_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import NotRequired, TypedDict, Unpack
 else:  # pragma: no cover
     from typing import NotRequired, TypedDict, Unpack
 
 
 class MetisCollectionsCreateKwargs(TypedDict):
-    "MetisCollectionsNamespace.create kwargs"
+    "MetisV0CollectionsNamespace.create kwargs"
     description: NotRequired[str]
     data_source_ids: NotRequired[Sequence[int]]
     user_ids: NotRequired[Sequence[int]]
 
 
-class MetisCollectionsNamespace(BaseNamespace):
+class MetisV0CollectionsNamespace(BaseNamespace):
     """Collections endpoints namespace"""
 
     async def create_event(
         self, type_id: int, title: str, **opts: Unpack[MetisCollectionsCreateKwargs]
     ) -> MetisRequestIdDTO:
         "Create collection"
         payload = MetisCollectionCreateDTO(
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/datasources.py` & `metis_client-0.4.0/metis_client/namespaces/v0_datasources.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Sequence
 else:  # pragma: no cover
     from collections.abc import Sequence
 
 
-class MetisDatasourcesNamespace(BaseNamespace):
+class MetisV0DatasourcesNamespace(BaseNamespace):
     """Datasources endpoints namespace"""
 
     async def create_event(
         self, content: str, fmt: Optional[str] = None, name: Optional[str] = None
     ) -> MetisRequestIdDTO:
         "Create data source"
         async with self._client.request(
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/root.py` & `metis_client-0.4.0/metis_client/namespaces/root.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Root namespace"""
 
 from yarl import URL
 
 from ..client import MetisClient
 from .base import BaseNamespace
+from .calculations import MetisCalculationsNamespace
 from .stream import MetisStreamNamespace
 from .v0 import MetisV0Namespace
 
 
 class MetisRootNamespace(BaseNamespace):
     """Root namespace"""
 
@@ -15,23 +16,31 @@
         self,
         client: MetisClient,
         base_url: URL,
         root=None,
         auth_req: bool = True,
     ) -> None:
         """Initialise the namespace."""
-        super().__init__(client, base_url, self, auth_req)
+        super().__init__(client, base_url, root or self, auth_req)
 
     def __post_init__(self) -> None:
+        self.__ns_calculations = MetisCalculationsNamespace(
+            self._client, self._base_url / "calculations", root=self
+        )
         self.__ns_v0 = MetisV0Namespace(self._client, self._base_url / "v0", root=self)
         self.__ns_stream = MetisStreamNamespace(
             self._client, self._base_url / "stream", root=self
         )
 
     @property
+    def calculations(self) -> "MetisCalculationsNamespace":
+        """Property to access the calculations namespace."""
+        return self.__ns_calculations
+
+    @property
     def v0(self) -> "MetisV0Namespace":  # pylint: disable=invalid-name
         """Property to access the v0 namespace."""
         return self.__ns_v0
 
     @property
     def stream(self) -> "MetisStreamNamespace":
         """Property to access the stream namespace."""
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/stream.py` & `metis_client-0.4.0/metis_client/namespaces/stream.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,12 +56,14 @@
                 await asyncio.sleep(0.1)
                 await self._root.v0.ping()
 
     def close(self):
         "Close background stream consumer"
         if self._stream_task:
             self._stream_task.cancel()
+        if self._sse_client_task:
+            self._sse_client_task.cancel()
 
     def subscribe(self, predicate: Optional[Callable[[MetisEventDTO], bool]] = None):
         "Subscribe to stream"
         self._subscribe_event.set()
         return MetisSubscription(self._hub, predicate=predicate)
```

### Comparing `metis_client-0.3.0/metis_client/namespaces/v0.py` & `metis_client-0.4.0/metis_client/namespaces/v0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 """v0 namespace"""
 
-from .auth import MetisAuthNamespace
 from .base import BaseNamespace
-from .calculations import MetisCalculationsNamespace
-from .collections import MetisCollectionsNamespace
-from .datasources import MetisDatasourcesNamespace
+from .v0_auth import MetisV0AuthNamespace
+from .v0_calculations import MetisV0CalculationsNamespace
+from .v0_collections import MetisV0CollectionsNamespace
+from .v0_datasources import MetisV0DatasourcesNamespace
 
 
 class MetisV0Namespace(BaseNamespace):
     """v0 namespace"""
 
     def __post_init__(self) -> None:
-        self.__ns_auth = MetisAuthNamespace(
+        self.__ns_auth = MetisV0AuthNamespace(
             self._client, self._base_url / "auth", root=self._root
         )
-        self.__ns_calculations = MetisCalculationsNamespace(
+        self.__ns_calculations = MetisV0CalculationsNamespace(
             self._client, self._base_url / "calculations", root=self._root
         )
-        self.__ns_collections = MetisCollectionsNamespace(
+        self.__ns_collections = MetisV0CollectionsNamespace(
             self._client, self._base_url / "collections", root=self._root
         )
-        self.__ns_datasources = MetisDatasourcesNamespace(
+        self.__ns_datasources = MetisV0DatasourcesNamespace(
             self._client, self._base_url / "datasources", root=self._root
         )
 
     async def ping(self) -> None:
         "Run ping pong game"
         await self._client.request(url=self._base_url, method="HEAD", json={})
 
     @property
-    def auth(self) -> MetisAuthNamespace:
+    def auth(self) -> MetisV0AuthNamespace:
         "Property to access the auth namespace."
         return self.__ns_auth
 
     @property
-    def calculations(self) -> MetisCalculationsNamespace:
+    def calculations(self) -> MetisV0CalculationsNamespace:
         "Property to access the calculations namespace."
         return self.__ns_calculations
 
     @property
-    def collections(self) -> MetisCollectionsNamespace:
+    def collections(self) -> MetisV0CollectionsNamespace:
         "Property to access the collections namespace."
         return self.__ns_collections
 
     @property
-    def datasources(self) -> MetisDatasourcesNamespace:
+    def datasources(self) -> MetisV0DatasourcesNamespace:
         "Property to access the datasources namespace."
         return self.__ns_datasources
```

### Comparing `metis_client-0.3.0/pyproject.toml` & `metis_client-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # build the package with [flit](https://flit.readthedocs.io)
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "metis-client"
-version = "0.3.0"
+version = "0.4.0"
 description = """Metis infra API client in Python"""
 authors = [{name = "Sergei Korolev", email = "knopki@duck.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
@@ -129,15 +129,15 @@
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = "--cov=metis_client --cov-report=term --no-cov-on-fail --cov-fail-under=99"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0"
+version = "0.4.0"
 tag_format = "v$version"
 major_version_zero = true
 version_files = [
     "pyproject.toml:^version",
     "metis_client/const.py:^PROJECT_VERSION",
 ]
 update_changelog_on_bump = true
```

### Comparing `metis_client-0.3.0/tests/models/test_auth_no_auth.py` & `metis_client-0.4.0/tests/models/test_auth_no_auth.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/tests/models/test_auth_password.py` & `metis_client-0.4.0/tests/models/test_auth_password.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/tests/models/test_auth_token.py` & `metis_client-0.4.0/tests/models/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/tests/models/test_subscription.py` & `metis_client-0.4.0/tests/models/test_subscription.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/tests/namespaces/test_auth.py` & `metis_client-0.4.0/tests/namespaces/test_v0_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"Test MetisAuthNamespace"
+"Test MetisV0AuthNamespace"
 
 import asyncio
 from copy import deepcopy
 from datetime import datetime
 
 import pytest
 from aiohttp import web
```

### Comparing `metis_client-0.3.0/tests/namespaces/test_calculations.py` & `metis_client-0.4.0/tests/namespaces/test_v0_calculations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"Test MetisCalculationsNamespace"
+"Test MetisV0CalculationsNamespace"
 
 import asyncio
 import json
 from contextlib import nullcontext as does_not_raise
 from copy import deepcopy
 from datetime import datetime
 from typing import List
@@ -15,28 +15,32 @@
 
 from metis_client import MetisAPI, MetisAPIAsync, MetisTokenAuth
 from metis_client.dtos import MetisCalculationDTO, MetisErrorDTO, MetisRequestIdDTO
 from metis_client.dtos.datasource import DataSourceType
 from metis_client.exc import MetisPayloadException, MetisQuotaException
 from metis_client.models import MetisMessageEvent
 from tests.helpers import random_word
-from tests.namespaces.test_datasources import (
+from tests.namespaces.test_calculations import (
+    PATH_C_ENGINES,
+    PATH_C_GET_ENGINES_RESPONSE,
+    get_engines_handler,
+)
+from tests.namespaces.test_v0_datasources import (
     DS_ID,
     PATH_DS_POST_RESPONSE_PAYLOAD,
     make_datasources_event,
 )
 
 dt = datetime.fromordinal(1)
 TOKEN = random_word(10)
 CALC_ID = 10
 PATH_STREAM = "/stream"
 PATH_PING = "/v0"
 PATH_C = "/v0/calculations"
 PATH_C_ID = "/v0/calculations/{id}"
-PATH_C_ENGINES = "/v0/calculations/engines"
 PATH_C_POST_RESPONSE_PAYLOAD: MetisCalculationDTO = {
     "id": CALC_ID,
     "name": random_word(10),
     "userId": 1,
     "progress": 1,
     "result": [],
     "createdAt": dt,
@@ -47,15 +51,14 @@
 PATH_C_GET_RESPONSE_PAYLOAD = deepcopy(PATH_C_POST_RESPONSE_PAYLOAD)
 PATH_C_GET_RESPONSE_ERROR_PAYLOAD: MetisErrorDTO = {"status": 402, "error": "oops"}
 PATH_C_DELETE_RESPONSE_ERROR_PAYLOAD = deepcopy(PATH_C_POST_RESPONSE_ERROR_PAYLOAD)
 PATH_C_DELETE_RESPONSE_ERROR404_PAYLOAD = {
     "status": HTTPNotFound.status_code,
     "error": "not found",
 }
-PATH_C_GET_ENGINES_RESPONSE = ["dummy", "other"]
 
 event_stream: List[MetisMessageEvent] = []
 
 
 def make_calculations_event(req_id: str, datas) -> MetisMessageEvent:
     "Create calculations event with content"
     evt_data_dto = {"reqId": req_id, "data": datas, "total": 1, "types": []}
@@ -169,19 +172,14 @@
         evt = make_calculations_event(body["reqId"], [])
 
     event_stream.append(evt)
 
     return web.json_response(body, status=HTTPOk.status_code)
 
 
-async def get_engines_handler(_: web.Request) -> web.Response:
-    "Request handler"
-    return web.json_response(PATH_C_GET_ENGINES_RESPONSE, status=HTTPOk.status_code)
-
-
 async def create_app() -> web.Application:
     "Create web application"
     app = web.Application()
     app.router.add_head(PATH_PING, ping_handler)
     app.router.add_get(PATH_STREAM, sse_handler)
     app.router.add_post(PATH_C, calculation_create_handler)
     app.router.add_get(PATH_C, list_calculations_handler)
@@ -363,13 +361,15 @@
         await asyncio.get_event_loop().run_in_executor(
             None, client.v0.calculations.cancel, cal_id
         )
 
 
 async def test_get_engines(client: MetisAPI, client_async: MetisAPIAsync):
     "Test get_engines()"
-    en_async = await client_async.v0.calculations.get_engines()
-    en_sync = await asyncio.get_event_loop().run_in_executor(
-        None, client.v0.calculations.get_engines
-    )
+    with pytest.warns(DeprecationWarning):
+        en_async = await client_async.v0.calculations.get_engines()
+    with pytest.warns(DeprecationWarning):
+        en_sync = await asyncio.get_event_loop().run_in_executor(
+            None, client.v0.calculations.get_engines
+        )
     assert en_async == en_sync, "Response matches"
     assert en_sync == PATH_C_GET_ENGINES_RESPONSE, "Response matches"
```

### Comparing `metis_client-0.3.0/tests/namespaces/test_collections.py` & `metis_client-0.4.0/tests/namespaces/test_v0_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"Test MetisCollectionsNamespace"
+"Test MetisV0CollectionsNamespace"
 
 import asyncio
 import json
 from contextlib import nullcontext as does_not_raise
 from copy import deepcopy
 from datetime import datetime
 from functools import partial
```

### Comparing `metis_client-0.3.0/tests/namespaces/test_datasources.py` & `metis_client-0.4.0/tests/namespaces/test_v0_datasources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-"Test MetisDatasourcesNamespace"
+"Test MetisV0DatasourcesNamespace"
 
 import asyncio
 import json
 from contextlib import nullcontext as does_not_raise
 from copy import deepcopy
 from datetime import datetime
+from functools import partial
 from typing import List
 
 import pytest
 from aiohttp import web
 from aiohttp.test_utils import TestClient, TestServer
 from aiohttp.web_exceptions import HTTPNotFound, HTTPOk
+from freezegun import freeze_time
 from yarl import URL
 
 from metis_client import MetisAPI, MetisAPIAsync, MetisTokenAuth
 from metis_client.dtos import (
     MetisDataSourceContentOnlyDTO,
     MetisDataSourceDTO,
     MetisErrorDTO,
@@ -121,14 +123,17 @@
 
 
 async def list_datasources_handler(request: web.Request) -> web.Response:
     "Request handler"
     auth_header = request.headers.get("Authorization", "")
     body: MetisRequestIdDTO = {"reqId": random_word(10)}
 
+    if auth_header == "Bearer slow":
+        await asyncio.sleep(10)
+
     if auth_header != f"Bearer {str(True)}":
         ds_dto = {
             **PATH_DS_GET_RESPONSE_PAYLOAD,
             "createdAt": dt.isoformat(),
             "updatedAt": dt.isoformat(),
         }
         evt = make_datasources_event(body["reqId"], [ds_dto])
@@ -248,14 +253,24 @@
         client = MetisAPI(base_url, auth=MetisTokenAuth(str(fail)))
         src = await asyncio.get_event_loop().run_in_executor(
             None, client.v0.datasources.list
         )
         assert src == expected, "Response matches"
 
 
+@freeze_time("1970-01-01", auto_tick_seconds=10)
+async def test_timeout(base_url: URL, client: MetisAPI):
+    "Test timeout"
+    client = MetisAPI(base_url, auth=MetisTokenAuth("slow"))
+    with pytest.raises(asyncio.TimeoutError):
+        await asyncio.get_event_loop().run_in_executor(
+            None, partial(client.v0.datasources.list, timeout=1)
+        )
+
+
 @pytest.mark.parametrize(
     "method_name, data_id, fail, expected, raises",
     [
         # get()
         ("get", -1, True, None, pytest.raises(MetisQuotaException)),
         ("get", DS_ID, False, PATH_DS_GET_RESPONSE_PAYLOAD, does_not_raise()),
         ("get", PARENT_DS_ID, False, None, does_not_raise()),
```

### Comparing `metis_client-0.3.0/tests/test_client.py` & `metis_client-0.4.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,32 +165,14 @@
     client: MetisClient,
 ):  # pylint: disable=redefined-outer-name
     "Test too many requests"
     resp = await client.request(URL(PATH_TOO_MANY))
     assert resp.ok, "Should tolerate too many requests"
 
 
-async def test_cancelled_error(
-    client: MetisClient,
-):  # pylint: disable=redefined-outer-name
-    "Test CancelledError"
-
-    async def fetch():
-        await client.request(URL(PATH_SLOW_RESPONSE))
-
-    task = asyncio.create_task(fetch())
-    await asyncio.sleep(0.0001)
-    task.cancel()
-    with pytest.raises(MetisConnectionException) as exc_info:
-        await task
-    assert (
-        "Request exception" in exc_info.value.args[0]
-    ), "MetisClient should handle CancelledError"
-
-
 async def test_client_connection_error(
     client: MetisClient,
 ):  # pylint: disable=redefined-outer-name
     "Test ClientConnectionError"
 
     with pytest.raises(MetisConnectionException) as exc_info:
         await client.request(URL("http://0.0.0.0:1"))
```

### Comparing `metis_client-0.3.0/tests/test_helpers_convert_dict_items_to_datetime.py` & `metis_client-0.4.0/tests/test_helpers_convert_dict_items_to_datetime.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/tests/test_helpers_rfc3339.py` & `metis_client-0.4.0/tests/test_helpers_rfc3339.py`

 * *Files identical despite different names*

### Comparing `metis_client-0.3.0/PKG-INFO` & `metis_client-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metis-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Metis infra API client in Python
 Keywords: metis,client
 Author-email: Sergei Korolev <knopki@duck.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -86,25 +86,24 @@
 ### Synchronous client
 
 A synchronous client is `MetisAPI`. Example of usage:
 
 ```python
 from metis_client import MetisAPI, MetisTokenAuth
 
-client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"))
+client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"), timeout=5)
 data = client.v0.datasources.create(content)
-results = client.v0.calculations.create_get_results(data["id"])
+results = client.v0.calculations.create_get_results(data["id"], timeout=False)
 print(results)
 ```
 
 NB in development one can replace a `VERY_SECRET_TOKEN` string with the development user email, e.g.
 `admin@test.com` (refer to **users_emails** BFF table).
 
 ## License
 
 Author Sergey Korolev, Tilde Materials Informatics
 
 Copyright 2023 BASF SE
 
 BSD 3-Clause
-  * [ ]
```

