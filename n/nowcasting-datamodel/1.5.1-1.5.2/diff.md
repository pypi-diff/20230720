# Comparing `tmp/nowcasting_datamodel-1.5.1.tar.gz` & `tmp/nowcasting_datamodel-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.5.1.tar", last modified: Thu Jul 20 12:12:09 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.5.2.tar", last modified: Thu Jul 20 14:05:51 2023, max compression
```

## Comparing `nowcasting_datamodel-1.5.1.tar` & `nowcasting_datamodel-1.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.820907 nowcasting_datamodel-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-20 12:12:09.820907 nowcasting_datamodel-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.812907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.812907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.816907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.816907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.816907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.820907 nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.812907 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-20 12:12:09.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-20 12:12:09.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:12:09.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 12:12:09.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 12:12:09.000000 nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:12:09.820907 nowcasting_datamodel-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:12:09.820907 nowcasting_datamodel-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 12:11:56.000000 nowcasting_datamodel-1.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.284723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.284723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.284723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.284723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.284723 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-20 14:05:51.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-20 14:05:51.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:05:51.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 14:05:51.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 14:05:51.000000 nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:05:51.288723 nowcasting_datamodel-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 14:05:38.000000 nowcasting_datamodel-1.5.2/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.5.1/PKG-INFO` & `nowcasting_datamodel-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.5.1
+Version: 1.5.2
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.5.1/README.md` & `nowcasting_datamodel-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/diagram.png` & `nowcasting_datamodel-1.5.2/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/diagram_pv.png` & `nowcasting_datamodel-1.5.2/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/blend.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
             logger.debug(
                 f"No forecast values for {model_name} for gsp_id {gsp_id} "
                 f"and start_datetime {start_datetime}"
             )
         else:
             logger.debug(
                 f"Found {len(forecast_values_one_model)} values for {model_name} "
-                f"for gsp_id {gsp_id} and start_datetime {start_datetime}"
+                f"for gsp_id {gsp_id} and start_datetime {start_datetime}. "
+                f"First value is {forecast_values_one_model[0].target_time}"
             )
             forecast_values_all_model.append([model_name, forecast_values_one_model])
 
     # check the created_utc is valid for each forecast
     forecast_values_all_model_valid = check_forecast_created_utc(forecast_values_all_model)
 
     # make into dataframe
