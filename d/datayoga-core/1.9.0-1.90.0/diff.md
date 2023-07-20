# Comparing `tmp/datayoga_core-1.9.0.tar.gz` & `tmp/datayoga_core-1.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga_core-1.9.0.tar", max compression
+gzip compressed data, was "datayoga_core-1.90.0.tar", max compression
```

## Comparing `datayoga_core-1.9.0.tar` & `datayoga_core-1.90.0.tar`

### file list

```diff
@@ -1,62 +1,97 @@
--rw-r--r--   0        0        0    10712 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/README.md
--rw-r--r--   0        0        0     1479 2022-11-23 19:29:20.562231 datayoga_core-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1987 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/__init__.py
--rw-r--r--   0        0        0     2287 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/block.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/__init__.py
--rw-r--r--   0        0        0     1413 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py
--rw-r--r--   0        0        0     2062 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json
--rw-r--r--   0        0        0     1826 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/__init__.py
--rw-r--r--   0        0        0     1047 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py
--rw-r--r--   0        0        0     1494 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/__init__.py
--rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.py
--rw-r--r--   0        0        0      464 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.schema.json
--rw-r--r--   0        0        0     2572 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/tests/test_filter.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/__init__.py
--rw-r--r--   0        0        0     1077 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.py
--rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
--rw-r--r--   0        0        0     2703 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py
--rw-r--r--   0        0        0      586 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
--rw-r--r--   0        0        0      493 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/utils.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/__init__.py
--rw-r--r--   0        0        0     1439 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.py
--rw-r--r--   0        0        0      605 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/__init__.py
--rw-r--r--   0        0        0     1650 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.py
--rw-r--r--   0        0        0     2485 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/__init__.py
--rw-r--r--   0        0        0     1180 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py
--rw-r--r--   0        0        0     1182 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json
--rw-r--r--   0        0        0     1907 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/__init__.py
--rw-r--r--   0        0        0     1972 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py
--rw-r--r--   0        0        0     1716 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json
--rw-r--r--   0        0        0     2282 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/__init__.py
--rw-r--r--   0        0        0      347 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.py
--rw-r--r--   0        0        0      517 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/__init__.py
--rw-r--r--   0        0        0     1263 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py
--rw-r--r--   0        0        0       75 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/__init__.py
--rw-r--r--   0        0        0      862 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.py
--rw-r--r--   0        0        0       76 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.schema.json
--rw-r--r--   0        0        0      633 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/context.py
--rw-r--r--   0        0        0     5473 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/expression.py
--rw-r--r--   0        0        0     4546 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/jmespath_custom_functions.py
--rw-r--r--   0        0        0     4408 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/job.py
--rw-r--r--   0        0        0      712 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/producer.py
--rw-r--r--   0        0        0       23 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/.gitignore
--rw-r--r--   0        0        0      955 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md
--rw-r--r--   0        0        0      154 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/connections.yaml
--rw-r--r--   0        0        0      188 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/data/sample.csv
--rw-r--r--   0        0        0      445 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
--rw-r--r--   0        0        0     2226 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json
--rw-r--r--   0        0        0     1757 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json
--rw-r--r--   0        0        0     4378 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/step.py
--rw-r--r--   0        0        0     2317 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/utils.py
--rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/setup.py
--rw-r--r--   0        0        0    12379 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     5118 2023-07-20 11:40:02.255293 datayoga_core-1.90.0/README.md
+-rw-r--r--   0        0        0     2757 2023-07-20 11:40:24.044059 datayoga_core-1.90.0/pyproject.toml
+-rw-r--r--   0        0        0     3558 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/block.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/block.py
+-rw-r--r--   0        0        0     2062 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/block.schema.json
+-rw-r--r--   0        0        0     1815 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/azure/read_event_hub/__init__.py
+-rw-r--r--   0        0        0     4348 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/azure/read_event_hub/block.py
+-rw-r--r--   0        0        0     1232 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/azure/read_event_hub/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/cassandra/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/cassandra/write/__init__.py
+-rw-r--r--   0        0        0     4609 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/cassandra/write/block.py
+-rw-r--r--   0        0        0     1751 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/cassandra/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/files/read_csv/__init__.py
+-rw-r--r--   0        0        0     2023 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/files/read_csv/block.py
+-rw-r--r--   0        0        0     1665 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/filter/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/filter/block.py
+-rw-r--r--   0        0        0      464 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/filter/block.schema.json
+-rw-r--r--   0        0        0     4200 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/filter/tests/test_filter.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/http/receiver/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/http/receiver/block.py
+-rw-r--r--   0        0        0      468 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/http/receiver/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/map/__init__.py
+-rw-r--r--   0        0        0     2517 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/map/block.py
+-rw-r--r--   0        0        0     1167 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/map/block.schema.json
+-rw-r--r--   0        0        0     6070 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/map/tests/test_map.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/read/__init__.py
+-rw-r--r--   0        0        0     1115 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/read/block.py
+-rw-r--r--   0        0        0      352 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/read/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/write/__init__.py
+-rw-r--r--   0        0        0     1271 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/write/block.py
+-rw-r--r--   0        0        0      352 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
+-rw-r--r--   0        0        0     2690 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/read_stream/block.py
+-rw-r--r--   0        0        0      586 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
+-rw-r--r--   0        0        0      493 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/write/__init__.py
+-rw-r--r--   0        0        0     2197 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/write/block.py
+-rw-r--r--   0        0        0      886 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/redis/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/read/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/read/block.py
+-rw-r--r--   0        0        0     1315 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/read/block.schema.json
+-rw-r--r--   0        0        0     1669 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/write/__init__.py
+-rw-r--r--   0        0        0    10167 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/write/block.py
+-rw-r--r--   0        0        0     3312 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/relational/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/block.py
+-rw-r--r--   0        0        0     1182 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/block.schema.json
+-rw-r--r--   0        0        0     1893 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/__init__.py
+-rw-r--r--   0        0        0     1942 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/block.py
+-rw-r--r--   0        0        0     1716 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/block.schema.json
+-rw-r--r--   0        0        0     2279 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/sequence/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/sequence/block.py
+-rw-r--r--   0        0        0      517 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/sequence/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/read/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/read/block.py
+-rw-r--r--   0        0        0       75 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/read/block.schema.json
+-rw-r--r--   0        0        0        0 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/write/__init__.py
+-rw-r--r--   0        0        0      870 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/write/block.py
+-rw-r--r--   0        0        0       76 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/blocks/std/write/block.schema.json
+-rw-r--r--   0        0        0      337 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/context.py
+-rw-r--r--   0        0        0     7618 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/expression.py
+-rw-r--r--   0        0        0     8300 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/jmespath_custom_functions.py
+-rw-r--r--   0        0        0    10326 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/job.py
+-rw-r--r--   0        0        0      116 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/opcode.py
+-rw-r--r--   0        0        0      739 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/producer.py
+-rw-r--r--   0        0        0      522 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/prometheus.py
+-rw-r--r--   0        0        0       23 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/.gitignore
+-rw-r--r--   0        0        0      955 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/README.md
+-rw-r--r--   0        0        0      151 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/connections.yaml
+-rw-r--r--   0        0        0      188 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/data/sample.csv
+-rw-r--r--   0        0        0      444 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
+-rw-r--r--   0        0        0      981 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json
+-rw-r--r--   0        0        0     1169 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json
+-rw-r--r--   0        0        0     1489 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json
+-rw-r--r--   0        0        0     1270 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json
+-rw-r--r--   0        0        0      641 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/redis.schema.json
+-rw-r--r--   0        0        0     1009 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json
+-rw-r--r--   0        0        0      981 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections.schema.json
+-rw-r--r--   0        0        0     1833 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/resources/schemas/job.schema.json
+-rw-r--r--   0        0        0     1048 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/result.py
+-rw-r--r--   0        0        0     5505 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/step.py
+-rw-r--r--   0        0        0     2112 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/step_buffer.py
+-rw-r--r--   0        0        0     4536 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/utils.py
+-rw-r--r--   0        0        0     2485 2023-07-20 11:40:02.259293 datayoga_core-1.90.0/src/datayoga_core/write_utils.py
+-rw-r--r--   0        0        0     8050 1970-01-01 00:00:00.000000 datayoga_core-1.90.0/PKG-INFO
```

### Comparing `datayoga_core-1.9.0/pyproject.toml` & `datayoga_core-1.90.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga-core"
-version = "1.9.0"
+version = "1.90.0"
 description = "DataYoga for Python"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
 
