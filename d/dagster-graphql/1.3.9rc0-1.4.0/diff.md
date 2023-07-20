# Comparing `tmp/dagster-graphql-1.3.9rc0.tar.gz` & `tmp/dagster-graphql-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.9rc0.tar", last modified: Thu Jun  8 18:27:41 2023, max compression
+gzip compressed data, was "dagster-graphql-1.4.0.tar", last modified: Thu Jul 20 21:54:05 2023, max compression
```

## Comparing `dagster-graphql-1.3.9rc0.tar` & `dagster-graphql-1.4.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.886160 dagster-graphql-1.3.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:27:41.886160 dagster-graphql-1.3.9rc0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.818159 dagster-graphql-1.3.9rc0/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.822159 dagster-graphql-1.3.9rc0/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17963 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.838159 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.838159 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11422 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25777 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12470 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.862160 dagster-graphql-1.3.9rc0/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40571 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     8183 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16867 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6708 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.866160 dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.878160 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39668 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.882160 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    26830 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    37813 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.886160 dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.886160 dagster-graphql-1.3.9rc0/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:41.818159 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4286 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:27:41.000000 dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-08 18:27:41.890160 dagster-graphql-1.3.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-08 18:20:45.000000 dagster-graphql-1.3.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.555195 dagster-graphql-1.4.0/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.555195 dagster-graphql-1.4.0/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17963 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.559195 dagster-graphql-1.4.0/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.559195 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11422 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25530 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12589 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.567195 dagster-graphql-1.4.0/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40455 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     8466 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.567195 dagster-graphql-1.4.0/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.567195 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11058 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39668 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    26779 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37803 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:05.555195 dagster-graphql-1.4.0/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 21:54:05.000000 dagster-graphql-1.4.0/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-20 21:54:05.571195 dagster-graphql-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-20 21:53:15.000000 dagster-graphql-1.4.0/setup.py
```

### Comparing `dagster-graphql-1.3.9rc0/LICENSE` & `dagster-graphql-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/PKG-INFO` & `dagster-graphql-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.9rc0
+Version: 1.4.0
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/cli.py` & `dagster-graphql-1.4.0/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/client/client.py` & `dagster-graphql-1.4.0/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.4.0/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/client/query.py` & `dagster-graphql-1.4.0/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/client/utils.py` & `dagster-graphql-1.4.0/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/events.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Union, cast
+from typing import TYPE_CHECKING, List, Optional, Sequence, Union, cast
 
 import dagster._check as check
 import pendulum
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.selector import RepositorySelector
 from dagster._core.errors import DagsterError, DagsterUserCodeProcessError
 from dagster._core.events import AssetKey
@@ -27,19 +27,28 @@
         GrapheneLaunchBackfillSuccess,
         GrapheneResumeBackfillSuccess,
     )
     from ...schema.errors import GraphenePartitionSetNotFoundError
 
 
 def _assert_permission_for_asset_graph(
-    graphene_info: "ResolveInfo", asset_graph: ExternalAssetGraph, permission: str
+    graphene_info: "ResolveInfo",
+    asset_graph: ExternalAssetGraph,
+    asset_selection: Optional[Sequence[AssetKey]],
+    permission: str,
 ) -> None:
+    if asset_selection:
+        repo_handles = [
+            asset_graph.get_repository_handle(asset_key) for asset_key in asset_selection
+        ]
+    else:
+        repo_handles = asset_graph.repository_handles_by_key.values()
+
     location_names = set(
-        repo_handle.code_location_origin.location_name
-        for repo_handle in asset_graph.repository_handles_by_key.values()
+        repo_handle.code_location_origin.location_name for repo_handle in repo_handles
     )
 
     if not location_names:
         assert_permission(
             graphene_info,
             permission,
         )
