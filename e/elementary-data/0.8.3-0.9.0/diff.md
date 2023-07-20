# Comparing `tmp/elementary-data-0.8.3.tar.gz` & `tmp/elementary-data-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-p06fmgba/elementary-data-0.8.3.tar", last modified: Wed Jul 19 06:31:48 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-liqejza_/elementary-data-0.9.0.tar", last modified: Thu Jul 20 09:11:04 2023, max compression
```

## Comparing `elementary-data-0.8.3.tar` & `elementary-data-0.9.0.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-07-19 06:31:32.000000 elementary-data-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-07-19 06:31:32.000000 elementary-data-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-19 06:31:48.000000 elementary-data-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-07-19 06:31:32.000000 elementary-data-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/dbt/dbt_log.py
--rw-r--r--   0 runner    (1001) docker     (122)     8424 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7780 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8288 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8170 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5214 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    13504 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6275 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     8053 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4252 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/groups/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/groups/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10013 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7891 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    20989 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/api/totals_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    19950 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7919 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10595 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11902 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1791216 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/owners.sql
--rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/resources.sql
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/tags.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/tests.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/internal_tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/nothing.sql
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/test_conn.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/tests/unique_if_exists.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/elementary.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/update_alerts/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5214 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8086 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/operations/upload_source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4598 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-07-19 06:31:32.000000 elementary-data-0.8.3/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-19 06:31:48.000000 elementary-data-0.8.3/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 06:31:48.000000 elementary-data-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-07-19 06:31:32.000000 elementary-data-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12751 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7342 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:48.000000 elementary-data-0.8.3/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-19 06:31:32.000000 elementary-data-0.8.3/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-07-20 09:10:49.000000 elementary-data-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-07-20 09:10:49.000000 elementary-data-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-20 09:11:04.000000 elementary-data-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-07-20 09:10:49.000000 elementary-data-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/dbt/dbt_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8424 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7780 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8288 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8170 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5214 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13504 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6275 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8747 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4252 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/groups/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/groups/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10013 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7891 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20989 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/api/totals_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20226 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7919 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10695 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11902 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1791216 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/owners.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/resources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/tags.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/tests.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/internal_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/nothing.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/test_conn.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/tests/unique_if_exists.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/elementary.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/update_alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8086 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/operations/upload_source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4598 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-07-20 09:10:49.000000 elementary-data-0.9.0/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-20 09:11:04.000000 elementary-data-0.9.0/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 09:11:04.000000 elementary-data-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-07-20 09:10:49.000000 elementary-data-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12751 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7342 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:11:04.000000 elementary-data-0.9.0/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-20 09:10:50.000000 elementary-data-0.9.0/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.8.3/LICENSE` & `elementary-data-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/PKG-INFO` & `elementary-data-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.8.3
+Version: 0.9.0
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.8.3 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.9.0 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.8.3/README.md` & `elementary-data-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/cli/cli.py` & `elementary-data-0.9.0/elementary/cli/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/cli/upgrade.py` & `elementary-data-0.9.0/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.9.0/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/dbt/dbt_log.py` & `elementary-data-0.9.0/elementary/clients/dbt/dbt_log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.9.0/elementary/clients/dbt/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.9.0/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/gcs/client.py` & `elementary-data-0.9.0/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/s3/client.py` & `elementary-data-0.9.0/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/slack/client.py` & `elementary-data-0.9.0/elementary/clients/slack/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/slack/schema.py` & `elementary-data-0.9.0/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.9.0/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/config/config.py` & `elementary-data-0.9.0/elementary/config/config.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/exceptions/exceptions.py` & `elementary-data-0.9.0/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/alert.py` & `elementary-data-0.9.0/elementary/monitor/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/alerts.py` & `elementary-data-0.9.0/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.9.0/elementary/monitor/alerts/group_of_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/malformed.py` & `elementary-data-0.9.0/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/model.py` & `elementary-data-0.9.0/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.9.0/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/alerts/test.py` & `elementary-data-0.9.0/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.9.0/elementary/monitor/api/alerts/alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.9.0/elementary/monitor/api/alerts/alerts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 from datetime import datetime
-from typing import DefaultDict, Dict, List, Sequence, Union
+from typing import DefaultDict, Dict, List, Optional, Sequence, Union
 
 from elementary.clients.api.api_client import APIClient
 from elementary.clients.dbt.dbt_runner import DbtRunner
 from elementary.config.config import Config
 from elementary.monitor.alerts.alert import Alert, AlertType
 from elementary.monitor.alerts.alerts import Alerts, AlertsQueryResult
 from elementary.monitor.alerts.malformed import MalformedAlert