@@ -13,37 +13,78 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Topic :: Database'
 ]
 
 [tool.poetry.dependencies]
-click = "^8.0.3"
+certifi = "^2022.12.7"
+pysqlite3-binary = { version = "^0.4.0", platform = "linux" }
+cryptography = ">=39.0.1"
 jmespath = "^1.0.0"
 jsonschema = "^4.4.0"
+orjson = "^3.8.7"
 python = "^3.7"
 PyYAML = "^6.0"
 
 mock = { version = "^4.0.3", optional = true }
 pytest = { version = "^7.1.2", optional = true }
+pytest-asyncio = { version = "^0.20.2", optional = true }
 pytest-describe = { version = "^2.0.1", optional = true }
 pytest-mock = { version = "^3.7.0", optional = true }
 pytest-timeout = { version = "^2.1.0", optional = true }
 requests-mock = { version = "^1.9.3", optional = true }
 testcontainers = { version = "^3.7.0", optional = true }
 
-psycopg2 = { version="^2.9.3", optional = true}
-redis = { version = "^4.1.4", optional = true}
-SQLAlchemy = { version = "^1.4.41", optional = true}
+azure-eventhub = { version = "^5.11.2", optional= true }
+azure-eventhub-aio = { version = "^5.11.2", optional = true }
+azure-eventhub-checkpointstoreblob-aio = { version = "^1.1.4", optional = true }
+aiohttp = { version = "^3.8.4", optional = true }
+cassandra-driver = { version = "^3.25.0", optional = true }
+fastparquet = { version = "^2023.2.0", optional = true, platform = "python>=3.8" }
+psycopg2-binary = { version="^2.9.5", optional = true}
+oracledb = { version="^1.2.2", optional = true}
+prometheus-client = "^0.16.0"
+pymssql = { version="^2.2.7", optional = true }
+PyMySQL = { version="^1.0.2", optional = true }
+redis = { version = "^4.3.5", optional = true }
+SQLAlchemy = { version = "^2.0.4", optional = true }
+sqlglot = "^10.4.3"
 
 [tool.poetry.extras]
+azure = ["azure-eventhub", "azure-eventhub-aio", "azure-eventhub-checkpointstoreblobaio"]
+cassandra = ["cassandra-driver"]
+mysql = ["PyMySQL", "SQLAlchemy"]
+oracle = ["oracledb", "SQLAlchemy"]
+parquet = ["fastparquet"]
+pg = ["psycopg2-binary", "SQLAlchemy"]
 redis = ["redis"]
-pg = ["psycopg2","SQLAlchemy"]
-test = ["mock", "pytest", "pytest-asyncio", "pytest-describe", "pytest-mock", "pytest-timeout", "requests-mock", "redis", "psycopg2","SQLAlchemy", "testcontainers"]
+sqlserver = ["pymssql", "SQLAlchemy"]
+http = ["aiohttp"]
+
+test = [
+        "cassandra-driver",
+        "fastparquet",
+        "aiohttp",
+        "mock",
+        "psycopg2-binary",
+        "oracledb",
+        "pymssql",
+        "PyMySQL",
+        "pytest",
+        "pytest-asyncio",
+        "pytest-describe",
+        "pytest-mock",
+        "pytest-timeout",
+        "redis",
+        "requests-mock",
+        "SQLAlchemy",
+        "testcontainers"
+]
 
 [tool.poetry.urls]
 url = "https://datayoga.io"
 [tool.poetry.scripts]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/block.py` & `datayoga_core-1.90.0/src/datayoga_core/block.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,101 @@
+from __future__ import annotations
+
 import importlib
 import logging
 import os
 import sys
-from enum import Enum
+from abc import ABCMeta, abstractmethod
 from os import path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 from datayoga_core import utils
 from datayoga_core.context import Context
+from datayoga_core.result import BlockResult
 from jsonschema import validate
 
 logger = logging.getLogger("dy")
 
 
-Result = Enum("Result", "SUCCESS REJECTED FILTERED")
-
-
-class Block():
-    MSG_ID_FIELD = "__$$msg_id"
+class Block(metaclass=ABCMeta):
+    INTERNAL_FIELD_PREFIX = "__$$"
+    MSG_ID_FIELD = f"{INTERNAL_FIELD_PREFIX}msg_id"
+    RESULT_FIELD = f"{INTERNAL_FIELD_PREFIX}result"
+    OPCODE_FIELD = f"{INTERNAL_FIELD_PREFIX}opcode"
     """
     Block
 
     Attributes:
         properties Dict[str, Any]: Block properties
     """
 
-    def __init__(self, properties: Dict[str, Any] = {}):
+    def __init__(self, properties: Optional[Dict[str, Any]] = None):
         """
         Constructs a block
 
         Args:
-            properties (Dict[str, Any]): Block [properties]
+            properties (Optional[Dict[str, Any]]): Block [properties]
         """
-        self.properties = properties
+        self.properties = properties or {}
         self.validate()
 
     def validate(self):
         """
         Validates block against its JSON Schema
         """
+        logger.debug(f"validating {self.properties}")
+        validate(instance=self.properties, schema=self.get_json_schema())
+
+    def get_json_schema(self) -> Dict[str, Any]:
+        """
+        Returns the JSON Schema for this block
+
+        Returns:
+            Dict[str, Any]: JSON Schema
+        """
         json_schema_file = path.join(
-            utils.get_bundled_dir(), "blocks", self.get_block_name(),
+            utils.get_bundled_dir(),
+            os.path.relpath(
+                os.path.dirname(sys.modules[self.__module__].__file__),
+                start=os.path.dirname(__file__)),
             "block.schema.json") if utils.is_bundled() else path.join(
             os.path.dirname(os.path.realpath(sys.modules[self.__module__].__file__)),
             "block.schema.json")
+        logger.debug(f"loading schema from {json_schema_file}")
+        return utils.read_json(json_schema_file)
 
-        logger.debug(f"validating {self.properties} against {json_schema_file}")
-        validate(instance=self.properties, schema=utils.read_json(json_schema_file))
-
+    @abstractmethod
     def init(self, context: Optional[Context] = None):
         """
-        Initializes block (abstract, should be implemented by the sub class)
+        Initializes block
 
         Args:
             context (Context, optional): Context. Defaults to None.
         """
