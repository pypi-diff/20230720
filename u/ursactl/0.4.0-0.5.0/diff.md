# Comparing `tmp/ursactl-0.4.0.tar.gz` & `tmp/ursactl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-pmq_iku0/ursactl-0.4.0.tar", last modified: Tue Jul 18 20:54:55 2023, max compression
+gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-nzs4hdo3/ursactl-0.5.0.tar", last modified: Thu Jul 20 12:43:14 2023, max compression
```

## Comparing `ursactl-0.4.0.tar` & `ursactl-0.5.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.4.0/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.4.0/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.4.0/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-18 20:54:55.000000 ursactl-0.4.0/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.4.0/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.4.0/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.4.0/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.4.0/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-18 20:54:55.000000 ursactl-0.4.0/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.4.0/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.4.0/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.4.0/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.4.0/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.4.0/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.4.0/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.4.0/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.4.0/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.4.0/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.4.0/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.4.0/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.4.0/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8139 2023-07-18 14:03:09.000000 ursactl-0.4.0/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.4.0/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/agent.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2323 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.4.0/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2184 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/pipeline.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1414 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/pipeline_run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1487 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/pipeline_sweep.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3658 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/project.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      865 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/core/running_agent.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.4.0/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 20:42:41.000000 ursactl-0.4.0/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    32670 2023-07-18 20:29:53.000000 ursactl-0.4.0/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.4.0/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.4.0/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.4.0/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.4.0/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.4.0/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-18 20:29:53.000000 ursactl-0.4.0/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-05 18:27:53.000000 ursactl-0.4.0/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.4.0/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-18 20:54:55.000000 ursactl-0.4.0/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.4.0/ursactl.egg-info/zip-safe
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/
+-rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.5.0/CHANGELOG.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.5.0/LICENSE.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.5.0/MANIFEST.in
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-20 12:43:14.000000 ursactl-0.5.0/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.5.0/README.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.5.0/pyproject.toml
+-rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.5.0/requirements-dev.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.5.0/requirements.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-20 12:43:14.000000 ursactl-0.5.0/setup.cfg
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/tests/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.5.0/tests/test_ursactl.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/airflow_provider/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.5.0/ursactl/airflow_provider/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.5.0/ursactl/airflow_provider/hooks.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/controllers/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/controllers/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.5.0/ursactl/controllers/base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.5.0/ursactl/controllers/create.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.5.0/ursactl/controllers/delete.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.5.0/ursactl/controllers/get.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.5.0/ursactl/controllers/init.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.5.0/ursactl/controllers/list.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.5.0/ursactl/controllers/refresh.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.5.0/ursactl/controllers/run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.5.0/ursactl/controllers/send.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.5.0/ursactl/controllers/show.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.5.0/ursactl/controllers/stop.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8139 2023-07-18 14:03:09.000000 ursactl-0.5.0/ursactl/controllers/sync.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.5.0/ursactl/controllers/update.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/controllers/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.5.0/ursactl/controllers/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.5.0/ursactl/controllers/utils/transforms.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/core/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/core/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/agent.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2323 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/dataset.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.5.0/ursactl/core/exc.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 12:42:32.000000 ursactl-0.5.0/ursactl/core/pipeline.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.5.0/ursactl/core/pipeline_run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.5.0/ursactl/core/pipeline_sweep.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3658 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/project.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.5.0/ursactl/core/running_agent.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/core/services/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.5.0/ursactl/core/services/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 20:42:41.000000 ursactl-0.5.0/ursactl/core/services/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    32670 2023-07-18 20:29:53.000000 ursactl-0.5.0/ursactl/core/services/ape_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/services/dss_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.5.0/ursactl/core/services/iam_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.5.0/ursactl/core/services/planning_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.5.0/ursactl/core/services/project_client.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/core/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.5.0/ursactl/core/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.5.0/ursactl/core/utils/magic.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-20 12:42:32.000000 ursactl-0.5.0/ursactl/core/version.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/ext/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/ext/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-20 12:23:03.000000 ursactl-0.5.0/ursactl/main.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/plugins/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/plugins/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl/templates/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.0/ursactl/templates/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/SOURCES.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/dependency_links.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/entry_points.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/requires.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-20 12:43:14.000000 ursactl-0.5.0/ursactl.egg-info/top_level.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.5.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.4.0/PKG-INFO` & `ursactl-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.4.0
+Version: 0.5.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.4.0/README.md` & `ursactl-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/setup.cfg` & `ursactl-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/airflow_provider/hooks.py` & `ursactl-0.5.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/base.py` & `ursactl-0.5.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/create.py` & `ursactl-0.5.0/ursactl/controllers/create.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/delete.py` & `ursactl-0.5.0/ursactl/controllers/delete.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/get.py` & `ursactl-0.5.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/init.py` & `ursactl-0.5.0/ursactl/controllers/init.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/list.py` & `ursactl-0.5.0/ursactl/controllers/list.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/run.py` & `ursactl-0.5.0/ursactl/controllers/run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/send.py` & `ursactl-0.5.0/ursactl/controllers/send.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/show.py` & `ursactl-0.5.0/ursactl/controllers/show.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/stop.py` & `ursactl-0.5.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/sync.py` & `ursactl-0.5.0/ursactl/controllers/sync.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/update.py` & `ursactl-0.5.0/ursactl/controllers/update.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/controllers/utils/transforms.py` & `ursactl-0.5.0/ursactl/controllers/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/_base.py` & `ursactl-0.5.0/ursactl/core/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/agent.py` & `ursactl-0.5.0/ursactl/core/agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/dataset.py` & `ursactl-0.5.0/ursactl/core/dataset.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/pipeline.py` & `ursactl-0.5.0/ursactl/core/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,14 @@
     """
     @property
     def client(self):
         if self._client is None:
             self._client = client('ape', self.app)
         return self._client
 
-    # @property
-    # def project(self):
-    #     from ursactl.core.project import Project
-
-    #     return Project(self._data['project_uuid'], app=self.app)
-
     @property
     def name(self):
         return self._data['name']
 
     @property
     def description(self):
         return self._data['description']
```

### Comparing `ursactl-0.4.0/ursactl/core/pipeline_run.py` & `ursactl-0.5.0/ursactl/core/pipeline_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ursactl.core.services import client
 from ursactl.core._base import Base
+import time
 
 
 class PipelineRun(Base):
     """
     Provides access to a pipeline run.
     """
     def __init__(self, *args, pipeline=None, **kwargs):
@@ -46,7 +47,23 @@
                     'jobStatus': None,
                     'provenance': None,
                     'parameters': None,
                 }
             else:
                 self._cached_data = self.client.get_pipeline_run(uuid=self.uuid)
         return self._cached_data
+
+    def __enter__(self):
+        while not self.completed:
+            time.sleep(5)
+            try:
+                self.refresh()
+            except ConnectionError:
+                pass
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        pass
+
+    @property
+    def completed(self):
+        return self.job_status == 'completed'
```

### Comparing `ursactl-0.4.0/ursactl/core/project.py` & `ursactl-0.5.0/ursactl/core/project.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/running_agent.py` & `ursactl-0.5.0/ursactl/core/running_agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,7 +26,13 @@
     def send_events(self, events):
         actions = []
         for event in events:
             result = self.client.send_event_to_agent(self.uuid, event)
             if result['result']:
                 actions.extend(result['result'])
         return actions
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.client.stop_agent(self.uuid)
```

### Comparing `ursactl-0.4.0/ursactl/core/services/__init__.py` & `ursactl-0.5.0/ursactl/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/_base.py` & `ursactl-0.5.0/ursactl/core/services/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/ape_client.py` & `ursactl-0.5.0/ursactl/core/services/ape_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/dss_client.py` & `ursactl-0.5.0/ursactl/core/services/dss_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/iam_client.py` & `ursactl-0.5.0/ursactl/core/services/iam_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/planning_client.py` & `ursactl-0.5.0/ursactl/core/services/planning_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/services/project_client.py` & `ursactl-0.5.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/core/utils/magic.py` & `ursactl-0.5.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl/main.py` & `ursactl-0.5.0/ursactl/main.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.4.0/ursactl.egg-info/PKG-INFO` & `ursactl-0.5.0/ursactl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.4.0
+Version: 0.5.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.4.0/ursactl.egg-info/SOURCES.txt` & `ursactl-0.5.0/ursactl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