@@ -150,27 +159,30 @@
                 "forceSynchronousSubmission is not supported for pure asset backfills"
             )
 
         if backfill_params.get("fromFailure"):
             raise DagsterError("fromFailure is not supported for pure asset backfills")
 
         asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+
         _assert_permission_for_asset_graph(
-            graphene_info, asset_graph, Permissions.LAUNCH_PARTITION_BACKFILL
+            graphene_info, asset_graph, asset_selection, Permissions.LAUNCH_PARTITION_BACKFILL
         )
 
         backfill = PartitionBackfill.from_asset_partitions(
             asset_graph=asset_graph,
             backfill_id=backfill_id,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
             partition_names=backfill_params.get("partitionNames"),
             dynamic_partitions_store=CachingInstanceQueryer(
-                graphene_info.context.instance, utc_datetime_from_timestamp(backfill_timestamp)
+                graphene_info.context.instance,
+                asset_graph,
+                utc_datetime_from_timestamp(backfill_timestamp),
             ),
             all_partitions=backfill_params.get("allPartitions", False),
         )
     else:
         raise DagsterError(
             "Backfill requested without specifying partition set selector or asset selection"
         )
@@ -187,15 +199,18 @@
     backfill = graphene_info.context.instance.get_backfill(backfill_id)
     if not backfill:
         check.failed(f"No backfill found for id: {backfill_id}")
 
     if backfill.serialized_asset_backfill_data:
         asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
         _assert_permission_for_asset_graph(
-            graphene_info, asset_graph, Permissions.CANCEL_PARTITION_BACKFILL
+            graphene_info,
+            asset_graph,
+            backfill.asset_selection,
+            Permissions.CANCEL_PARTITION_BACKFILL,
         )
         graphene_info.context.instance.update_backfill(
             backfill.with_status(BulkActionStatus.CANCELING)
         )
 
     else:
         partition_set_origin = check.not_none(backfill.partition_set_origin)
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/external.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,20 +289,14 @@
             after_timestamp=after_timestamp,
         ),
         limit=limit,
     )
     return [event_record.event_log_entry for event_record in event_records]
 
 
-def get_asset_run_ids(graphene_info: "ResolveInfo", asset_key: AssetKey) -> Sequence[str]:
-    check.inst_param(asset_key, "asset_key", AssetKey)
-    instance = graphene_info.context.instance
-    return instance.run_ids_for_asset_key(asset_key)
-
-
 def get_assets_for_run_id(graphene_info: "ResolveInfo", run_id: str) -> Sequence["GrapheneAsset"]:
     from ..schema.pipelines.pipeline import GrapheneAsset
 
     check.str_param(run_id, "run_id")
 
     records = graphene_info.context.instance.all_logs(run_id, of_type=ASSET_EVENTS)
     asset_keys = set(
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ExternalPartitionSet,
     RepositoryHandle,
 )
 from dagster._core.host_representation.external_data import (
     ExternalPartitionExecutionErrorData,
     ExternalPartitionNamesData,
 )
-from dagster._core.storage.dagster_run import RunPartitionData, RunsFilter
+from dagster._core.storage.dagster_run import DagsterRunStatus, RunPartitionData, RunsFilter
 from dagster._core.storage.tags import (
     PARTITION_NAME_TAG,
     PARTITION_SET_TAG,
     REPOSITORY_LABEL_TAG,
     TagType,
     get_tag_type,
 )
