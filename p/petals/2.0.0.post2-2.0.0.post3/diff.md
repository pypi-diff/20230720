# Comparing `tmp/petals-2.0.0.post2.tar.gz` & `tmp/petals-2.0.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petals-2.0.0.post2.tar", last modified: Thu Jul 20 08:56:17 2023, max compression
+gzip compressed data, was "petals-2.0.0.post3.tar", last modified: Thu Jul 20 17:08:19 2023, max compression
```

## Comparing `petals-2.0.0.post2.tar` & `petals-2.0.0.post3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.761741 petals-2.0.0.post2/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2022-11-26 05:33:56.000000 petals-2.0.0.post2/LICENSE
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12469 2023-07-20 08:56:17.761741 petals-2.0.0.post2/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11284 2023-07-19 17:16:10.000000 petals-2.0.0.post2/README.md
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-25 09:55:28.000000 petals-2.0.0.post2/pyproject.toml
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1752 2023-07-20 08:56:17.761741 petals-2.0.0.post2/setup.cfg
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.753741 petals-2.0.0.post2/src/
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.753741 petals-2.0.0.post2/src/petals/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      784 2023-07-20 08:55:30.000000 petals-2.0.0.post2/src/petals/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.753741 petals-2.0.0.post2/src/petals/cli/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.0.post2/src/petals/cli/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-01-13 00:54:42.000000 petals-2.0.0.post2/src/petals/cli/run_dht.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13931 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/cli/run_server.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/client/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      282 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/client/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3600 2023-07-12 11:02:03.000000 petals-2.0.0.post2/src/petals/client/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15296 2023-07-18 23:25:43.000000 petals-2.0.0.post2/src/petals/client/inference_session.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3526 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/client/lm_head.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3493 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/client/ptune.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-02-06 20:57:31.000000 petals-2.0.0.post2/src/petals/client/remote_forward_backward.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 21:02:40.000000 petals-2.0.0.post2/src/petals/client/remote_generation.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2675 2023-07-12 12:22:35.000000 petals-2.0.0.post2/src/petals/client/remote_sequential.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/client/routing/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2022-12-01 12:24:57.000000 petals-2.0.0.post2/src/petals/client/routing/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4629 2023-07-17 09:46:40.000000 petals-2.0.0.post2/src/petals/client/routing/sequence_info.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    22818 2023-07-19 10:53:04.000000 petals-2.0.0.post2/src/petals/client/routing/sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2022-12-01 12:24:57.000000 petals-2.0.0.post2/src/petals/client/routing/spending_policy.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12405 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/client/sequential_autograd.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      906 2023-07-20 08:54:06.000000 petals-2.0.0.post2/src/petals/constants.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2348 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/data_structures.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4511 2023-07-17 06:29:38.000000 petals-2.0.0.post2/src/petals/dht_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/models/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       68 2023-07-13 20:49:11.000000 petals-2.0.0.post2/src/petals/models/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/models/bloom/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/models/bloom/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1414 2023-07-13 20:49:11.000000 petals-2.0.0.post2/src/petals/models/bloom/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1380 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/models/bloom/config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5243 2023-07-19 01:15:47.000000 petals-2.0.0.post2/src/petals/models/bloom/model.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/models/llama/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/models/llama/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3582 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/models/llama/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/models/llama/config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5998 2023-07-19 01:15:47.000000 petals-2.0.0.post2/src/petals/models/llama/model.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/server/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.0.post2/src/petals/server/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9994 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/server/backend.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-06 15:09:40.000000 petals-2.0.0.post2/src/petals/server/block_selection.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-12 11:02:03.000000 petals-2.0.0.post2/src/petals/server/block_utils.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6655 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/server/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    35230 2023-07-19 10:53:04.000000 petals-2.0.0.post2/src/petals/server/handler.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8718 2023-07-15 01:19:46.000000 petals-2.0.0.post2/src/petals/server/memory_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7703 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/server/reachability.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    30183 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/server/server.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-06 15:09:40.000000 petals-2.0.0.post2/src/petals/server/task_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-01-22 05:16:17.000000 petals-2.0.0.post2/src/petals/server/task_prioritizer.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8552 2023-07-18 22:29:14.000000 petals-2.0.0.post2/src/petals/server/throughput.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.757741 petals-2.0.0.post2/src/petals/utils/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      182 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/utils/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2022-12-29 20:33:47.000000 petals-2.0.0.post2/src/petals/utils/asyncio.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2189 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/utils/auto_config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6594 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/utils/convert_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2963 2023-07-09 23:10:48.000000 petals-2.0.0.post2/src/petals/utils/disk_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5560 2023-07-18 09:05:08.000000 petals-2.0.0.post2/src/petals/utils/generation_algorithms.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2022-12-03 11:35:20.000000 petals-2.0.0.post2/src/petals/utils/generation_constraints.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      270 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/utils/hf_auth.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      745 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/utils/logging.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/utils/misc.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12164 2023-07-19 16:28:49.000000 petals-2.0.0.post2/src/petals/utils/peft.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2283 2023-07-18 09:05:08.000000 petals-2.0.0.post2/src/petals/utils/ping.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      310 2023-07-18 09:05:08.000000 petals-2.0.0.post2/src/petals/utils/random.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1438 2023-06-29 20:31:16.000000 petals-2.0.0.post2/src/petals/utils/version.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.753741 petals-2.0.0.post2/src/petals.egg-info/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12469 2023-07-20 08:56:17.000000 petals-2.0.0.post2/src/petals.egg-info/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2331 2023-07-20 08:56:17.000000 petals-2.0.0.post2/src/petals.egg-info/SOURCES.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-07-20 08:56:17.000000 petals-2.0.0.post2/src/petals.egg-info/dependency_links.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      456 2023-07-20 08:56:17.000000 petals-2.0.0.post2/src/petals.egg-info/requires.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-07-20 08:56:17.000000 petals-2.0.0.post2/src/petals.egg-info/top_level.txt
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 08:56:17.761741 petals-2.0.0.post2/tests/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1646 2023-07-17 09:46:40.000000 petals-2.0.0.post2/tests/test_aux_functions.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1603 2023-06-30 00:37:10.000000 petals-2.0.0.post2/tests/test_block_exact_match.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2947 2023-06-29 20:31:16.000000 petals-2.0.0.post2/tests/test_chained_calls.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      672 2023-06-29 20:31:16.000000 petals-2.0.0.post2/tests/test_dtype.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8121 2023-07-12 12:22:35.000000 petals-2.0.0.post2/tests/test_full_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1535 2023-07-12 12:22:35.000000 petals-2.0.0.post2/tests/test_peft.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-25 15:58:19.000000 petals-2.0.0.post2/tests/test_priority_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6055 2023-07-09 23:10:48.000000 petals-2.0.0.post2/tests/test_remote_sequential.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1924 2023-07-14 15:21:17.000000 petals-2.0.0.post2/tests/test_sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1707 2023-06-29 20:31:16.000000 petals-2.0.0.post2/tests/test_server_stats.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-06-29 20:31:16.000000 petals-2.0.0.post2/tests/test_tensor_parallel.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      466 2023-07-12 12:22:35.000000 petals-2.0.0.post2/tests/test_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.855064 petals-2.0.0.post3/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2022-11-26 05:33:56.000000 petals-2.0.0.post3/LICENSE
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12478 2023-07-20 17:08:19.855064 petals-2.0.0.post3/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11293 2023-07-20 17:00:05.000000 petals-2.0.0.post3/README.md
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-25 09:55:28.000000 petals-2.0.0.post3/pyproject.toml
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1752 2023-07-20 17:08:19.855064 petals-2.0.0.post3/setup.cfg
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.847063 petals-2.0.0.post3/src/
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      784 2023-07-20 17:08:09.000000 petals-2.0.0.post3/src/petals/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/cli/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.0.post3/src/petals/cli/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-01-13 00:54:42.000000 petals-2.0.0.post3/src/petals/cli/run_dht.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13932 2023-07-20 17:00:05.000000 petals-2.0.0.post3/src/petals/cli/run_server.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/client/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      282 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/client/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3600 2023-07-12 11:02:03.000000 petals-2.0.0.post3/src/petals/client/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15296 2023-07-18 23:25:43.000000 petals-2.0.0.post3/src/petals/client/inference_session.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3526 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/client/lm_head.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3493 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/client/ptune.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-02-06 20:57:31.000000 petals-2.0.0.post3/src/petals/client/remote_forward_backward.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 21:02:40.000000 petals-2.0.0.post3/src/petals/client/remote_generation.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2675 2023-07-12 12:22:35.000000 petals-2.0.0.post3/src/petals/client/remote_sequential.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/client/routing/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2022-12-01 12:24:57.000000 petals-2.0.0.post3/src/petals/client/routing/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4629 2023-07-17 09:46:40.000000 petals-2.0.0.post3/src/petals/client/routing/sequence_info.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    22820 2023-07-20 17:00:05.000000 petals-2.0.0.post3/src/petals/client/routing/sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2022-12-01 12:24:57.000000 petals-2.0.0.post3/src/petals/client/routing/spending_policy.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12405 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/client/sequential_autograd.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      904 2023-07-20 17:00:05.000000 petals-2.0.0.post3/src/petals/constants.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2348 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/data_structures.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4511 2023-07-17 06:29:38.000000 petals-2.0.0.post3/src/petals/dht_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/models/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       68 2023-07-13 20:49:11.000000 petals-2.0.0.post3/src/petals/models/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/models/bloom/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/models/bloom/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1414 2023-07-13 20:49:11.000000 petals-2.0.0.post3/src/petals/models/bloom/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1380 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/models/bloom/config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5243 2023-07-19 01:15:47.000000 petals-2.0.0.post3/src/petals/models/bloom/model.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals/models/llama/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/models/llama/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3582 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/models/llama/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/models/llama/config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5998 2023-07-19 01:15:47.000000 petals-2.0.0.post3/src/petals/models/llama/model.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.855064 petals-2.0.0.post3/src/petals/server/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.0.post3/src/petals/server/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9994 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/server/backend.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-06 15:09:40.000000 petals-2.0.0.post3/src/petals/server/block_selection.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-12 11:02:03.000000 petals-2.0.0.post3/src/petals/server/block_utils.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6655 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/server/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    35230 2023-07-19 10:53:04.000000 petals-2.0.0.post3/src/petals/server/handler.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8718 2023-07-15 01:19:46.000000 petals-2.0.0.post3/src/petals/server/memory_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7706 2023-07-20 17:00:05.000000 petals-2.0.0.post3/src/petals/server/reachability.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    30183 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/server/server.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-06 15:09:40.000000 petals-2.0.0.post3/src/petals/server/task_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-01-22 05:16:17.000000 petals-2.0.0.post3/src/petals/server/task_prioritizer.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8552 2023-07-18 22:29:14.000000 petals-2.0.0.post3/src/petals/server/throughput.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.855064 petals-2.0.0.post3/src/petals/utils/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      182 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/utils/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2022-12-29 20:33:47.000000 petals-2.0.0.post3/src/petals/utils/asyncio.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2189 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/utils/auto_config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6594 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/utils/convert_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2963 2023-07-09 23:10:48.000000 petals-2.0.0.post3/src/petals/utils/disk_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5560 2023-07-18 09:05:08.000000 petals-2.0.0.post3/src/petals/utils/generation_algorithms.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2022-12-03 11:35:20.000000 petals-2.0.0.post3/src/petals/utils/generation_constraints.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      270 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/utils/hf_auth.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      745 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/utils/logging.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/utils/misc.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12164 2023-07-19 16:28:49.000000 petals-2.0.0.post3/src/petals/utils/peft.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2283 2023-07-18 09:05:08.000000 petals-2.0.0.post3/src/petals/utils/ping.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      310 2023-07-18 09:05:08.000000 petals-2.0.0.post3/src/petals/utils/random.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1438 2023-06-29 20:31:16.000000 petals-2.0.0.post3/src/petals/utils/version.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.851063 petals-2.0.0.post3/src/petals.egg-info/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12478 2023-07-20 17:08:19.000000 petals-2.0.0.post3/src/petals.egg-info/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2331 2023-07-20 17:08:19.000000 petals-2.0.0.post3/src/petals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-07-20 17:08:19.000000 petals-2.0.0.post3/src/petals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      456 2023-07-20 17:08:19.000000 petals-2.0.0.post3/src/petals.egg-info/requires.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-07-20 17:08:19.000000 petals-2.0.0.post3/src/petals.egg-info/top_level.txt
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-20 17:08:19.855064 petals-2.0.0.post3/tests/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1646 2023-07-17 09:46:40.000000 petals-2.0.0.post3/tests/test_aux_functions.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1603 2023-06-30 00:37:10.000000 petals-2.0.0.post3/tests/test_block_exact_match.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2947 2023-06-29 20:31:16.000000 petals-2.0.0.post3/tests/test_chained_calls.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      672 2023-06-29 20:31:16.000000 petals-2.0.0.post3/tests/test_dtype.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8121 2023-07-12 12:22:35.000000 petals-2.0.0.post3/tests/test_full_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1535 2023-07-12 12:22:35.000000 petals-2.0.0.post3/tests/test_peft.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-25 15:58:19.000000 petals-2.0.0.post3/tests/test_priority_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6055 2023-07-09 23:10:48.000000 petals-2.0.0.post3/tests/test_remote_sequential.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1924 2023-07-14 15:21:17.000000 petals-2.0.0.post3/tests/test_sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1707 2023-06-29 20:31:16.000000 petals-2.0.0.post3/tests/test_server_stats.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-06-29 20:31:16.000000 petals-2.0.0.post3/tests/test_tensor_parallel.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      466 2023-07-12 12:22:35.000000 petals-2.0.0.post3/tests/test_utils.py
```

### Comparing `petals-2.0.0.post2/LICENSE` & `petals-2.0.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/PKG-INFO` & `petals-2.0.0.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 2.0.0.post2
+Version: 2.0.0.post3
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -88,28 +88,28 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](http://chat.petals.ml) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.ml)
-- [Monitor](http://health.petals.ml) for the public swarm: [source code](https://github.com/borzunov/health.petals.ml)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
 
 ## How does it work?
 
 - Petals runs large language models like [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom) **collaboratively** — you load a small part of the model, then team up with people serving the other parts to run inference or fine-tuning.
-- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
+- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](https://chat.petals.dev) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
 - Beyond classic language model APIs — you can employ any fine-tuning and sampling methods, execute custom paths through the model, or see its hidden states. You get the comforts of an API with the flexibility of PyTorch.
 
 <p align="center">
     <img src="https://i.imgur.com/RTYF3yW.png" width="800">
 </p>
 
 <p align="center">
@@ -241,9 +241,9 @@
 
 --------------------------------------------------------------------------------
 
 <p align="center">
     This project is a part of the <a href="https://bigscience.huggingface.co/">BigScience</a> research workshop.
 </p>
 <p align="center">
-    <img src="https://petals.ml/bigscience.png" width="150">
+    <img src="https://petals.dev/bigscience.png" width="150">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 2.0.0.post2 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 2.0.0.post3 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -69,36 +69,36 @@
 more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
-guides: - [Chatbot web app](http://chat.petals.ml) (connects to Petals via an
+guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
 HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
-chat.petals.ml) - [Monitor](http://health.petals.ml) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.ml) - Launch your own
+chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
+[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
 swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
 own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
 people serving the other parts to run inference or fine-tuning. - Single-batch
 inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec
 for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-
-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://
-chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds
-of tokens/sec. - Beyond classic language model APIs â you can employ any
-fine-tuning and sampling methods, execute custom paths through the model, or
-see its hidden states. You get the comforts of an API with the flexibility of
-PyTorch.
+workshop/petals#benchmarks) than offloading, enough for [chatbots](https://
+chat.petals.dev) and other interactive apps. Parallel inference reaches
+hundreds of tokens/sec. - Beyond classic language model APIs â you can employ
+any fine-tuning and sampling methods, execute custom paths through the model,
+or see its hidden states. You get the comforts of an API with the flexibility
+of PyTorch.
                        [https://i.imgur.com/RTYF3yW.png]
                    ð  See_FAQ            ð  Read_paper
 ## Installation Here's how to install Petals with [Anaconda](https://
 www.anaconda.com/products/distribution) on Linux: ```bash conda install pytorch
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install --upgrade petals ``` If you
 don't use Anaconda, you can install PyTorch in [any other way](https://
 pytorch.org/get-started/locally/). If you want to run models with 8-bit
@@ -145,8 +145,8 @@
 {borzunov2022petals, title = {Petals: Collaborative Inference and Fine-tuning
 of Large Models}, author = {Borzunov, Alexander and Baranchuk, Dmitry and
 Dettmers, Tim and Ryabinin, Max and Belkada, Younes and Chumachenko, Artem and
 Samygin, Pavel and Raffel, Colin}, journal = {arXiv preprint arXiv:2209.01188},
 year = {2022}, url = {https://arxiv.org/abs/2209.01188} } ``` -----------------
 ---------------------------------------------------------------
           This project is a part of the BigScience research workshop.
-                      [https://petals.ml/bigscience.png]
+                      [https://petals.dev/bigscience.png]
```

### Comparing `petals-2.0.0.post2/README.md` & `petals-2.0.0.post3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,28 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](http://chat.petals.ml) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.ml)
-- [Monitor](http://health.petals.ml) for the public swarm: [source code](https://github.com/borzunov/health.petals.ml)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
 
 ## How does it work?
 
 - Petals runs large language models like [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom) **collaboratively** — you load a small part of the model, then team up with people serving the other parts to run inference or fine-tuning.
-- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
+- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](https://chat.petals.dev) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
 - Beyond classic language model APIs — you can employ any fine-tuning and sampling methods, execute custom paths through the model, or see its hidden states. You get the comforts of an API with the flexibility of PyTorch.
 
 <p align="center">
     <img src="https://i.imgur.com/RTYF3yW.png" width="800">
 </p>
 
 <p align="center">
@@ -214,9 +214,9 @@
 
 --------------------------------------------------------------------------------
 
 <p align="center">
     This project is a part of the <a href="https://bigscience.huggingface.co/">BigScience</a> research workshop.
 </p>
 <p align="center">
-    <img src="https://petals.ml/bigscience.png" width="150">
+    <img src="https://petals.dev/bigscience.png" width="150">
 </p>
```

#### html2text {}

```diff
@@ -53,36 +53,36 @@
 more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
-guides: - [Chatbot web app](http://chat.petals.ml) (connects to Petals via an
+guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
 HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
-chat.petals.ml) - [Monitor](http://health.petals.ml) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.ml) - Launch your own
+chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
+[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
 swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
 own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
 people serving the other parts to run inference or fine-tuning. - Single-batch
 inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec
 for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-
-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://
-chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds
-of tokens/sec. - Beyond classic language model APIs â you can employ any
-fine-tuning and sampling methods, execute custom paths through the model, or
-see its hidden states. You get the comforts of an API with the flexibility of
-PyTorch.
+workshop/petals#benchmarks) than offloading, enough for [chatbots](https://
+chat.petals.dev) and other interactive apps. Parallel inference reaches
+hundreds of tokens/sec. - Beyond classic language model APIs â you can employ
+any fine-tuning and sampling methods, execute custom paths through the model,
+or see its hidden states. You get the comforts of an API with the flexibility
+of PyTorch.
                        [https://i.imgur.com/RTYF3yW.png]
                    ð  See_FAQ            ð  Read_paper
 ## Installation Here's how to install Petals with [Anaconda](https://
 www.anaconda.com/products/distribution) on Linux: ```bash conda install pytorch
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install --upgrade petals ``` If you
 don't use Anaconda, you can install PyTorch in [any other way](https://
 pytorch.org/get-started/locally/). If you want to run models with 8-bit
@@ -129,8 +129,8 @@
 {borzunov2022petals, title = {Petals: Collaborative Inference and Fine-tuning
 of Large Models}, author = {Borzunov, Alexander and Baranchuk, Dmitry and
 Dettmers, Tim and Ryabinin, Max and Belkada, Younes and Chumachenko, Artem and
 Samygin, Pavel and Raffel, Colin}, journal = {arXiv preprint arXiv:2209.01188},
 year = {2022}, url = {https://arxiv.org/abs/2209.01188} } ``` -----------------
 ---------------------------------------------------------------
           This project is a part of the BigScience research workshop.
-                      [https://petals.ml/bigscience.png]
+                      [https://petals.dev/bigscience.png]
```

### Comparing `petals-2.0.0.post2/setup.cfg` & `petals-2.0.0.post3/setup.cfg`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/__init__.py` & `petals-2.0.0.post3/src/petals/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from packaging import version
 
 from petals.client import *
 from petals.models import *
 from petals.utils import *
 from petals.utils.logging import initialize_logs as _initialize_logs
 
-__version__ = "2.0.0.post2"
+__version__ = "2.0.0.post3"
 
 
 if not os.getenv("PETALS_IGNORE_DEPENDENCY_VERSION"):
     assert (
         version.parse("4.31.0") <= version.parse(transformers.__version__) < version.parse("5.0.0")
     ), "Please install a proper transformers version: pip install transformers>=4.31.0,<5.0.0"
```

### Comparing `petals-2.0.0.post2/src/petals/cli/run_dht.py` & `petals-2.0.0.post3/src/petals/cli/run_dht.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/cli/run_server.py` & `petals-2.0.0.post3/src/petals/cli/run_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                              "Default: 'int8' if GPU is available, 'none' otherwise")
     parser.add_argument("--tensor_parallel_devices", nargs='+', default=None,
                         help=
                         "Split each block between the specified GPUs such that each device holds a portion of every "
                         "weight matrix. See https://huggingface.co/transformers/v4.9.0/parallelism.html#tensor-parallelism")
 
     parser.add_argument("--skip_reachability_check", action='store_true',
-                        help="Skip checking this server's reachability via health.petals.ml "
+                        help="Skip checking this server's reachability via health.petals.dev "
                              "when connecting to the public swarm. If you connect to a private swarm, "
                              "the check is skipped by default. Use this option only if you know what you are doing")
 
     parser.add_argument("--adapters", nargs='+', default=(),
                         help="List of pre-loaded LoRA adapters that can be used for inference or training")
 
     # fmt:on
```

### Comparing `petals-2.0.0.post2/src/petals/client/from_pretrained.py` & `petals-2.0.0.post3/src/petals/client/from_pretrained.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/inference_session.py` & `petals-2.0.0.post3/src/petals/client/inference_session.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/lm_head.py` & `petals-2.0.0.post3/src/petals/client/lm_head.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/ptune.py` & `petals-2.0.0.post3/src/petals/client/ptune.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/remote_forward_backward.py` & `petals-2.0.0.post3/src/petals/client/remote_forward_backward.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/remote_generation.py` & `petals-2.0.0.post3/src/petals/client/remote_generation.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/remote_sequential.py` & `petals-2.0.0.post3/src/petals/client/remote_sequential.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/routing/sequence_info.py` & `petals-2.0.0.post3/src/petals/client/routing/sequence_info.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/routing/sequence_manager.py` & `petals-2.0.0.post3/src/petals/client/routing/sequence_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,11 +509,11 @@
     logger.log(traceback_level, "See detailed traceback below:", exc_info=True)
 
 
 class MissingBlocksError(RuntimeError):
     def __init__(self, block_indices: Union[int, Sequence[int]]):
         super().__init__(
             f"No servers holding blocks {block_indices} are online. "
-            f"You can check the public swarm's state at http://health.petals.ml "
+            f"You can check the public swarm's state at https://health.petals.dev "
             f"If there are not enough servers, please connect your GPU: "
             f"https://github.com/bigscience-workshop/petals#connect-your-gpu-and-increase-petals-capacity "
         )
```

### Comparing `petals-2.0.0.post2/src/petals/client/routing/spending_policy.py` & `petals-2.0.0.post3/src/petals/client/routing/spending_policy.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/client/sequential_autograd.py` & `petals-2.0.0.post3/src/petals/client/sequential_autograd.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/data_structures.py` & `petals-2.0.0.post3/src/petals/data_structures.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/dht_utils.py` & `petals-2.0.0.post3/src/petals/dht_utils.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/bloom/__init__.py` & `petals-2.0.0.post3/src/petals/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/bloom/block.py` & `petals-2.0.0.post3/src/petals/models/bloom/block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/bloom/config.py` & `petals-2.0.0.post3/src/petals/models/bloom/config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/bloom/model.py` & `petals-2.0.0.post3/src/petals/models/bloom/model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/llama/__init__.py` & `petals-2.0.0.post3/src/petals/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/llama/block.py` & `petals-2.0.0.post3/src/petals/models/llama/block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/llama/config.py` & `petals-2.0.0.post3/src/petals/models/llama/config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/models/llama/model.py` & `petals-2.0.0.post3/src/petals/models/llama/model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/backend.py` & `petals-2.0.0.post3/src/petals/server/backend.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/block_selection.py` & `petals-2.0.0.post3/src/petals/server/block_selection.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/block_utils.py` & `petals-2.0.0.post3/src/petals/server/block_utils.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/from_pretrained.py` & `petals-2.0.0.post3/src/petals/server/from_pretrained.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/handler.py` & `petals-2.0.0.post3/src/petals/server/handler.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/memory_cache.py` & `petals-2.0.0.post3/src/petals/server/memory_cache.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/reachability.py` & `petals-2.0.0.post3/src/petals/server/reachability.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     for attempt_no in range(math.floor(wait_time / retry_delay) + 1):
         try:
             r = requests.get(f"{REACHABILITY_API_URL}/api/v1/is_reachable/{peer_id}", timeout=10)
             r.raise_for_status()
             response = r.json()
 
             if response["success"]:
-                logger.info("Server is reachable from the Internet. It will appear at http://health.petals.ml soon")
+                logger.info("Server is reachable from the Internet. It will appear at https://health.petals.dev soon")
                 return
 
             if attempt_no == 0:
                 # Usually, libp2p manages to set up relays before we finish loading blocks.
                 # In other cases, we may need to wait for up to `wait_time` seconds before it's done.
                 logger.info("Detected a NAT or a firewall, connecting to libp2p relays. This takes a few minutes")
             time.sleep(retry_delay)
         except Exception as e:
-            logger.warning(f"Skipping reachability check because health.petals.ml is down: {repr(e)}")
+            logger.warning(f"Skipping reachability check because health.petals.dev is down: {repr(e)}")
             return
 
     raise RuntimeError(
         f"Server has not become reachable from the Internet:\n\n"
         f"{response['message']}\n\n"
         f"You need to fix your port forwarding and/or firewall settings. How to do that:\n\n"
         f"    1. Choose a specific port for the Petals server, for example, 31337.\n"
```

### Comparing `petals-2.0.0.post2/src/petals/server/server.py` & `petals-2.0.0.post3/src/petals/server/server.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/task_pool.py` & `petals-2.0.0.post3/src/petals/server/task_pool.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/task_prioritizer.py` & `petals-2.0.0.post3/src/petals/server/task_prioritizer.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/server/throughput.py` & `petals-2.0.0.post3/src/petals/server/throughput.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/asyncio.py` & `petals-2.0.0.post3/src/petals/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/auto_config.py` & `petals-2.0.0.post3/src/petals/utils/auto_config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/convert_block.py` & `petals-2.0.0.post3/src/petals/utils/convert_block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/disk_cache.py` & `petals-2.0.0.post3/src/petals/utils/disk_cache.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/generation_algorithms.py` & `petals-2.0.0.post3/src/petals/utils/generation_algorithms.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/generation_constraints.py` & `petals-2.0.0.post3/src/petals/utils/generation_constraints.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/logging.py` & `petals-2.0.0.post3/src/petals/utils/logging.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/peft.py` & `petals-2.0.0.post3/src/petals/utils/peft.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/ping.py` & `petals-2.0.0.post3/src/petals/utils/ping.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals/utils/version.py` & `petals-2.0.0.post3/src/petals/utils/version.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/src/petals.egg-info/PKG-INFO` & `petals-2.0.0.post3/src/petals.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 2.0.0.post2
+Version: 2.0.0.post3
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -88,28 +88,28 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](http://chat.petals.ml) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.ml)
-- [Monitor](http://health.petals.ml) for the public swarm: [source code](https://github.com/borzunov/health.petals.ml)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
 
 ## How does it work?
 
 - Petals runs large language models like [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom) **collaboratively** — you load a small part of the model, then team up with people serving the other parts to run inference or fine-tuning.
-- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
+- Single-batch inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-workshop/petals#benchmarks) than offloading, enough for [chatbots](https://chat.petals.dev) and other interactive apps. Parallel inference reaches hundreds of tokens/sec.
 - Beyond classic language model APIs — you can employ any fine-tuning and sampling methods, execute custom paths through the model, or see its hidden states. You get the comforts of an API with the flexibility of PyTorch.
 
 <p align="center">
     <img src="https://i.imgur.com/RTYF3yW.png" width="800">
 </p>
 
 <p align="center">
@@ -241,9 +241,9 @@
 
 --------------------------------------------------------------------------------
 
 <p align="center">
     This project is a part of the <a href="https://bigscience.huggingface.co/">BigScience</a> research workshop.
 </p>
 <p align="center">
-    <img src="https://petals.ml/bigscience.png" width="150">
+    <img src="https://petals.dev/bigscience.png" width="150">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 2.0.0.post2 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 2.0.0.post3 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -69,36 +69,36 @@
 more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
-guides: - [Chatbot web app](http://chat.petals.ml) (connects to Petals via an
+guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
 HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
-chat.petals.ml) - [Monitor](http://health.petals.ml) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.ml) - Launch your own
+chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
+[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
 swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
 own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
 people serving the other parts to run inference or fine-tuning. - Single-batch
 inference runs at up to 6 steps/sec for LLaMA 2 (70B) and &approx; 1 step/sec
 for BLOOM-176B. This is [up to 10x faster](https://github.com/bigscience-
-workshop/petals#benchmarks) than offloading, enough for [chatbots](http://
-chat.petals.ml) and other interactive apps. Parallel inference reaches hundreds
-of tokens/sec. - Beyond classic language model APIs â you can employ any
-fine-tuning and sampling methods, execute custom paths through the model, or
-see its hidden states. You get the comforts of an API with the flexibility of
-PyTorch.
+workshop/petals#benchmarks) than offloading, enough for [chatbots](https://
+chat.petals.dev) and other interactive apps. Parallel inference reaches
+hundreds of tokens/sec. - Beyond classic language model APIs â you can employ
+any fine-tuning and sampling methods, execute custom paths through the model,
+or see its hidden states. You get the comforts of an API with the flexibility
+of PyTorch.
                        [https://i.imgur.com/RTYF3yW.png]
                    ð  See_FAQ            ð  Read_paper
 ## Installation Here's how to install Petals with [Anaconda](https://
 www.anaconda.com/products/distribution) on Linux: ```bash conda install pytorch
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install --upgrade petals ``` If you
 don't use Anaconda, you can install PyTorch in [any other way](https://
 pytorch.org/get-started/locally/). If you want to run models with 8-bit
@@ -145,8 +145,8 @@
 {borzunov2022petals, title = {Petals: Collaborative Inference and Fine-tuning
 of Large Models}, author = {Borzunov, Alexander and Baranchuk, Dmitry and
 Dettmers, Tim and Ryabinin, Max and Belkada, Younes and Chumachenko, Artem and
 Samygin, Pavel and Raffel, Colin}, journal = {arXiv preprint arXiv:2209.01188},
 year = {2022}, url = {https://arxiv.org/abs/2209.01188} } ``` -----------------
 ---------------------------------------------------------------
           This project is a part of the BigScience research workshop.
-                      [https://petals.ml/bigscience.png]
+                      [https://petals.dev/bigscience.png]
```

### Comparing `petals-2.0.0.post2/src/petals.egg-info/SOURCES.txt` & `petals-2.0.0.post3/src/petals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_aux_functions.py` & `petals-2.0.0.post3/tests/test_aux_functions.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_block_exact_match.py` & `petals-2.0.0.post3/tests/test_block_exact_match.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_chained_calls.py` & `petals-2.0.0.post3/tests/test_chained_calls.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_dtype.py` & `petals-2.0.0.post3/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_full_model.py` & `petals-2.0.0.post3/tests/test_full_model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_peft.py` & `petals-2.0.0.post3/tests/test_peft.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_priority_pool.py` & `petals-2.0.0.post3/tests/test_priority_pool.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_remote_sequential.py` & `petals-2.0.0.post3/tests/test_remote_sequential.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_sequence_manager.py` & `petals-2.0.0.post3/tests/test_sequence_manager.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_server_stats.py` & `petals-2.0.0.post3/tests/test_server_stats.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.0.post2/tests/test_tensor_parallel.py` & `petals-2.0.0.post3/tests/test_tensor_parallel.py`

 * *Files identical despite different names*

