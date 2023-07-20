# Comparing `tmp/coba-7.0.0.tar.gz` & `tmp/coba-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Mark\Projects\coba\dist\.tmp-b59ppplj\coba-7.0.0.tar", last modified: Mon Jul 17 05:11:17 2023, max compression
+gzip compressed data, was "coba-7.0.1.tar", last modified: Thu Jul 20 08:51:42 2023, max compression
```

## Comparing `coba-7.0.0.tar` & `coba-7.0.1.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/
--rw-rw-rw-   0        0        0       40 2023-05-11 00:41:22.000000 coba-7.0.0/AUTHORS
--rw-rw-rw-   0        0        0     1593 2023-05-11 00:41:22.000000 coba-7.0.0/LICENSE
--rw-rw-rw-   0        0        0     7942 2023-07-17 05:11:17.000000 coba-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7327 2023-06-16 06:32:50.000000 coba-7.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/
--rw-rw-rw-   0        0        0     1378 2023-07-17 05:09:07.000000 coba-7.0.0/coba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/backports/
--rw-rw-rw-   0        0        0       93 2023-06-18 23:59:19.000000 coba-7.0.0/coba/backports/__init__.py
--rw-rw-rw-   0        0        0      363 2023-06-18 23:59:52.000000 coba-7.0.0/coba/backports/metadata.py
--rw-rw-rw-   0        0        0      159 2023-06-14 06:26:06.000000 coba-7.0.0/coba/backports/typing.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/contexts/
--rw-rw-rw-   0        0        0      703 2023-06-19 00:00:10.000000 coba-7.0.0/coba/contexts/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-05-11 00:41:22.000000 coba-7.0.0/coba/contexts/cachers.py
--rw-rw-rw-   0        0        0     9263 2023-06-18 23:38:55.000000 coba-7.0.0/coba/contexts/core.py
--rw-rw-rw-   0        0        0     9726 2023-05-11 00:41:22.000000 coba-7.0.0/coba/contexts/loggers.py
--rw-rw-rw-   0        0        0    15634 2023-05-11 00:41:22.000000 coba-7.0.0/coba/encodings.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/environments/
--rw-rw-rw-   0        0        0     1448 2023-07-04 19:28:10.000000 coba-7.0.0/coba/environments/__init__.py
--rw-rw-rw-   0        0        0    22778 2023-07-17 04:57:59.000000 coba-7.0.0/coba/environments/core.py
--rw-rw-rw-   0        0        0    52607 2023-07-13 04:00:27.000000 coba-7.0.0/coba/environments/filters.py
--rw-rw-rw-   0        0        0    14347 2023-07-02 16:51:02.000000 coba-7.0.0/coba/environments/openml.py
--rw-rw-rw-   0        0        0     7646 2023-06-30 15:24:01.000000 coba-7.0.0/coba/environments/primitives.py
--rw-rw-rw-   0        0        0     2966 2023-07-04 17:42:06.000000 coba-7.0.0/coba/environments/serialized.py
--rw-rw-rw-   0        0        0     9551 2023-06-30 15:23:55.000000 coba-7.0.0/coba/environments/supervised.py
--rw-rw-rw-   0        0        0    24201 2023-06-25 05:50:30.000000 coba-7.0.0/coba/environments/synthetics.py
--rw-rw-rw-   0        0        0     6179 2023-05-11 00:41:22.000000 coba-7.0.0/coba/environments/templates.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/evaluators/
--rw-rw-rw-   0        0        0      217 2023-06-20 04:16:24.000000 coba-7.0.0/coba/evaluators/__init__.py
--rw-rw-rw-   0        0        0    15064 2023-06-18 22:54:36.000000 coba-7.0.0/coba/evaluators/offline.py
--rw-rw-rw-   0        0        0    22185 2023-07-13 05:34:25.000000 coba-7.0.0/coba/evaluators/online.py
--rw-rw-rw-   0        0        0     2095 2023-06-25 05:45:51.000000 coba-7.0.0/coba/evaluators/primitives.py
--rw-rw-rw-   0        0        0     1126 2023-05-11 00:41:22.000000 coba-7.0.0/coba/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/experiments/
--rw-rw-rw-   0        0        0      379 2023-06-19 00:00:43.000000 coba-7.0.0/coba/experiments/__init__.py
--rw-rw-rw-   0        0        0    10512 2023-07-09 16:24:44.000000 coba-7.0.0/coba/experiments/core.py
--rw-rw-rw-   0        0        0     7686 2023-07-04 17:08:08.000000 coba-7.0.0/coba/experiments/process.py
--rw-rw-rw-   0        0        0    65268 2023-07-14 04:53:15.000000 coba-7.0.0/coba/experiments/results.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/learners/
--rw-rw-rw-   0        0        0      761 2023-06-25 04:18:42.000000 coba-7.0.0/coba/learners/__init__.py
--rw-rw-rw-   0        0        0     7907 2023-05-11 00:41:22.000000 coba-7.0.0/coba/learners/bandit.py
--rw-rw-rw-   0        0        0     8055 2023-05-24 19:10:26.000000 coba-7.0.0/coba/learners/corral.py
--rw-rw-rw-   0        0        0     4947 2023-07-17 04:57:59.000000 coba-7.0.0/coba/learners/linucb.py
--rw-rw-rw-   0        0        0      958 2023-07-03 04:52:50.000000 coba-7.0.0/coba/learners/misguided.py
--rw-rw-rw-   0        0        0     4376 2023-05-27 01:06:49.000000 coba-7.0.0/coba/learners/primitives.py
--rw-rw-rw-   0        0        0     8927 2023-07-09 04:29:49.000000 coba-7.0.0/coba/learners/safety.py
--rw-rw-rw-   0        0        0    31011 2023-06-25 05:22:07.000000 coba-7.0.0/coba/learners/vowpal.py
--rw-rw-rw-   0        0        0     4139 2023-07-04 16:30:02.000000 coba-7.0.0/coba/multiprocessing.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/pipes/
--rw-rw-rw-   0        0        0     1456 2023-07-04 23:11:40.000000 coba-7.0.0/coba/pipes/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-05-15 13:57:18.000000 coba-7.0.0/coba/pipes/core.py
--rw-rw-rw-   0        0        0    16751 2023-07-03 07:12:05.000000 coba-7.0.0/coba/pipes/filters.py
--rw-rw-rw-   0        0        0    14968 2023-07-04 17:01:11.000000 coba-7.0.0/coba/pipes/multiprocessing.py
--rw-rw-rw-   0        0        0     6622 2023-07-04 16:53:56.000000 coba-7.0.0/coba/pipes/primitives.py
--rw-rw-rw-   0        0        0    13003 2023-05-18 00:30:21.000000 coba-7.0.0/coba/pipes/readers.py
--rw-rw-rw-   0        0        0    19485 2023-07-05 00:06:18.000000 coba-7.0.0/coba/pipes/rows.py
--rw-rw-rw-   0        0        0     4474 2023-07-02 17:30:52.000000 coba-7.0.0/coba/pipes/sinks.py
--rw-rw-rw-   0        0        0     6510 2023-06-04 18:59:11.000000 coba-7.0.0/coba/pipes/sources.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/primitives/
--rw-rw-rw-   0        0        0      477 2023-06-19 00:01:57.000000 coba-7.0.0/coba/primitives/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-16 03:47:25.000000 coba-7.0.0/coba/primitives/feedbacks.py
--rw-rw-rw-   0        0        0     4494 2023-06-16 05:48:36.000000 coba-7.0.0/coba/primitives/rewards.py
--rw-rw-rw-   0        0        0     4421 2023-07-05 00:02:17.000000 coba-7.0.0/coba/primitives/rows.py
--rw-rw-rw-   0        0        0      219 2023-06-16 03:47:51.000000 coba-7.0.0/coba/primitives/semantic.py
--rw-rw-rw-   0        0        0      657 2023-05-16 05:30:40.000000 coba-7.0.0/coba/primitives/types.py
--rw-rw-rw-   0        0        0    11151 2023-07-17 04:57:59.000000 coba-7.0.0/coba/random.py
--rw-rw-rw-   0        0        0     1479 2023-07-03 01:30:21.000000 coba-7.0.0/coba/register.py
--rw-rw-rw-   0        0        0    10657 2023-05-11 00:41:22.000000 coba-7.0.0/coba/registry.py
--rw-rw-rw-   0        0        0     9049 2023-07-13 05:09:41.000000 coba-7.0.0/coba/statistics.py
--rw-rw-rw-   0        0        0     5212 2023-06-05 02:30:05.000000 coba-7.0.0/coba/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba.egg-info/
--rw-rw-rw-   0        0        0     7942 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1283 2023-06-18 23:54:01.000000 coba-7.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 05:11:17.000000 coba-7.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.981982 coba-7.0.1/
+-rw-rw-rw-   0        0        0       40 2023-06-12 16:34:36.000000 coba-7.0.1/AUTHORS
+-rw-rw-rw-   0        0        0     1593 2023-06-12 16:34:36.000000 coba-7.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7942 2023-07-20 08:51:42.981982 coba-7.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7327 2023-06-16 20:10:41.000000 coba-7.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.825193 coba-7.0.1/coba/
+-rw-rw-rw-   0        0        0     1378 2023-07-20 08:47:42.000000 coba-7.0.1/coba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.856504 coba-7.0.1/coba/backports/
+-rw-rw-rw-   0        0        0       50 2023-07-20 03:01:25.000000 coba-7.0.1/coba/backports/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-07-20 02:54:01.000000 coba-7.0.1/coba/backports/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.872079 coba-7.0.1/coba/contexts/
+-rw-rw-rw-   0        0        0      703 2023-06-22 17:38:27.000000 coba-7.0.1/coba/contexts/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-06-12 16:34:36.000000 coba-7.0.1/coba/contexts/cachers.py
+-rw-rw-rw-   0        0        0     9236 2023-07-20 02:56:24.000000 coba-7.0.1/coba/contexts/core.py
+-rw-rw-rw-   0        0        0     9726 2023-06-12 16:34:36.000000 coba-7.0.1/coba/contexts/loggers.py
+-rw-rw-rw-   0        0        0    15875 2023-07-20 03:19:10.000000 coba-7.0.1/coba/encodings.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.903838 coba-7.0.1/coba/environments/
+-rw-rw-rw-   0        0        0     1448 2023-07-16 19:49:49.000000 coba-7.0.1/coba/environments/__init__.py
+-rw-rw-rw-   0        0        0    22841 2023-07-20 03:16:24.000000 coba-7.0.1/coba/environments/core.py
+-rw-rw-rw-   0        0        0    52590 2023-07-20 07:40:57.000000 coba-7.0.1/coba/environments/filters.py
+-rw-rw-rw-   0        0        0    14347 2023-07-16 19:49:49.000000 coba-7.0.1/coba/environments/openml.py
+-rw-rw-rw-   0        0        0     7646 2023-07-16 19:49:49.000000 coba-7.0.1/coba/environments/primitives.py
+-rw-rw-rw-   0        0        0     2966 2023-07-16 19:49:49.000000 coba-7.0.1/coba/environments/serialized.py
+-rw-rw-rw-   0        0        0     9524 2023-07-20 02:57:00.000000 coba-7.0.1/coba/environments/supervised.py
+-rw-rw-rw-   0        0        0    24174 2023-07-20 02:57:08.000000 coba-7.0.1/coba/environments/synthetics.py
+-rw-rw-rw-   0        0        0     6179 2023-06-12 16:34:36.000000 coba-7.0.1/coba/environments/templates.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.919584 coba-7.0.1/coba/evaluators/
+-rw-rw-rw-   0        0        0      217 2023-06-24 23:45:33.000000 coba-7.0.1/coba/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    15064 2023-07-20 07:42:27.000000 coba-7.0.1/coba/evaluators/offline.py
+-rw-rw-rw-   0        0        0    22265 2023-07-20 08:43:00.000000 coba-7.0.1/coba/evaluators/online.py
+-rw-rw-rw-   0        0        0     2095 2023-07-16 19:49:49.000000 coba-7.0.1/coba/evaluators/primitives.py
+-rw-rw-rw-   0        0        0     1126 2023-06-12 16:34:36.000000 coba-7.0.1/coba/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.935170 coba-7.0.1/coba/experiments/
+-rw-rw-rw-   0        0        0      379 2023-06-22 17:38:27.000000 coba-7.0.1/coba/experiments/__init__.py
+-rw-rw-rw-   0        0        0    10512 2023-07-16 19:49:49.000000 coba-7.0.1/coba/experiments/core.py
+-rw-rw-rw-   0        0        0     7686 2023-07-16 19:49:49.000000 coba-7.0.1/coba/experiments/process.py
+-rw-rw-rw-   0        0        0    65241 2023-07-20 02:57:27.000000 coba-7.0.1/coba/experiments/results.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.966364 coba-7.0.1/coba/learners/
+-rw-rw-rw-   0        0        0      761 2023-07-16 19:49:49.000000 coba-7.0.1/coba/learners/__init__.py
+-rw-rw-rw-   0        0        0     7907 2023-06-24 23:48:29.000000 coba-7.0.1/coba/learners/bandit.py
+-rw-rw-rw-   0        0        0     8028 2023-07-20 02:57:43.000000 coba-7.0.1/coba/learners/corral.py
+-rw-rw-rw-   0        0        0     4947 2023-06-23 09:01:59.000000 coba-7.0.1/coba/learners/linucb.py
+-rw-rw-rw-   0        0        0      958 2023-07-16 19:49:49.000000 coba-7.0.1/coba/learners/misguided.py
+-rw-rw-rw-   0        0        0     4376 2023-06-12 16:34:36.000000 coba-7.0.1/coba/learners/primitives.py
+-rw-rw-rw-   0        0        0     8887 2023-07-20 08:32:14.000000 coba-7.0.1/coba/learners/safety.py
+-rw-rw-rw-   0        0        0    30984 2023-07-20 02:58:04.000000 coba-7.0.1/coba/learners/vowpal.py
+-rw-rw-rw-   0        0        0     4139 2023-07-16 19:49:49.000000 coba-7.0.1/coba/multiprocessing.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.981982 coba-7.0.1/coba/pipes/
+-rw-rw-rw-   0        0        0     1456 2023-07-16 19:49:49.000000 coba-7.0.1/coba/pipes/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-06-12 16:34:36.000000 coba-7.0.1/coba/pipes/core.py
+-rw-rw-rw-   0        0        0    16751 2023-07-16 19:49:49.000000 coba-7.0.1/coba/pipes/filters.py
+-rw-rw-rw-   0        0        0    16062 2023-07-20 05:27:58.000000 coba-7.0.1/coba/pipes/multiprocessing.py
+-rw-rw-rw-   0        0        0     6622 2023-06-12 16:34:36.000000 coba-7.0.1/coba/pipes/primitives.py
+-rw-rw-rw-   0        0        0    13003 2023-06-12 16:34:36.000000 coba-7.0.1/coba/pipes/readers.py
+-rw-rw-rw-   0        0        0    19458 2023-07-20 02:58:18.000000 coba-7.0.1/coba/pipes/rows.py
+-rw-rw-rw-   0        0        0     4474 2023-07-16 19:49:49.000000 coba-7.0.1/coba/pipes/sinks.py
+-rw-rw-rw-   0        0        0     6483 2023-07-20 02:58:25.000000 coba-7.0.1/coba/pipes/sources.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.981982 coba-7.0.1/coba/primitives/
+-rw-rw-rw-   0        0        0      477 2023-06-22 17:38:27.000000 coba-7.0.1/coba/primitives/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-16 20:10:41.000000 coba-7.0.1/coba/primitives/feedbacks.py
+-rw-rw-rw-   0        0        0     4624 2023-07-20 08:45:03.000000 coba-7.0.1/coba/primitives/rewards.py
+-rw-rw-rw-   0        0        0     4421 2023-07-16 19:49:49.000000 coba-7.0.1/coba/primitives/rows.py
+-rw-rw-rw-   0        0        0      219 2023-07-19 06:20:25.000000 coba-7.0.1/coba/primitives/semantic.py
+-rw-rw-rw-   0        0        0      657 2023-06-12 16:34:36.000000 coba-7.0.1/coba/primitives/types.py
+-rw-rw-rw-   0        0        0    11151 2023-07-16 18:38:46.000000 coba-7.0.1/coba/random.py
+-rw-rw-rw-   0        0        0     1479 2023-07-16 19:49:49.000000 coba-7.0.1/coba/register.py
+-rw-rw-rw-   0        0        0    10657 2023-06-12 16:34:36.000000 coba-7.0.1/coba/registry.py
+-rw-rw-rw-   0        0        0     9022 2023-07-20 02:56:10.000000 coba-7.0.1/coba/statistics.py
+-rw-rw-rw-   0        0        0     5212 2023-06-12 16:34:36.000000 coba-7.0.1/coba/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:51:42.840824 coba-7.0.1/coba.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1583 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-20 08:51:42.000000 coba-7.0.1/coba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1194 2023-07-20 03:21:22.000000 coba-7.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:51:42.981982 coba-7.0.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `coba-7.0.0/LICENSE` & `coba-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/PKG-INFO` & `coba-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.0
+Version: 7.0.1
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 License-File: AUTHORS
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![badge](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,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)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=examples/notebooks)
```

