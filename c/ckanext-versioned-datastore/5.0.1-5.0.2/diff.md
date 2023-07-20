# Comparing `tmp/ckanext-versioned-datastore-5.0.1.tar.gz` & `tmp/ckanext-versioned-datastore-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-versioned-datastore-5.0.1.tar", last modified: Tue Jul 18 09:33:20 2023, max compression
+gzip compressed data, was "ckanext-versioned-datastore-5.0.2.tar", last modified: Thu Jul 20 16:03:36 2023, max compression
```

## Comparing `ckanext-versioned-datastore-5.0.1.tar` & `ckanext-versioned-datastore-5.0.2.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/servers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/servers/direct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.186709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/queuing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/query_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/slug_words.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/v1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/basic_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.190709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    36112 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/multisearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.178709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/README
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/download-popup.less
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/download-status.less
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/search.less
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/slugerator.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.194709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.198709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/resource_data.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/search/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/search/slugerator.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/status/
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/status/download.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/versioned_datastore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:33:19.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 09:33:20.000000 ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.206709 ckanext-versioned-datastore-5.0.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/helpers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/helpers/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/helpers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/integration/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)    21716 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/integration/downloads/test_downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_runmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/importing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/importing/ingestion/test_ingestion_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/query/test_query_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/query/test_query_v1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/lib/test_datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.182709 ckanext-versioned-datastore-5.0.1/tests/unit/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:33:20.210709 ckanext-versioned-datastore-5.0.1/tests/unit/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/logic/actions/test_actions_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-18 09:33:09.000000 ckanext-versioned-datastore-5.0.1/tests/unit/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.599043 ckanext-versioned-datastore-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-20 16:03:36.599043 ckanext-versioned-datastore-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22671 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/servers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/servers/direct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.567041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.571041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.571041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/queuing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.571041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/query_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/slug_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/v1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.571041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/basic_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36112 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/multisearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.555040 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.575042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/download-popup.less
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/download-status.less
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/slugerator.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.579042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/search/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/status/download.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/versioned_datastore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.591042 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 16:03:36.000000 ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:03:36.599043 ckanext-versioned-datastore-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/helpers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/helpers/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/helpers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.559041 ckanext-versioned-datastore-5.0.2/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/integration/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)    21716 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/integration/downloads/test_downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_runmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/tests/unit/lib/importing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/query/test_query_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/query/test_query_v1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/lib/test_datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.563041 ckanext-versioned-datastore-5.0.2/tests/unit/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:36.595043 ckanext-versioned-datastore-5.0.2/tests/unit/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/logic/actions/test_actions_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-20 16:03:22.000000 ckanext-versioned-datastore-5.0.2/tests/unit/test_helpers.py
```

### Comparing `ckanext-versioned-datastore-5.0.1/LICENSE` & `ckanext-versioned-datastore-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/PKG-INFO` & `ckanext-versioned-datastore-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 5.0.1
+Version: 5.0.2
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-datastore-5.0.1/README.md` & `ckanext-versioned-datastore-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/cli.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/helpers.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/interfaces.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/geo.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/search.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/basic_query/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/basic_query/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/common.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/common.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/datastore_utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/base.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/json.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/download.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,25 +131,25 @@
         """
         return os.path.join(self.core_dir, self.query.hash)
 
     def run(self):
         """
         Run the download process.
         """
-        self.notifier.notify_start()
-        self.request.update_status(DownloadRequest.state_initial)
-
         try:
             # refresh the db objects because they were probably retrieved in a
             # different session (the __init__ is run by the main ckan process,
             # this is run by the download worker)
             self.request = DownloadRequest.get(self.request.id)
             self.core_record = CoreFileRecord.get(self.core_record.id)
             self.derivative_record = DerivativeFileRecord.get(self.derivative_record.id)
 
+            self.notifier.notify_start()
+            self.request.update_status(DownloadRequest.state_initial)
+
             # generate core file if needed
             # technically we don't need core files if the format is 'raw', but we'll
             # generate them anyway for consistency/avoidance of thousands of ifs, and
             # also so we have some field metadata
             self.generate_core()
 
             # generate derivative file if needed
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/loaders.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/loaders.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/base.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABCMeta, abstractmethod
-from ckan.plugins import toolkit, PluginImplementations
 from jinja2 import Template
 
+from ckan.plugins import toolkit, PluginImplementations
 from ....interfaces import IVersionedDatastoreDownloads
 from ....model.downloads import DownloadRequest
 
 
 class BaseNotifier(metaclass=ABCMeta):
     name = 'base'
 
@@ -107,7 +107,11 @@
     @abstractmethod
     def notify_end(self, file_url):
         raise NotImplemented
 
     @abstractmethod
     def notify_error(self):
         raise NotImplemented
+
+    @classmethod
+    def validate_args(cls, type_args):
+        return True
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,7 +31,14 @@
 
     def notify_error(self):
         request_method = 'POST' if self.post else 'GET'
         text, _ = self.error_text()
         context = self.template_context()
         params = {self.url_param: context['status_page'], self.text_param: text}
         requests.request(request_method, self.url, params=params)
+
+    @classmethod
+    def validate_args(cls, type_args):
+        url = type_args.get('url')
+        if not url:
+            raise toolkit.Invalid('URL must be provided')
+        return True
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/query.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/downloads/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/details.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/importing.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/importing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/indexing.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/indexing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/readers.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/records.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/ingestion/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/queuing.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/queuing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/stats.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/importing/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/importing/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/fields.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/fields.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/query_log.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/query_log.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/schema.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/slug_words.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/slug_words.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/slugs.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/slugs.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/utils.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/lib/query/v1_0_0.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/lib/query/v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/basic_search.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/basic_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/crud.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/downloads.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/downloads.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from ckantools.decorators import action
 
 from ckan.plugins import toolkit
 from .meta import help, schema
 from .meta.arg_objects import ServerArgs, NotifierArgs, QueryArgs, DerivativeArgs
 from ...lib.downloads.download import DownloadRunManager
 from ...model.downloads import DownloadRequest
+from ...lib.downloads.notifiers import validate_notifier_args
 
 
 @action(schema.datastore_queue_download(), help.datastore_queue_download)
 def datastore_queue_download(
     context,
     query: QueryArgs,
     file: DerivativeArgs,
     server: ServerArgs = None,
     notifier: NotifierArgs = None,
 ):
     server = server or ServerArgs(**ServerArgs.defaults)
     notifier = notifier or NotifierArgs(**NotifierArgs.defaults)
 
+    validate_notifier_args(notifier.type, notifier.type_args)
+
     if server.custom_filename:
         # check if admin
         try:
             toolkit.check_access('datastore_custom_download_filename', context)
         except toolkit.NotAuthorized:
             server.custom_filename = None
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/extras.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/extras.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/help.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/help.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/meta/schema.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/meta/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/actions/multisearch.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/actions/multisearch.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/logic/auth.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/env.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/details.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/downloads.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/slugs.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/slugs.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/model/stats.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/model/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/plugin.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/datastore.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/datastore.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/downloads.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/search.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/routes/status.py` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/routes/status.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/less/download-popup.less` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/less/download-popup.less`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -122,18 +122,21 @@
                 this.el.popover('hide');
             });
 
             // hide/show the email group when user changes notif type
             const notifierSelect = this.popoverForm.find('#vds-dl-notifier');
             notifierSelect.on('change', () => {
                 let emailGroup = this.popoverForm.find('#vds-dl-email-group');
+                let emailBox = this.popoverForm.find('#vds-dl-email');
                 if (notifierSelect.val() === 'email') {
                     emailGroup.removeClass('hidden');
+                    emailBox.attr('required', true);
                 } else {
                     emailGroup.addClass('hidden');
+                    emailBox.removeAttr('required');
                 }
             });
 
             // prevent the form submitting until we're ready
             const submitButton = this.popoverForm.find('#vds-dl-submit');
             submitButton.attr('disabled', true);
             this.popoverForm.on('submit', (e) => {
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/assets/webassets.yml` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/api.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/api.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html`

 * *Files 7% similar despite different names*

```diff
@@ -41,22 +41,18 @@
                     </option>
                     <option value="none">
                         I'll check the download status manually
                     </option>
                 </select>
             </div>
             <div class="form-row" id="vds-dl-email-group">
-                <label for="vds-dl-email">Email address(es)</label>
-                <input id="vds-dl-email" type="text"
+                <label for="vds-dl-email">Email address</label>
+                <input id="vds-dl-email" type="email" required
                        placeholder="data@nhm.ac.uk"
                        class="full-width-input" name="notifier.type_args.emails">
-                <p>
-                    <small>Multiple email addresses can be added as a comma-separated
-                           list.</small>
-                </p>
             </div>
         </div>
 
         <div class="privacy-warning">
             <p><i>Data Protection</i></p>
             <p>
                 The Natural History Museum will use your personal data in accordance
```

#### html2text {}

```diff
@@ -5,16 +5,15 @@
 One file per resource ⁰
 {% endif %}
 Skip empty columns ⁰
 {% endif %}
 Notifications
 Should we notify you when your download is ready?
 [One of: Email me/I'll check the download status manually]
-Email address(es) [notifier.type_args.emails]
-Multiple email addresses can be added as a comma-separated list.
+Email address [Unknown INPUT type]
 Data Protection
 The Natural History Museum will use your personal data in accordance with data
 protection legislation to process your requests. For more information please
 read our privacy_notice.
   {{ _('Submit') }}    {{ _('Cancel') }}
 Your download has been queued. You can follow its progress at the link below:
  Download_status
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/resource_data.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/search/search.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/search/slugerator.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/status/download.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/status/download.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html` & `ckanext-versioned-datastore-5.0.2/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/PKG-INFO` & `ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 5.0.1
+Version: 5.0.2
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-datastore-5.0.1/ckanext_versioned_datastore.egg-info/SOURCES.txt` & `ckanext-versioned-datastore-5.0.2/ckanext_versioned_datastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/docs/_scripts/gen_api_pages.py` & `ckanext-versioned-datastore-5.0.2/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/pyproject.toml` & `ckanext-versioned-datastore-5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-versioned-datastore"
-version = "5.0.1"
+version = "5.0.2"
 description = "A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -71,15 +71,15 @@
 
 [tool.setuptools.package-data]
 "ckanext.versioned_datastore.theme" = ["*", "**/*"]
 "ckanext.versioned_datastore.migration" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "5.0.1"
+version = "5.0.2"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-versioned-datastore-5.0.1/tests/helpers/data.py` & `ckanext-versioned-datastore-5.0.2/tests/helpers/data.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/helpers/patches.py` & `ckanext-versioned-datastore-5.0.2/tests/helpers/patches.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/helpers/utils.py` & `ckanext-versioned-datastore-5.0.2/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/integration/downloads/test_downloads.py` & `ckanext-versioned-datastore-5.0.2/tests/integration/downloads/test_downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_geo.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_search.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/basic_query/test_basic_query_utils.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/basic_query/test_basic_query_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_notifiers.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_notifiers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_query.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_runmanager.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_runmanager.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/downloads/test_downloads_utils.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/downloads/test_downloads_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/importing/ingestion/test_ingestion_records.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/query/test_query_query.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/query/test_query_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/query/test_query_v1_0_0.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/query/test_query_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/lib/test_datastore_utils.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/lib/test_datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/logic/actions/test_actions_downloads.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/logic/actions/test_actions_downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-5.0.1/tests/unit/test_helpers.py` & `ckanext-versioned-datastore-5.0.2/tests/unit/test_helpers.py`

 * *Files identical despite different names*