@@ -225,14 +225,15 @@
     check.inst_param(external_partition_set, "external_partition_set", ExternalPartitionSet)
 
     repository_handle = external_partition_set.repository_handle
     partition_set_name = external_partition_set.name
 
     run_partition_data = graphene_info.context.instance.run_storage.get_run_partition_data(
         runs_filter=RunsFilter(
+            statuses=[status for status in DagsterRunStatus if status != DagsterRunStatus.CANCELED],
             tags={
                 PARTITION_SET_TAG: partition_set_name,
                 REPOSITORY_LABEL_TAG: repository_handle.get_external_origin().get_label(),
             },
         )
     )
     names_result = graphene_info.context.get_external_partition_names(
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.4.0/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import graphene
 
-from .roots.mutation import GrapheneDagitMutation
-from .roots.query import GrapheneDagitQuery
-from .roots.subscription import GrapheneDagitSubscription
+from .roots.mutation import GrapheneMutation
+from .roots.query import GrapheneQuery
+from .roots.subscription import GrapheneSubscription
 
 
 def types():
     from .asset_key import GrapheneAssetKey
     from .backfill import GrapheneLaunchBackfillResult, GrapheneLaunchBackfillSuccess
     from .config_type_or_error import GrapheneConfigTypeOrError
     from .config_types import types as config_types
@@ -66,12 +66,12 @@
         + [GraphenePipelineTag, GraphenePipelineTagAndValues]
         + [GrapheneNodeInvocationSite, GrapheneUsedSolid]
     )
 
 
 def create_schema() -> graphene.Schema:
     return graphene.Schema(
-        query=GrapheneDagitQuery,
-        mutation=GrapheneDagitMutation,
-        subscription=GrapheneDagitSubscription,
+        query=GrapheneQuery,
+        mutation=GrapheneMutation,
+        subscription=GrapheneSubscription,
         types=types(),
     )
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,18 +453,18 @@
 
         instance = graphene_info.context.instance
         asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
         asset_key = self._external_asset_node.asset_key
 
         # in the future, we can share this same CachingInstanceQueryer across all
         # GrapheneMaterializationEvent which share an external repository for improved performance