### Comparing `coba-7.0.0/README.md` & `coba-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/__init__.py` & `coba-7.0.1/coba/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 from coba.utilities import peek_first
 from coba.exceptions import CobaException
 
 from coba.primitives.semantic import Batch
 from coba.primitives.rewards import L1Reward, HammingReward, BinaryReward, IPSReward
 from coba.primitives.rewards import SequenceReward, MappingReward, MulticlassReward, BatchReward
 
-__version__ = "7.0.0"
+__version__ = "7.0.1"
```

### Comparing `coba-7.0.0/coba/contexts/__init__.py` & `coba-7.0.1/coba/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/contexts/cachers.py` & `coba-7.0.1/coba/contexts/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/contexts/core.py` & `coba-7.0.1/coba/contexts/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 import json
 import collections
 import traceback
 
 from pathlib import Path
-from typing import Iterable, Dict, Any, Sequence, Union
-from coba.backports import Literal
+from typing import Iterable, Dict, Any, Sequence, Union, Literal
 
 from coba.exceptions import CobaException
 from coba.registry import JsonMakerV1, CobaRegistry
 from coba.utilities import coba_exit
 
 from coba.contexts.cachers import Cacher
 from coba.contexts.loggers import Logger
```

### Comparing `coba-7.0.0/coba/contexts/loggers.py` & `coba-7.0.1/coba/contexts/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/encodings.py` & `coba-7.0.1/coba/encodings.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,14 +302,22 @@
         try:
             return list(map(self._levels.__getitem__,values))
         except KeyError as e:
             raise CobaException(f"We were unable to find {e} in {self._levels.keys()}") from None
 
 class CobaJsonEncoder(json.JSONEncoder):
     """A json encoder that allows for potential COBA extensions in the future."""