-        pass
+        raise NotImplementedError
 
-    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
-        """ Transforms data (abstract, should be implemented by the sub class)
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+        """Transforms data
 
         Args:
             data (List[Dict[str, Any]]): Data
 
         Returns:
-            List[Dict[str, Any]]: Transformed data
+            BlockResult: Block result
+        """
+        pass
+
+    def stop(self):
+        """
+        Cleans the block connections and state
         """
         pass
 
     def get_block_name(self):
         return os.path.basename(os.path.dirname(sys.modules[self.__module__].__file__))
 
-
-#
-# static utility methods
-#
-
-def create_block(block_name: str, properties: Dict[str, Any]) -> Block:
-    module_name = f"datayoga_core.blocks.{block_name}.block"
-    module = importlib.import_module(module_name)
-    block: Block = getattr(module, "Block")(properties)
-    return block
+    @staticmethod
+    def create(block_name: str, properties: Dict[str, Any]) -> Block:
+        module_name = f"datayoga_core.blocks.{block_name}.block"
+        module = importlib.import_module(module_name)
+        block: Block = getattr(module, "Block")(properties)
+        return block
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import logging
-from typing import Any, Dict, List, Tuple
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional
 
 from datayoga_core import expression, utils
 from datayoga_core.block import Block as DyBlock
-from datayoga_core.block import Result
 from datayoga_core.context import Context
+from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock):
-    def init(self, context: Context = None):
+class Block(DyBlock, metaclass=ABCMeta):
+
+    def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
         self.fields = {}
-        for property in self.properties["fields"]:
-            self.fields[property["field"]] = expression.compile(
-                property["language"],
-                property["expression"])
+        for prop in self.properties["fields"]:
+            self.fields[prop["field"]] = expression.compile(
+                prop["language"],
+                prop["expression"])
 
-    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
         logger.debug(f"Running {self.get_block_name()}")
-        results = []
-        for row in data:
-            for field in self.fields:
-                obj = row
-                field_path = utils.split_field(field)
+        for field in self.fields:
+            expression_results = self.fields[field].search_bulk(data)
+            field_path = utils.split_field(field)
 
+            for i, row in enumerate(data):
+                obj = row
+                # handle nested fields. in that case, the obj points at the nested entity
                 for key in field_path[:-1]:
                     key = utils.unescape_field(key)
                     if key in obj:
                         obj = obj[key]
                     else:
                         obj[key] = {}
+                # assign the new values
+                obj[utils.unescape_field(field_path[-1:][0])] = expression_results[i]
 
-                obj[utils.unescape_field(field_path[-1:][0])] = self.fields[field].search(row)
-            results.append(Result.SUCCESS)
-        return data, results
+        return utils.all_success(data)
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pytest
-from datayoga_core.block import Result
+from datayoga_core import utils
 from datayoga_core.blocks.add_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_add_field():
     block = Block({"field": "full_name",
                    "language": "jmespath",
                    "expression": "[fname,lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([
-        {"fname": "john", "lname": "doe", "full_name": "john doe"}], [Result.SUCCESS]
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
+        {"fname": "john", "lname": "doe", "full_name": "john doe"}]
     )
 
 
 @pytest.mark.asyncio
 async def test_add_nested_field():
     block = Block({"field": "name.full_name",
                    "language": "jmespath",
                   "expression": "[name.fname,name.lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
-        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
+        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe"}}])
 
 
 @pytest.mark.asyncio
 async def test_add_multiple_fields():
     block = Block({"fields": [{"field": "name.full_name", "language": "jmespath", "expression": "concat([name.fname, ' ', name.lname])"}, {
                   "field": "name.fname_upper", "language": "jmespath", "expression": "upper(name.fname)"}]})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
-        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe", "fname_upper": "JOHN"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
+        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe", "fname_upper": "JOHN"}}])
 
 
 @pytest.mark.asyncio
 async def test_add_field_with_dot():
     block = Block({"field": "name\.full_name",
                    "language": "jmespath",
                    "expression": "[fname,lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([
-        {"fname": "john", "lname": "doe", "name.full_name": "john doe"}], [Result.SUCCESS])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
+        {"fname": "john", "lname": "doe", "name.full_name": "john doe"}])
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/parquet/write/block.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import logging
 import os
-from csv import DictReader
-from typing import Generator, Optional
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional
 
+from datayoga_core import utils
+from datayoga_core.block import Block as DyBlock
 from datayoga_core.context import Context
-from datayoga_core.producer import Message
-from datayoga_core.producer import Producer as DyProducer
+from datayoga_core.result import BlockResult
+from datayoga_core.utils import remove_msg_id
+from fastparquet import write
+from pandas import DataFrame
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyProducer):
+class Block(DyBlock, metaclass=ABCMeta):
 
     def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
-        csv_file = self.properties["file"]
+        parquet_file = self.properties["file"]
 
-        if os.path.isabs(csv_file) or context is None:
-            self.file = csv_file
+        if os.path.isabs(parquet_file) or context is None:
+            self.file = parquet_file
         else:
-            self.file = os.path.join(context.properties.get("data_path"), csv_file)
+            self.file = os.path.join(context.properties.get("data_path"), parquet_file)
 
         logger.debug(f"file: {self.file}")
-        self.batch_size = self.properties.get("batch_size", 1000)
 
-    def produce(self) -> Generator[Message, None, None]:
-        logger.debug("Reading CSV")
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+        logger.debug("Writing parquet")
 
-        with open(self.file, "r") as read_obj:
-            records = list(DictReader(read_obj))
+        out = [{"data": remove_msg_id(record)} for record in data]
+        append = os.path.exists(self.file)
+        write(self.file, DataFrame(out), append=append, has_nulls=True)
 
-        for i, record in enumerate(records):
-            yield {self.MSG_ID_FIELD: str(i), **record}
+        # if we made it here, it is a success. return the data and the success result
+        return utils.all_success(data)
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/files/read_csv/block.schema.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666852678571428%*

 * *Differences: {"'properties'": "{'fields': {'default': None, 'minLength': 1}, 'delimiter': {'minLength': 1, "*

 * *                 "'maxLength': 1}, 'batch_size': {'default': 1000, 'minimum': 1}, 'quotechar': "*

 * *                 '{\'default\': \'"\', \'minLength\': 1, \'maxLength\': 1}, \'encoding\': '*

 * *                 "OrderedDict([('description', 'Encoding to use for reading the file'), ('type', "*

 * *                 "'string'), ('default', 'utf-8')]), 'skip': OrderedDict([('description', 'Number "*

 * *                 "of lines t […]*

```diff
@@ -5,56 +5,68 @@
         {
             "delimiter": ";",
             "file": "archive.csv"
         }
     ],
     "properties": {
         "batch_size": {
-            "default": "1000",
+            "default": 1000,
             "description": "Number of records to read per batch",
+            "minimum": 1,
             "type": "number"
         },
         "delimiter": {
             "default": ",",
             "description": "Delimiter to use for splitting the csv records",
+            "maxLength": 1,
+            "minLength": 1,
+            "type": "string"
+        },
+        "encoding": {
+            "default": "utf-8",
+            "description": "Encoding to use for reading the file",
             "type": "string"
         },
         "fields": {
             "additionalItems": true,
-            "default": [],
+            "default": null,
             "description": "List of columns to use for extract",
             "examples": [
                 [
                     "fname",
                     "lname"
                 ]
             ],
             "items": {
                 "description": "field name",
                 "examples": [
                     "fname"
                 ],
                 "type": "string"
             },
+            "minLength": 1,
             "title": "List of columns to use",
             "type": "array"
         },
         "file": {
             "description": "Filename. Can contain a regexp or glob expression",
             "type": "string"
         },
         "quotechar": {
-            "default": ",",
+            "default": "\"",
             "description": "A one-character string used to quote fields containing special characters, such as the delimiter or quotechar, or which contain new-line characters. It defaults to '",
+            "maxLength": 1,
+            "minLength": 1,
             "type": "string"
         },
-        "use_header": {
-            "default": true,
-            "description": "Determines whether or not to use the first line as the header containing column names. If `false`, field names must be specified",
-            "type": "boolean"
+        "skip": {
+            "default": 0,
+            "description": "Number of lines to skip",
+            "minimum": 0,
+            "type": "number"
         }
     },
     "required": [
         "file"
     ],
     "title": "files.read_csv",
     "type": "object"
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/filter/block.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import logging
-from typing import Any, Dict, List, Tuple
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional
 
 from datayoga_core import expression
 from datayoga_core.block import Block as DyBlock
-from datayoga_core.block import Result
 from datayoga_core.context import Context
+from datayoga_core.result import BlockResult, Result, Status
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock):
-    def init(self, context: Context = None):
+class Block(DyBlock, metaclass=ABCMeta):
+
+    def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.expression = expression.compile(self.properties["language"], self.properties["expression"])
 
-    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+        result = BlockResult()
         logger.debug(f"Running {self.get_block_name()}")
-        return_data = self.expression.filter(data)
-        return return_data, [Result.SUCCESS] * len(return_data)
+        return_data = self.expression.filter(data, tombstone=True)
+        # mark filtered rows
+        for i, row in enumerate(return_data):
+            if row is None:
+                result.filtered.append(Result(Status.FILTERED, payload=data[i]))
+            else:
+                result.processed.append(Result(Status.SUCCESS, payload=row))
+
+        return result
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/redis.schema.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42857142857142855%*

 * *Differences: {"'description'": "'Redis'",*

 * * "'examples'": "[OrderedDict([('cache', OrderedDict([('type', 'redis'), ('host', 'localhost'), "*

 * *               "('port', 6379)]))])]",*

 * * "'properties'": "{replace: OrderedDict([('type', OrderedDict([('description', 'DB type'), "*

 * *                 "('type', 'string'), ('enum', ['redis'])])), ('host', "*

 * *                 "OrderedDict([('description', 'Redis DB host'), ('type', 'string')])), ('port', "*

 * *                 "OrderedDict([('description', 'Redis DB port'), ('type', 'integer […]*

```diff
@@ -1,36 +1,41 @@
 {
     "additionalProperties": false,
-    "description": "Maps a record into a new output based on expressions",
+    "description": "Redis",
     "examples": [
         {
-            "expression": {
-                "country": "country",
-                "first_name": "first_name",
-                "full_name": "full_name",
-                "greeting": "'Hello ' || CASE WHEN gender = 'F' THEN 'Ms.' WHEN gender = 'M' THEN 'Mr.' ELSE 'N/A' END || ' ' || full_name",
-                "last_name": "last_name"
-            },
-            "language": "sql"
+            "cache": {
+                "host": "localhost",
+                "port": 6379,
+                "type": "redis"
+            }
         }
     ],
     "properties": {
-        "expression": {
-            "description": "Expression",
-            "type": "object"
+        "host": {
+            "description": "Redis DB host",
+            "type": "string"
+        },
+        "password": {
+            "description": "Redis DB password",
+            "type": "string"
         },
-        "language": {
-            "description": "Language",
+        "port": {
+            "description": "Redis DB port",
+            "maximum": 65535,
+            "minimum": 1,
+            "type": "integer"
+        },
+        "type": {
+            "description": "DB type",
             "enum": [
-                "jmespath",
-                "sql"
+                "redis"
             ],
             "type": "string"
         }
     },
     "required": [
-        "expression",
-        "language"
-    ],
-    "title": "map",
-    "type": "object"
+        "type",
+        "host",
+        "port"
+    ]
 }
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/redis/read_stream/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import json
 import logging
-from typing import Generator, List, Optional
+from typing import AsyncGenerator, List, Optional
 
 import datayoga_core.blocks.redis.utils as redis_utils
+import orjson
 from datayoga_core.context import Context
 from datayoga_core.producer import Message
 from datayoga_core.producer import Producer as DyProducer
 from datayoga_core.utils import get_connection_details
 
 logger = logging.getLogger("dy")
 
@@ -26,29 +26,29 @@
         self.consumer_group = f'datayoga_job_{context.properties.get("job_name", "") if context else ""}'
         self.requesting_consumer = "dy_consumer_a"
         stream_groups = self.redis_client.xinfo_groups(self.stream)
         if next(filter(lambda x: x["name"] == self.consumer_group, stream_groups), None) is None:
             logger.info(f"Creating a new {self.consumer_group} consumer group associated with the {self.stream}")
             self.redis_client.xgroup_create(self.stream, self.consumer_group, 0)
 
-    def produce(self) -> Generator[Message, None, None]:
+    async def produce(self) -> AsyncGenerator[List[Message], None]:
         logger.debug(f"Running {self.get_block_name()}")
 
         read_pending = True
         while True:
             # Read pending messages (fetched by us before but not acknowledged) in the first time, then consume new messages
             streams = self.redis_client.xreadgroup(self.consumer_group, self.requesting_consumer, {
-                                                   self.stream: "0" if read_pending else ">"}, None, 100 if self.snapshot else 0)
+                self.stream: "0" if read_pending else ">"}, None, 100 if self.snapshot else 0)
 
             for stream in streams:
                 logger.debug(f"Messages in {self.stream} stream (pending: {read_pending}):\n\t{stream}")
                 for key, value in stream[1]:
-                    payload = json.loads(value[next(iter(value))])
+                    payload = orjson.loads(value[next(iter(value))])
                     payload[self.MSG_ID_FIELD] = key
-                    yield payload
+                    yield [payload]
 
             # Quit after consuming pending current messages in case of snapshot
             if self.snapshot and not read_pending:
                 break
 
             read_pending = False
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/relational/read/block.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 import logging
-from functools import reduce
-from typing import Any, Dict, List, Optional, Tuple
+from typing import AsyncGenerator, List, Optional
 
-import datayoga_core.blocks.redis.utils as redis_utils
-from datayoga_core.block import Block as DyBlock
-from datayoga_core.block import Result
+import sqlalchemy as sa
+from datayoga_core import utils
+from datayoga_core.blocks.relational import utils as relational_utils
 from datayoga_core.context import Context
-from datayoga_core.utils import get_connection_details
+from datayoga_core.producer import Message
+from datayoga_core.producer import Producer as DyProducer
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock):
+class Block(DyProducer):
+
     def init(self, context: Optional[Context] = None):
-        logger.debug(f"Initializing {self.get_block_name()}")
-        self.command = self.properties.get("command")
-        self.key_field = self.properties.get("key_field")
-        connection = get_connection_details(self.properties.get("connection"), context)
-        self.redis_client = redis_utils.get_client(
-            connection.get("host"),
-            connection.get("port"),
-            connection.get("password"))
-        logger.info(f"Writing to Redis connection '{self.properties.get('connection')}'")
-
-    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
-        pipeline = self.redis_client.pipeline()
-        for record in data:
-            dict_as_list = list(reduce(lambda x, y: x + y, record.items()))
-            pipeline.execute_command(self.command, record[self.key_field], *dict_as_list)
-        pipeline.execute()
-        # TODO: check the return value from the pipeline
-        return data, [Result.SUCCESS]*len(data)
+        self.engine, self.db_type = relational_utils.get_engine(
+            self.properties.get("connection"),
+            context,
+            autocommit=False
+        )
+
+        self.schema = self.properties.get("schema")
+        self.table = self.properties.get("table")
+        self.opcode_field = self.properties.get("opcode_field")
+        self.load_strategy = self.properties.get("load_strategy")
+        self.keys = self.properties.get("keys")
+        self.mapping = self.properties.get("mapping")
+
+        self.tbl = sa.Table(self.table, sa.MetaData(schema=self.schema), autoload_with=self.engine)
+
+        logger.debug(f"Connecting to {self.db_type}")
+        self.connection = self.engine.connect()
+
+    async def produce(self) -> AsyncGenerator[List[Message], None]:
+        result = self.connection.execution_options(stream_results=True).execute(self.tbl.select())
+
+        while True:
+            chunk = result.fetchmany(10000)
+            if not chunk:
+                break
+            for row in chunk:
+                yield [utils.add_uid(dict(row._asdict()))]
+
+    def stop(self):
+        self.connection.close()
+        self.engine.dispose()
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/relational/write/block.schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8391504329004329%*

 * *Differences: {"'allOf'": "[OrderedDict([('not', OrderedDict([('required', ['opcode_field', "*

 * *            "'load_strategy'])]))])]",*

 * * "'examples'": "{0: {'properties': {'table': 'employees', 'schema': 'dbo', delete: ['table_name', "*

 * *               "'table_schema', 'target_type']}}}",*

 * * "'properties'": "{'keys': OrderedDict([('type', 'array'), ('title', 'Business keys to use in case "*

 * *                 "of `load_strategy` is UPSERT or working with `opcode_field`'), ('items', "*

 * *                 "OrderedDict([('type', ['strin […]*

```diff
@@ -1,51 +1,60 @@
 {
     "additionalProperties": false,
+    "allOf": [
+        {
+            "not": {
+                "required": [
+                    "opcode_field",
+                    "load_strategy"
+                ]
+            }
+        }
+    ],
     "description": "Write into a SQL-compatible data store",
     "examples": [
         {
             "id": "load_snowflake",
             "properties": {
                 "connection": "eu_datalake",
                 "load_strategy": "APPEND",
-                "table_name": "employees",
-                "table_schema": "dbo",
-                "target_type": "database"
+                "schema": "dbo",
+                "table": "employees"
             },
             "type": "relational.write"
         }
     ],
     "properties": {
         "active_record_indicator": {
             "description": "Used for `TYPE2` load_strategy. An SQL expression used to identify which rows are active",
             "examples": [
                 "is_active='Y'",
                 "deletedAt is null"
             ],
             "type": "string"
         },
-        "business_keys": {
-            "items": {
-                "description": "The business key is used for performing an upsert in case the load strategy is UPSERT",
-                "title": "name of column",
-                "type": "string"
-            },
-            "title": "Business keys to use for upsert in case of an UPSERT",
-            "type": "array"
-        },
         "connection": {
             "description": "Logical connection name as defined in the connections.yaml",
             "examples": [
                 "europe_db",
                 "target",
                 "eu_dwh"
             ],
             "title": "The connection to use for loading",
             "type": "string"
         },
+        "foreach": {
+            "description": "Use a JMESPath expression to split a column into multiple records. The expression should be in the format column: expression.",
+            "examples": [
+                "order_line: lines[]"
+            ],
+            "pattern": "^(?!:).*:.*(?<!:)$",
+            "title": "Split a column into multiple records with a JMESPath expression",
+            "type": "string"
+        },
         "inactive_record_mapping": {
             "default": [],
             "description": "A list of columns to use. Use any valid SQL expression for the source. If 'target' is omitted, will default to the name of the source column",
             "examples": [
                 [
                     {
                         "source": "CURRENT_DATE",
@@ -56,25 +65,69 @@
                         "target": "is_active"
                     }
                 ]
             ],
             "title": "Used for `TYPE2` load_strategy. The columns mapping to use to close out an active record",
             "type": "array"
         },
+        "keys": {
+            "examples": [
+                [
+                    "fname",
+                    {
+                        "lname": "last_name"
+                    }
+                ]
+            ],
+            "items": {
+                "title": "name of column",
+                "type": [
+                    "string",
+                    "object"
+                ]
+            },
+            "title": "Business keys to use in case of `load_strategy` is UPSERT or working with `opcode_field`",
+            "type": "array"
+        },
         "load_strategy": {
             "default": "APPEND",
             "description": "type of target",
             "enum": [
                 "APPEND",
                 "REPLACE",
                 "UPSERT",
                 "TYPE2"
             ],
             "type": "string"
         },
+        "mapping": {
+            "examples": [
+                [
+                    "fname",
+                    {
+                        "lname": "last_name"
+                    },
+                    "address",
+                    "gender"
+                ]
+            ],
+            "items": {
+                "title": "name of column",
+                "type": [
+                    "string",
+                    "object"
+                ]
+            },
+            "title": "Fields to write",
+            "type": "array"
+        },
+        "opcode_field": {
+            "description": "Name of the field in the payload that holds the operation (c - create, d - delete, u - update) for this record in the DB",
+            "type": "string"
+        },
         "schema": {
             "description": "If left blank, the default schema of this connection will be used as defined in the connections.yaml",
             "examples": [
                 "dbo"
             ],
             "title": "The table schema of the target table",
             "type": "string"
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import logging
-from typing import Any, Dict, List
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional
 
 from datayoga_core import utils
 from datayoga_core.block import Block as DyBlock
-from datayoga_core.block import Result
 from datayoga_core.context import Context
+from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock):
-    def init(self, context: Context = None):
+class Block(DyBlock, metaclass=ABCMeta):
+
+    def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
-    async def run(self, data: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
         logger.debug(f"Running {self.get_block_name()}")
-        results = []
-
         for row in data:
-            for property in self.properties["fields"]:
+            for prop in self.properties["fields"]:
                 obj = row
-                from_field_path = utils.split_field(property["field"])
+                from_field_path = utils.split_field(prop["field"])
 
                 for index, key in enumerate(from_field_path):
                     key = utils.unescape_field(key)
                     if key in obj:
                         if len(from_field_path) == index + 1:
                             del obj[key]
                         else:
                             obj = obj[key]
-        results.append(Result.SUCCESS)
 
-        return data, results
+        return utils.all_success(data)
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import pytest
-from datayoga_core.block import Result
+from datayoga_core import utils
 from datayoga_core.blocks.remove_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_remove_existing_field():
     block = Block({"field": "fname"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"lname": "doe"}])
 
 
 @pytest.mark.asyncio
 async def test_remove_missing_field():
     block = Block({"field": "mname"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"fname": "john", "lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"fname": "john", "lname": "doe"}])
 
 
 @pytest.mark.asyncio
 async def test_remove_deep_nested_field():
     block = Block({"field": "employee.name.fname"})
     block.init()
-    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == ([
-        {"employee": {"name": {"lname": "doe"}}}], [Result.SUCCESS])
+    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == utils.all_success([
+        {"employee": {"name": {"lname": "doe"}}}])
 
 
 @pytest.mark.asyncio
 async def test_remove_nested_field():
     block = Block({"field": "name.fname"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {"lname": "doe"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {"lname": "doe"}}])
 
 
 @pytest.mark.asyncio
 async def test_remove_missing_nested_field():
     block = Block({"field": "full_name.fname"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {"fname": "john", "lname": "doe"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {"fname": "john", "lname": "doe"}}])
 
 
 @pytest.mark.asyncio
 async def test_remove_multiple_fields():
     block = Block({"fields": [{"field": "name.fname"}, {"field": "name.lname"}]})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {}}])
 
 
 @pytest.mark.asyncio
 async def test_remove_field_with_dot():
     block = Block({"field": "name\.fname"})
     block.init()
-    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == ([{"lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == utils.all_success([{"lname": "doe"}])
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
-from typing import Any, Dict, List, Tuple
+from abc import ABCMeta
+from typing import Any, Dict, List, Optional
 
 from datayoga_core import utils
 from datayoga_core.block import Block as DyBlock
-from datayoga_core.block import Result
 from datayoga_core.context import Context
+from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock):
-    def init(self, context: Context = None):
+class Block(DyBlock, metaclass=ABCMeta):
+
+    def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
-    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
+    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
         logger.debug(f"Running {self.get_block_name()}")
-        results = []
-
         for row in data:
-            for property in self.properties["fields"]:
+            for prop in self.properties["fields"]:
                 key_found = True
                 obj = row
                 value = None
-                from_field_path = utils.split_field(property["from_field"])
+                from_field_path = utils.split_field(prop["from_field"])
 
                 for index, key in enumerate(from_field_path):
                     key = utils.unescape_field(key)
 
                     if key in obj:
                         if len(from_field_path) == index + 1:
                             value = obj[key]
@@ -36,24 +36,23 @@
                             obj = obj[key]
                     else:
                         key_found = False
                         break
 
                 if key_found:
                     obj = row
-                    to_field_path = utils.split_field(property["to_field"])
+                    to_field_path = utils.split_field(prop["to_field"])
 
                     for key in to_field_path[:-1]:
                         key = utils.unescape_field(key)
 
                         if key in obj:
                             obj = obj[key]
                         else:
                             obj[key] = {}
 
                     if key in obj:
                         obj = obj[key]
 
                     obj[utils.unescape_field(to_field_path[-1:][0])] = value
 
-        results.append(Result.SUCCESS)
-        return data, results
+        return utils.all_success(data)
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,80 @@
 import pytest
-from datayoga_core.block import Result
+from datayoga_core import utils
 from datayoga_core.blocks.rename_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_rename_existing_field():
     block = Block(
         {
             "from_field": "fname",
             "to_field": "first_name"
         }
     )
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"first_name": "john", "lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"first_name": "john", "lname": "doe"}])
 
 
 @pytest.mark.asyncio
 async def test_rename_missing_field():
     block = Block(
         {
             "from_field": "mname",
             "to_field": "middle_name"
         }
     )
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"fname": "john", "lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
+        {"fname": "john", "lname": "doe"}])
 
 
 @pytest.mark.asyncio
 async def test_rename_deep_nested_field():
     block = Block(
         {
             "from_field": "employee.name.fname",
             "to_field": "employee.name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == ([
-        {"employee": {"name": {"first_name": "john", "lname": "doe"}}}], [Result.SUCCESS])
+    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == utils.all_success([
+
+        {"employee": {"name": {"first_name": "john", "lname": "doe"}}}])
 
 
 @pytest.mark.asyncio
 async def test_rename_nested_field():
     block = Block(
         {
             "from_field": "name.fname",
             "to_field": "name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
-        {"name": {"first_name": "john", "lname": "doe"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
+        {"name": {"first_name": "john", "lname": "doe"}}])
 
 
 @pytest.mark.asyncio
 async def test_rename_nested_field_missing_to_field_parent():
     block = Block(
         {
             "from_field": "name.fname",
             "to_field": "new_name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
-        {"name": {"lname": "doe"}, "new_name": {"first_name": "john"}}], [Result.SUCCESS])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
+        {"name": {"lname": "doe"}, "new_name": {"first_name": "john"}}])
 
 
 @pytest.mark.asyncio
 async def test_rename_field_with_dot():
     block = Block(
         {
             "from_field": "name\.fname",
             "to_field": "name\.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == ([{"name.first_name": "john", "lname": "doe"}], [Result.SUCCESS])
+    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == utils.all_success([{"name.first_name": "john", "lname": "doe"}])
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/blocks/sequence/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py` & `datayoga_core-1.90.0/src/datayoga_core/blocks/std/read/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-import json
 import logging
 import select
 import sys
 import uuid
-from typing import Any, Dict, Generator, List, Optional
+from typing import Any, AsyncGenerator, Dict, List, Optional
 
+import orjson
 from datayoga_core.context import Context
 from datayoga_core.producer import Message
 from datayoga_core.producer import Producer as DyProducer
 
 logger = logging.getLogger("dy")
 
 
 class Block(DyProducer):
 
     def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
 
-    def produce(self) -> Generator[Message, None, None]:
+    async def produce(self) -> AsyncGenerator[List[Message], None]:
         if select.select([sys.stdin, ], [], [], 0.0)[0]:
             # piped data exists
             for data in sys.stdin:
                 for record in self.get_records(data):
-                    yield self.get_message(record)
+                    yield [self.get_message(record)]
         else:
             # interactive mode
             print("Enter data to process:")
             data = input()
             for record in self.get_records(data):
-                yield self.get_message(record)
+                yield [self.get_message(record)]
 
-    def get_records(self, data: str) -> List[Dict[str, Any]]:
-        records = json.loads(data)
+    @staticmethod
+    def get_records(data: str) -> List[Dict[str, Any]]:
+        records = orjson.loads(data)
 
         if isinstance(records, dict):
             records = [records]
 
         return records
 
     def get_message(self, record: Dict[str, Any]) -> Message:
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md` & `datayoga_core-1.90.0/src/datayoga_core/resources/scaffold/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('properties', OrderedDict([('host', OrderedDict([('description', 'DB "*

 * *            "host'), ('type', 'string')])), ('port', OrderedDict([('description', 'DB port'), "*

 * *            "('type', 'integer'), ('minimum', 1), ('maximum', 65535)])), ('database', "*

 * *            "OrderedDict([('description', 'DB name'), ('type', 'string')])), ('user', "*

 * *            "OrderedDict([('description', 'DB user'), ('type', 'string')])), ('password', "*

 * *            "OrderedDict([('description', 'DB pass […]*

```diff
@@ -1,107 +1,54 @@
 {
-    "additionalProperties": false,
-    "description": "Connection catalog",
-    "patternProperties": {
-        ".": {
-            "anyOf": [
-                {
-                    "additionalProperties": false,
-                    "description": "SQL database",
-                    "examples": [
-                        {
-                            "database": "postgres",
-                            "host": "localhost",
-                            "name": "hr",
-                            "password": "postgres",
-                            "port": 5432,
-                            "type": "postgresql",
-                            "user": "postgres"
-                        }
-                    ],
-                    "properties": {
-                        "database": {
-                            "description": "DB name",
-                            "type": "string"
-                        },
-                        "host": {
-                            "description": "DB host",
-                            "type": "string"
-                        },
-                        "password": {
-                            "description": "DB password",
-                            "type": "string"
-                        },
-                        "port": {
-                            "description": "DB port",
-                            "maximum": 65535,
-                            "minimum": 1,
-                            "type": "integer"
-                        },
-                        "type": {
-                            "description": "DB type",
-                            "pattern": "^(?!redis$)",
-                            "type": "string"
-                        },
-                        "user": {
-                            "description": "DB user",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "type",
-                        "host",
-                        "database",
-                        "user"
-                    ]
-                },
-                {
-                    "additionalProperties": false,
-                    "description": "Redis",
-                    "examples": [
-                        {
-                            "cache": {
-                                "host": "localhost",
-                                "port": 6379,
-                                "type": "redis"
-                            }
-                        }
-                    ],
-                    "properties": {
-                        "host": {
-                            "description": "Redis DB host",
-                            "type": "string"
-                        },
-                        "password": {
-                            "description": "Redis DB password",
-                            "type": "string"
-                        },
-                        "port": {
-                            "description": "Redis DB port",
-                            "maximum": 65535,
-                            "minimum": 1,
-                            "type": "integer"
-                        },
-                        "type": {
-                            "description": "DB type",
-                            "enum": [
-                                "redis"
-                            ],
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "type",
-                        "host",
-                        "port"
-                    ]
-                }
-            ],
+    "examples": [
+        {
+            "hr": {
+                "database": "hr",
+                "host": "localhost",
+                "password": "mypass",
+                "port": 1433,
+                "type": "sqlserver",
+                "user": "myuser"
+            }
+        }
+    ],
+    "properties": {
+        "connect_args": {
+            "additionalProperties": true,
+            "description": "Additional arguments to use when connecting to the DB",
+            "type": "object"
+        },
+        "database": {
+            "description": "DB name",
+            "type": "string"
+        },
+        "host": {
+            "description": "DB host",
+            "type": "string"
+        },
+        "password": {
+            "description": "DB password",
+            "type": "string"
+        },
+        "port": {
+            "description": "DB port",
+            "maximum": 65535,
+            "minimum": 1,
+            "type": "integer"
+        },
+        "query_args": {
+            "additionalProperties": true,
+            "description": "Additional query string arguments to use when connecting to the DB",
             "type": "object"
+        },
+        "user": {
+            "description": "DB user",
+            "type": "string"
         }
     },
-    "title": "Connections",
-    "type": [
-        "object",
-        "null"
+    "required": [
+        "type",
+        "host",
+        "database",
+        "user"
     ]
 }
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json` & `datayoga_core-1.90.0/src/datayoga_core/resources/schemas/job.schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'definitions'": "{'block': {'examples': {3: {'with': {'key': OrderedDict([('expression', 'id'), "*

 * *                  "('language', 'jmespath')]), delete: ['key_field']}}}}}"}*

```diff
@@ -31,15 +31,18 @@
                     }
                 },
                 {
                     "uses": "redis.write",
                     "with": {
                         "command": "HSET",
                         "connection": "cache",
-                        "key_field": "id"
+                        "key": {
+                            "expression": "id",
+                            "language": "jmespath"
+                        }
                     }
                 }
             ],
             "properties": {
                 "uses": {
                     "description": "Block type",
                     "type": "string"
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/step.py` & `datayoga_core-1.90.0/src/datayoga_core/step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,131 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+from asyncio import Task
 from typing import Any, Callable, Dict, List, Optional
 
-from datayoga_core.block import Block, Result
+from datayoga_core import prometheus
+from datayoga_core.block import Block
 from datayoga_core.context import Context
+from datayoga_core.result import Result, Status
 
 logger = logging.getLogger("dy")
 
 
-class Step():
-    def __init__(self, id: str, block: Block, concurrency=1):
-        self.id = id
+class Step:
+    def __init__(self, step_id: str, block: Optional[Block], concurrency=1):
+        self.id = step_id
         self.block = block
         self.next_step = None
         self.active_entries = set()
         self.concurrency = concurrency
-        self.workers = [None]*self.concurrency
+        self.workers: List[Optional[Task]] = [None]*self.concurrency
         self.done_callback = None
         self.initialized = False
 
     def init(self, context: Optional[Context] = None):
         # initialize the block
         self.block.init(context)
-        # start pool of workers for parallelization
 
     async def start_pool(self):
+        # start pool of workers for parallelization
         logger.debug("starting pool")
         self.queue = asyncio.Queue(maxsize=1)
-        for id in range(self.concurrency):
-            worker = self.workers[id]
+        for worker_id in range(self.concurrency):
+            worker = self.workers[worker_id]
             if worker is None or not worker.done():
-                self.workers[id] = asyncio.create_task(self.run(id))
+                self.workers[worker_id] = asyncio.create_task(self.run(worker_id))
             else:
-                logger.debug(f"worker {id} is running: {not worker.done()}")
+                logger.debug(f"worker {worker_id} is running: {not worker.done()}")
 
-    def add_done_callback(self, callback: Callable[[str], None]):
+    def add_done_callback(self, callback: Callable[[List[str], List[Result]], None]):
         self.done_callback = callback
 
     def __or__(self, other: Step):
         return self.append(other)
 
     def append(self, next_step: Step):
         self.next_step = next_step
         self.next_step.add_done_callback(self.done)
         return self.next_step
 
     async def process(self, messages: List[Dict[str, Any]]):
         if not self.initialized:
             await self.start_pool()
             self.initialized = True
-
         self.active_entries.update([x[Block.MSG_ID_FIELD] for x in messages])
         await self.queue.put(messages)
 
     async def run(self, worker_id: int):
         while True:
             entry = await self.queue.get()
             logger.debug(f"{self.id}-{worker_id} processing {[i[Block.MSG_ID_FIELD] for i in entry]}")
             try:
-                processed_entries, results = await self.block.run(entry)
+                processed_entries, filtered_entries, rejected_entries = await self.block.run(entry)
+
+                prometheus.processed_entries.labels(step=self.id).inc(len(processed_entries))
+                prometheus.filtered_records.labels(step=self.id).inc(len(filtered_entries))
+                prometheus.rejected_records.labels(step=self.id).inc(len(rejected_entries))
+
+                # handle filtered. anything not processed or rejected
+                logger.debug(
+                    f"filtered entries: {filtered_entries}, processed entries: {processed_entries}, rejected entries: {rejected_entries}")
+                if filtered_entries:
+                    # ack the filtered entries
+                    self.done([row.payload[Block.MSG_ID_FIELD] for row in filtered_entries],
+                              [Result(Status.FILTERED)] * len(filtered_entries))
+
+                # handle rejected
+                if rejected_entries:
+                    # ack the rejected entries
+                    self.done([row.payload[Block.MSG_ID_FIELD] for row in rejected_entries], rejected_entries)
+
+                if processed_entries:
+                    # check if we have a next step
+                    if self.next_step:
+                        # process downstream
+                        await self.next_step.process([result.payload for result in processed_entries])
+                    else:
+                        # we are a last channel, propagate the ack upstream
+                        # TODO: verify that all entries have a msg id otherwise raise consistency error
+                        self.done([row.payload[Block.MSG_ID_FIELD] for row in processed_entries], processed_entries)
 
-                # TODO: handle filtered. anything not processed or rejected
-                # check if we have a next step
-                if self.next_step:
-                    # process downstream
-                    await self.next_step.process(processed_entries)
-                else:
-                    # we are a last channel, propagate the ack upstream
-                    # TODO: verify that all entries have a msg id otherwise raise consistency error
-                    self.done([x[Block.MSG_ID_FIELD] for x in processed_entries], Result.SUCCESS)
-
-                    # indicate rejected records if any
-                    if Result.REJECTED in results:
-                        self.done([entry[i][Block.MSG_ID_FIELD]
-                                  for i, v in enumerate(results) if v == Result.REJECTED], Result.REJECTED)
             except Exception as e:
                 # we caught an exception. the entire batch is considered rejected
                 logger.exception(e)
                 # verify that all messages still have a msg_id property
                 # if next(filter(lambda x: not Block.MSG_ID_FIELD in x,entry),None) is not None
-                self.done([x[Block.MSG_ID_FIELD] for x in entry],
-                          Result.REJECTED, f"Error in step {self.id}: {repr(e)}")
+                self.done([x[Block.MSG_ID_FIELD] for x in entry], [
+                          Result(Status.REJECTED, f"Error in step {self.id}: {repr(e)}")] * len(entry))
             finally:
                 self.queue.task_done()
-            logger.debug(f"{self.id}-{worker_id} done processing {entry[0][Block.MSG_ID_FIELD]}")
+            logger.debug(f"{self.id}-{worker_id} done processing {entry}")
 
-    def done(self, msg_ids: List[str], result: Optional[Result] = None, reason: Optional[str] = None):
-        logger.debug(f"{self.id} acking {msg_ids} with result {result}")
+    def done(self, msg_ids: List[str], results: List[Result]):
+        logger.debug(f"{self.id} acking {msg_ids}")
         self.active_entries.difference_update(msg_ids)
         if self.done_callback is not None:
-            self.done_callback(msg_ids, result, reason)
+            self.done_callback(msg_ids, results)
 
     async def join(self):
         # wait for all active entries to be processed
         while len(self.active_entries) > 0:
+            logger.debug(f"{self.id} waiting for dangling messages: {self.active_entries}")
             await asyncio.sleep(0.2)
 
     async def stop(self):
         # wait for all tasks to finish
         await self.join()
+        logger.debug("joined")
+
+        # stop the block
+        if self.block:
+            self.block.stop()
 
         # stop any downstream workers
         if self.next_step:
             await self.next_step.stop()
 
         # stop all workers in the pool
         for worker in self.workers:
```

### Comparing `datayoga_core-1.9.0/src/datayoga_core/utils.py` & `datayoga_core-1.90.0/src/datayoga_core/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-import json
+import copy
 import os
 import re
 import sys
+import uuid
 from os import path
 from typing import Any, Dict, List
 
+import orjson
 import yaml
+from datayoga_core import result
+from datayoga_core.block import Block
 from datayoga_core.context import Context
+from datayoga_core.expression import JMESPathExpression
+from datayoga_core.result import BlockResult, Result, Status
 
 
 def read_json(filename: str) -> Any:
     """
     Loads a filename as a JSON object
 
     Args:
         filename (str): JSON filename to load
 
     Returns:
         Any: JSON object
     """
-    with open(filename, "r", encoding="utf8") as f:
-        return json.load(f)
+    with open(filename, "r", encoding="utf8") as json_file:
+        return orjson.loads(json_file.read())
 
 
 def read_yaml(filename: str) -> Dict[str, Any]:
     """
     Loads a filename as a YAML object
 
     Args:
