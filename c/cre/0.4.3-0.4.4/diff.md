# Comparing `tmp/cre-0.4.3.tar.gz` & `tmp/cre-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cre-0.4.3.tar", last modified: Thu Jul 20 17:57:45 2023, max compression
+gzip compressed data, was "cre-0.4.4.tar", last modified: Thu Jul 20 19:02:33 2023, max compression
```

## Comparing `cre-0.4.3.tar` & `cre-0.4.4.tar`

### file list

```diff
@@ -1,87 +1,86 @@
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.439347 cre-0.4.3/
--rw-rw-r--   0 danny     (1000) danny     (1000)       61 2023-07-18 17:53:58.000000 cre-0.4.3/.gitignore
--rw-rw-r--   0 danny     (1000) danny     (1000)     1073 2023-07-18 16:48:38.000000 cre-0.4.3/LICENSE.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-07-20 17:57:45.439347 cre-0.4.3/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)    11270 2023-02-21 03:43:23.000000 cre-0.4.3/README.md
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.431347 cre-0.4.3/console/
--rw-rw-r--   0 danny     (1000) danny     (1000)      573 2022-06-12 05:16:49.000000 cre-0.4.3/console/cre_exec.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.431347 cre-0.4.3/cre/
--rw-rw-r--   0 danny     (1000) danny     (1000)     1107 2023-02-21 20:06:54.000000 cre-0.4.3/cre/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2116 2023-02-27 02:33:38.000000 cre-0.4.3/cre/attr_filter.py
--rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.3/cre/caching.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.431347 cre-0.4.3/cre/cfuncs/
--rw-rw-r--   0 danny     (1000) danny     (1000)      137 2022-06-12 05:16:49.000000 cre-0.4.3/cre/cfuncs/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2768 2022-09-06 21:55:51.000000 cre-0.4.3/cre/cfuncs/cre_cfuncs.c
--rw-rw-r--   0 danny     (1000) danny     (1000)     3603 2023-05-01 14:43:41.000000 cre-0.4.3/cre/change_event.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    77543 2023-06-02 04:34:43.000000 cre-0.4.3/cre/conditions.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    15471 2023-06-02 04:46:55.000000 cre-0.4.3/cre/context.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8289 2023-05-01 16:10:37.000000 cre-0.4.3/cre/core.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2621 2023-05-14 16:29:49.000000 cre-0.4.3/cre/default_funcs.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    17363 2023-06-02 01:45:53.000000 cre-0.4.3/cre/dynamic_exec.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    47344 2023-05-27 16:52:23.000000 cre-0.4.3/cre/fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    16306 2023-02-21 03:58:09.000000 cre-0.4.3/cre/fact_intrinsics.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    93320 2023-07-01 20:52:29.000000 cre-0.4.3/cre/func.py
--rw-rw-r--   0 danny     (1000) danny     (1000)      656 2023-05-08 03:39:17.000000 cre-0.4.3/cre/garbage3.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     1088 2023-04-15 18:57:56.000000 cre-0.4.3/cre/garbage31.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    80851 2023-06-01 22:01:56.000000 cre-0.4.3/cre/garbage_sc_stash.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    80080 2023-06-01 22:09:06.000000 cre-0.4.3/cre/garbage_sc_stash2.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     3850 2023-06-05 14:24:45.000000 cre-0.4.3/cre/gval.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2270 2023-05-11 22:41:34.000000 cre-0.4.3/cre/hashing.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8288 2022-06-12 05:16:49.000000 cre-0.4.3/cre/make_source.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    81594 2023-06-05 04:30:24.000000 cre-0.4.3/cre/matching.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    38451 2023-06-05 03:56:00.000000 cre-0.4.3/cre/memset.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    20497 2023-05-25 18:45:58.000000 cre-0.4.3/cre/obj.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     5440 2023-02-21 03:58:09.000000 cre-0.4.3/cre/rule.py
--rwxrwxr-x   0 danny     (1000) danny     (1000)      217 2022-06-12 05:16:49.000000 cre-0.4.3/cre/run_tests
--rw-rw-r--   0 danny     (1000) danny     (1000)    81185 2023-07-01 04:12:55.000000 cre-0.4.3/cre/sc_planner.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     9511 2023-02-20 22:35:46.000000 cre-0.4.3/cre/structref.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     4365 2023-06-30 10:50:15.000000 cre-0.4.3/cre/token.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.435347 cre-0.4.3/cre/transform/
--rw-rw-r--   0 danny     (1000) danny     (1000)      313 2023-01-22 23:11:50.000000 cre-0.4.3/cre/transform/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     5393 2023-04-28 19:00:06.000000 cre-0.4.3/cre/transform/enumerizer.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    19609 2023-04-28 21:18:52.000000 cre-0.4.3/cre/transform/feature_applier.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    12239 2023-04-28 18:41:19.000000 cre-0.4.3/cre/transform/flattener.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2198 2023-02-20 05:54:27.000000 cre-0.4.3/cre/transform/incr_processor.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2682 2023-06-20 17:57:39.000000 cre-0.4.3/cre/transform/memset_builder.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    30398 2023-02-21 03:58:09.000000 cre-0.4.3/cre/transform/relative_encoder.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6866 2023-05-08 03:06:41.000000 cre-0.4.3/cre/transform/vectorizer.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    12224 2023-04-28 20:21:41.000000 cre-0.4.3/cre/tuple_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    10483 2023-05-07 23:44:51.000000 cre-0.4.3/cre/type_conv.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    47635 2023-05-08 00:32:29.000000 cre-0.4.3/cre/utils.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    38375 2023-06-13 20:23:15.000000 cre-0.4.3/cre/var.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6072 2022-06-12 05:16:49.000000 cre-0.4.3/cre/vector.py
--rw-rw-r--   0 danny     (1000) danny     (1000)       22 2023-04-29 18:30:06.000000 cre-0.4.3/cre/version.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.431347 cre-0.4.3/cre.egg-info/
--rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)     1588 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/SOURCES.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/dependency_links.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       47 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/entry_points.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       55 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/requires.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       27 2023-07-20 17:57:45.000000 cre-0.4.3/cre.egg-info/top_level.txt
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.435347 cre-0.4.3/cre_caching/
--rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.3/cre_caching/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8199 2023-05-24 20:20:42.000000 cre-0.4.3/cre_caching/caching.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.435347 cre-0.4.3/notes/
--rw-rw-r--   0 danny     (1000) danny     (1000)     3560 2022-06-12 05:16:49.000000 cre-0.4.3/notes/SeqGrammarInduction.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 17:37:22.000000 cre-0.4.3/pyproject.toml
--rw-rw-r--   0 danny     (1000) danny     (1000)       24 2023-07-18 17:53:26.000000 cre-0.4.3/requirements.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       38 2023-07-20 17:57:45.439347 cre-0.4.3/setup.cfg
--rw-rw-r--   0 danny     (1000) danny     (1000)     3850 2023-07-19 12:45:39.000000 cre-0.4.3/setup.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 17:57:45.439347 cre-0.4.3/tests/
--rw-rw-r--   0 danny     (1000) danny     (1000)    16694 2023-06-02 04:03:51.000000 cre-0.4.3/tests/test_conditions.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    19089 2023-06-02 05:12:00.000000 cre-0.4.3/tests/test_cre_func.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    28780 2023-02-21 03:58:22.000000 cre-0.4.3/tests/test_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6378 2023-05-08 00:34:10.000000 cre-0.4.3/tests/test_feature_applier.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     5101 2023-05-15 19:52:19.000000 cre-0.4.3/tests/test_flattener.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2466 2023-01-22 23:11:50.000000 cre-0.4.3/tests/test_incr_processor.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     1326 2022-06-12 05:16:49.000000 cre-0.4.3/tests/test_make_source.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    23167 2023-05-08 00:29:11.000000 cre-0.4.3/tests/test_matching.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    19201 2023-05-08 03:49:51.000000 cre-0.4.3/tests/test_memset.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    16939 2023-05-08 00:36:44.000000 cre-0.4.3/tests/test_processing_pipeline.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    10230 2023-05-08 00:39:06.000000 cre-0.4.3/tests/test_relative_encoder.py
--rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-02-16 07:15:18.000000 cre-0.4.3/tests/test_rule.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    32453 2023-07-01 04:32:30.000000 cre-0.4.3/tests/test_sc_planner.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6565 2023-02-21 03:58:22.000000 cre-0.4.3/tests/test_tuple_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     3440 2023-02-20 06:20:35.000000 cre-0.4.3/tests/test_type_conv.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     7282 2023-02-20 05:54:27.000000 cre-0.4.3/tests/test_utils.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     4416 2023-04-29 17:16:43.000000 cre-0.4.3/tests/test_vectorizer.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.427258 cre-0.4.4/
+-rw-rw-r--   0 danny     (1000) danny     (1000)       61 2023-07-18 17:53:58.000000 cre-0.4.4/.gitignore
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1073 2023-07-18 16:48:38.000000 cre-0.4.4/LICENSE.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-07-20 19:02:33.427258 cre-0.4.4/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)    11270 2023-02-21 03:43:23.000000 cre-0.4.4/README.md
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/cre/
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1107 2023-02-21 20:06:54.000000 cre-0.4.4/cre/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2116 2023-02-27 02:33:38.000000 cre-0.4.4/cre/attr_filter.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.4/cre/caching.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/cre/cfuncs/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      137 2022-06-12 05:16:49.000000 cre-0.4.4/cre/cfuncs/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2768 2022-09-06 21:55:51.000000 cre-0.4.4/cre/cfuncs/cre_cfuncs.c
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3603 2023-05-01 14:43:41.000000 cre-0.4.4/cre/change_event.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    77543 2023-06-02 04:34:43.000000 cre-0.4.4/cre/conditions.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      573 2022-06-12 05:16:49.000000 cre-0.4.4/cre/console_script.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    15471 2023-06-02 04:46:55.000000 cre-0.4.4/cre/context.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8289 2023-05-01 16:10:37.000000 cre-0.4.4/cre/core.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2621 2023-05-14 16:29:49.000000 cre-0.4.4/cre/default_funcs.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    17363 2023-06-02 01:45:53.000000 cre-0.4.4/cre/dynamic_exec.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    47344 2023-05-27 16:52:23.000000 cre-0.4.4/cre/fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16306 2023-02-21 03:58:09.000000 cre-0.4.4/cre/fact_intrinsics.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    93320 2023-07-01 20:52:29.000000 cre-0.4.4/cre/func.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      656 2023-05-08 03:39:17.000000 cre-0.4.4/cre/garbage3.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1088 2023-04-15 18:57:56.000000 cre-0.4.4/cre/garbage31.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    80851 2023-06-01 22:01:56.000000 cre-0.4.4/cre/garbage_sc_stash.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    80080 2023-06-01 22:09:06.000000 cre-0.4.4/cre/garbage_sc_stash2.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3850 2023-06-05 14:24:45.000000 cre-0.4.4/cre/gval.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2270 2023-05-11 22:41:34.000000 cre-0.4.4/cre/hashing.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8288 2022-06-12 05:16:49.000000 cre-0.4.4/cre/make_source.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    81594 2023-06-05 04:30:24.000000 cre-0.4.4/cre/matching.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    38451 2023-06-05 03:56:00.000000 cre-0.4.4/cre/memset.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    20497 2023-05-25 18:45:58.000000 cre-0.4.4/cre/obj.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     5446 2023-07-20 18:51:24.000000 cre-0.4.4/cre/rule.py
+-rwxrwxr-x   0 danny     (1000) danny     (1000)      217 2022-06-12 05:16:49.000000 cre-0.4.4/cre/run_tests
+-rw-rw-r--   0 danny     (1000) danny     (1000)    81185 2023-07-01 04:12:55.000000 cre-0.4.4/cre/sc_planner.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     9511 2023-02-20 22:35:46.000000 cre-0.4.4/cre/structref.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     4365 2023-06-30 10:50:15.000000 cre-0.4.4/cre/token.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/cre/transform/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      313 2023-01-22 23:11:50.000000 cre-0.4.4/cre/transform/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     5393 2023-04-28 19:00:06.000000 cre-0.4.4/cre/transform/enumerizer.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    19609 2023-04-28 21:18:52.000000 cre-0.4.4/cre/transform/feature_applier.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    12239 2023-04-28 18:41:19.000000 cre-0.4.4/cre/transform/flattener.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2198 2023-02-20 05:54:27.000000 cre-0.4.4/cre/transform/incr_processor.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2682 2023-06-20 17:57:39.000000 cre-0.4.4/cre/transform/memset_builder.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    30398 2023-02-21 03:58:09.000000 cre-0.4.4/cre/transform/relative_encoder.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6866 2023-05-08 03:06:41.000000 cre-0.4.4/cre/transform/vectorizer.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    12224 2023-04-28 20:21:41.000000 cre-0.4.4/cre/tuple_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    10483 2023-05-07 23:44:51.000000 cre-0.4.4/cre/type_conv.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    47635 2023-05-08 00:32:29.000000 cre-0.4.4/cre/utils.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    38334 2023-07-20 18:51:59.000000 cre-0.4.4/cre/var.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6072 2022-06-12 05:16:49.000000 cre-0.4.4/cre/vector.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)       22 2023-04-29 18:30:06.000000 cre-0.4.4/cre/version.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/cre.egg-info/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1590 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/SOURCES.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/dependency_links.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       49 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/entry_points.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       55 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/requires.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       27 2023-07-20 19:02:33.000000 cre-0.4.4/cre.egg-info/top_level.txt
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/cre_caching/
+-rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.4/cre_caching/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8199 2023-05-24 20:20:42.000000 cre-0.4.4/cre_caching/caching.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.423258 cre-0.4.4/notes/
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3560 2022-06-12 05:16:49.000000 cre-0.4.4/notes/SeqGrammarInduction.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 17:37:22.000000 cre-0.4.4/pyproject.toml
+-rw-rw-r--   0 danny     (1000) danny     (1000)       24 2023-07-18 17:53:26.000000 cre-0.4.4/requirements.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       38 2023-07-20 19:02:33.431258 cre-0.4.4/setup.cfg
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3852 2023-07-20 18:45:48.000000 cre-0.4.4/setup.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-20 19:02:33.427258 cre-0.4.4/tests/
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16694 2023-06-02 04:03:51.000000 cre-0.4.4/tests/test_conditions.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    19089 2023-06-02 05:12:00.000000 cre-0.4.4/tests/test_cre_func.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    28780 2023-02-21 03:58:22.000000 cre-0.4.4/tests/test_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6378 2023-05-08 00:34:10.000000 cre-0.4.4/tests/test_feature_applier.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     5101 2023-05-15 19:52:19.000000 cre-0.4.4/tests/test_flattener.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2466 2023-01-22 23:11:50.000000 cre-0.4.4/tests/test_incr_processor.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1326 2022-06-12 05:16:49.000000 cre-0.4.4/tests/test_make_source.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    23167 2023-05-08 00:29:11.000000 cre-0.4.4/tests/test_matching.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    19201 2023-05-08 03:49:51.000000 cre-0.4.4/tests/test_memset.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16939 2023-05-08 00:36:44.000000 cre-0.4.4/tests/test_processing_pipeline.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    10230 2023-05-08 00:39:06.000000 cre-0.4.4/tests/test_relative_encoder.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-02-16 07:15:18.000000 cre-0.4.4/tests/test_rule.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    32453 2023-07-01 04:32:30.000000 cre-0.4.4/tests/test_sc_planner.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6565 2023-02-21 03:58:22.000000 cre-0.4.4/tests/test_tuple_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3440 2023-02-20 06:20:35.000000 cre-0.4.4/tests/test_type_conv.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     7282 2023-02-20 05:54:27.000000 cre-0.4.4/tests/test_utils.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     4416 2023-04-29 17:16:43.000000 cre-0.4.4/tests/test_vectorizer.py
```

### Comparing `cre-0.4.3/LICENSE.txt` & `cre-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/PKG-INFO` & `cre-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cre
-Version: 0.4.3
+Version: 0.4.4
 Summary: A rule engine for Python powered by numba.
 Home-page: https://github.com/DannyWeitekamp/Cognitive-Rule-Engine
 Author: Daniel Weitekamp
 Author-email: dannyweitekamp@gmail.com
 License: MIT
 Keywords: rule engine,expert system,production rules
 Platform: UNKNOWN