+    def default(self, o: Any) -> Any:
+        try:
+            return o.to_json()
+        except AttributeError:
+            try:
+                return vars(o)
+            except TypeError:
+                return super().default(o)
 
 class CobaJsonDecoder(json.JSONDecoder):
     """A json decoder that allows for potential COBA extensions in the future."""
 
 class InteractionsEncoder:
 
     def __init__(self, interactions: Sequence[Union[str,float]]) -> None:
```

### Comparing `coba-7.0.0/coba/environments/__init__.py` & `coba-7.0.1/coba/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/environments/core.py` & `coba-7.0.1/coba/environments/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import collections.abc
 
 from zipfile import ZipFile, BadZipFile
 from pathlib import Path
-from typing import Sequence, overload, Union, Iterable, Iterator, Any, Optional, Tuple, Callable, Mapping, Type
-from coba.backports import Literal
+from typing import Sequence, overload, Union, Iterable, Iterator, Any, Optional, Tuple, Callable, Mapping, Type, Literal
 
 from coba                 import pipes
 from coba.contexts        import CobaContext, DiskCacher, DecoratedLogger, ExceptLog, NameLog, StampLog
 from coba.pipes.sources   import DataFrameSource
 from coba.primitives      import Context, Action
 from coba.random          import CobaRandom
 from coba.pipes           import Pipes, Source, HttpSource, IterableSource, JsonDecode