@@ -33,16 +39,16 @@
     Raises:
         ValueError: In case of invalid YAML
 
     Returns:
          Dict[str, Any]: YAML python object
     """
     try:
-        with open(filename, "r", encoding="utf8") as stream:
-            return yaml.safe_load(stream)
+        with open(filename, "r", encoding="utf8") as yaml_file:
+            return yaml.safe_load(yaml_file)
     except Exception as e:
         raise ValueError(f"Malformed YAML: {e}")
 
 
 def format_block_properties(properties: Dict[str, Any]) -> Dict[str, Any]:
     """Adds `fields` array with the passed properties in case it's missing
 
@@ -56,15 +62,15 @@
 
 
 def is_bundled() -> bool:
     return getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS")
 
 
 def get_bundled_dir() -> str:
-    datayoga_dir = path.join(sys._MEIPASS, "datayoga")
+    datayoga_dir = path.join(sys._MEIPASS, "datayoga_core")
     return datayoga_dir if os.path.isdir(datayoga_dir) else sys._MEIPASS
 
 
 def get_resource_path(relative_path: str) -> str:
     if is_bundled():
         # we are running in a bundle
         return path.join(get_bundled_dir(), "resources", relative_path)
@@ -78,13 +84,62 @@
 
 
 def unescape_field(field: str) -> str:
     return field.replace("\\.", ".")
 
 
 def get_connection_details(connection_name: str, context: Context) -> Dict[str, Any]:
