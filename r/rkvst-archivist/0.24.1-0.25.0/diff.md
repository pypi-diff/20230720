# Comparing `tmp/rkvst-archivist-0.24.1.tar.gz` & `tmp/rkvst-archivist-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rkvst-archivist-0.24.1.tar", last modified: Wed Jul  5 13:44:13 2023, max compression
+gzip compressed data, was "rkvst-archivist-0.25.0.tar", last modified: Thu Jul 20 10:54:47 2023, max compression
```

## Comparing `rkvst-archivist-0.24.1.tar` & `rkvst-archivist-0.25.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/archivist/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 13:44:05.000000 rkvst-archivist-0.24.1/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/archivist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 13:41:20.000000 rkvst-archivist-0.24.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 13:44:13.000000 rkvst-archivist-0.24.1/rkvst_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-05 13:44:13.585877 rkvst-archivist-0.24.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 10:54:39.000000 rkvst-archivist-0.25.0/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/setup.cfg
```

### Comparing `rkvst-archivist-0.24.1/LICENSE` & `rkvst-archivist-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/PKG-INFO` & `rkvst-archivist-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.24.1
+Version: 0.25.0
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
 Project-URL: Tracker, https://github.com/rkvst/rkvst-python/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. _readme:
 
 RKVST Python Client
@@ -30,18 +30,18 @@
 
 Please note that the canonical API for RKVST is always the REST API
 documented at https://docs.rkvst.com
 
 Support
 =======
 
-This package currently is tested against Python versions 3.7,3.8,3.9,3.10 and 3.11.
+This package currently is tested against Python versions 3.8,3.9,3.10 and 3.11.
 
-The current default version is 3.7 - this means that this package will not
-use any features specific to versions 3.8 and later.
+The current default version is 3.8 - this means that this package will not
+use any features specific to versions 3.9 and later.
 
 After End of Life of a particular Python version, support is offered on a best effort
 basis. We may ask you to update your Python version to help solve the problem,
 if it cannot be reasonably resolved in your current version.
 
 Installation
 =============
```

### Comparing `rkvst-archivist-0.24.1/README.rst` & `rkvst-archivist-0.25.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 Please note that the canonical API for RKVST is always the REST API
 documented at https://docs.rkvst.com
 
 Support
 =======
 
-This package currently is tested against Python versions 3.7,3.8,3.9,3.10 and 3.11.
+This package currently is tested against Python versions 3.8,3.9,3.10 and 3.11.
 
-The current default version is 3.7 - this means that this package will not
-use any features specific to versions 3.8 and later.
+The current default version is 3.8 - this means that this package will not
+use any features specific to versions 3.9 and later.
 
 After End of Life of a particular Python version, support is offered on a best effort
 basis. We may ask you to update your Python version to help solve the problem,
 if it cannot be reasonably resolved in your current version.
 
 Installation
 =============
```

### Comparing `rkvst-archivist-0.24.1/archivist/access_policies.py` & `rkvst-archivist-0.25.0/archivist/access_policies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/appidp.py` & `rkvst-archivist-0.25.0/archivist/appidp.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/applications.py` & `rkvst-archivist-0.25.0/archivist/applications.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/archivist.py` & `rkvst-archivist-0.25.0/archivist/archivist.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/archivistpublic.py` & `rkvst-archivist-0.25.0/archivist/archivistpublic.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/asset.py` & `rkvst-archivist-0.25.0/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/assetattachments.py` & `rkvst-archivist-0.25.0/archivist/assetattachments.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/assets.py` & `rkvst-archivist-0.25.0/archivist/assets.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/attachments.py` & `rkvst-archivist-0.25.0/archivist/attachments.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/cmds/runner/main.py` & `rkvst-archivist-0.25.0/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/cmds/runner/run.py` & `rkvst-archivist-0.25.0/archivist/cmds/runner/run.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/cmds/template/main.py` & `rkvst-archivist-0.25.0/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/cmds/template/run.py` & `rkvst-archivist-0.25.0/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/compliance.py` & `rkvst-archivist-0.25.0/archivist/compliance.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/compliance_policies.py` & `rkvst-archivist-0.25.0/archivist/compliance_policies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/compliance_policy_requests.py` & `rkvst-archivist-0.25.0/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/compliance_policy_type.py` & `rkvst-archivist-0.25.0/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/composite.py` & `rkvst-archivist-0.25.0/archivist/composite.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/confirmer.py` & `rkvst-archivist-0.25.0/archivist/confirmer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional, Union, overload
 
 import backoff
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
+    from backoff._typing import Details
+
     from . import assets, events
 
+
 from .constants import (
     CONFIRMATION_CONFIRMED,
     CONFIRMATION_FAILED,
     CONFIRMATION_PENDING,
     CONFIRMATION_STATUS,
 )
 from .errors import ArchivistUnconfirmedError