@@ -289,17 +288,18 @@
         ...
 
     def shuffle(self, *args,**kwargs) -> 'Environments':
         """Shuffle the order of the interactions in the Environments."""
 
         flat = lambda a: next(pipes.Flatten().filter([a]))
 
-        if kwargs:
+        if kwargs and 'n' in kwargs:
             seeds = range(kwargs['n'])
         else:
+            args = kwargs.get('seed',kwargs.get('seeds',args))        
             seeds = flat(args) or [1]
 
         if isinstance(seeds,int): seeds = [seeds]
 
         shuffled = self.filter([Shuffle(seed) for seed in seeds])
 
         #Experience has shown that most of the time we want to sort.
```

### Comparing `coba-7.0.0/coba/environments/filters.py` & `coba-7.0.1/coba/environments/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from statistics import median, stdev, mode
 from numbers import Number
 from zlib import crc32
 from operator import eq, getitem, methodcaller, itemgetter
 from collections import defaultdict
 from functools import lru_cache
 from itertools import islice, chain, tee, compress, repeat
-from typing import Optional, Sequence, Union, Iterable, Any, Tuple, Callable, Mapping
-from coba.backports import Literal
+from typing import Optional, Sequence, Union, Iterable, Any, Tuple, Callable, Mapping, Literal
 
 from coba            import pipes, primitives
 from coba.random     import CobaRandom
 from coba.exceptions import CobaException
 from coba.statistics import iqr
 from coba.utilities  import peek_first, PackageChecker
 from coba.primitives import BinaryReward, SequenceReward, BatchReward, argmax
@@ -1040,16 +1039,17 @@
         for batch in self._batched(interactions, self._batch_size):
             new = { k: primitives.Batch(i[k] for i in batch) for k in batch[0] }
             if 'rewards' in new: new['rewards'] = BatchReward(new['rewards'])
             if 'feedbacks' in new: new['feedbacks'] = BatchFeedback(new['feedbacks'])
             yield new
 
     def _batched(self, iterable, n):
-        "Batch data into lists of length n. The last batch may be shorter."
-        #taken from python itertools recipes
+        #Batch data into lists of length n.
+        #The last batch may be shorter.
+        #Taken from python itertools recipes.
         it = iter(iterable)
         batch = list(islice(it, n))
         while (batch):
             yield batch
             batch = list(islice(it, n))
 
 class Unbatch(EnvironmentFilter):