-    if context:
-        connection = context.properties.get("connections").get(connection_name)
+    if context and context.properties:
+        connection = context.properties.get("connections", {}).get(connection_name)
         if connection:
             return connection
 
     raise ValueError(f"{connection_name} connection not found")
+
+
+def all_success(records: List[Dict[str, Any]]) -> BlockResult:
+    return BlockResult(processed=[Result(Status.SUCCESS, payload=row) for row in records])
+
+
+def is_rejected(record: Dict[str, Any]) -> bool:
+    return record.get(Block.RESULT_FIELD, result.SUCCESS).status == Status.REJECTED
+
+
+def add_uid(record: Dict[str, Any]) -> Dict[str, Any]:
+    return {Block.MSG_ID_FIELD: f"{uuid.uuid4()}", **record}
+
+
+def remove_msg_id(record: dict) -> dict:
+    return {k: v for k, v in record.items() if k != Block.MSG_ID_FIELD}
+
+
+def explode_records(records: List[Dict[str, Any]], field_expression: str) -> List[Dict[str, Any]]:
+    """
+    Takes a list of records and a JMESPath expression specifying a field to be exploded, and returns a new list of records
+    where each record has been "exploded" into multiple records based on the values in the specified field.
+
+    Args:
+        records (List[Dict[str, Any]]): A list of dictionaries representing records.
+        field_expression (str): A string specifying the field to be exploded, in the form "field_name: expression".
+
+    Returns:
+        List[Dict[str, Any]]: A new list of dictionaries representing the exploded records.
+    """
+    field_name, expression = map(str.strip, field_expression.split(":", maxsplit=1))
+
+    jmespath_expr = JMESPathExpression()
+    jmespath_expr.compile(expression)
+
+    exploded_records = []
+
+    for record in records:
+        # Apply the JMESPath expression to the current record to obtain the values to be exploded.
+        field_values = jmespath_expr.search(record)
+
+        # If the JMESPath expression returned any values, create a new record for each value and add it to the output list.
+        if field_values:
+            for field_value in field_values:
+                new_record = copy.deepcopy(record)
+                new_record[field_name] = field_value
+                exploded_records.append(new_record)
+
+    return exploded_records
```