@@ -34,17 +37,17 @@
     ReturnTypes = Union[assets.Asset, events.Event]
 
 
 def __lookup_max_time():
     return MAX_TIME
 
 
-def __on_giveup_confirmation(details: dict[str, Any]):
+def __on_giveup_confirmation(details: "Details"):
     identity: str = details["args"][1]
-    elapsed: str = details["elapsed"]
+    elapsed: float = details["elapsed"]
     raise ArchivistUnconfirmedError(
         f"confirmation for {identity} timed out after {elapsed} seconds"
     )
 
 
 # These overloads are used for type hinting, if self is events client then
 # an event will be returned. If self is Asset client then an asset will be
@@ -101,18 +104,18 @@
 
     if entity[CONFIRMATION_STATUS] == CONFIRMATION_CONFIRMED:
         return entity
 
     return None  # pyright: ignore
 
 
-def __on_giveup_confirmed(details: dict[str, Any]):
+def __on_giveup_confirmed(details: "Details"):
     self: PrivateManagers = details["args"][0]
     count = self.pending_count
-    elapsed: int = details["elapsed"]
+    elapsed: float = details["elapsed"]
     raise ArchivistUnconfirmedError(
         f"{count} pending assets still present after {elapsed} seconds"
     )
 
 
 @backoff.on_predicate(
     backoff.expo,
```

### Comparing `rkvst-archivist-0.24.1/archivist/constants.py` & `rkvst-archivist-0.25.0/archivist/constants.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/dictmerge.py` & `rkvst-archivist-0.25.0/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/errors.py` & `rkvst-archivist-0.25.0/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/events.py` & `rkvst-archivist-0.25.0/archivist/events.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/locations.py` & `rkvst-archivist-0.25.0/archivist/locations.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/logger.py` & `rkvst-archivist-0.25.0/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/parser.py` & `rkvst-archivist-0.25.0/archivist/parser.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/retry429.py` & `rkvst-archivist-0.25.0/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/runner.py` & `rkvst-archivist-0.25.0/archivist/runner.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/sboms.py` & `rkvst-archivist-0.25.0/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/subjects.py` & `rkvst-archivist-0.25.0/archivist/subjects.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/subjects_confirmer.py` & `rkvst-archivist-0.25.0/archivist/subjects_confirmer.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/tenancies.py` & `rkvst-archivist-0.25.0/archivist/tenancies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/timestamp.py` & `rkvst-archivist-0.25.0/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/archivist/utils.py` & `rkvst-archivist-0.25.0/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/pyproject.toml` & `rkvst-archivist-0.25.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 # load-plugins =
 
 # Pickle collected data for later comparisons.
 persistent = true
 
 # Minimum Python version to use for version dependent checks. Will default to the
 # version used to run pylint.
-py-version = "3.7"
+py-version = "3.8"
 
 # Discover python modules and packages in the file system subtree.
 # recursive =
 
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode = true
```

### Comparing `rkvst-archivist-0.24.1/rkvst_archivist.egg-info/PKG-INFO` & `rkvst-archivist-0.25.0/rkvst_archivist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.24.1
+Version: 0.25.0
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
 Project-URL: Tracker, https://github.com/rkvst/rkvst-python/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. _readme:
 
 RKVST Python Client
@@ -30,18 +30,18 @@
 
 Please note that the canonical API for RKVST is always the REST API
 documented at https://docs.rkvst.com
 
 Support
 =======
 
-This package currently is tested against Python versions 3.7,3.8,3.9,3.10 and 3.11.
+This package currently is tested against Python versions 3.8,3.9,3.10 and 3.11.
 
-The current default version is 3.7 - this means that this package will not
-use any features specific to versions 3.8 and later.
+The current default version is 3.8 - this means that this package will not
+use any features specific to versions 3.9 and later.
 
 After End of Life of a particular Python version, support is offered on a best effort
 basis. We may ask you to update your Python version to help solve the problem,
 if it cannot be reasonably resolved in your current version.
 
 Installation
 =============
```

### Comparing `rkvst-archivist-0.24.1/rkvst_archivist.egg-info/SOURCES.txt` & `rkvst-archivist-0.25.0/rkvst_archivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.24.1/setup.cfg` & `rkvst-archivist-0.25.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 	Topic :: Utilities
 project_urls = 
 	Documentation = https://python.rkvst.com
 	Source = https://github.com/rkvst/rkvst-python
 	Tracker = https://github.com/rkvst/rkvst-python/issues
 
 [options]
@@ -31,15 +31,15 @@
 packages = 
 	archivist
 	archivist.cmds
 	archivist.cmds.runner
 	archivist.cmds.template
 include_package_data = True
 platforms = any
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = setuptools-git-versioning
 
 [options.entry_points]
 console_scripts = 
 	archivist_runner = archivist.cmds.runner.main:main
 	archivist_template = archivist.cmds.template.main:main
```