```

### Comparing `coba-7.0.0/coba/environments/openml.py` & `coba-7.0.1/coba/environments/openml.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/environments/primitives.py` & `coba-7.0.1/coba/environments/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/environments/serialized.py` & `coba-7.0.1/coba/environments/serialized.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/environments/supervised.py` & `coba-7.0.1/coba/environments/supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from itertools import chain
-from typing import Any, Iterable, Union, Sequence, overload, Dict, MutableSequence, MutableMapping
-from coba.backports import Literal
+from typing import Any, Iterable, Union, Sequence, overload, Dict, MutableSequence, MutableMapping, Literal
 
 from coba.pipes import Pipes, Source, IterableSource, LabelRows, Reservoir, UrlSource, CsvReader
 from coba.pipes import CsvReader, ArffReader, LibsvmReader, ManikReader
 
 from coba.utilities import peek_first
 from coba.primitives import Categorical, L1Reward, MulticlassReward, HammingReward
```

### Comparing `coba-7.0.0/coba/environments/synthetics.py` & `coba-7.0.1/coba/environments/synthetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 
 from statistics import mean
 from itertools import count, islice, cycle
-from typing import Sequence, Dict, Tuple, Any, Callable, Optional, overload, Iterable
-from coba.backports import Literal
+from typing import Sequence, Dict, Tuple, Any, Callable, Optional, overload, Iterable, Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.encodings import InteractionsEncoder, OneHotEncoder
 
 from coba.environments.primitives import Context, Action, Environment, SimulatedInteraction, SequenceReward
```

### Comparing `coba-7.0.0/coba/environments/templates.py` & `coba-7.0.1/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/evaluators/offline.py` & `coba-7.0.1/coba/evaluators/offline.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/evaluators/online.py` & `coba-7.0.1/coba/evaluators/online.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import warnings
 
 from operator import __mul__
 from statistics import mean
 from bisect import insort
-from typing import Any, Iterable, Sequence, Mapping, Optional
-from coba.backports import Literal
+from typing import Any, Iterable, Sequence, Mapping, Optional, Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.contexts import CobaContext
 from coba.environments import Environment
 from coba.learners import Learner, SafeLearner
 from coba.primitives import Batch, argmax
@@ -43,20 +42,20 @@
         interactions = environment.read()
         learner = SafeLearner(learner, self._seed if self._seed is not None else CobaContext.store.get("experiment_seed"))
 
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
 
-        batched  = first and isinstance(first['context'], Batch)
-
         for key in ['rewards','context','actions']:
             if key not in first:
                 raise CobaException(f"OnPolicyEvaluator requires every interaction to have '{key}'")
 
+        batched  = first and (isinstance(first['context'],Batch) or isinstance(first['actions'],Batch))
+
         for key in ['rewards','actions']:
             if (first[key][0] if batched else first[key]) is None:
                 raise CobaException(f"OnPolicyEvaluator requires every interaction to have a not None '{key}'")
 
         discrete = len(first['actions'][0] if batched else first['actions']) > 0
         if not discrete:
             for metric in set(self._record).intersection(OnPolicyEvaluator.ONLY_DISCRETE):
@@ -91,15 +90,15 @@
             interaction = interaction.copy()
 
             context   = interaction.pop('context')
             actions   = interaction.pop('actions')
             rewards   = interaction.pop('rewards')
             feedbacks = interaction.pop('feedbacks',None)
 
-            batched  = isinstance(context, Batch)
+            batched  = isinstance(context,Batch) or isinstance(actions,Batch)
             discrete = len(actions[0] if batched else actions) > 0
 
             if record_context: out['context'] = context
             if record_actions: out['actions'] = actions
             if record_rewards: out['rewards'] = list(map(get_reward_list,rewards,actions)) if batched else get_reward_list(rewards,actions)
 
             start_time         = time.time()
@@ -144,15 +143,15 @@
         record: Sequence[Literal['reward','time','ope_loss','probability','action','context','actions','rewards']] = ['reward'],
         learn: bool = True,
         predict: bool = True,
         seed: float = None) -> None:
         """
         Args:
             record: The datapoints to record for each interaction.
-            learn: Indicates that off-policy learning should occur as parrt of the off-policy task.
+            learn: Indicates that off-policy learning should occur as part of the off-policy task.
             evals: Indicates that off-policy evaluation should occur as part of the off-policy task.
             seed: Provide an explicit seed to use during evaluation. If not provided a default is used.
         """
 
         self._record  = [record] if isinstance(record,str) else record
         self._learn   = learn
         self._predict = predict
