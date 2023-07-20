# Comparing `tmp/asynq-1.5.0.tar.gz` & `tmp/asynq-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynq-1.5.0.tar", last modified: Fri May 26 03:42:55 2023, max compression
+gzip compressed data, was "asynq-1.5.1.tar", last modified: Thu Jul 20 19:56:06 2023, max compression
```

## Comparing `asynq-1.5.0.tar` & `asynq-1.5.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:42:55.019339 asynq-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-26 03:42:16.000000 asynq-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-26 03:42:55.019339 asynq-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-26 03:42:16.000000 asynq-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:42:55.011339 asynq-1.5.0/asynq/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/_debug.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/_debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/async_task.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/async_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/async_task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/batching.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/batching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/batching.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/contexts.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/contexts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/decorators.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/futures.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/generator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/mock_.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/mock_.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/profiler.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/profiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scheduler.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scheduler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scoped_value.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scoped_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/scoped_value.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:42:55.019339 asynq-1.5.0/asynq/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/debug_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_active_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_async_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_batching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_recursion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_recursive_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_scoped_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tests/test_yield_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/tools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 03:42:16.000000 asynq-1.5.0/asynq/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:42:55.015339 asynq-1.5.0/asynq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-26 03:42:54.000000 asynq-1.5.0/asynq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-26 03:42:54.000000 asynq-1.5.0/asynq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:42:54.000000 asynq-1.5.0/asynq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 03:42:54.000000 asynq-1.5.0/asynq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 03:42:54.000000 asynq-1.5.0/asynq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 03:42:16.000000 asynq-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:42:55.019339 asynq-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-26 03:42:16.000000 asynq-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:06.785541 asynq-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 19:55:59.000000 asynq-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-20 19:56:06.785541 asynq-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-07-20 19:55:59.000000 asynq-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:06.781541 asynq-1.5.1/asynq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/_debug.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/_debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/async_task.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/async_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/async_task.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/batching.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/batching.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/contexts.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/contexts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/decorators.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/futures.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/mock_.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/mock_.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/profiler.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/profiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scheduler.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scheduler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scoped_value.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scoped_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/scoped_value.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:06.785541 asynq-1.5.1/asynq/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/debug_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_active_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_async_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_recursion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_recursive_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_scoped_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tests/test_yield_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 19:55:59.000000 asynq-1.5.1/asynq/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:06.781541 asynq-1.5.1/asynq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-20 19:56:06.000000 asynq-1.5.1/asynq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-20 19:56:06.000000 asynq-1.5.1/asynq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:56:06.000000 asynq-1.5.1/asynq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 19:56:06.000000 asynq-1.5.1/asynq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 19:56:06.000000 asynq-1.5.1/asynq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 19:55:59.000000 asynq-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:56:06.785541 asynq-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 19:55:59.000000 asynq-1.5.1/setup.py
```

### Comparing `asynq-1.5.0/LICENSE` & `asynq-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/PKG-INFO` & `asynq-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynq
-Version: 1.5.0
+Version: 1.5.1
 Summary: Quora's asynq library
 Home-page: https://github.com/quora/asynq
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
 Keywords: quora asynq common utility
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `asynq-1.5.0/README.rst` & `asynq-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/__init__.py` & `asynq-1.5.1/asynq/__init__.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/__init__.pyi` & `asynq-1.5.1/asynq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/_debug.pxd` & `asynq-1.5.1/asynq/_debug.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/_debug.py` & `asynq-1.5.1/asynq/_debug.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/_debug.pyi` & `asynq-1.5.1/asynq/_debug.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/async_task.pxd` & `asynq-1.5.1/asynq/async_task.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/async_task.py` & `asynq-1.5.1/asynq/async_task.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/async_task.pyi` & `asynq-1.5.1/asynq/async_task.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/batching.pxd` & `asynq-1.5.1/asynq/batching.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/batching.py` & `asynq-1.5.1/asynq/batching.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/batching.pyi` & `asynq-1.5.1/asynq/batching.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/contexts.pxd` & `asynq-1.5.1/asynq/contexts.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/contexts.py` & `asynq-1.5.1/asynq/contexts.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/contexts.pyi` & `asynq-1.5.1/asynq/contexts.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/debug.py` & `asynq-1.5.1/asynq/debug.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/debug.pyi` & `asynq-1.5.1/asynq/debug.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/decorators.pxd` & `asynq-1.5.1/asynq/decorators.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/decorators.py` & `asynq-1.5.1/asynq/decorators.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/decorators.pyi` & `asynq-1.5.1/asynq/decorators.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/futures.pxd` & `asynq-1.5.1/asynq/futures.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/futures.py` & `asynq-1.5.1/asynq/futures.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/futures.pyi` & `asynq-1.5.1/asynq/futures.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/generator.py` & `asynq-1.5.1/asynq/generator.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/generator.pyi` & `asynq-1.5.1/asynq/generator.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/mock_.py` & `asynq-1.5.1/asynq/mock_.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/profiler.py` & `asynq-1.5.1/asynq/profiler.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scheduler.pxd` & `asynq-1.5.1/asynq/scheduler.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scheduler.py` & `asynq-1.5.1/asynq/scheduler.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scheduler.pyi` & `asynq-1.5.1/asynq/scheduler.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scoped_value.pxd` & `asynq-1.5.1/asynq/scoped_value.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scoped_value.py` & `asynq-1.5.1/asynq/scoped_value.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/scoped_value.pyi` & `asynq-1.5.1/asynq/scoped_value.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/__init__.py` & `asynq-1.5.1/asynq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/caching.py` & `asynq-1.5.1/asynq/tests/caching.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/debug_cache.py` & `asynq-1.5.1/asynq/tests/debug_cache.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/helpers.py` & `asynq-1.5.1/asynq/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_active_task.py` & `asynq-1.5.1/asynq/tests/test_active_task.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_async_task.py` & `asynq-1.5.1/asynq/tests/test_async_task.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_base.py` & `asynq-1.5.1/asynq/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_batching.py` & `asynq-1.5.1/asynq/tests/test_batching.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_channels.py` & `asynq-1.5.1/asynq/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_contexts.py` & `asynq-1.5.1/asynq/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_debug.py` & `asynq-1.5.1/asynq/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_decorators.py` & `asynq-1.5.1/asynq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_exceptions.py` & `asynq-1.5.1/asynq/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_futures.py` & `asynq-1.5.1/asynq/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_generator.py` & `asynq-1.5.1/asynq/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_mock.py` & `asynq-1.5.1/asynq/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_multiple_inheritance.py` & `asynq-1.5.1/asynq/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_performance.py` & `asynq-1.5.1/asynq/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_profiler.py` & `asynq-1.5.1/asynq/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_recursion.py` & `asynq-1.5.1/asynq/tests/test_recursion.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_recursive_task.py` & `asynq-1.5.1/asynq/tests/test_recursive_task.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_scoped_value.py` & `asynq-1.5.1/asynq/tests/test_scoped_value.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_tools.py` & `asynq-1.5.1/asynq/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_utils.py` & `asynq-1.5.1/asynq/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tests/test_yield_result.py` & `asynq-1.5.1/asynq/tests/test_yield_result.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tools.py` & `asynq-1.5.1/asynq/tools.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/tools.pyi` & `asynq-1.5.1/asynq/tools.pyi`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/utils.pxd` & `asynq-1.5.1/asynq/utils.pxd`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq/utils.py` & `asynq-1.5.1/asynq/utils.py`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/asynq.egg-info/PKG-INFO` & `asynq-1.5.1/asynq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynq
-Version: 1.5.0
+Version: 1.5.1
 Summary: Quora's asynq library
 Home-page: https://github.com/quora/asynq
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
 Keywords: quora asynq common utility
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `asynq-1.5.0/asynq.egg-info/SOURCES.txt` & `asynq-1.5.1/asynq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asynq-1.5.0/setup.py` & `asynq-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 DATA_FILES = (
     ["py.typed"]
     + ["%s.pxd" % module for module in CYTHON_MODULES]
     + [os.path.relpath(f, "asynq/") for f in glob.glob("asynq/*.pyi")]
 )
 
-VERSION = "1.5.0"
+VERSION = "1.5.1"
 
 
 EXTENSIONS = [
     Extension("asynq.%s" % module, ["asynq/%s.py" % module])
     for module in CYTHON_MODULES
 ]
 
@@ -71,10 +71,10 @@
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
         keywords="quora asynq common utility",
         packages=["asynq", "asynq.tests"],
         package_data={"asynq": DATA_FILES},
         ext_modules=EXTENSIONS,
-        setup_requires=["Cython>=0.27.1", "qcore", "setuptools"],
+        setup_requires=["Cython==0.29.36", "qcore", "setuptools"],
         install_requires=["Cython>=0.27.1", "qcore", "pygments"],
     )
```

