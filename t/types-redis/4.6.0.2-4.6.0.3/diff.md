# Comparing `tmp/types-redis-4.6.0.2.tar.gz` & `tmp/types-redis-4.6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-redis-4.6.0.2.tar", last modified: Tue Jul  4 12:35:40 2023, max compression
+gzip compressed data, was "types-redis-4.6.0.3.tar", last modified: Thu Jul 20 15:21:45 2023, max compression
```

## Comparing `types-redis-4.6.0.2.tar` & `types-redis-4.6.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-07-04 12:35:39.000000 types-redis-4.6.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 12:35:39.000000 types-redis-4.6.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.071445 types-redis-4.6.0.2/redis-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 12:35:39.000000 types-redis-4.6.0.2/redis-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.071445 types-redis-4.6.0.2/redis-stubs/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47591 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/asyncio/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/backoff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41603 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.071445 types-redis-4.6.0.2/redis-stubs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.071445 types-redis-4.6.0.2/redis-stubs/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/bf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/bf/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/bf/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    72403 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/redis-stubs/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/edge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/graph/query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/redis-stubs/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/json/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/json/decoders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/json/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/redismodules.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/redis-stubs/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/search/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/search/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/search/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/search/result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/sentinel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/redis-stubs/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/timeseries/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/timeseries/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/timeseries/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/commands/timeseries/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/ocsp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 12:35:20.000000 types-redis-4.6.0.2/redis-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-04 12:35:39.000000 types-redis-4.6.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:35:40.075445 types-redis-4.6.0.2/types_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 12:35:40.000000 types-redis-4.6.0.2/types_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-04 12:35:40.000000 types-redis-4.6.0.2/types_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:35:40.000000 types-redis-4.6.0.2/types_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 12:35:40.000000 types-redis-4.6.0.2/types_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 12:35:40.000000 types-redis-4.6.0.2/types_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.785192 types-redis-4.6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-20 15:21:45.785192 types-redis-4.6.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.777192 types-redis-4.6.0.3/redis-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/redis-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.777192 types-redis-4.6.0.3/redis-stubs/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47591 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/asyncio/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/backoff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41603 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.777192 types-redis-4.6.0.3/redis-stubs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.777192 types-redis-4.6.0.3/redis-stubs/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/bf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/bf/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/bf/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    72403 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.781192 types-redis-4.6.0.3/redis-stubs/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/graph/query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.781192 types-redis-4.6.0.3/redis-stubs/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/json/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/json/decoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/json/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/redismodules.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.781192 types-redis-4.6.0.3/redis-stubs/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/search/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/search/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/search/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/search/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/sentinel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.781192 types-redis-4.6.0.3/redis-stubs/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/timeseries/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/timeseries/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/timeseries/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/commands/timeseries/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/ocsp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-20 15:15:13.000000 types-redis-4.6.0.3/redis-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:45.785192 types-redis-4.6.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-20 15:21:44.000000 types-redis-4.6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:45.785192 types-redis-4.6.0.3/types_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/types_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/types_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/types_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/types_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:21:45.000000 types-redis-4.6.0.3/types_redis.egg-info/top_level.txt
```

### Comparing `types-redis-4.6.0.2/CHANGELOG.md` & `types-redis-4.6.0.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.6.0.3 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 4.6.0.2 (2023-07-04)
 
 Redis: Add missing types for id in xadd (#10403)
 
 ## 4.6.0.1 (2023-07-01)
 
 Use proper return types for `__await__` methods in `redis.asyncio.client` (#10379)
```

### Comparing `types-redis-4.6.0.2/PKG-INFO` & `types-redis-4.6.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.6.0.2
+Version: 4.6.0.3
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc7d4722eaa54803926cee5730e1f784979c0531` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-redis-4.6.0.2/redis-stubs/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/client.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/cluster.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/connection.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/lock.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/retry.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/sentinel.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/asyncio/utils.pyi` & `types-redis-4.6.0.3/redis-stubs/asyncio/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/backoff.pyi` & `types-redis-4.6.0.3/redis-stubs/backoff.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/client.pyi` & `types-redis-4.6.0.3/redis-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/cluster.pyi` & `types-redis-4.6.0.3/redis-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/bf/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/bf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/bf/commands.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/bf/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/bf/info.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/bf/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/cluster.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/core.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/core.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/graph/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/graph/commands.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/graph/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/graph/query_result.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/graph/query_result.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/json/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/json/commands.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/json/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/search/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/search/aggregation.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/search/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/search/commands.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/search/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/search/query.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/search/query.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/sentinel.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/timeseries/__init__.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/timeseries/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/timeseries/commands.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/timeseries/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/commands/timeseries/info.pyi` & `types-redis-4.6.0.3/redis-stubs/commands/timeseries/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/connection.pyi` & `types-redis-4.6.0.3/redis-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/exceptions.pyi` & `types-redis-4.6.0.3/redis-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/lock.pyi` & `types-redis-4.6.0.3/redis-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/ocsp.pyi` & `types-redis-4.6.0.3/redis-stubs/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/sentinel.pyi` & `types-redis-4.6.0.3/redis-stubs/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/typing.pyi` & `types-redis-4.6.0.3/redis-stubs/typing.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/redis-stubs/utils.pyi` & `types-redis-4.6.0.3/redis-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.2/setup.py` & `types-redis-4.6.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc7d4722eaa54803926cee5730e1f784979c0531` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.6.0.2",
+      version="4.6.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md",
```

### Comparing `types-redis-4.6.0.2/types_redis.egg-info/PKG-INFO` & `types-redis-4.6.0.3/types_redis.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.6.0.2
+Version: 4.6.0.3
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc7d4722eaa54803926cee5730e1f784979c0531` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-redis-4.6.0.2/types_redis.egg-info/SOURCES.txt` & `types-redis-4.6.0.3/types_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

