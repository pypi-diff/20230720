# Comparing `tmp/taskcluster-taskgraph-5.6.2.tar.gz` & `tmp/taskcluster-taskgraph-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taskcluster-taskgraph-5.6.2.tar", last modified: Mon Jul 17 18:57:47 2023, max compression
+gzip compressed data, was "taskcluster-taskgraph-5.7.0.tar", last modified: Thu Jul 20 14:25:19 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.6.2.tar` & `taskcluster-taskgraph-5.7.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/MANIFEST.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/README.rst
--rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.2/pyproject.toml
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/requirements/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      179 2023-07-17 18:56:50.000000 taskcluster-taskgraph-5.6.2/requirements/base.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)    20339 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/requirements/base.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/requirements/dev.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.2/requirements/dev.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.2/requirements/test.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9241 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/requirements/test.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)      203 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-07-17 18:56:50.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1836 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/cancel.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13122 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9387 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/actions/util.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4822 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/config.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/filter_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15541 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4680 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/graph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/loader/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/loader/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/loader/default.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/loader/transform.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/morph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/parameters.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/hgrc
--rw-r--r--   0 ahal      (1000) ahal      (1000)    30813 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    45128 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/run-task
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3240 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2434 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5146 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10479 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/from_deps.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5897 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9814 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    52086 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/archive.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2592 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11699 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/hash.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/shell.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/templates.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18780 2023-07-06 14:16:59.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8947 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2498 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      990 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-17 18:57:47.000000 taskcluster-taskgraph-5.6.2/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.6.2/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_actions_registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.6.2/test/test_create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_graph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.2/test/test_main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_morph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.2/test/test_optimize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_optimize_strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_parameters.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_scripts_fetch_content.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.2/test/test_scripts_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_transform_docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6985 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_from_deps.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_job.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_job_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_job_toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    25785 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/test/test_transforms_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.2/test/test_util_dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_util_parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.6.2/test/test_util_python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_util_taskcluster.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_templates.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15598 2023-07-06 14:10:15.000000 taskcluster-taskgraph-5.6.2/test/test_util_vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.2/test/test_util_verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.2/test/test_util_workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1005 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.2/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      179 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20339 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9241 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      203 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-07-20 14:24:45.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1836 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13122 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9387 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4822 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15667 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4680 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11918 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30813 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    45128 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3240 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2434 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5146 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10479 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17324 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5897 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9814 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    52254 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2592 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11699 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18780 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8947 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2498 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      990 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.7.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.7.0/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8883 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6985 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    25785 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.7.0/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15598 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1005 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taskcluster-taskgraph-5.6.2/LICENSE` & `taskcluster-taskgraph-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/PKG-INFO` & `taskcluster-taskgraph-5.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.6.2
+Version: 5.7.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.6.2/README.rst` & `taskcluster-taskgraph-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/pyproject.toml` & `taskcluster-taskgraph-5.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/requirements/base.txt` & `taskcluster-taskgraph-5.7.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/requirements/dev.txt` & `taskcluster-taskgraph-5.7.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/requirements/test.txt` & `taskcluster-taskgraph-5.7.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/setup.py` & `taskcluster-taskgraph-5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.6.2
+Version: 5.7.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.6.2"
+__version__ = "5.7.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/config.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/create.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,16 @@
         logger.info("Generating target task graph")
         # include all tasks with `always_target` set
         if parameters["enable_always_target"]:
             always_target_tasks = {
                 t.label
                 for t in full_task_graph.tasks.values()
                 if t.attributes.get("always_target")
+                if parameters["enable_always_target"] is True
+                or t.kind in parameters["enable_always_target"]
             }
         else:
             always_target_tasks = set()
         logger.info(
             "Adding %d tasks with `always_target` attribute"
             % (len(always_target_tasks) - len(always_target_tasks & target_tasks))
         )
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/main.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     {
         Required("base_repository"): str,
         Required("base_ref"): str,
         Required("base_rev"): str,
         Required("build_date"): int,
         Required("build_number"): int,
         Required("do_not_optimize"): [str],
-        Required("enable_always_target"): bool,
+        Required("enable_always_target"): Any(bool, [str]),
         Required("existing_tasks"): {str: str},
         Required("filters"): [str],
         Required("head_ref"): str,
         Required("head_repository"): str,
         Required("head_rev"): str,
         Required("head_tag"): str,
         Required("level"): str,
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/task.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,17 @@
     the task description is already set up, but without a payload."""
 
     def wrap(func):
         for_run_using = registry.setdefault(run_using, {})
         if worker_implementation in for_run_using:
             raise Exception(
                 "run_job_using({!r}, {!r}) already exists: {!r}".format(
-                    run_using, worker_implementation, for_run_using[run_using]
+                    run_using,
+                    worker_implementation,
+                    for_run_using[worker_implementation],
                 )
             )
         for_run_using[worker_implementation] = (func, schema, defaults)
         return func
 
     return wrap
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,26 +240,28 @@
 
 def payload_builder(name, schema):
     schema = Schema({Required("implementation"): name, Optional("os"): str}).extend(
         schema
     )
 
     def wrap(func):
+        assert name not in payload_builders, f"duplicate payload builder name {name}"
         payload_builders[name] = PayloadBuilder(schema, func)
         return func
 
     return wrap
 
 
 # define a collection of index builders, depending on the type implementation
 index_builders = {}
 
 
 def index_builder(name):
     def wrap(func):
+        assert name not in index_builders, f"duplicate index builder name {name}"
         index_builders[name] = func
         return func
 
     return wrap
 
 
 UNSUPPORTED_INDEX_PRODUCT_ERROR = """\
```

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.7.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.7.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_actions_registry.py` & `taskcluster-taskgraph-5.7.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_create.py` & `taskcluster-taskgraph-5.7.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_decision.py` & `taskcluster-taskgraph-5.7.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_files_changed.py` & `taskcluster-taskgraph-5.7.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_generator.py` & `taskcluster-taskgraph-5.7.0/test/test_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,50 @@
     assert sorted(tgg.target_task_graph.tasks.keys()) == sorted(
         ["_fake-t-0", "_fake-t-1", "_ignore-t-0", "_ignore-t-1"]
     )
     assert sorted(t.label for t in tgg.optimized_task_graph.tasks.values()) == sorted(
         ["_fake-t-0", "_fake-t-1", "_ignore-t-0", "_ignore-t-1"]
     )
 
+    # Test `enable_always_target: ["_fake"]`
+    tgg_args = {
+        "target_tasks": ["_fake-t-0", "_fake-t-1", "_ignore-t-0", "_ignore-t-1"],
+        "kinds": [
+            (
+                "_fake",
+                {
+                    "task-defaults": {
+                        "attributes": {"always_target": True},
+                        "optimization": {"odd": None},
+                    }
+                },
+            ),
+            (
+                "_ignore",
+                {
+                    "task-defaults": {
+                        "attributes": {"always_target": True},
+                        "optimization": {"even": None},
+                    }
+                },
+            ),
+        ],
+        "params": {"enable_always_target": ["_fake"], "optimize_target_tasks": False},
+    }
+    tgg = maketgg(**tgg_args)
+    assert sorted(tgg.target_task_set.tasks.keys()) == sorted(
+        ["_fake-t-0", "_fake-t-1", "_ignore-t-0", "_ignore-t-1"]
+    )
+    assert sorted(tgg.target_task_graph.tasks.keys()) == sorted(
+        ["_fake-t-0", "_fake-t-1", "_fake-t-2", "_ignore-t-0", "_ignore-t-1"]
+    )
+    assert sorted(t.label for t in tgg.optimized_task_graph.tasks.values()) == sorted(
+        ["_fake-t-0", "_fake-t-1", "_fake-t-2", "_ignore-t-0", "_ignore-t-1"]
+    )
+
 
 def test_optimized_task_graph(maketgg):
     "The optimized task graph contains task ids"
     tgg = maketgg(["_fake-t-2"])
     tid = tgg.label_to_taskid
     assert tgg.optimized_task_graph.graph == graph.Graph(
         {tid["_fake-t-0"], tid["_fake-t-1"], tid["_fake-t-2"]},
```

### Comparing `taskcluster-taskgraph-5.6.2/test/test_graph.py` & `taskcluster-taskgraph-5.7.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_main.py` & `taskcluster-taskgraph-5.7.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_morph.py` & `taskcluster-taskgraph-5.7.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_optimize.py` & `taskcluster-taskgraph-5.7.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.7.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_parameters.py` & `taskcluster-taskgraph-5.7.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.7.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.7.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_target_tasks.py` & `taskcluster-taskgraph-5.7.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_taskgraph.py` & `taskcluster-taskgraph-5.7.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.7.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_base.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_job.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_transforms_task.py` & `taskcluster-taskgraph-5.7.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_attributes.py` & `taskcluster-taskgraph-5.7.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_dependencies.py` & `taskcluster-taskgraph-5.7.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_docker.py` & `taskcluster-taskgraph-5.7.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_memoize.py` & `taskcluster-taskgraph-5.7.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.7.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_path.py` & `taskcluster-taskgraph-5.7.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_python_path.py` & `taskcluster-taskgraph-5.7.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.7.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_schema.py` & `taskcluster-taskgraph-5.7.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.7.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_templates.py` & `taskcluster-taskgraph-5.7.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_time.py` & `taskcluster-taskgraph-5.7.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.7.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_vcs.py` & `taskcluster-taskgraph-5.7.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_verify.py` & `taskcluster-taskgraph-5.7.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.7.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.2/test/test_util_yaml.py` & `taskcluster-taskgraph-5.7.0/test/test_util_yaml.py`

 * *Files identical despite different names*

