# Comparing `tmp/pastis-framework-1.0.3.tar.gz` & `tmp/pastis-framework-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastis-framework-1.0.3.tar", last modified: Wed Jun 28 20:39:28 2023, max compression
+gzip compressed data, was "pastis-framework-1.0.4.tar", last modified: Thu Jul 20 13:50:18 2023, max compression
```

## Comparing `pastis-framework-1.0.3.tar` & `pastis-framework-1.0.4.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15144 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/bin/pastis-benchmark
--rwxr-xr-x   0 runner    (1001) docker     (123)     5013 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/bin/pastis-broker
--rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/bin/pastisd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.487368 pastis-framework-1.0.3/engines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.487368 pastis-framework-1.0.3/engines/pastis-aflpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-aflpp/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/bin/pastis-aflpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.487368 pastis-framework-1.0.3/engines/pastis-aflpp/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-aflpp/broker-addon/aflppbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/aflpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.487368 pastis-framework-1.0.3/engines/pastis-honggfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-honggfuzz/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/bin/pastis-honggfuzz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.487368 pastis-framework-1.0.3/engines/pastis-honggfuzz/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-honggfuzz/broker-addon/hfbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/honggfuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-triton/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-triton/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9813 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-triton/bin/pastis-triton
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-triton/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-triton/broker-addon/pastisttbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/engines/pastis-triton/pastisdse/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-triton/pastisdse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40781 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/engines/pastis-triton/pastisdse/pastisdse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.491368 pastis-framework-1.0.3/libpastis/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/enginedesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/libpastis/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/proto/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/sast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/libpastis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/pastis_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-28 20:39:28.000000 pastis-framework-1.0.3/pastis_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-28 20:39:28.000000 pastis-framework-1.0.3/pastis_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:39:28.000000 pastis-framework-1.0.3/pastis_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-28 20:39:28.000000 pastis-framework-1.0.3/pastis_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-28 20:39:28.000000 pastis-framework-1.0.3/pastis_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/pastisbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbenchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbenchmark/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbenchmark/replayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbenchmark/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/pastisbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31511 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/stat_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/pastisbroker/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 20:39:28.495368 pastis-framework-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-28 20:39:27.000000 pastis-framework-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16319 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastis-benchmark
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastis-broker
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastisd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/bin/pastis-aflpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/aflpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/pastis-honggfuzz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/honggfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-triton/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/bin/pastis-triton
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40564 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/pastisdse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/libpastis/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/enginedesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/libpastis/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/proto/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/sast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastis_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastisbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/replayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastisbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35282 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10450 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/stat_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/setup.py
```

### Comparing `pastis-framework-1.0.3/LICENSE` & `pastis-framework-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/PKG-INFO` & `pastis-framework-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.3
+Version: 1.0.4
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.3/README.md` & `pastis-framework-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/bin/pastis-benchmark` & `pastis-framework-1.0.4/bin/pastis-benchmark`

 * *Files 4% similar despite different names*

```diff
@@ -154,28 +154,49 @@
 @click.option('-p', '--port', type=int, default=5555, help="Port to bind to", multiple=False)
 @click.option('--hfuzz-path', type=click.Path(exists=True, file_okay=True, dir_okay=True, readable=True), required=False, help="Custom Honggfuzz path")
 @click.option('--hfuzz-threads', type=int, default=0, help="Number of threads to launch Honggfuzz with")
 @click.option('--spawn/--no-spawn', type=bool, is_flag=True, default=True, help="Either to spawn engines or not")
 @click.option("--allow-remote", type=bool, is_flag=True, default=False, help="Enable remote connection")
 @click.option('--probe', type=str, help="Probe to load as a python module (should contain a ProbeInterface)", multiple=True)
 @click.option('--skip-cpufreq', is_flag=True, type=bool, default=False, help="Skip CPU frequency scaling check")
+@click.option('--mem-threshold', type=int, default=85, help="RAM consumption limit", show_default=True)
 @click.option('--start-quorum', type=int, default=0, help="Number of client connection to receive before triggering startup", show_default=True)
-@click.option('--proxy', type=str, default="", help="Run the broker as a proxy to another broker")
+@click.option('--filter-inputs', type=bool, is_flag=True, default=False, help="Filter inputs that do not generate coverage", show_default=True)
+@click.option('--stream', type=bool, is_flag=True, default=False, help="Stream input and coverage info in the given file", show_default=True)
+@click.option('--replay-threads', type=int, default=4, help="number of threads to use for input replay", show_default=True)
+@click.option('--proxy', type=str, default="", help="Run the broker as a proxy to another broker: pymodule@ip:port")
+@click.argument('pargs', nargs=-1)
 def run(workspace: str, bins: str, seeds: str, mode: str, injloc: str, aflpp: bool, hfuzz: bool, triton: bool,
         debug: bool, timeout: Optional[int], port: int, hfuzz_path: str, hfuzz_threads: int, spawn: bool,
-        allow_remote: bool, probe: Tuple[str], skip_cpufreq: bool, start_quorum: int, proxy: str):
+        allow_remote: bool, probe: Tuple[str], skip_cpufreq: bool,  mem_threshold: int, start_quorum: int,  proxy: str,
+        filter_inputs: bool, stream: bool, replay_threads: int, pargs: Tuple[str]):
 
     configure_logging(logging.DEBUG if debug else logging.INFO, "%(asctime)s %(name)s [%(levelname)s] %(message)s")
 