@@ -286,15 +285,15 @@
                     yield from ({k:v[i] for k,v in out.items()} for i in range(len(log_context)))
                 else:
                     yield out
 
 class ExplorationEvaluator(Evaluator):
 
     def __init__(self,
-        record: Sequence[Literal['context','actions','action','reward','probability','time']] = ['reward'],
+        record: Sequence[Literal['context','actions','action','reward','probability','time','rewards']] = ['reward'],
         ope: bool = None,
         qpct: float = .005,
         cmax: float = 1.0,
         cinit: float = None,
         seed: float = None) -> None:
         """
         Args:
@@ -363,14 +362,15 @@
         record_time     = 'time'        in self._record
         record_reward   = 'reward'      in self._record
         record_action   = 'action'      in self._record
         record_actions  = 'actions'     in self._record
         record_context  = 'context'     in self._record
         record_prob     = 'probability' in self._record
         record_ope_loss = 'ope_loss'    in self._record
+        record_rewards  = 'rewards'     in self._record
 
         request = learner.request
         learn   = learner.learn
         info    = CobaContext.learning_info
 
         info.clear()
 
@@ -391,18 +391,14 @@
             log_actions      = interaction.pop('actions')
             log_action       = interaction.pop('action')
             log_reward       = interaction.pop('reward')
             log_prob         = interaction.pop('probability')
             log_rewards      = interaction.pop('rewards',None)
             log_action_index = log_actions.index(log_action)
 
-            if record_time:
-                predict_time = 0
-                learn_time   = 0
-
             start_time = time.time()
             on_probs = request(log_context,log_actions,log_actions)
             on_prob = on_probs[log_action_index]
             predict_time = time.time()-start_time
 
             if self._ope and log_rewards: ope_rewards.append(sum(map(__mul__, on_probs, map(log_rewards.eval,log_actions))))
 
@@ -436,14 +432,16 @@
                 if record_time    : out['learn_time']   = learn_time
                 if record_context : out['context']      = log_context
                 if record_actions : out['actions']      = log_actions
                 if record_action  : out['action']       = log_action
                 if record_reward  : out['reward']       = mean(ope_rewards)
                 if record_prob    : out['probability']  = on_prob
                 if record_ope_loss: out['ope_loss']     = get_ope_loss(learner)
+                if record_rewards : out['rewards']      = ope_rewards
+
 
                 if info: out.update(info)
                 if out : yield out
 
                 ope_rewards.clear()
                 c = min(percentile(Q,self._qpct,sort=False), self._cmax)
```

### Comparing `coba-7.0.0/coba/evaluators/primitives.py` & `coba-7.0.1/coba/evaluators/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/exceptions.py` & `coba-7.0.1/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/experiments/core.py` & `coba-7.0.1/coba/experiments/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/experiments/process.py` & `coba-7.0.1/coba/experiments/process.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/experiments/results.py` & `coba-7.0.1/coba/experiments/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from pathlib import Path
 from numbers import Number
 from operator import truediv, sub, itemgetter
 from functools import cmp_to_key
 from abc import abstractmethod
 from dataclasses import dataclass, astuple, field, replace
 from itertools import chain, repeat, accumulate, groupby, count, compress, groupby
-from typing import Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, List, Any, overload
-from coba.backports import Literal
+from typing import Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, List, Any, overload, Literal
 
 from coba.primitives import Batch
 from coba.environments import Environment
 from coba.statistics import mean, StdDevCI, StdErrCI, BootstrapCI, BinomialCI, PointAndInterval
 from coba.contexts import CobaContext
 from coba.exceptions import CobaException
 from coba.utilities import PackageChecker, peek_first
```

### Comparing `coba-7.0.0/coba/learners/__init__.py` & `coba-7.0.1/coba/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/learners/bandit.py` & `coba-7.0.1/coba/learners/bandit.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/learners/corral.py` & `coba-7.0.1/coba/learners/corral.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 
-from typing import Any, Sequence, Optional, Mapping, Tuple
-from coba.backports import Literal
+from typing import Any, Sequence, Optional, Mapping, Tuple, Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.primitives import Context, Action
 
 from coba.learners.safety import SafeLearner
 from coba.learners.primitives import Learner, PMF, kwargs, Actions, Prob
```

### Comparing `coba-7.0.0/coba/learners/linucb.py` & `coba-7.0.1/coba/learners/linucb.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/learners/misguided.py` & `coba-7.0.1/coba/learners/misguided.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/learners/primitives.py` & `coba-7.0.1/coba/learners/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/learners/safety.py` & `coba-7.0.1/coba/learners/safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from collections import abc
 from math import isclose
-from itertools import repeat
-from typing import Any, Sequence, Tuple, Mapping
-from coba.backports import Literal
+from typing import Any, Sequence, Tuple, Mapping, Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.primitives import Batch, Context, Action, Actions
 from coba.learners.primitives import Learner, PMF, ActionProb, Actions, Prob, kwargs, Prediction
 
 def pred_format(pred:Prediction, batch_order:Literal['not','row','col'], has_kwarg:bool, actions:Actions):
@@ -64,15 +62,15 @@
         " action index (i.e., actions.index(action)). Alternatively, this can"
         " also happen for two action problems. In this case we suggest using"
         " coba.learners.PMF or coba.learners.ActionProb to provide explicit"
         " type information (e.g., return coba.learners.PMF([1,0])).")
 
 def batch_order(predictor, pred: Prediction, context, actions) -> Literal['not','col','row']:
 
-    if not isinstance(actions,Batch) or not isinstance(context,Batch): return 'not'
+    if not isinstance(actions,Batch) and not isinstance(context,Batch): return 'not'
 
     n_rows = len(actions)
     n_dim1 = len(pred)
     n_dim2 = len(pred[0])
 
     if n_dim1 == n_dim2:
         #The major order of pred is not determinable. So we
@@ -153,15 +151,15 @@
         try:
             self._method[key] = 1
             return self._safe_call(key, method, args, kwargs)
         except:
             try:
                 self._method[key] = 2
                 return self._safe_call(key, method, args, kwargs)
-            except:
+            except Exception as ex:
                 del self._method[key]
             raise
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
 
         try:
             return self._safe_call('request', self.learner.request, (context,actions,request))
```

### Comparing `coba-7.0.0/coba/learners/vowpal.py` & `coba-7.0.1/coba/learners/vowpal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from itertools import repeat, compress
 from sys import platform
-from typing import Any, Dict, Union, Sequence, Mapping, Optional, Tuple
+from typing import Any, Dict, Union, Sequence, Mapping, Optional, Tuple, Literal
 
-from coba.backports import Literal
 from coba.exceptions import CobaException
 from coba.learners.primitives import Learner, PMF, Prob
 from coba.primitives import Sparse, Context, Action, Actions, Batch
 from coba.utilities import PackageChecker
 
 Feature       = Union[str,int,float]
 Features      = Union[Feature, Sequence[Feature], Dict[str,Union[int,float]]]
```

### Comparing `coba-7.0.0/coba/multiprocessing.py` & `coba-7.0.1/coba/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/__init__.py` & `coba-7.0.1/coba/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/core.py` & `coba-7.0.1/coba/pipes/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/filters.py` & `coba-7.0.1/coba/pipes/filters.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/multiprocessing.py` & `coba-7.0.1/coba/pipes/multiprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pickle
+import importlib.util
 import threading as mt
 import multiprocessing as mp
 
 from collections.abc import Iterator
 from queue import Empty
 from traceback import format_tb
-from typing import Iterable, Mapping, Callable, Optional, Union, Sequence, Any
-from coba.backports import Literal
+from typing import Iterable, Mapping, Callable, Optional, Union, Sequence, Any, Literal
 
 from coba.utilities import peek_first
 from coba.exceptions import CobaException
 from coba.pipes.primitives import Filter, Line, SourceSink
 from coba.pipes.filters import Slice
 from coba.pipes.sources import IterableSource, QueueSource
 from coba.pipes.sinks import QueueSink
@@ -51,14 +51,15 @@
         super().__init__(daemon=True)
 
     def start(self) -> None:
         callback               = self._callback
         self._callback         = None
         self._recv, self._send = spawn_context.Pipe(False)
         self._lock             = spawn_context.Lock()
+
         super().start()
 
         if callback:
             def join_and_call(self=self):
                 self.join()
                 callback(self)
             mt.Thread(target=join_and_call,daemon=True).start()
@@ -68,18 +69,19 @@
             self._line.run()
         except Exception as e:
             if str(e).startswith("Can't get attribute"):
                 ex,tb = CobaException(
                     "We attempted to evaluate your code in multiple processes but we were unable to find all the code "
                     "definitions needed to pass the tasks to the processes. The two most common causes of this error are: "
                     "1) a learner or simulation is defined in a Jupyter Notebook cell or 2) a necessary class definition "
-                    "exists inside the `__name__=='__main__'` code block in the main execution script. In either case "
-                    "you can choose one of three simple solutions: 1) evaluate your code on a single process with no limit on "
-                    "child tasks, 2) if in Jupyter notebook define all necessary classes in a separate file and include the "
-                    "classes via import statements, or 3) move your class definitions outside the `__name__=='__main__'` check."
+                    "exists inside the `__name__=='__main__'` code block in the main execution script. In either case you "
+                    "can choose one of four simple solutions: 1) pip install cloudpickle into your python environment, 2) "
+                    "evaluate your code on a single process, 3) if in Jupyter notebook define all necessary classes in a "
+                    "separate file and include the classes via import statements, or 4) move your class definitions outside "
+                    "the `__name__ == '__main__'` check."
                 ),None
             else:
                 ex,tb = e,format_tb(e.__traceback__)
         except KeyboardInterrupt as e:
             ex,tb = e,None
         else:
             ex,tb = None,None
@@ -178,46 +180,74 @@
             worker = ThreadLine(line=self, callback=callback)
         else:
             raise CobaException(f"Unrecognized pipe async mode {mode}. Valid values are 'process' and 'thread'.")
 
         worker.start()
         return worker
 
+class Safe:
+    def __init__(self, filter: Filter):
+        if importlib.util.find_spec('cloudpickle'):
+            import cloudpickle
+            try:
+                self._filter = cloudpickle.dumps(filter)
+            except:
+                self._filter = filter
+        else:
+            self._filter = filter
+
+    def filter(self,items):
+        if importlib.util.find_spec('cloudpickle') and isinstance(self._filter,bytes):
+            import cloudpickle
+            filter = cloudpickle.loads(self._filter)
+        else:
+            filter = self._filter
+
+        yield from filter.filter(items)
+
 class Foreach:
     def __init__(self,pipe:Filter) -> None:
         self._pipe = pipe
 
     def filter(self, items: Iterable[Any]) -> Iterable[Any]:
         for item in items:
             out = self._pipe.filter(item)
             out = out if isinstance(out,Iterator) else [out]
             yield from out
 
 class Pickler:
-
     def filter(self, items) -> Iterable[bytes]:
         try:
-            yield from map(pickle.dumps,items)
+            if importlib.util.find_spec('cloudpickle'):
+                import cloudpickle
+                yield from map(cloudpickle.dumps,items)
+            else:
+                yield from map(pickle.dumps,items)
         except Exception as e:
             if "pickle" in str(e) or "Pickling" in str(e):
                 message = (
                     f"We attempted to process your code on multiple processes but were unable to do so due to a pickle "
-                    f"error. The exact error received was '{str(e)}'. Errors this kind can often be fixed in one of two "
-                    f"ways: 1) evaluate the experiment in question on a single process with no limit on the tasks per child "
-                    f"or 2) modify the named class to be picklable. The easiest way to make a given class picklable is to "
-                    f"add `def __reduce__(self): return (<the class in question>, (<tuple of constructor arguments>))` to "
-                    f"the class. For more information see https://docs.python.org/3/library/pickle.html#object.__reduce__."
+                    f"error. The exact error received was '{str(e)}'. Errors of this kind can often be fixed in one of three "
+                    f"ways: 1) pip install cloudpickle in your conda environment, 2) evaluate the experiment in question on "
+                    f"a single process with no limit on the tasks per child or 3) modify the named class to be picklable. "
+                    f"The easiest way to make a given class picklable is to add `def __reduce__(self): return (<the class "
+                    f"in question>, (<tuple of constructor arguments>))` to the class. For more information see "
+                    f"https://docs.python.org/3/library/pickle.html#object.__reduce__."
                 )
                 raise CobaException(message)
             else: #pragma: no cover
                 raise
 
 class Unpickler:
     def filter(self, items):
-        yield from map(pickle.loads,items)
+        if importlib.util.find_spec('cloudpickle'):
+            import cloudpickle
+            yield from map(cloudpickle.loads,items)
+        else:
+            yield from map(pickle.loads,items)
 
 class EventSetter:
     def __init__(self, event: mt.Event) -> None:
         self._event = event
     def filter(self, items):
         self._event.set()
         return items
@@ -283,15 +313,15 @@
             self._n_procs      = self._max_processes
             self._exceptions   = []
             self._poison       = None
             self._main_err     = False
             self._load_stopper = Stopper() #this works because the loader is a thread which means we have shared memory
 
             load_line   = SourceSink(IterableSource(items), self._load_stopper, pickler, in_put)
-            filter_line = SourceSink(in_get, setter, unpickler, get_max, Foreach(self._filter), out_put)
+            filter_line = SourceSink(in_get, setter, unpickler, get_max, Safe(Foreach(self._filter)), out_put)
 
             def loader_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
                 if worker.exception: self._exceptions.append(worker.exception)
                 in_put.write(self._load_stopper.filter([self._poison]*self._n_procs))
 
             def filter_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
                 if worker.exception: self._exceptions.append(worker.exception)
```

### Comparing `coba-7.0.0/coba/pipes/primitives.py` & `coba-7.0.1/coba/pipes/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/readers.py` & `coba-7.0.1/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/rows.py` & `coba-7.0.1/coba/pipes/rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import abc
 from itertools import count, compress, chain, filterfalse, islice, repeat
-from typing import Dict, Any, Union, Callable, Iterator, Sequence, Mapping, Iterable, Tuple
-from coba.backports import Literal
+from typing import Dict, Any, Union, Callable, Iterator, Sequence, Mapping, Iterable, Tuple, Literal
 
 from coba.primitives import Sparse, Dense, Categorical
 from coba.primitives.rows import Dense_, Sparse_
 from coba.utilities import peek_first
 from coba.pipes.primitives import Filter
 from coba.pipes.filters import Flatten
```

### Comparing `coba-7.0.0/coba/pipes/sinks.py` & `coba-7.0.1/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/pipes/sources.py` & `coba-7.0.1/coba/pipes/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
 import gzip
 
 from queue import Queue
-from typing import Any, Callable, Iterable, Union, Mapping, Sequence
-from coba.backports import Literal
+from typing import Any, Callable, Iterable, Union, Mapping, Sequence, Literal
 
 from coba.exceptions import CobaException
 from coba.pipes.primitives import Source
 
 class NullSource(Source[Any]):
     """A source which always returns an empty list."""
```

### Comparing `coba-7.0.0/coba/primitives/feedbacks.py` & `coba-7.0.1/coba/primitives/feedbacks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/primitives/rewards.py` & `coba-7.0.1/coba/primitives/rewards.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Sequence, Optional, Mapping, overload
+from typing import Sequence, Optional, Mapping
 
 from coba.exceptions import CobaException
 from coba.primitives.semantic import Action, Batch
 
 def argmax(actions: Sequence[Action], rewards: 'Reward') -> Action:
     max_r = -float('inf')
     max_a = 0
@@ -18,18 +18,21 @@
 class Reward(ABC):
     __slots__ = ()
 
     @abstractmethod
     def eval(self, action: Action) -> float:
         ...
 
+    def to_json(self) -> Mapping[str, str]:
+        return {key.lstrip('_'): getattr(self, key, None) for key in self.__slots__}
+
 class IPSReward(Reward):
     __slots__ = ('_reward','_action')
 
-    def __init__(self, reward: float, action: Action, probability: Optional[float]) -> None:
+    def __init__(self, reward: float, action: Action, probability: Optional[float] = None) -> None:
         self._reward = reward/(probability or 1)
         self._action = action
 
     def eval(self, arg: Action) -> float:
         return self._reward if arg == self._action else 0
 
     def __reduce__(self):
```

### Comparing `coba-7.0.0/coba/primitives/rows.py` & `coba-7.0.1/coba/primitives/rows.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/primitives/types.py` & `coba-7.0.1/coba/primitives/types.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/random.py` & `coba-7.0.1/coba/random.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/register.py` & `coba-7.0.1/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/registry.py` & `coba-7.0.1/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba/statistics.py` & `coba-7.0.1/coba/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from math import hypot, isnan, erf, sqrt, fsum
 from sys import version_info
 from operator import mul, sub
 from bisect import bisect_left
 from itertools import repeat, accumulate, compress, chain
 from abc import abstractmethod, ABC
-from typing import Sequence, Tuple, Union, Callable, Optional
-from coba.backports import Literal
+from typing import Sequence, Tuple, Union, Callable, Optional, Literal
 
 from coba.exceptions import CobaException
 from coba.utilities import PackageChecker
 
 def iqr(values: Sequence[float]) -> float:
 
     if len(values) <= 1: return 0.
```

### Comparing `coba-7.0.0/coba/utilities.py` & `coba-7.0.1/coba/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.0/coba.egg-info/PKG-INFO` & `coba-7.0.1/coba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.0
+Version: 7.0.1
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 License-File: AUTHORS
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![badge](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,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)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=examples/notebooks)
```

### Comparing `coba-7.0.0/coba.egg-info/SOURCES.txt` & `coba-7.0.1/coba.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 coba.egg-info/SOURCES.txt
 coba.egg-info/dependency_links.txt
 coba.egg-info/entry_points.txt
 coba.egg-info/requires.txt
 coba.egg-info/top_level.txt
 coba/backports/__init__.py
 coba/backports/metadata.py
-coba/backports/typing.py
 coba/contexts/__init__.py
 coba/contexts/cachers.py
 coba/contexts/core.py
 coba/contexts/loggers.py
 coba/environments/__init__.py
 coba/environments/core.py
 coba/environments/filters.py
```

### Comparing `coba-7.0.0/pyproject.toml` & `coba-7.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,25 @@
 name = "coba"
 dynamic = ["version"]
 authors = [
     {name = "Mark Rucker", email = "rucker.mark@gmail.com"},
 ]
 description = "A contextual bandit research package"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3.7",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering"
 ]
 dependencies = [
     'requests>=2',
-    'importlib-metadata>=1.0;python_version<"3.8"',
-    'typing-extensions>=4.1,<4.2;python_version<"3.8"'
 ]
 
 [project.urls]
 Homepage = "https://github.com/vowpalwabbit/coba"
 
 [project.entry-points."coba.register"]
 coba = "coba.register"
@@ -40,9 +38,10 @@
 [project.optional-dependencies]
 full = [
     "vowpalwabbit",
     "scikit-learn",
     "pandas",
     "matplotlib",
     "numpy",
-    "scipy"
+    "scipy",
+    "cloudpickle"
 ]
```

