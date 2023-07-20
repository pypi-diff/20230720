# Comparing `tmp/toucan_connectors-4.7.1.tar.gz` & `tmp/toucan_connectors-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-4.7.1.tar", max compression
+gzip compressed data, was "toucan_connectors-4.7.2.tar", max compression
```

## Comparing `toucan_connectors-4.7.1.tar` & `toucan_connectors-4.7.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1510 2023-07-19 09:02:51.110257 toucan_connectors-4.7.1/LICENSE
--rw-r--r--   0        0        0     9969 2023-07-19 09:02:51.110257 toucan_connectors-4.7.1/README.md
--rw-r--r--   0        0        0     5594 2023-07-19 09:02:51.118258 toucan_connectors-4.7.1/pyproject.toml
--rw-r--r--   0        0        0    10795 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/adobe_analytics/__init__.py
--rw-r--r--   0        0        0    13648 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/adobe_analytics/adobe-analytics.png
--rw-r--r--   0        0        0     1740 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/anaplan/__init__.py
--rw-r--r--   0        0        0     7277 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/anaplan/anaplan.png
--rw-r--r--   0        0        0     7005 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/anaplan/anaplan_connector.py
--rw-r--r--   0        0        0     4622 2023-07-19 09:02:51.130259 toucan_connectors-4.7.1/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8464 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2404 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     4541 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15322 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/common.py
--rw-r--r--   0        0        0     5549 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8162 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5236 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1100 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5118 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/__init__.py
--rw-r--r--   0        0        0      452 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/doc.md
--rw-r--r--   0        0        0      183 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/enums.py
--rw-r--r--   0        0        0     5283 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/facebook_ads_connector.py
--rw-r--r--   0        0        0    27755 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/facebook_logo.png
--rw-r--r--   0        0        0      126 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_ads/helpers.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_insights/__init__.py
--rw-r--r--   0        0        0    38402 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_insights/facebook-insights.png
--rw-r--r--   0        0        0     3985 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/facebook_insights/facebook_insights_connector.py
--rw-r--r--   0        0        0    13001 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    17081 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15902 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/google_adwords/__init__.py
--rw-r--r--   0        0        0      469 2023-07-19 09:02:51.134259 toucan_connectors-4.7.1/toucan_connectors/google_adwords/doc.md
--rw-r--r--   0        0        0    68711 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_adwords/google_adwords.jpg
--rw-r--r--   0        0        0     9049 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_adwords/google_adwords_connector.py
--rw-r--r--   0        0        0      834 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_adwords/helpers.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6799 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    14501 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2488 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2473 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_my_business/__init__.py
--rw-r--r--   0        0        0     4045 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_my_business/google-my-business.png
--rw-r--r--   0        0        0     3024 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_my_business/google_my_business_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9061 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9559 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2986 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     8020 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/__init__.py
--rw-r--r--   0        0        0      380 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/doc.md
--rw-r--r--   0        0        0      294 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/enums.py
--rw-r--r--   0        0        0      173 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/helpers.py
--rw-r--r--   0        0        0    33203 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/hubspot.png
--rw-r--r--   0        0        0     5738 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot/hubspot_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0     5197 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      726 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      509 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0      926 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      706 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/linkedinads/__init__.py
--rw-r--r--   0        0        0      365 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/linkedinads/doc.md
--rw-r--r--   0        0        0     9990 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/linkedinads/linkedinads.png
--rw-r--r--   0        0        0     7544 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/linkedinads/linkedinads_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/micro_strategy/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/micro_strategy/client.py
--rw-r--r--   0        0        0     4454 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/micro_strategy/data.py
--rw-r--r--   0        0        0     4664 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/micro_strategy/micro_strategy_connector.py
--rw-r--r--   0        0        0    13133 2023-07-19 09:02:51.138259 toucan_connectors-4.7.1/toucan_connectors/micro_strategy/microstrategy.png
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    17096 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4673 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     4893 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14692 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0     2401 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/net_explorer/net_explorer.png
--rwxr-xr-x   0        0        0     3536 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/net_explorer/net_explorer_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     6028 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2047 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1298 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12312 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3375 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3948 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2638 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      509 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10400 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    17824 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1498 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16551 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1850 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0      410 2023-07-19 09:02:51.142260 toucan_connectors-4.7.1/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7429 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1264 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      143 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18251 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12795 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12246 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4325 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3080 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    21205 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/toucan_toco/__init__.py
--rwxr-xr-x   0        0        0     4372 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/toucan_toco/toucan.png
--rw-r--r--   0        0        0     1289 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/toucan_toco/toucan_toco_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/trello/__init__.py
--rw-r--r--   0        0        0     3966 2023-07-19 09:02:51.146260 toucan_connectors-4.7.1/toucan_connectors/trello/trello.png
--rw-r--r--   0        0        0     6603 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/trello/trello_connector.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0      629 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0        0 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/wootric/__init__.py
--rw-r--r--   0        0        0     8734 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/wootric/wootric.png
--rw-r--r--   0        0        0     5228 2023-07-19 09:02:51.150260 toucan_connectors-4.7.1/toucan_connectors/wootric/wootric_connector.py
--rw-r--r--   0        0        0    14612 1970-01-01 00:00:00.000000 toucan_connectors-4.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-07-20 12:20:06.347701 toucan_connectors-4.7.2/LICENSE
+-rw-r--r--   0        0        0     9969 2023-07-20 12:20:06.347701 toucan_connectors-4.7.2/README.md
+-rw-r--r--   0        0        0     5594 2023-07-20 12:20:06.351702 toucan_connectors-4.7.2/pyproject.toml
+-rw-r--r--   0        0        0    10795 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/adobe_analytics/__init__.py
+-rw-r--r--   0        0        0    13648 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/adobe_analytics/adobe-analytics.png
+-rw-r--r--   0        0        0     1740 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/anaplan/__init__.py
+-rw-r--r--   0        0        0     7277 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/anaplan/anaplan.png
+-rw-r--r--   0        0        0     7005 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/anaplan/anaplan_connector.py
+-rw-r--r--   0        0        0     4622 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8464 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2404 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     4541 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15322 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5549 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8162 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5236 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1100 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5118 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/doc.md
+-rw-r--r--   0        0        0      183 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/enums.py
+-rw-r--r--   0        0        0     5283 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/facebook_ads_connector.py
+-rw-r--r--   0        0        0    27755 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/facebook_logo.png
+-rw-r--r--   0        0        0      126 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_ads/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.367702 toucan_connectors-4.7.2/toucan_connectors/facebook_insights/__init__.py
+-rw-r--r--   0        0        0    38402 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/facebook_insights/facebook-insights.png
+-rw-r--r--   0        0        0     3985 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/facebook_insights/facebook_insights_connector.py
+-rw-r--r--   0        0        0    13001 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    17081 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15902 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_adwords/__init__.py
+-rw-r--r--   0        0        0      469 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_adwords/doc.md
+-rw-r--r--   0        0        0    68711 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_adwords/google_adwords.jpg
+-rw-r--r--   0        0        0     9049 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_adwords/google_adwords_connector.py
+-rw-r--r--   0        0        0      834 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_adwords/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6799 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    14501 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2488 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2473 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_my_business/__init__.py
+-rw-r--r--   0        0        0     4045 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_my_business/google-my-business.png
+-rw-r--r--   0        0        0     3024 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_my_business/google_my_business_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9061 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9559 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2986 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     8020 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/hubspot/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/hubspot/doc.md
+-rw-r--r--   0        0        0      294 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/hubspot/enums.py
+-rw-r--r--   0        0        0      173 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/hubspot/helpers.py
+-rw-r--r--   0        0        0    33203 2023-07-20 12:20:06.371702 toucan_connectors-4.7.2/toucan_connectors/hubspot/hubspot.png
+-rw-r--r--   0        0        0     5738 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/hubspot/hubspot_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0     5197 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      726 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      509 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0      926 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      706 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/linkedinads/__init__.py
+-rw-r--r--   0        0        0      365 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/linkedinads/doc.md
+-rw-r--r--   0        0        0     9990 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/linkedinads/linkedinads.png
+-rw-r--r--   0        0        0     7544 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/linkedinads/linkedinads_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/micro_strategy/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/micro_strategy/client.py
+-rw-r--r--   0        0        0     4454 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/micro_strategy/data.py
+-rw-r--r--   0        0        0     4664 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/micro_strategy/micro_strategy_connector.py
+-rw-r--r--   0        0        0    13133 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/micro_strategy/microstrategy.png
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    17096 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4673 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     4893 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14692 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0     2401 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/net_explorer/net_explorer.png
+-rwxr-xr-x   0        0        0     3536 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/net_explorer/net_explorer_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     6028 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2047 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1298 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12312 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3375 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3948 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2638 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      509 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10400 2023-07-20 12:20:06.375702 toucan_connectors-4.7.2/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    17824 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1498 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16627 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1850 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0      410 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7429 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1264 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      143 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18251 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12795 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12246 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-20 12:20:06.379702 toucan_connectors-4.7.2/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4325 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3080 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    21205 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/toucan_toco/__init__.py
+-rwxr-xr-x   0        0        0     4372 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/toucan_toco/toucan.png
+-rw-r--r--   0        0        0     1289 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/toucan_toco/toucan_toco_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/trello/__init__.py
+-rw-r--r--   0        0        0     3966 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/trello/trello.png
+-rw-r--r--   0        0        0     6603 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/trello/trello_connector.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0      629 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/wootric/__init__.py
+-rw-r--r--   0        0        0     8734 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/wootric/wootric.png
+-rw-r--r--   0        0        0     5228 2023-07-20 12:20:06.383702 toucan_connectors-4.7.2/toucan_connectors/wootric/wootric_connector.py
+-rw-r--r--   0        0        0    14612 1970-01-01 00:00:00.000000 toucan_connectors-4.7.2/PKG-INFO
```

### Comparing `toucan_connectors-4.7.1/LICENSE` & `toucan_connectors-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/README.md` & `toucan_connectors-4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/pyproject.toml` & `toucan_connectors-4.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 profile = "black"
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
 [tool.poetry]
 name = "toucan-connectors"