-    broker = PastisBroker(workspace, bins, BrokingMode[mode], CheckMode.CHECK_ALL, SeedInjectLoc[injloc], None, [], start_quorum=start_quorum)
+    broker = PastisBroker(workspace,
+                          bins,
+                          BrokingMode[mode],
+                          CheckMode.CHECK_ALL,
+                          SeedInjectLoc[injloc],
+                          None,
+                          list(pargs),
+                          mem_threshold,
+                          start_quorum,
+                          filter_inputs,
+                          stream,
+                          replay_threads)
 
     if proxy:  # proxy format should be:  IP:port@py_module
-        url, py_module = proxy.split("@")
-        proxy_ip, proxy_port = url.split(":")
-        broker.set_proxy(proxy_ip, int(proxy_port), py_module)
+        try:
+            py_module, url = proxy.split("@")
+            proxy_ip, proxy_port = url.split(":")
+            broker.set_proxy(proxy_ip, int(proxy_port), py_module)
+        except ValueError:
+            logging.error(f"Cannot parse proxy: {proxy}, format need to be: py_module@ip:port")
+            return
 
     # Add all given seeds as initial seed
     if seeds is None:
         logging.warning("no initial corpus provided")
     else:
         for s in iterate_seeds(seeds):  # File if one file, or iterate dir if directory
             broker.add_seed_file(s, initial=True)
```

### Comparing `pastis-framework-1.0.3/bin/pastis-broker` & `pastis-framework-1.0.4/bin/pastis-broker`

 * *Files 11% similar despite different names*

```diff
@@ -50,27 +50,42 @@
 @click.option('--tt-config', type=click.Path(exists=True, file_okay=True, dir_okay=True, readable=True), help="Triton configuration file")
 @click.option('--hf-config', type=click.Path(exists=True, file_okay=True, dir_okay=True, readable=True), help="Honggfuzz configuration file")
 @click.option('-s', "--seed", type=click.Path(exists=True, file_okay=True, dir_okay=True, readable=True), help="Initial seed or directory of seeds to give as initial corpus", multiple=True)
 @click.option('-t', "--timeout", type=int, default=None, help="Timeout of the campaign. Time after which stopping the campaign")
 @click.option('-p', '--port', type=int, default=5555, help="Port to bind to", multiple=False, show_default=True)
 @click.option('--mem-threshold', type=int, default=85, help="RAM consumption limit", show_default=True)
 @click.option('--start-quorum', type=int, default=0, help="Number of client connection to receive before triggering startup", show_default=True)
+@click.option('--filter-inputs', type=bool, is_flag=True, default=False, help="Filter inputs that do not generate coverage", show_default=True)
+@click.option('--stream', type=bool, is_flag=True, default=False, help="Stream input and coverage info in the given file", show_default=True)
+@click.option('--replay-threads', type=int, default=4, help="number of threads to use for input replay", show_default=True)
 @click.argument('pargvs', nargs=-1)
 def main(workspace: str, sast_report: Optional[str], bins: str, mode: str, chkmode: str, injloc: str, engine: Tuple[str],
          tt_config: Optional[str], hf_config: Optional[str], seed: Tuple[str], timeout: Optional[int],
-         port: Optional[int], pargvs: Tuple[str], mem_threshold: int, start_quorum: int):
+         port: Optional[int], pargvs: Tuple[str], mem_threshold: int, start_quorum: int, filter_inputs: bool,
+         stream: bool, replay_threads: int):
     global broker
     # Instanciate the broker
 
     chkmode = CheckMode[chkmode]
     if chkmode in [CheckMode.ALERT_ONLY, CheckMode.ALERT_ONE] and not sast_report:
         logging.error(f"Check mode {chkmode.name} requires a SAST report (use -r) to provide it")
         sys.exit(1)
 
-    broker = PastisBroker(workspace, bins, BrokingMode[mode], chkmode, SeedInjectLoc[injloc], sast_report, list(pargvs), mem_threshold, start_quorum)
+    broker = PastisBroker(workspace,
+                          bins,
+                          BrokingMode[mode],
+                          chkmode,
+                          SeedInjectLoc[injloc],
+                          sast_report,
+                          list(pargvs),
+                          mem_threshold,
+                          start_quorum,
+                          filter_inputs,
+                          stream,
+                          replay_threads)
 
     # Preload all Fuzzing engine if needed
     for eng in engine:
         broker.load_engine_addon(eng)
 
     # Add all the triton configuration if the parameter was a directory
     if tt_config:
```

### Comparing `pastis-framework-1.0.3/bin/pastisd` & `pastis-framework-1.0.4/bin/pastisd`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/bin/pastis-aflpp` & `pastis-framework-1.0.4/engines/pastis-aflpp/bin/pastis-aflpp`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/__init__.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/aflpp.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/aflpp.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,22 @@
         if root_dir:
             bin_path = Path(root_dir) / AFLPPProcess.BINARY
             return bin_path if bin_path.exists() else None
         else:
             aflpp_path = os.environ.get(AFLPPProcess.AFLPP_ENV_VAR)
             return Path(aflpp_path) / 'afl-fuzz' if aflpp_path else shutil.which(AFLPPProcess.BINARY)
 