```

### Comparing `cre-0.4.3/README.md` & `cre-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/console/cre_exec.py` & `cre-0.4.4/cre/console_script.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/__init__.py` & `cre-0.4.4/cre/__init__.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/attr_filter.py` & `cre-0.4.4/cre/attr_filter.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/cfuncs/cre_cfuncs.c` & `cre-0.4.4/cre/cfuncs/cre_cfuncs.c`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/change_event.py` & `cre-0.4.4/cre/change_event.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/conditions.py` & `cre-0.4.4/cre/conditions.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/context.py` & `cre-0.4.4/cre/context.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/core.py` & `cre-0.4.4/cre/core.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/default_funcs.py` & `cre-0.4.4/cre/default_funcs.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/dynamic_exec.py` & `cre-0.4.4/cre/dynamic_exec.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/fact.py` & `cre-0.4.4/cre/fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/fact_intrinsics.py` & `cre-0.4.4/cre/fact_intrinsics.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/func.py` & `cre-0.4.4/cre/func.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/garbage3.py` & `cre-0.4.4/cre/garbage3.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/garbage31.py` & `cre-0.4.4/cre/garbage31.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/garbage_sc_stash.py` & `cre-0.4.4/cre/garbage_sc_stash.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/garbage_sc_stash2.py` & `cre-0.4.4/cre/garbage_sc_stash2.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/gval.py` & `cre-0.4.4/cre/gval.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/hashing.py` & `cre-0.4.4/cre/hashing.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/make_source.py` & `cre-0.4.4/cre/make_source.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/matching.py` & `cre-0.4.4/cre/matching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/memset.py` & `cre-0.4.4/cre/memset.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/obj.py` & `cre-0.4.4/cre/obj.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/rule.py` & `cre-0.4.4/cre/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 from cre.memset import MemSetType
 import cloudpickle
 # from numba.experimental.function_type import _get_wrapper_address
 
 match_types = cloudpickle.loads({cloudpickle.dumps(match_types)})
 rhs_pyfunc = cloudpickle.loads({cloudpickle.dumps(rhs_pyfunc)})
 
-print(match_types)
+# print(match_types)
 signature = types.void(MemSetType, *match_types)
-print(signature)
+# print(signature)
 rhs = njit(signature, cache=True)(rhs_pyfunc)
 
 @njit(types.void(MemSetType, i8[::1]), cache=True)
 def rhs_ptrs(wm, ptrs):
     args = _struct_tuple_from_pointer_arr(match_types, ptrs)
     rhs(wm, *args)
 
@@ -131,15 +131,15 @@
             long_hash = unique_hash([match_types, func_src])
             if(not source_in_cache('Rule_RHS', long_hash)):
                 source = gen_rhs_source(match_types, rhs)
                 source_to_cache('Rule_RHS', long_hash, source)
 
         with PrintElapse("run"):
             rhs_ptrs = import_from_cached('Rule_RHS', long_hash, ['rhs_ptrs'])['rhs_ptrs']
-            print(list(rhs_ptrs.overloads.keys()))
+            # print(list(rhs_ptrs.overloads.keys()))
         with PrintElapse("assign"):
             rule_assign_imper_rhs(st, rhs_ptrs)
             st._rhs_pyfunc = rhs
         return st
 
 
 @njit(cache=True)
```