-        instance_queryer = CachingInstanceQueryer(instance=graphene_info.context.instance)
-        data_time_resolver = CachingDataTimeResolver(
-            instance_queryer=instance_queryer, asset_graph=asset_graph
+        instance_queryer = CachingInstanceQueryer(
+            instance=graphene_info.context.instance, asset_graph=asset_graph
         )
+        data_time_resolver = CachingDataTimeResolver(instance_queryer=instance_queryer)
         event_records = instance.get_event_records(
             EventRecordsFilter(
                 event_type=DagsterEventType.ASSET_MATERIALIZATION,
                 before_timestamp=int(timestampMillis) / 1000.0 + 1,
                 after_timestamp=int(timestampMillis) / 1000.0 - 1,
                 asset_key=asset_key,
             ),
@@ -687,17 +687,17 @@
             asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
             return get_freshness_info(
                 asset_key=self._external_asset_node.asset_key,
                 # in the future, we can share this same CachingInstanceQueryer across all
                 # GrapheneAssetNodes which share an external repository for improved performance
                 data_time_resolver=CachingDataTimeResolver(
                     instance_queryer=CachingInstanceQueryer(
-                        instance=graphene_info.context.instance
+                        instance=graphene_info.context.instance,
+                        asset_graph=asset_graph,
                     ),
-                    asset_graph=asset_graph,
                 ),
             )
         return None
 
     def resolve_freshnessPolicy(
         self, _graphene_info: ResolveInfo
     ) -> Optional[GrapheneFreshnessPolicy]:
@@ -847,25 +847,20 @@
                 materialized_partition_subset is None
                 or failed_partition_subset is None
                 or in_progress_subset is None
             ):
                 check.failed("Expected partitions subset for a partitioned asset")
 
             failed_keys = failed_partition_subset.get_partition_keys()
+            in_progress_keys = in_progress_subset.get_partition_keys()
+            failed_and_in_progress_keys = {*failed_keys, *in_progress_keys}
 
-            num_materialized_and_not_failed = len(materialized_partition_subset) - len(
-                [k for k in failed_keys if k in materialized_partition_subset]
-            )
-            num_materialized_and_not_failed_or_in_progress = num_materialized_and_not_failed - len(
-                [
-                    k
-                    for k in in_progress_subset.get_partition_keys()
-                    if k in materialized_partition_subset
-                ]
-            )
+            num_materialized_and_not_failed_or_in_progress = len(
+                materialized_partition_subset
+            ) - len([k for k in failed_and_in_progress_keys if k in materialized_partition_subset])
 
             num_failed_and_not_in_progress = len(
                 [k for k in failed_keys if k not in in_progress_subset]
             )
 
             return GraphenePartitionStats(
                 numMaterialized=num_materialized_and_not_failed_or_in_progress,
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ParentOutdatedAutoMaterializeCondition,
 )
 from dagster._core.definitions.partition import SerializedPartitionsSubset
 from dagster._core.scheduler.instigation import AutoMaterializeAssetEvaluationRecord
 
 from dagster_graphql.schema.errors import GrapheneError
 
+from .asset_key import GrapheneAssetKey
 from .util import non_null_list
 
 GrapheneAutoMaterializeDecisionType = graphene.Enum.from_enum(AutoMaterializeDecisionType)
 
 
 class GraphenePartitionKeys(graphene.ObjectType):
     partitionKeys = non_null_list(graphene.String)
@@ -73,14 +74,16 @@
 class GrapheneMissingAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
         name = "MissingAutoMaterializeCondition"
         interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
 
 
 class GrapheneParentOutdatedAutoMaterializeCondition(graphene.ObjectType):
+    waitingOnAssetKeys = graphene.List(graphene.NonNull(GrapheneAssetKey))
+
     class Meta:
         name = "ParentOutdatedAutoMaterializeCondition"
         interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
 
 
 class GrapheneMaxMaterializationsExceededAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
@@ -138,15 +141,17 @@
         )
     elif isinstance(condition, MissingAutoMaterializeCondition):
         return GrapheneMissingAutoMaterializeCondition(
             decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     elif isinstance(condition, ParentOutdatedAutoMaterializeCondition):
         return GrapheneParentOutdatedAutoMaterializeCondition(
-            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
+            decisionType=condition.decision_type,
+            partitionKeysOrError=partition_keys_or_error,
+            waitingOnAssetKeys=condition.waiting_on_asset_keys,
         )
     elif isinstance(condition, MaxMaterializationsExceededAutoMaterializeCondition):
         return GrapheneMaxMaterializationsExceededAutoMaterializeCondition(
             decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     else:
         check.failed(f"Unexpected condition type {type(condition)}")
@@ -156,14 +161,15 @@
     id = graphene.NonNull(graphene.ID)
     evaluationId = graphene.NonNull(graphene.Int)
     numRequested = graphene.NonNull(graphene.Int)
     numSkipped = graphene.NonNull(graphene.Int)
     numDiscarded = graphene.NonNull(graphene.Int)
     conditions = non_null_list(GrapheneAutoMaterializeCondition)
     timestamp = graphene.NonNull(graphene.Float)
+    runIds = non_null_list(graphene.String)
 
     class Meta:
         name = "AutoMaterializeAssetEvaluationRecord"
 
     def __init__(
         self,
         record: AutoMaterializeAssetEvaluationRecord,
@@ -176,14 +182,15 @@
             numSkipped=record.evaluation.num_skipped,
             numDiscarded=record.evaluation.num_discarded,
             conditions=[
                 create_graphene_auto_materialize_condition(c, partitions_def)
                 for c in record.evaluation.partition_subsets_by_condition
             ],
             timestamp=record.timestamp,
+            runIds=record.evaluation.run_ids,
         )
 
 
 class GrapheneAutoMaterializeAssetEvaluationRecords(graphene.ObjectType):
     records = non_null_list(GrapheneAutoMaterializeAssetEvaluationRecord)
     currentEvaluationId = graphene.Int()
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/errors.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/execution.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/external.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/instance.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 message=error.message,
                 path=[],  # TODO: remove
                 stack=GrapheneEvaluationStack(config_schema_snapshot, error.stack),
                 reason=error.reason.value,
                 incoming_fields=error.error_data.incoming_fields,
             )
         else:
-            check.failed(f"Error type not supported {repr(error.error_data)}")
+            check.failed(f"Error type not supported {error.error_data!r}")
 
 
 class GrapheneRuntimeMismatchConfigError(graphene.ObjectType):
     value_rep = graphene.Field(graphene.String)
 
     class Meta:
         interfaces = (GraphenePipelineConfigValidationError,)
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/resources.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,41 +744,41 @@
     @capture_error
     @check_permission(Permissions.EDIT_CONCURRENCY_LIMIT)
     def mutate(self, graphene_info, runId: str):
         graphene_info.context.instance.event_log_storage.free_concurrency_slots_for_run(runId)
         return True
 
 
-class GrapheneDagitMutation(graphene.ObjectType):
+class GrapheneMutation(graphene.ObjectType):
     """The root for all mutations to modify data in your Dagster instance."""
 
     class Meta:
-        name = "DagitMutation"
+        name = "Mutation"
 
-    launch_pipeline_execution = GrapheneLaunchRunMutation.Field()
-    launch_run = GrapheneLaunchRunMutation.Field()
-    launch_pipeline_reexecution = GrapheneLaunchRunReexecutionMutation.Field()
-    launch_run_reexecution = GrapheneLaunchRunReexecutionMutation.Field()
-    start_schedule = GrapheneStartScheduleMutation.Field()
-    stop_running_schedule = GrapheneStopRunningScheduleMutation.Field()
-    start_sensor = GrapheneStartSensorMutation.Field()
-    set_sensor_cursor = GrapheneSetSensorCursorMutation.Field()
-    stop_sensor = GrapheneStopSensorMutation.Field()
-    sensor_dry_run = GrapheneSensorDryRunMutation.Field()
-    schedule_dry_run = GrapheneScheduleDryRunMutation.Field()
-    terminate_pipeline_execution = GrapheneTerminateRunMutation.Field()
-    terminate_run = GrapheneTerminateRunMutation.Field()
-    delete_pipeline_run = GrapheneDeleteRunMutation.Field()
-    delete_run = GrapheneDeleteRunMutation.Field()
-    reload_repository_location = GrapheneReloadRepositoryLocationMutation.Field()
-    reload_workspace = GrapheneReloadWorkspaceMutation.Field()
-    shutdown_repository_location = GrapheneShutdownRepositoryLocationMutation.Field()
-    wipe_assets = GrapheneAssetWipeMutation.Field()
-    launch_partition_backfill = GrapheneLaunchBackfillMutation.Field()
-    resume_partition_backfill = GrapheneResumeBackfillMutation.Field()
-    cancel_partition_backfill = GrapheneCancelBackfillMutation.Field()
-    log_telemetry = GrapheneLogTelemetryMutation.Field()
-    set_nux_seen = GrapheneSetNuxSeenMutation.Field()
-    add_dynamic_partition = GrapheneAddDynamicPartitionMutation.Field()
+    launchPipelineExecution = GrapheneLaunchRunMutation.Field()
+    launchRun = GrapheneLaunchRunMutation.Field()
+    launchPipelineReexecution = GrapheneLaunchRunReexecutionMutation.Field()
+    launchRunReexecution = GrapheneLaunchRunReexecutionMutation.Field()
+    startSchedule = GrapheneStartScheduleMutation.Field()
+    stopRunningSchedule = GrapheneStopRunningScheduleMutation.Field()
+    startSensor = GrapheneStartSensorMutation.Field()
+    setSensorCursor = GrapheneSetSensorCursorMutation.Field()
+    stopSensor = GrapheneStopSensorMutation.Field()
+    sensorDryRun = GrapheneSensorDryRunMutation.Field()
+    scheduleDryRun = GrapheneScheduleDryRunMutation.Field()
+    terminatePipelineExecution = GrapheneTerminateRunMutation.Field()
+    terminateRun = GrapheneTerminateRunMutation.Field()
+    deletePipelineRun = GrapheneDeleteRunMutation.Field()
+    deleteRun = GrapheneDeleteRunMutation.Field()
+    reloadRepositoryLocation = GrapheneReloadRepositoryLocationMutation.Field()
+    reloadWorkspace = GrapheneReloadWorkspaceMutation.Field()
+    shutdownRepositoryLocation = GrapheneShutdownRepositoryLocationMutation.Field()
+    wipeAssets = GrapheneAssetWipeMutation.Field()
+    launchPartitionBackfill = GrapheneLaunchBackfillMutation.Field()
+    resumePartitionBackfill = GrapheneResumeBackfillMutation.Field()
+    cancelPartitionBackfill = GrapheneCancelBackfillMutation.Field()
+    logTelemetry = GrapheneLogTelemetryMutation.Field()
+    setNuxSeen = GrapheneSetNuxSeenMutation.Field()
+    addDynamicPartition = GrapheneAddDynamicPartitionMutation.Field()
     setAutoMaterializePaused = GrapheneSetAutoMaterializePausedMutation.Field()
     setConcurrencyLimit = GrapheneSetConcurrencyLimitMutation.Field()
     freeConcurrencySlotsForRun = GrapheneFreeConcurrencySlotsForRunMutation.Field()
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,19 +147,19 @@
 from ..test import GrapheneTestFields
 from ..util import ResolveInfo, get_compute_log_manager, non_null_list
 from .assets import GrapheneAssetOrError, GrapheneAssetsOrError
 from .execution_plan import GrapheneExecutionPlanOrError
 from .pipeline import GrapheneGraphOrError, GraphenePipelineOrError
 
 
-class GrapheneDagitQuery(graphene.ObjectType):
+class GrapheneQuery(graphene.ObjectType):
     """The root for all queries to retrieve data from the Dagster instance."""
 
     class Meta:
-        name = "DagitQuery"
+        name = "Query"
 
     version = graphene.Field(
         graphene.NonNull(graphene.String),
         description="Retrieve the version of Dagster running in the Dagster deployment.",
     )
 
     repositoriesOrError = graphene.Field(
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/roots/subscription.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from ...implementation.execution import gen_captured_log_data, gen_compute_logs, gen_events_for_run
 from ..external import GrapheneLocationStateChangeSubscription, gen_location_state_changes
 from ..logs.compute_logs import GrapheneCapturedLogs, GrapheneComputeIOType, GrapheneComputeLogFile
 from ..pipelines.subscription import GraphenePipelineRunLogsSubscriptionPayload
 from ..util import ResolveInfo, non_null_list
 
 
-class GrapheneDagitSubscription(graphene.ObjectType):
+class GrapheneSubscription(graphene.ObjectType):
     """The root for all subscriptions to retrieve real-time data from the Dagster instance."""
 
     class Meta:
-        name = "DagitSubscription"
+        name = "Subscription"
 
     pipelineRunLogs = graphene.Field(
         graphene.NonNull(GraphenePipelineRunLogsSubscriptionPayload),
         runId=graphene.Argument(graphene.NonNull(graphene.ID)),
         cursor=graphene.Argument(
             graphene.String,
             description=(
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/runs.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/solids.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/table.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/tags.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/schema/util.py` & `dagster-graphql-1.4.0/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql/test/utils.py` & `dagster-graphql-1.4.0/dagster_graphql/test/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,22 +98,34 @@
     result = execute_dagster_graphql(context, query, variables)
     wait_for_runs_to_finish(context.instance, timeout=30)
     return result
 
 
 @contextmanager
 def define_out_of_process_context(
-    python_file: str, fn_name: str, instance: DagsterInstance, read_only: bool = False
+    python_file: str,
+    fn_name: str,
+    instance: DagsterInstance,
+    read_only: bool = False,
+    read_only_locations: Optional[Mapping[str, bool]] = None,
 ) -> Iterator[WorkspaceRequestContext]:
     check.inst_param(instance, "instance", DagsterInstance)
 
     with define_out_of_process_workspace(
         python_file, fn_name, instance, read_only=read_only
     ) as workspace_process_context:
-        yield workspace_process_context.create_request_context()
+        yield WorkspaceRequestContext(
+            instance=instance,
+            workspace_snapshot=workspace_process_context.create_snapshot(),
+            process_context=workspace_process_context,
+            version=workspace_process_context.version,
+            source=None,
+            read_only=read_only,
+            read_only_locations=read_only_locations,
+        )
 
 
 def define_out_of_process_workspace(
     python_file: str, fn_name: str, instance: DagsterInstance, read_only: bool = False
 ) -> WorkspaceProcessContext:
     return WorkspaceProcessContext(
         instance,
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.4.0/dagster_graphql.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.9rc0
+Version: 1.4.0
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-graphql-1.3.9rc0/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.4.0/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.9rc0/setup.py` & `dagster-graphql-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="The GraphQL frontend to python dagster.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
+    include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
+        "dagster==1.4.0",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