-    def start(self, target: str, target_arguments: str, workspace: Workspace, exmode: ExecMode, fuzzmode: FuzzMode, stdin: bool, engine_args: str, cmplog: Optional[str] = None, dictionary: Optional[str] = None):
+    def start(self, target: str, target_arguments: list[str], workspace: Workspace, exmode: ExecMode, fuzzmode: FuzzMode, stdin: bool, engine_args: str, cmplog: Optional[str] = None, dictionary: Optional[str] = None):
+        # Check that we have '@@' if input provided via argv
+        if not stdin:
+            if "@@" not in target_arguments:
+                logging.error(f"seed provided via ARGV but can't find '@@' on program argv")
+                return
         # Build target command line.
-        target_cmdline = f"{target} {target_arguments}"
+        target_cmdline = f"{target} {' '.join(target_arguments)}"
 
         # Build fuzzer arguments.
         # NOTE: Assuming the target receives inputs from stdin.
         aflpp_arguments = ' '.join([
             re.sub(r"\s", " ", engine_args),  # Any arguments coming right from the broker (remove \r\n)
             f"-Q" if fuzzmode == FuzzMode.BINARY_ONLY else "",
             f"-M main", # Master MODE, seed distribution is ensured by the broker
@@ -74,18 +79,14 @@
         # TODO Should we skip these steps?
         os.environ["AFL_SKIP_CPUFREQ"] = "1"
         os.environ["AFL_I_DONT_CARE_ABOUT_MISSING_CRASHES"] = "1"
 
         # Build fuzzer command line.
         aflpp_cmdline = f'{self.__path} {aflpp_arguments} -- {target_cmdline}'
 
-        # NOTE: Assuming fixed location for the input file.
-        if not stdin:
-            aflpp_cmdline += " @@"
-
         logging.info(f"Run AFL++: {aflpp_cmdline}")
         logging.debug(f"\tWorkspace: {workspace.root_dir}")
 
         # Remove empty strings when converting the command to a list.
         command = list(filter(None, aflpp_cmdline.split(' ')))
 
         # Open logfile (stdout will be redirected to this file).
```

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/driver.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.__package = package
         self.__target_args = argv
 
         self.workspace.start()  # Start looking at directories
 
         logging.info(f"Start process (injectloc: {seed_inj.name})")
         self.aflpp.start(str(package.executable_path.absolute()),
-                         " ".join(argv),
+                         argv,
                          self.workspace,
                          exmode,
                          fuzzmode,
                          seed_inj == SeedInjectLoc.STDIN,
                          engine_args,
                          str(package.cmplog.absolute()) if package.cmplog else None,
                          str(package.dictionary.absolute()) if package.dictionary else None)
```

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/replay.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-aflpp/pastisaflpp/workspace.py` & `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/bin/pastis-honggfuzz` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/pastis-honggfuzz`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/__init__.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/driver.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,23 +74,23 @@
         # Write target to disk.
         self.__package = package
         self.__target_args = argv
 
         self.workspace.start()  # Start looking at directories
 
         logging.info("Start process")
-        if not self.honggfuzz.start(self.__package.executable_path.absolute(),
-                             " ".join(argv),
+        if not self.honggfuzz.start(str(self.__package.executable_path.absolute()),
+                             argv,
                              self.workspace,
                              exmode,
                              fuzzmode,
                              seed_inj == SeedInjectLoc.STDIN,
                              engine_args,
                              str(package.dictionary.absolute()) if package.dictionary else None):
-            self._agent.send_log(LogLevel.ERROR, "Cannot start target, HFQBDIPRELAOD not found")
+            self._agent.send_log(LogLevel.ERROR, "Cannot start target")
         self._started = True
 
         # Start the replay worker (note that the queue might already have started to be filled by agent thread)
         self._replay_thread = threading.Thread(target=self.replay_worker, daemon=True)
         self._replay_thread.start()
 
     def stop(self):
```

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/honggfuzz.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/honggfuzz.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,27 @@
             if not path.exists():
                 raise Exception("Can't find honggfuzz in HFUZZ_PATH path!")
 
         self._threads = os.environ.get(self.HFUZZ_THREADS_VAR)
 
         self.__process = None
 
-    def start(self, target: str, target_arguments: str, workspace: Workspace, exmode: ExecMode, fuzzmode: FuzzMode,
+    def start(self, target: str, target_arguments: list[str], workspace: Workspace, exmode: ExecMode, fuzzmode: FuzzMode,
               stdin: bool, engine_args: str, dictionary: Optional[str] = None) -> bool:
+        if not stdin:
+            if "@@" in target_arguments:  # Change '@@' for ___FILE___
+                idx = target_arguments.index("@@")
+                target_arguments[idx] = "___FILE___"
+            else:
+                if "___FILE___" not in target_arguments:
+                    logging.error(f"seed provided via ARGV but can't find '@@'/___FILE___ on program argv")
+                    return False
+
         # Build target command line.
-        target_cmdline = f"{target} {target_arguments}"
+        target_cmdline = f"{target} {' '.join(target_arguments)}"
 
         HFQBDI_LIB_PATH = os.getenv('HFQBDI_LIB_PATH')
 
         if fuzzmode == FuzzMode.BINARY_ONLY and HFQBDI_LIB_PATH is None:
             logging.error(f"target in BINARY_ONLY but can't find HFQBDI_LIB_PATH")
             return False
 
@@ -74,18 +83,14 @@
             f"--threads {self._threads}" if self._threads else "",
             f"--dict {dictionary}" if dictionary is not None else ""
         ])
 
         # Build fuzzer command line.
         hfuzz_cmdline = f'{self.__path} {hfuzz_arguments} -- {target_cmdline}'
 
-        # NOTE: Assuming fixed location for the input file.
-        if not stdin:
-            hfuzz_cmdline += " ___FILE___"
-
         logging.info(f"Run Honggfuzz with: {hfuzz_cmdline}")
         logging.debug(f"\tWorkspace: {workspace.root_dir}")
 
         # Remove empty strings when converting the command to a list.
         command = list(filter(None, hfuzz_cmdline.split(' ')))
 
         # Create a new fuzzer process and set it apart into a new process group.
```

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/replay.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-honggfuzz/pastishf/workspace.py` & `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-triton/bin/pastis-triton` & `pastis-framework-1.0.4/engines/pastis-triton/bin/pastis-triton`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 from libpastis import ClientAgent, FileAgent
 from libpastis.types import ExecMode, CoverageMode, SeedInjectLoc, CheckMode, FuzzingEngineInfo, SeedType, FuzzMode
 
 # Local imports
 from pastisdse import PastisDSE, __version__
 from tritondse import CoverageStrategy, ProbeInterface, Config, SmtSolver
 from tritondse.probes.basic_trace import BasicDebugTrace
+import tritondse.logging
 
 pastis = None
 
 
 def configure_logs(level: int):
+    tritondse.logging.enable(level)  # Enable tritondse to print logging information
     coloredlogs.install(level=level,
                         fmt="%(asctime)s %(threadName)s [%(levelname)s] %(message)s",
                         level_styles={'debug': {'color': 'blue'}, 'info': {'color': 'white'}, 'warning': {'color': 'yellow'},
                                       'error': {'color': 'red'}, 'critical': {'bold': True, 'color': 'red'}},
                         field_styles={'asctime': {'color': 'white'}, 'levelname': {'bold': True}})
 
 
@@ -52,26 +54,29 @@
 def cli():
     pass
 
 
 @cli.command()
 @click.option('-h', '--host', type=str, default='localhost', help='Host to connect to')
 @click.option('-p', '--port', type=int, default=5555, help='Port to connect to')
+@click.option('--debug', type=bool,  is_flag=True, show_default=True, default=False, help='Enable debug logs')
 @click.option('--probe', type=str, help="Probe to load as a python module (should contain a ProbeInterface)", multiple=True)
-def online(host: str, port: int, probe: Tuple[str]):
+def online(host: str, port: int, debug: bool, probe: Tuple[str]):
     """
     This is the online mode of the pastis-triton exploration. With this mode,
     the client (pastis-triton) will try to connect to the broker. Then, the broker
     will send us the binary to explore, the configuration and initiale seeds.
 
     :param host: The remote host to connect
     :param port: The remote host's port to connect
+    :param debug: Configure debugging logs
+    :param probe: Probes to enable (Python modules imported with importlib)
     """
 
-    configure_logs(logging.INFO)
+    configure_logs(logging.DEBUG if debug else logging.INFO)
 
     # Create the network agent and connect to the broker
     agent = ClientAgent()
 
     # Instanciate the pastis that will register the appropriate callbacks
     pastis = PastisDSE(agent)
 
@@ -166,19 +171,15 @@
     pastis = PastisDSE(agent)
 
     if config:
         config = Config.from_file(config)
     else:
         config = Config()
 
-    if debug:
-        configure_logs(logging.DEBUG)
-        config.debug = True
-    else:
-        configure_logs(logging.INFO)
+    configure_logs(logging.DEBUG if debug else logging.INFO)
 
     if trace:
         pastis.add_probe(BasicDebugTrace())
 
     if workspace:
         config.workspace = workspace
```

### Comparing `pastis-framework-1.0.3/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py` & `pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/engines/pastis-triton/pastisdse/pastisdse.py` & `pastis-framework-1.0.4/engines/pastis-triton/pastisdse/pastisdse.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     TMP_SEED = "seed.seed"
     TMP_TRACE = "result.trace"
 
     def __init__(self, agent: ClientAgent):
         self.agent = agent
         self._init_callbacks()  # register callbacks on the given agent
 
-        self.config = Config(debug=False)
+        self.config = Config()
         self.config.workspace = ""  # Reset workspace so that it will computed in start_received
         self.dse        = None
         self.program    = None
         self._stop      = False
         self.sast_report= None
         self._last_id = None
         self._last_id_pc = None
@@ -96,15 +96,15 @@
     def start(self):
         self._th = threading.Thread(target=self.run, daemon=True)
         self._th.start()
 
     def reset(self):
         """ Reset the current DSE to be able to restart from fresh settings """
         self.dse = None  # remove DSE object
-        self.config = Config(debug=False)
+        self.config = Config()
         self.config.workspace = ""  # Reset workspace so that it will computed in start_received
         self._last_id_pc = None
         self._last_id = None
         self.sast_report = None
         self._program_slice = None
         self._seed_received = set()
         self.program = None
@@ -308,21 +308,20 @@
             return
 
         self._seedloc = seed_inj
 
         # ------- Create the TritonDSE configuration file ---------
         if engine_args:
             self.config = Config.from_json(engine_args)
-            logging.root.level = logging.DEBUG if self.config.debug else logging.INFO  # dynamically change level
         else:
             self.config = Config()  # Empty configuration
-
-        # Override config argv if provided
-        if argv:
-            self.config.program_argv = argv
+            # Use argv ONLY if no configuration provided
+            self.config.program_argv = [f"./{fname}"]
+            if argv:
+                self.config.program_argv.extend(argv) # Preprend the binary to argv
 
         """
         Actions taken depending on seed format & co:
         Config    |  Inject  |  Result
         RAW          STDIN      /
         COMPOSITE    STDIN      / (but need 'stdin' in files)
         RAW          ARGV       change to COMPOSITE to be able to inject on argv (and convert seeds on the fly)
@@ -531,17 +530,14 @@
                         argv = self.config.program_argv[:]
                         idx = argv.index(self.INPUT_FILE_NAME)
                         argv[idx] = str(self.replay_seed_file)
                     except ValueError:
                         logging.error(f"seed injection {self._seedloc.name} but can't find 'input_file' on program argv")
                         return
 
-                # set the longjmp addr if defined
-                if hasattr(self.program, "longjmp_addr"):
-                    os.environ["TT_LONGJMP_ADDR"] = str(self.program.longjmp_addr)
                 try:
                     # Run the seed and determine whether it improves our current coverage.
                     t0 = time.time()
                     if QBDITrace.run(self.config.coverage_strategy,
                                           str(self.program.path.resolve()),
                                           argv[1:] if len(argv) > 1 else [],
                                           output_path=str(self.replay_trace_file),
@@ -563,15 +559,15 @@
                     # Add the seed anyway, if it was not possible to re-run the seed.
                     # TODO Set seed.coverage_objectives as "empty" (use ellipsis
                     # object). Modify WorklistAddressToSet to support it.
                     self.seeds_merged += 1
                     self.dse.add_input_seed(seed)
                 else:
                     # Check whether the seed improves the current coverage.
-                    if self.dse.coverage.improves_coverage(coverage):
+                    if self.dse.coverage.improve_coverage(coverage):
                         logging.info(f"seed added {seed.hash} [{typ.name}] (coverage merged)")
                         self.seeds_merged += 1
                         self.dse.coverage.merge(coverage)
                         self.dse.seeds_manager.worklist.update_worklist(coverage)
 
                         seed.coverage_objectives = self.dse.coverage.new_items_to_cover(coverage)
                         self.dse.add_input_seed(seed)
```

### Comparing `pastis-framework-1.0.3/libpastis/agent.py` & `pastis-framework-1.0.4/libpastis/agent.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/enginedesc.py` & `pastis-framework-1.0.4/libpastis/enginedesc.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/package.py` & `pastis-framework-1.0.4/libpastis/package.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/proto/message_pb2.py` & `pastis-framework-1.0.4/libpastis/proto/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/sast.py` & `pastis-framework-1.0.4/libpastis/sast.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/types.py` & `pastis-framework-1.0.4/libpastis/types.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/libpastis/utils.py` & `pastis-framework-1.0.4/libpastis/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/pastis_framework.egg-info/PKG-INFO` & `pastis-framework-1.0.4/pastis_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.3
+Version: 1.0.4
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.3/pastis_framework.egg-info/SOURCES.txt` & `pastis-framework-1.0.4/pastis_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,11 +40,12 @@
 pastisbenchmark/models.py
 pastisbenchmark/plotter.py
 pastisbenchmark/replayer.py
 pastisbenchmark/results.py
 pastisbroker/__init__.py
 pastisbroker/broker.py
 pastisbroker/client.py
+pastisbroker/coverage.py
 pastisbroker/dashboard.py
 pastisbroker/stat_manager.py
 pastisbroker/utils.py
 pastisbroker/workspace.py
```

### Comparing `pastis-framework-1.0.3/pastisbenchmark/models.py` & `pastis-framework-1.0.4/pastisbenchmark/models.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/pastisbenchmark/plotter.py` & `pastis-framework-1.0.4/pastisbenchmark/plotter.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/pastisbenchmark/replayer.py` & `pastis-framework-1.0.4/pastisbenchmark/replayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,33 +39,18 @@
         self._args = list(args)
         self._fails = []
         self._tracing_times = []
 
         # initiatialize directories
         self._init_directories()
 
-        # set longjmp ENV var if applicable
-        self._set_longjump_plt()
-
     def _init_directories(self):
         if not self.corpus_replay_dir.exists():
             self.corpus_replay_dir.mkdir()
 
-    def _set_longjump_plt(self):
-        try:
-            proc = subprocess.Popen(['objdump', '-D', self.program.absolute()], stdout=subprocess.PIPE)
-            out, err = proc.communicate()
-            for line in out.split(b"\n"):
-                if b"<longjmp@plt>:" in line:
-                    addr = line.split()[0]
-                    logging.info(f"lonjmp address found at: {addr}")
-                    os.environ["TT_LONGJMP_ADDR"] = str(int(addr, 16))
-        except:
-            return 0
-
     @property
     def corpus_replay_dir(self) -> Path:
         if self.type == ReplayType.qbdi:
             return self.workspace.root / self.QBDI_REPLAY_DIR
         else:
             return self.workspace.root / self.LLVMPROFILE_REPLAY_DIR
```

### Comparing `pastis-framework-1.0.3/pastisbenchmark/results.py` & `pastis-framework-1.0.4/pastisbenchmark/results.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/pastisbroker/broker.py` & `pastis-framework-1.0.4/pastisbroker/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 # built-in imports
+import hashlib
 import logging
 from typing import Generator, List, Optional, Union
 from pathlib import Path
 import time
 from hashlib import md5
 from enum import Enum
 from collections import Counter
 import datetime
 import random
+import queue
 
 # Third-party imports
 import psutil
 from libpastis import BrokerAgent, FuzzingEngineDescriptor, EngineConfiguration, BinaryPackage, SASTReport, ClientAgent
 from libpastis.types import SeedType, FuzzingEngineInfo, LogLevel, Arch, State, SeedInjectLoc, CheckMode, CoverageMode, \
                             ExecMode, AlertData, PathLike, Platform, FuzzMode
+from libpastis.utils import get_local_architecture
 import lief
 from tritondse import QuokkaProgram
 
 # Local imports
 from pastisbroker.client import PastisClient
 from pastisbroker.stat_manager import StatManager
 from pastisbroker.workspace import Workspace, WorkspaceStatus
-from pastisbroker.utils import load_engine_descriptor
+from pastisbroker.utils import load_engine_descriptor, Bcolors, COLORS
+from pastisbroker.coverage import CoverageManager, ClientInput
 
 
 lief.logging.disable()
 
 
 class BrokingMode(Enum):
     FULL = 1              # Transmit all seeds to all peers
     NO_TRANSMIT = 2       # Does not transmit seed to peers (for comparing perfs of tools against each other)
 
 
-COLORS = [32, 33, 34, 35, 36, 37, 39, 91, 93, 94, 95, 96]
-
-
-class Bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
 
 
 class PastisBroker(BrokerAgent):
 
     def __init__(self, workspace: PathLike,
                  binaries_dir: PathLike,
                  broker_mode: BrokingMode,
                  check_mode: CheckMode = CheckMode.CHECK_ALL,
                  inject_loc: SeedInjectLoc = SeedInjectLoc.STDIN,
                  sast_report: PathLike = None,
                  p_argv: List[str] = None,
                  memory_threshold: int = 85,
-                 start_quorum: int = 0):
+                 start_quorum: int = 0,
+                 filter_inputs: bool = False,
+                 stream: bool = False,
+                 replay_threads: int = 4):
         super(PastisBroker, self).__init__()
 
         # Initialize workspace
         self.workspace = Workspace(Path(workspace))
         params = {"binaries_dir": str(Path(binaries_dir).absolute()),
                   "broker_mode": broker_mode.name,
                   "check_mode": check_mode.name,
@@ -82,15 +76,15 @@
         self.engines_args = {}
         self.engines = {}  # name->FuzzingEngineDescriptor
 
         # for slicing mode (otherwise not used)
         self._slicing_ongoing = {}  # Program -> {Addr -> [cli]}
 
         # Initialize availables binaries
-        self.programs = {}  # Tuple[(Arch, Fuzzer, ExecMode)] -> Path
+        self.programs = {}  # Tuple[(Platform, Arch)] -> List[BinaryPackage]
         self._find_binaries(binaries_dir)
 
         # Klocwork informations
         self.sast_report = None
         if sast_report:
             self.initialize_sast_report(sast_report)
 
@@ -118,14 +112,48 @@
         # startup quorum
         self._startup_quorum = start_quorum
         self._current_quorum = 0
 
         # Proxy feature
         self._proxy = None
         self._proxy_cli = None
+        self._proxy_start_signal = False
+        self._proxy_seed_queue = queue.Queue()
+
+        # Coverage + filtering feature
+        self._coverage_manager = None
+        self.filter_inputs: bool = filter_inputs
+        if filter_inputs or stream:
+            if (path := self.find_vanilla_binary()) is not None:  # Find an executable suitable for coverage
+                logging.info(f"Coverage binary: {path}")
+                stream_file = self.workspace.coverage_history if stream else ""
+                self._coverage_manager = CoverageManager(replay_threads, filter_inputs, path, self.argv, self.inject, stream_file)
+            else:
+                logging.warning("filtering or stream enabled but cannot find vanilla binary")
+
+
+    def find_vanilla_binary(self) -> Optional[str]:
+        """
+        Find a binary without instrumentation to be used for coverage
+        computation. It also has to match local architecture.
+        :return: Path to the progam
+        """
+        local_arch = get_local_architecture()
+        for pkg in self.programs.get((Platform.LINUX, local_arch)):
+            path = str(pkg.executable_path.absolute())
+            p = lief.parse(str(path))
+            ok = True
+            for f in p.functions:
+                if "hfuzz_" in f.name or "__afl_" in f.name or "__gcov_" in f.name or "__asan_" in f.name:
+                    ok = False
+                    break
+            if ok:
+                return path
+        return None
+
 
     def load_engine_addon(self, py_module: str) -> bool:
         desc = load_engine_descriptor(py_module)
         if desc is not None:
             self.engines[desc.NAME] = desc
             self.engines_args[desc.NAME] = []
             return True
@@ -190,25 +218,34 @@
         is_new = seed not in self._seed_pool
         h = md5(seed).hexdigest()
 
         # Show log message and save seed to file
         self.statmanager.update_seed_stat(cli, typ)  # Add info only if new
         cli.log(LogLevel.INFO, f"seed {h} [{self._colored_seed_type(typ)}][{self._colored_seed_newness(is_new)}]")
         cli.add_own_seed(seed)  # Add seed in client's seed
-        self.write_seed(typ, cli.strid, seed) # Write seed to file
+        fname = self.write_seed(typ, cli.strid, seed) # Write seed to file
 
         if is_new:
             self._seed_pool[seed] = typ  # Save it in the local pool
+
+            if self._coverage_manager:
+                sp = fname.split("_")
+                covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], h, fname, typ, cli.netid, cli.strid, "GRANTED", "", -1, [])
+                self._coverage_manager.push_input(covi)
+
+            if not self.filter_inputs:  # If seed are not filtered send it right away
+                self.seed_granted(cli.netid, typ, seed)
         else:
-            pass
-            # logging.warning(f"receive duplicate seed {h} by {cli.strid}")
+            logging.debug(f"receive duplicate seed {h} by {cli.strid}")
+
 
+    def seed_granted(self, cli_id: bytes, typ: SeedType, seed: bytes):
         # Iterate on all clients and send it to whomever never received it
         if self.broker_mode == BrokingMode.FULL:
-            self.send_seed_to_all_others(cli.netid, typ, seed)
+            self.send_seed_to_all_others(cli_id, typ, seed)
 
         if self.is_proxied:  # Forward it to the proxy
             self._proxy.send_seed(typ, seed)
 
     def send_seed_to_all_others(self, origin_id: bytes, typ: SeedType, seed: bytes) -> None:
         for c in self.iter_other_clients(origin_id):
             if c.is_new_seed(seed):
@@ -222,19 +259,23 @@
         self.workspace.save_seed_file(SeedType.INPUT, p, initial)
 
         seed = p.read_bytes()
         self._seed_pool[seed] = SeedType.INPUT
         if initial:
             self._init_seed_pool[seed] = SeedType.INPUT
 
-    def write_seed(self, typ: SeedType, cli_id: str, seed: bytes):
+    def write_seed(self, typ: SeedType, cli_id: str, seed: bytes) -> str:
+        fname = self.mk_input_name(cli_id, seed)
+        self.workspace.save_seed(typ, fname, seed)
+        return fname
+
+    def mk_input_name(self, cli_id: str, seed: bytes) -> str:
         t = time.strftime("%Y-%m-%d_%H:%M:%S", time.localtime())
         elapsed = str(datetime.timedelta(seconds=time.time() - self._start_time)).replace(" day, ", "d:").replace(" days, ", "d:")
-        fname = f"{t}_{elapsed}_{cli_id}_{md5(seed).hexdigest()}.cov"
-        self.workspace.save_seed(typ, fname, seed)
+        return f"{t}_{elapsed}_{cli_id}_{md5(seed).hexdigest()}.cov"
 
     def hello_received(self, cli_id: bytes, engines: List[FuzzingEngineInfo], arch: Arch, cpus: int, memory: int, hostname: str, platform: Platform):
         uid = self.new_uid()
         client = PastisClient(uid, cli_id, engines, arch, cpus, memory, hostname, platform)
         logging.info(f"[{client.strid}] [HELLO] Name:{hostname} Arch:{arch.name} engines:{[x.name for x in engines]} (cpu:{cpus}, mem:{memory})")
         self.clients[client.netid] = client
 
@@ -359,14 +400,18 @@
 
     def stop_broker(self):
         for client in self.clients.values():
             logging.info(f"Send stop to {client.strid}")
             self.send_stop(client.netid)
         self._stop = True
 
+        # Stop coverage manager if any
+        if self._coverage_manager:
+            self._coverage_manager.stop()
+
         # Call the statmanager to wrap-up values
         self.statmanager.post_execution(list(self.clients.values()), self.workspace)
 
         if self.is_proxied:
             self._proxy.stop()
 
         if self.sast_report:  # If a SAST report was loaded
@@ -531,14 +576,22 @@
     def start(self, running: bool = True):
         super(PastisBroker, self).start()  # Start the listening thread
         self._start_time = time.time()
         self._running = running
         self.workspace.status = WorkspaceStatus.RUNNING
         logging.info("start broking")
 
+        if self._coverage_manager:  # if it has been instanciated start it
+            self._coverage_manager.start()
+            for seed in self._init_seed_pool.keys():  # Push initial corpus to set baseline coverage
+                fname = self.mk_input_name("INITIAL", seed)
+                sp = fname.split("_")
+                covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], sp[4], fname, SeedType.INPUT, b"INITIAL", "INITIAL", "GRANTED", "", -1, [])
+                self._coverage_manager.push_input(covi)
+
         if self.is_proxied and self._proxy_cli:
             self._running = False  # disable running wait start broker
             self._proxy.send_hello([self._proxy_cli])
         else:
             # Send the start message to all clients (already connected)
             if self._running:  # If we want to run now (cmdline mode)
                 self.start_pending_clients()
@@ -546,15 +599,15 @@
     def run(self, timeout: int = None):
         self.start()
         last_t = time.time()
 
         # Start infinite loop
         try:
             while True:
-                time.sleep(1)
+                time.sleep(0.05)
                 t = time.time()
 
                 # Check if the campaign have to be stopped
                 if timeout is not None:
                     if t > (self._start_time + timeout):
                         logging.info("Campaign timeout reached, stop campaign.")
                         self._stop = True
@@ -564,14 +617,33 @@
                     if not self._check_memory_usage():
                         # The machine starts being overloaded
                         # For security kill triton instance
                         for cli in list(self.clients.values()):
                             if cli.engine.SHORT_NAME == "TT":  # is triton
                                 self.kick_client(cli.netid)
 
+                # if inputs are filtered. Get granted inputs and forward them to appropriate clients
+                if self.filter_inputs:
+                    for item in self._coverage_manager.iter_granted_inputs():
+                        self.seed_granted(item.fuzzer_id, item.seed_status, item.content)
+
+                # Check if we received the start signal from the proxy-master
+                if self._proxy_start_signal:
+                    self._proxy_start_signal = False
+                    self.start_pending_clients()
+
+                # Check if there are seed coming from the proxy-master to forward to clients
+                if not self._proxy_seed_queue.empty():
+                    try:
+                        while True:
+                            origin, typ, seed = self._proxy_seed_queue.get_nowait()
+                            self.send_seed_to_all_others(origin, typ, seed)
+                    except queue.Empty:
+                        pass
+
                 if self._stop:
                     logging.info("broker terminate")
                     break
         except KeyboardInterrupt:
             logging.info("stop required (Ctrl+C)")
         self.workspace.status = WorkspaceStatus.FINISHED
         self.stop_broker()
@@ -700,25 +772,26 @@
 
     def _proxy_start_received(self, fname: str, binary: bytes, engine: FuzzingEngineInfo, exmode: ExecMode,
                               fuzzmode: FuzzMode, chkmode: CheckMode, covmode: CoverageMode, seed_inj: SeedInjectLoc,
                               engine_args: str, argv: List[str], sast_report: str = None):
         # FIXME: Use parameters received
         logging.info("[PROXY] start received !")
         self._running = True
-        if self._running:
-            self.start_pending_clients()
+        # if self._running:
+        #     self.start_pending_clients()
 
     def _proxy_seed_received(self, typ: SeedType, seed: bytes):
         # Forward the seed to underlying clients
         logging.info(f"[PROXY] seed {typ.name} received forward to agents")
 
         # Save the seed locally
         self.write_seed(typ, "PROXY", seed)
         self._seed_pool[seed] = typ  # add it to the pool
         self._init_seed_pool[seed] = typ  # also consider it as initial corpus
 
         # Forward it to all clients
-        self.send_seed_to_all_others(b"PROXY", typ, seed)
+        self._proxy_seed_queue.put((b"PROXY", typ, seed))
+        # self.send_seed_to_all_others(b"PROXY", typ, seed)
 
     def _proxy_stop_received(self):
         logging.info(f"[PROXY] stop received!")
         self._stop = True
```

### Comparing `pastis-framework-1.0.3/pastisbroker/client.py` & `pastis-framework-1.0.4/pastisbroker/client.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.3/pastisbroker/stat_manager.py` & `pastis-framework-1.0.4/pastisbroker/stat_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,8 +92,8 @@
         """
         Called at the end of the execution. Export
         :return: None
         """
         self._tel_file.flush()  # Flush the csv if it has not been
 
         with open(workspace.clients_stat_file, "w") as f:
-            json.dump([cli.to_dict() for cli in clients], f, indent=2)
+            json.dump([cli.to_dict() for cli in clients if cli.is_running()], f, indent=2)
```

### Comparing `pastis-framework-1.0.3/pastisbroker/workspace.py` & `pastis-framework-1.0.4/pastisbroker/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     SAST_REPORT_COPY = "sast-report.bin"
     CSV_FILE = "results.csv"
     TELEMETRY_FILE = "telemetry.csv"
     CLIENTS_STATS = "clients-stats.json"
     LOG_FILE = "broker.log"
     STATUS_FILE = "STATUS"
     RUNTIME_CONFIG_FILE = "config.json"
+    COVERAGE_HISTORY = "coverage-history.csv"
 
     def __init__(self, directory: Path, erase: bool = False):
         self.root = directory
 
         if erase:  # If want to erase the whole workspace
             shutil.rmtree(self.root)
 
@@ -108,14 +109,18 @@
     def broker_log_file(self) -> Path:
         return self.root / self.LOG_FILE
 
     @property
     def config_file(self) -> Path:
         return self.root / self.RUNTIME_CONFIG_FILE
 
+    @property
+    def coverage_history(self) -> Path:
+        return self.root / self.COVERAGE_HISTORY
+
     def add_binary(self, binary_path: Path) -> Path:
         """
         Add a binary in the workspace directory structure.
 
         :param binary_path: Path of the executable to copy
         :return: the final executable file path
         """
```

### Comparing `pastis-framework-1.0.3/setup.py` & `pastis-framework-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md") as f:
     lines = f.readlines()
     README = "\n".join(lines[4:7]+lines[51:])
 
 
 setup(
     name="pastis-framework",
-    version="1.0.3",
+    version="1.0.4",
     description="PASTIS framework for collaborative fuzzing",
     long_description=README,
     long_description_content_type='text/markdown',
     packages=[
         "libpastis",
         "libpastis.proto",
         "pastisbroker",
```

