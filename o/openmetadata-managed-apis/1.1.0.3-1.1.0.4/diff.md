# Comparing `tmp/openmetadata_managed_apis-1.1.0.3.tar.gz` & `tmp/openmetadata_managed_apis-1.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.1.0.3.tar", last modified: Thu Jul  6 10:45:34 2023, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.1.0.4.tar", last modified: Thu Jul 20 12:10:15 2023, max compression
```

## Comparing `openmetadata_managed_apis-1.1.0.3.tar` & `openmetadata_managed_apis-1.1.0.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.216525 openmetadata_managed_apis-1.1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-06 10:45:34.216525 openmetadata_managed_apis-1.1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.208526 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/health_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.208526 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.212525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.216525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.216525 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:45:34.208526 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:45:16.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 10:45:30.000000 openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:45:34.216525 openmetadata_managed_apis-1.1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 10:43:46.000000 openmetadata_managed_apis-1.1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.213029 openmetadata_managed_apis-1.1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-20 12:10:15.213029 openmetadata_managed_apis-1.1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.201029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.201029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.205029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/health_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.205029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.209030 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.209030 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.209030 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.197029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.209030 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.209030 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.213029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:10:15.201029 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:09:51.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 12:10:10.000000 openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:10:15.213029 openmetadata_managed_apis-1.1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-20 12:07:52.000000 openmetadata_managed_apis-1.1.0.4/setup.py
```

### Comparing `openmetadata_managed_apis-1.1.0.3/PKG-INFO` & `openmetadata_managed_apis-1.1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.1.0.3
+Version: 1.1.0.4
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.1.0.3/README.md` & `openmetadata_managed_apis-1.1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/health_auth.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/health_auth.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/ip.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/run_automation.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/delete.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/health.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-managed-apis
-Version: 1.1.0.3
+Version: 1.1.0.4
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.1.0.3/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.1.0.4/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.3/setup.py` & `openmetadata_managed_apis-1.1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 }
 
 setup(
     name=PLUGIN_NAME,
     packages=find_packages(include=[f"{PLUGIN_NAME}.*", PLUGIN_NAME]),
     include_package_data=True,
     package_data={PLUGIN_NAME: get_package_data()},
-    version="1.1.0.3",
+    version="1.1.0.4",
     url="https://open-metadata.org/",
     author="OpenMetadata Committers",
     license="Apache License 2.0",
     description="Airflow REST APIs to create and manage DAGS",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     entry_points={
```