-version = "4.7.1"
+version = "4.7.2"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `toucan_connectors-4.7.1/toucan_connectors/__init__.py` & `toucan_connectors-4.7.2/toucan_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/adobe_analytics/adobe-analytics.png` & `toucan_connectors-4.7.2/toucan_connectors/adobe_analytics/adobe-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/adobe_analytics/adobe_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/anaplan/anaplan.png` & `toucan_connectors-4.7.2/toucan_connectors/anaplan/anaplan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/anaplan/anaplan_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/anaplan/anaplan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/auth.py` & `toucan_connectors-4.7.2/toucan_connectors/auth.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/aws/aws.png` & `toucan_connectors-4.7.2/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/awsathena/athena.png` & `toucan_connectors-4.7.2/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-4.7.2/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-4.7.2/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/common.py` & `toucan_connectors-4.7.2/toucan_connectors/common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/condition_translator.py` & `toucan_connectors-4.7.2/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/connection_manager.py` & `toucan_connectors-4.7.2/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/databricks/databricks.png` & `toucan_connectors-4.7.2/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-4.7.2/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/denodo/denodo.png` & `toucan_connectors-4.7.2/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-4.7.2/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/facebook_ads/facebook_ads_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/facebook_ads/facebook_ads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/facebook_ads/facebook_logo.png` & `toucan_connectors-4.7.2/toucan_connectors/facebook_ads/facebook_logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/facebook_insights/facebook-insights.png` & `toucan_connectors-4.7.2/toucan_connectors/facebook_insights/facebook-insights.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/facebook_insights/facebook_insights_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/facebook_insights/facebook_insights_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-4.7.2/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/github/github_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/github/github_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/github/helpers.py` & `toucan_connectors-4.7.2/toucan_connectors/github/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_adwords/google_adwords.jpg` & `toucan_connectors-4.7.2/toucan_connectors/google_adwords/google_adwords.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_adwords/google_adwords_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_adwords/google_adwords_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_adwords/helpers.py` & `toucan_connectors-4.7.2/toucan_connectors/google_adwords/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-4.7.2/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-4.7.2/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-4.7.2/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_credentials.py` & `toucan_connectors-4.7.2/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_my_business/google-my-business.png` & `toucan_connectors-4.7.2/toucan_connectors/google_my_business/google-my-business.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_my_business/google_my_business_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_my_business/google_my_business_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-4.7.2/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-4.7.2/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/http_api/http-api.png` & `toucan_connectors-4.7.2/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/http_api/http_api_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/hubspot/hubspot.png` & `toucan_connectors-4.7.2/toucan_connectors/hubspot/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/hubspot/hubspot_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/hubspot/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-4.7.2/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-4.7.2/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-4.7.2/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-4.7.2/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/json_wrapper.py` & `toucan_connectors-4.7.2/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/linkedinads/linkedinads.png` & `toucan_connectors-4.7.2/toucan_connectors/linkedinads/linkedinads.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/linkedinads/linkedinads_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/linkedinads/linkedinads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/micro_strategy/client.py` & `toucan_connectors-4.7.2/toucan_connectors/micro_strategy/client.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/micro_strategy/data.py` & `toucan_connectors-4.7.2/toucan_connectors/micro_strategy/data.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/micro_strategy/micro_strategy_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/micro_strategy/micro_strategy_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/micro_strategy/microstrategy.png` & `toucan_connectors-4.7.2/toucan_connectors/micro_strategy/microstrategy.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-4.7.2/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/mongo/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-4.7.2/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mssql/mssql.png` & `toucan_connectors-4.7.2/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-4.7.2/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mysql/mysql.png` & `toucan_connectors-4.7.2/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/net_explorer/net_explorer.png` & `toucan_connectors-4.7.2/toucan_connectors/net_explorer/net_explorer.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/net_explorer/net_explorer_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/net_explorer/net_explorer_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-4.7.2/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/odata/odata.png` & `toucan_connectors-4.7.2/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/odata/odata_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/odbc/odbc.png` & `toucan_connectors-4.7.2/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/odbc/odbc_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-4.7.2/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-4.7.2/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/pagination.py` & `toucan_connectors-4.7.2/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/pandas_translator.py` & `toucan_connectors-4.7.2/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/peakina/peakina.png` & `toucan_connectors-4.7.2/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/postgres/postgres.png` & `toucan_connectors-4.7.2/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/postgres/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/postgres/utils.py` & `toucan_connectors-4.7.2/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/query_manager.py` & `toucan_connectors-4.7.2/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/redshift/redshift.png` & `toucan_connectors-4.7.2/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,28 +364,28 @@
         return table_infos
 
     def get_model(self, db_name: str | None = None) -> list[TableInfo]:
         """Retrieves the database tree structure using current connection"""
         tables_info = []
         dbs = self.available_dbs if db_name is None else [db_name]
         for db in dbs:
-            with suppress(redshift_connector.OperationalError):
+            with suppress(redshift_connector.OperationalError, redshift_connector.ProgrammingError):
                 tables_info += self._db_tables_info(db)
 
         return tables_info
 
     def get_model_with_info(self, db_name: str | None = None) -> tuple[list[TableInfo], dict]:
         """Retrieves the database tree structure using current connection"""
         databases_tree = []
         failed_databases = []
         dbs = self.available_dbs if db_name is None else [db_name]
         for db in dbs:
             try:
                 databases_tree += self._list_tables_info(db)
-            except redshift_connector.OperationalError:
+            except (redshift_connector.OperationalError, redshift_connector.ProgrammingError):
                 failed_databases.append(db)
 
         tables_info = DiscoverableConnector.format_db_model(databases_tree)
         metadata = {}
         if failed_databases:
             metadata['info'] = {'Could not reach databases': failed_databases}
         return (tables_info, metadata)
```