@@ -14,30 +14,34 @@
 from elementary.monitor.api.alerts.alert_filters import filter_alerts
 from elementary.monitor.data_monitoring.schema import SelectorFilterSchema
 from elementary.monitor.fetchers.alerts.alerts import AlertsFetcher
 from elementary.utils.log import get_logger
 
 logger = get_logger(__name__)
 
+DEFAULT_ALERT_SUPPRESSION_INTERVAL_HOURS = 24
+
 
 class AlertsAPI(APIClient):
     def __init__(
         self,
         dbt_runner: DbtRunner,
         config: Config,
         elementary_database_and_schema: str,
+        global_suppression_interval: Optional[int] = None,
     ):
         super().__init__(dbt_runner)
         self.config = config
         self.elementary_database_and_schema = elementary_database_and_schema
         self.alerts_fetcher = AlertsFetcher(
             dbt_runner=self.dbt_runner,
             config=self.config,
             elementary_database_and_schema=self.elementary_database_and_schema,
         )
+        self.global_suppression_interval = global_suppression_interval
 
     def get_new_alerts(
         self,
         days_back: int,
         disable_samples: bool = False,
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> Alerts:
@@ -112,15 +116,15 @@
     def _sort_alerts(
         self,
         pending_alerts: AlertsQueryResult[AlertType],
         last_alert_sent_times: Dict[str, str],
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> AlertsQueryResult[AlertType]:
         suppressed_alerts = self._get_suppressed_alerts(
-            pending_alerts, last_alert_sent_times
+            pending_alerts, last_alert_sent_times, self.global_suppression_interval
         )
         latest_alert_ids = self._get_latest_alerts(pending_alerts)
         alerts_to_skip: List[Union[AlertType, MalformedAlert]] = []
         alerts_to_send: List[AlertType] = []
         malformed_alerts_to_send: List[MalformedAlert] = []
 
         for valid_alert in pending_alerts.alerts:
@@ -143,30 +147,34 @@
 
         return AlertsQueryResult(
             alerts=filter_alerts(alerts_to_send, filter),
             malformed_alerts=filter_alerts(malformed_alerts_to_send, filter),
             alerts_to_skip=filter_alerts(alerts_to_skip, filter),
         )
 
-    @staticmethod
+    @classmethod
     def _get_suppressed_alerts(
+        cls,
         alerts: AlertsQueryResult[AlertType],
         last_alert_sent_times: Dict[str, str],
+        global_suppression_interval: Optional[int] = None,
     ) -> List[str]:
         suppressed_alerts = []
         current_time_utc = datetime.utcnow()
         all_alerts: List[Alert] = [*alerts.alerts, *alerts.malformed_alerts]
         for alert in all_alerts:
             alert_class_id = alert.alert_class_id
             if alert_class_id is None:
                 # Shouldn't happen, but logging in any case
                 logger.debug("Alert without an id detected!")
                 continue
 
-            suppression_interval = alert.alert_suppression_interval
+            suppression_interval = cls._get_suppression_interval(
+                alert.alert_suppression_interval, global_suppression_interval
+            )
             last_sent_time = (
                 datetime.fromisoformat(last_alert_sent_times[alert_class_id])
                 if last_alert_sent_times.get(alert_class_id)
                 else None
             )
             is_alert_in_suppression = (
                 (current_time_utc - last_sent_time).total_seconds() / 3600
@@ -202,7 +210,15 @@
                 alert_last_times[alert_class_id] = dict(
                     alert_id=alert.id, detected_at=alert_detected_at
                 )
 
         for alert_last_time in alert_last_times.values():
             latest_alert_ids.append(alert_last_time["alert_id"])
         return latest_alert_ids
+
+    @staticmethod
+    def _get_suppression_interval(interval_from_alert, interval_from_cli):
+        if interval_from_alert is not None:
+            return interval_from_alert
+        if interval_from_cli is not None:
+            return interval_from_cli
+        return DEFAULT_ALERT_SUPPRESSION_INTERVAL_HOURS
```

### Comparing `elementary-data-0.8.3/elementary/monitor/api/filters/filters.py` & `elementary-data-0.9.0/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/filters/schema.py` & `elementary-data-0.9.0/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/groups/groups.py` & `elementary-data-0.9.0/elementary/monitor/api/groups/groups.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.9.0/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.9.0/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.9.0/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/models/models.py` & `elementary-data-0.9.0/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/models/schema.py` & `elementary-data-0.9.0/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/report/report.py` & `elementary-data-0.9.0/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/report/schema.py` & `elementary-data-0.9.0/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/selector/selector.py` & `elementary-data-0.9.0/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/test_management/test_management.py` & `elementary-data-0.9.0/elementary/monitor/api/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/tests/schema.py` & `elementary-data-0.9.0/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/tests/tests.py` & `elementary-data-0.9.0/elementary/monitor/api/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/api/totals_schema.py` & `elementary-data-0.9.0/elementary/monitor/api/totals_schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/cli.py` & `elementary-data-0.9.0/elementary/monitor/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,20 @@
 @click.option(
     "--test",
     type=bool,
     default=False,
     help="Whether to send a test message in case there are no alerts.",
 )
 @click.option(
+    "--suppression-interval",
+    type=int,
+    default=24,
+    help="The number of hours to suppress alerts after an alert was sent (this is a global default setting).",
+)
+@click.option(
     "--group-by",
     type=click.Choice(["alert", "table"]),
     default=None,
     help="Whether to group alerts by 'alert' or by 'table'",
 )
 @click.pass_context
 def monitor(
@@ -240,14 +246,15 @@
     dbt_vars,
     test,
     disable_samples,
     env,
     select,
     group_by,
     target_path,
+    suppression_interval,
 ):
     """
     Get alerts on failures in dbt jobs.
     """
     if ctx.invoked_subcommand is not None:
         return
     if deprecated_slack_webhook is not None:
@@ -280,17 +287,18 @@
         data_monitoring = DataMonitoringAlerts(
             config=config,
             tracking=anonymous_tracking,
             force_update_dbt_package=update_dbt_package,
             send_test_message_on_success=test,
             disable_samples=disable_samples,
             filter=select,
+            global_suppression_interval=suppression_interval,
         )
-        # The call to track_cli_start must be after the constructor of DataMonitoringAlerts as it enriches the tracking properties.
-        # This is a tech-debt that should be fixed in the future.
+        # The call to track_cli_start must be after the constructor of DataMonitoringAlerts as it enriches the tracking
+        # properties. This is a tech-debt that should be fixed in the future.
         anonymous_tracking.track_cli_start(
             Command.MONITOR, get_cli_properties(), ctx.command.name
         )
         success = data_monitoring.run_alerts(
             days_back, full_refresh_dbt_package, dbt_vars=vars
         )
         anonymous_tracking.track_cli_end(
```

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,25 @@
         self,
         config: Config,
         tracking: Optional[Tracking] = None,
         filter: Optional[str] = None,
         force_update_dbt_package: bool = False,
         disable_samples: bool = False,
         send_test_message_on_success: bool = False,
+        global_suppression_interval: Optional[int] = None,
     ):
         super().__init__(
             config, tracking, force_update_dbt_package, disable_samples, filter
         )
 
         self.alerts_api = AlertsAPI(
             self.internal_dbt_runner,
             self.config,
             self.elementary_database_and_schema,
+            global_suppression_interval,
         )
         self.sent_alert_count = 0
         self.send_test_message_on_success = send_test_message_on_success
 
         if self.slack_client is None:
             raise Exception("Could not initialize slack client!")
```

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.9.0/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/README.md` & `elementary-data-0.9.0/elementary/monitor/dbt_project/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.9.0/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/owners.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/owners.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/resources.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/resources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/tags.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/tags.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/base_queries/tests.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/base_queries/tests.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.9.0/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project/models/elementary.yml` & `elementary-data-0.9.0/elementary/monitor/dbt_project/models/elementary.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.9.0/elementary/monitor/dbt_project_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/debug.py` & `elementary-data-0.9.0/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,24 +124,28 @@
         elif isinstance(model_attrs, str):
             attrs.append(model_attrs)
         return attrs
 
     def _get_alert_channel(self) -> Optional[str]:
         return self._get_field_from_test_meta_or_model_meta_or_default(key=CHANNEL_KEY)
 
-    def _get_alert_suppression_interval(self) -> int:
+    def _get_alert_suppression_interval(self) -> Optional[int]:
         return self._get_field_from_test_meta_or_model_meta_or_default(
-            key=ALERT_SUPRESSION_INTERVAL_KEY, default_val=0
+            key=ALERT_SUPRESSION_INTERVAL_KEY, default_val=None
         )
 
     def _get_alert_fields(self) -> Optional[List[str]]:
         # If there is no alerts_fields in the test meta object,
         # we return the model alerts_fields from the model meta object.
         # The fallback is DEFAULT_ALERT_FIELDS.
         return self._get_field_from_test_meta_or_model_meta_or_default(
             key=ALERT_FIELDS_KEY, default_val=DEFAULT_ALERT_FIELDS
         )
 
     def _get_field_from_test_meta_or_model_meta_or_default(
         self, key: str, default_val=None
     ) -> Any:
-        return self.test_meta.get(key) or self.model_meta.get(key) or default_val
+        if self.test_meta.get(key) is not None:
+            return self.test_meta.get(key)
+        if self.model_meta.get(key) is not None:
+            return self.model_meta.get(key)
+        return default_val
```

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/models/schema.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/test_management/schema.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/test_management/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/test_management/test_management.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.9.0/elementary/monitor/fetchers/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/operations/cli.py` & `elementary-data-0.9.0/elementary/operations/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/operations/upload_source_freshness.py` & `elementary-data-0.9.0/elementary/operations/upload_source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.9.0/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/tracking/runner.py` & `elementary-data-0.9.0/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/tracking/tracking_interface.py` & `elementary-data-0.9.0/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/cli_utils.py` & `elementary-data-0.9.0/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/json_utils.py` & `elementary-data-0.9.0/elementary/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/log.py` & `elementary-data-0.9.0/elementary/utils/log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/ordered_yaml.py` & `elementary-data-0.9.0/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/schema.py` & `elementary-data-0.9.0/elementary/utils/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary/utils/time.py` & `elementary-data-0.9.0/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.9.0/elementary_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.8.3
+Version: 0.9.0
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.8.3 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.9.0 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.8.3/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.9.0/elementary_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/elementary_data.egg-info/requires.txt` & `elementary-data-0.9.0/elementary_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/setup.py` & `elementary-data-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
 }
 
 
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.8.3",
+    version="0.9.0",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
```

### Comparing `elementary-data-0.8.3/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.9.0/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.9.0/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.9.0/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.9.0/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.9.0/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.9.0/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/group_alerts_by_table/utils.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/group_alerts_by_table/utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
     # No interval
     alert = dict(
         test_meta=json.dumps(dict()),
         model_meta=json.dumps(dict()),
     )
     normalized_alert = NormalizedAlert(alert)
-    assert normalized_alert._get_alert_suppression_interval() == 0
+    assert normalized_alert._get_alert_suppression_interval() is None
 
 
 def test_get_alert_fields():
     # Alert fields both for the test and the model
     alert = {
         TEST_META_KEY: json.dumps(
             {
```

### Comparing `elementary-data-0.8.3/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.9.0/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.9.0/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.9.0/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.9.0/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.9.0/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.3/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.9.0/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*