### Comparing `cre-0.4.3/cre/sc_planner.py` & `cre-0.4.4/cre/sc_planner.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/structref.py` & `cre-0.4.4/cre/structref.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/token.py` & `cre-0.4.4/cre/token.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/enumerizer.py` & `cre-0.4.4/cre/transform/enumerizer.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/feature_applier.py` & `cre-0.4.4/cre/transform/feature_applier.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/flattener.py` & `cre-0.4.4/cre/transform/flattener.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/incr_processor.py` & `cre-0.4.4/cre/transform/incr_processor.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/memset_builder.py` & `cre-0.4.4/cre/transform/memset_builder.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/relative_encoder.py` & `cre-0.4.4/cre/transform/relative_encoder.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/transform/vectorizer.py` & `cre-0.4.4/cre/transform/vectorizer.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/tuple_fact.py` & `cre-0.4.4/cre/tuple_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/type_conv.py` & `cre-0.4.4/cre/type_conv.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/utils.py` & `cre-0.4.4/cre/utils.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre/var.py` & `cre-0.4.4/cre/var.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 }
 
 class VarTypeClass(CREObjTypeClass):
     t_id = T_ID_VAR
     type_cache = {}
 
     def __new__(cls, base_type=None, head_type=None):
-        print(cls, base_type, head_type)
         if(head_type is None): head_type = base_type
         
         unq_tup = (base_type, head_type)
 
         self = cls.type_cache.get(unq_tup, None)
         if(self is not None):
             return self