```

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -85,14 +85,17 @@
         )
         value_df.reset_index(inplace=True, drop=False)
         forecast_values_all_model_df.append(value_df)
     # join into one dataframe
     forecast_values_all_model = pd.concat(forecast_values_all_model_df, axis=0)
     forecast_values_all_model.reset_index(inplace=True)
 
+    # sort by target time
+    forecast_values_all_model.sort_values(by=["target_time"], inplace=True)
+
     return forecast_values_all_model
 
 
 def convert_df_to_list_forecast_values(forecast_values_blended: pd.DataFrame):
     """
     Convert the blended dataframe to a list of ForecastValue objects
 
@@ -122,91 +125,160 @@
 
 def blend_forecasts_together(forecast_values_all_model, weights_df):
     """
     Blend the forecasts together using the weights_df
 
     :param forecast_values_all_model: Dataframe containing the columns 'target_time',
         'expected_power_generation_megawatts', 'adjust_mw', 'model_name'
-    :param weights_df: Dataframe of weights with columns 'model_name' and 'weight'
+    :param weights_df: Dataframe of weights with columns of the model name,
+        and index of target times
     :return: Dataframe with the columns
         'target_time',
         'expected_power_generation_megawatts',
         'adjust_mw'
     """
 
     # drop of the "properties" column
     if "properties" in forecast_values_all_model.columns:
         forecast_values_all_model = forecast_values_all_model.drop(columns=["properties"]).copy()
 
-    # blend together
-    # lets deal with unique target times first
-    logger.debug(forecast_values_all_model["target_time"])
     # get all unique target times
     all_target_times = forecast_values_all_model["target_time"].unique()
+    if len(all_target_times) == len(forecast_values_all_model):
+        # if we have the same number of unique target times as we have rows,
+        # then we only have one model, so just return that
+        return forecast_values_all_model
     logger.debug(f"Found in total {len(all_target_times)} target times")
 
-    # get the duplicated target times
-    duplicated_target_times = forecast_values_all_model[
-        forecast_values_all_model["target_time"].duplicated()
-    ]["target_time"].tolist()
-    logger.debug(f"Found {len(duplicated_target_times)} duplicated target times")
-    unique_target_times = [x for x in all_target_times if x not in duplicated_target_times]
-    logger.debug(f"Found in {len(unique_target_times)} unique target times")
-
-    # get the index of the duplicated and unique target times
-    duplicated_target_times_idx = forecast_values_all_model[
-        forecast_values_all_model["target_time"].isin(duplicated_target_times)
-    ].index
-    unique_target_times_idx = forecast_values_all_model[
-        forecast_values_all_model["target_time"].isin(unique_target_times)
-    ].index
-
-    # get the unique forecast values
-    forecast_values_blended = forecast_values_all_model.loc[unique_target_times_idx]
-
-    # now lets deal with the weights
-    duplicated = forecast_values_all_model.loc[duplicated_target_times_idx]
-    duplicated = duplicated.drop_duplicates()
-
-    # only do this if there are duplicated
-    if len(duplicated) > 0:
-        logger.debug(f"Now blending the duplicated target times using {weights_df}")
-
-        pd.DataFrame()
-        # unstack the weights
-        weights_one_df = weights_df.stack()
-        weights_one_df.name = "weight"
-        weights_one_df = weights_one_df.reset_index()
-        weights_one_df = weights_one_df.rename(columns={"level_1": "model_name"})
-        weights_one_df = weights_one_df.rename(columns={"level_0": "target_time"})
-
-        # join the weights to the duplicated
-        duplicated = pd.merge(
-            duplicated,
-            weights_one_df,
-            how="left",
-            left_on=["model_name", "target_time"],
-            right_on=["model_name", "target_time"],
+    # unstack weights, this makes a dataframe with columns "model_name", "target_time", "weight"
+    weights_one_df = weights_df.stack()
+    weights_one_df.name = "weight"
+    weights_one_df = weights_one_df.reset_index()
+    weights_one_df = weights_one_df.rename(columns={"level_1": "model_name"})
+    weights_one_df = weights_one_df.rename(columns={"level_0": "target_time"})
+
+    forecast_values_blended = []
+    # loop over datetimes, we could do this without looping,
+    # but I found it hard to read the code, and keep track of things
+    for target_time in all_target_times:
+        logger.debug(f"Blending forecasts for {target_time}")
+
+        # get the forecast values for this target time
+        forecast_values_one_target_time = forecast_values_all_model[
+            forecast_values_all_model["target_time"] == target_time
+        ]
+        logger.debug(f"Found {len(forecast_values_one_target_time)} forecasts for {target_time}")
+
+        # get the weights for this target time
+        weights_one_target_time = weights_one_df[weights_one_df["target_time"] == target_time]
+        logger.debug(f"Found {len(weights_one_target_time)} weights for {target_time}")
+
+        # merge the forecast values and weights together
+        forecast_values_one_target_time = forecast_values_one_target_time[
+            ["model_name", "expected_power_generation_megawatts", "adjust_mw"]
+        ]
+        logger.debug(weights_one_target_time)
+        weights_one_target_time = weights_one_target_time[["model_name", "weight"]]
+
+        forecast_values_one_target_time_blend = blend_together_one_target_time(
+            forecast_values_one_target_time, weights_one_target_time, target_time
         )
 
-        # multiply the expected power generation by the weight
-        for col in ["expected_power_generation_megawatts", "adjust_mw"]:
-            duplicated[col] = duplicated[col] * duplicated["weight"]
-        duplicated.drop(columns=["created_utc"], inplace=True)
-
-        # sum the weights
-        duplicated = duplicated.groupby(["target_time"]).sum()
-
-        # make sure target_time is a columns
-        duplicated["target_time"] = duplicated.index
-        duplicated.reset_index(inplace=True, drop=True)
-
-        # divide by the sum of the weights, # TODO should we be worried about dividing by zero?
-        for col in ["expected_power_generation_megawatts", "adjust_mw"]:
-            duplicated[col] /= duplicated["weight"]
-
-        logger.debug(duplicated)
-    # join unique and duplicates together
-    forecast_values_blended = pd.concat([forecast_values_blended, duplicated], axis=0)
-    # sort by target time
-    forecast_values_blended.sort_values(by="target_time", inplace=True)
+        total_weights_used = forecast_values_one_target_time_blend["weight"].iloc[0]
+        if total_weights_used == 0:
+            # the total weight is 0, which means the forecast is not available for the target time
+            # Therefore we find the model which model to use
+
+            logger.debug(
+                f"Trying to blend forecast for {target_time} "
+                f"but the weights for the forecasts with weights are not available, or add to 0"
+            )
+
+            if len(forecast_values_one_target_time) == 1:
+                logger.debug(f"Only found one forecast for {target_time} so using that")
+                forecast_values_one_target_time_blend = forecast_values_one_target_time
+                forecast_values_one_target_time_blend["target_time"] = target_time
+            else:
+                weights_target_time = weights_df[weights_df.index > target_time]
+
+                logger.debug(
+                    f"Found more than one forecast available for {target_time}"
+                    f"Going to try at the next weights "
+                )
+                for i, row in weights_target_time.iterrows():
+                    # format row into dataframe
+                    weights = pd.DataFrame(row)
+                    weights.index.name = "model_name"
+                    weights.reset_index(inplace=True)
+                    weights.columns = ["model_name", "weight"]
+
+                    logger.debug(f"Trying {weights}")
+
+                    # blend together
+                    forecast_values_one_target_time_blend = blend_together_one_target_time(
+                        forecast_values_one_target_time, weights, target_time
+                    )
+                    total_weights_used = forecast_values_one_target_time_blend["weight"].iloc[0]
+
+                    # keep looping unless the total weights used > 0. This means we have blended the
+                    # forecast together using the next weights possible
+                    if total_weights_used > 0:
+                        break
+
+        # append to the blended dataframe
+        forecast_values_blended.append(forecast_values_one_target_time_blend)
+
+    forecast_values_blended = pd.concat(forecast_values_blended, axis=0)
+
     return forecast_values_blended
+
+
+def blend_together_one_target_time(
+    forecast_values_one_target_time: pd.DataFrame,
+    weights_one_target_time: pd.DataFrame,
+    target_time: datetime,
+):
+    """
+    Blend forecasts for one target time together using the weights
+
+    :param forecast_values_one_target_time: dataframe with columns 'model_name',
+        'expected_power_generation_megawatts', 'adjust_mw'. The rows are the different models
+    :param weights_one_target_time: dataframe with columns 'model_name', 'weight'.
+        The rows are the different models
+    :param target_time: the target time of this forecast
+    :return: blended dataframe with columns 'target_time', 'expected_power_generation_megawatts',
+        'adjust_mw'. The column weight shows how much total weight was used for each model
+    """
+    forecast_values_one_target_time = forecast_values_one_target_time.merge(
+        weights_one_target_time,
+        how="left",
+        left_on=["model_name"],
+        right_on=["model_name"],
+    )
+    logger.debug(forecast_values_one_target_time)
+
+    # calculate the blended forecast
+    weight = np.sum(forecast_values_one_target_time["weight"])
+    expected_power_generation_megawatts = (
+        np.sum(
+            forecast_values_one_target_time["expected_power_generation_megawatts"]
+            * forecast_values_one_target_time["weight"]
+        )
+        / weight
+    )
+    adjust_mw = (
+        np.sum(
+            forecast_values_one_target_time["adjust_mw"] * forecast_values_one_target_time["weight"]
+        )
+        / weight
+    )
+
+    # make into dataframe
+    forecast_values_one_target_time_blend = pd.DataFrame(
+        data=[[expected_power_generation_megawatts, adjust_mw, weight]],
+        columns=["expected_power_generation_megawatts", "adjust_mw", "weight"],
+    )
+    # make sure target_time is a columns
+    forecast_values_one_target_time_blend["target_time"] = target_time
+    forecast_values_one_target_time_blend.reset_index(inplace=True, drop=True)
+
+    return forecast_values_one_target_time_blend
```

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.5.1
+Version: 1.5.2
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.5.1/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.5.2/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/setup.py` & `nowcasting_datamodel-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.5.2/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/tests/test_fake.py` & `nowcasting_datamodel-1.5.2/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/tests/test_fake_pv.py` & `nowcasting_datamodel-1.5.2/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/tests/test_national.py` & `nowcasting_datamodel-1.5.2/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.1/tests/test_utils.py` & `nowcasting_datamodel-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