### Comparing `toucan_connectors-4.7.1/toucan_connectors/redshift/utils.py` & `toucan_connectors-4.7.2/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-4.7.2/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-4.7.2/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/share_point/share_point.png` & `toucan_connectors-4.7.2/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-4.7.2/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/snowflake/snowflake_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/snowflake_common.py` & `toucan_connectors-4.7.2/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-4.7.2/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/soap/helpers.py` & `toucan_connectors-4.7.2/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/soap/soap.png` & `toucan_connectors-4.7.2/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/sql_query_helper.py` & `toucan_connectors-4.7.2/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/toucan_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/toucan_toco/toucan.png` & `toucan_connectors-4.7.2/toucan_connectors/toucan_toco/toucan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/toucan_toco/toucan_toco_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/toucan_toco/toucan_toco_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/trello/trello.png` & `toucan_connectors-4.7.2/toucan_connectors/trello/trello.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/trello/trello_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/trello/trello_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/utils/pem.py` & `toucan_connectors-4.7.2/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/wootric/wootric.png` & `toucan_connectors-4.7.2/toucan_connectors/wootric/wootric.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/toucan_connectors/wootric/wootric_connector.py` & `toucan_connectors-4.7.2/toucan_connectors/wootric/wootric_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.7.1/PKG-INFO` & `toucan_connectors-4.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 4.7.1
+Version: 4.7.2
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