```

### Comparing `cre-0.4.3/cre/vector.py` & `cre-0.4.4/cre/vector.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/cre.egg-info/PKG-INFO` & `cre-0.4.4/cre.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cre
-Version: 0.4.3
+Version: 0.4.4
 Summary: A rule engine for Python powered by numba.
 Home-page: https://github.com/DannyWeitekamp/Cognitive-Rule-Engine
 Author: Daniel Weitekamp
 Author-email: dannyweitekamp@gmail.com
 License: MIT
 Keywords: rule engine,expert system,production rules
 Platform: UNKNOWN
```

### Comparing `cre-0.4.3/cre.egg-info/SOURCES.txt` & `cre-0.4.4/cre.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .gitignore
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
-console/cre_exec.py
 cre/__init__.py
 cre/attr_filter.py
 cre/caching.py
 cre/change_event.py
 cre/conditions.py
+cre/console_script.py
 cre/context.py
 cre/core.py
 cre/default_funcs.py
 cre/dynamic_exec.py
 cre/fact.py
 cre/fact_intrinsics.py
 cre/func.py
```

### Comparing `cre-0.4.3/cre_caching/caching.py` & `cre-0.4.4/cre_caching/caching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/notes/SeqGrammarInduction.txt` & `cre-0.4.4/notes/SeqGrammarInduction.txt`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/setup.py` & `cre-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     __version__ = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # TODO: Remove once version dependancy issues in caching are fixed
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 
 # Read requirements.txt for requirements
 with open('requirements.txt') as f: 
     requirements = f.readlines() 
 
   
@@ -101,15 +101,15 @@
         long_description_content_type ="text/markdown", 
         license ='MIT', 
         packages = find_packages(), 
         include_package_data=True, # Prevents files being omitting from wheel. 
 
         entry_points={
             "console_scripts": [
-                "cre = console.cre_exec:main"
+                "cre = cre.console_script:main"
             ]
         },
         ext_modules = get_ext_modules(),
 
 
         classifiers =[ 
             "Programming Language :: Python :: 3",
```

### Comparing `cre-0.4.3/tests/test_conditions.py` & `cre-0.4.4/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_cre_func.py` & `cre-0.4.4/tests/test_cre_func.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_fact.py` & `cre-0.4.4/tests/test_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_feature_applier.py` & `cre-0.4.4/tests/test_feature_applier.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_flattener.py` & `cre-0.4.4/tests/test_flattener.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_incr_processor.py` & `cre-0.4.4/tests/test_incr_processor.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_make_source.py` & `cre-0.4.4/tests/test_make_source.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_matching.py` & `cre-0.4.4/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_memset.py` & `cre-0.4.4/tests/test_memset.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_processing_pipeline.py` & `cre-0.4.4/tests/test_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_relative_encoder.py` & `cre-0.4.4/tests/test_relative_encoder.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_rule.py` & `cre-0.4.4/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_sc_planner.py` & `cre-0.4.4/tests/test_sc_planner.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_tuple_fact.py` & `cre-0.4.4/tests/test_tuple_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_type_conv.py` & `cre-0.4.4/tests/test_type_conv.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_utils.py` & `cre-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.3/tests/test_vectorizer.py` & `cre-0.4.4/tests/test_vectorizer.py`

 * *Files identical despite different names*

