# Comparing `tmp/idds-doma-1.3.0.tar.gz` & `tmp/idds-doma-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.3.0.tar", last modified: Wed Jul 12 16:01:39 2023, max compression
+gzip compressed data, was "idds-doma-1.3.1.tar", last modified: Thu Jul 20 07:28:49 2023, max compression
```

## Comparing `idds-doma-1.3.0.tar` & `idds-doma-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-doma-1.3.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 16:01:39.786002 idds-doma-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 16:01:25.000000 idds-doma-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-07-12 16:01:25.000000 idds-doma-1.3.0/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-07-12 16:01:25.000000 idds-doma-1.3.0/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.782002 idds-doma-1.3.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-doma-1.3.0/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domaeventmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandaeswork.py
--rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domatree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:39.786002 idds-doma-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-12 16:01:25.000000 idds-doma-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 16:01:34.000000 idds-doma-1.3.0/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 07:28:35.000000 idds-doma-1.3.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-20 07:28:49.266109 idds-doma-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 07:28:35.000000 idds-doma-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-07-20 07:28:35.000000 idds-doma-1.3.1/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-07-20 07:28:35.000000 idds-doma-1.3.1/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 07:28:43.000000 idds-doma-1.3.1/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflowv2/domaeventmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflowv2/domapandaeswork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflowv2/domapandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-20 07:28:35.000000 idds-doma-1.3.1/lib/idds/doma/workflowv2/domatree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-20 07:28:49.000000 idds-doma-1.3.1/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-20 07:28:49.000000 idds-doma-1.3.1/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:28:49.000000 idds-doma-1.3.1/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 07:28:49.000000 idds-doma-1.3.1/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 07:28:49.000000 idds-doma-1.3.1/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 07:28:49.266109 idds-doma-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-20 07:28:35.000000 idds-doma-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:49.266109 idds-doma-1.3.1/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-20 07:28:43.000000 idds-doma-1.3.1/tools/env/environment.yml
```

### Comparing `idds-doma-1.3.0/LICENSE.rst` & `idds-doma-1.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/PKG-INFO` & `idds-doma-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.3.0
+Version: 1.3.1
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.3.0/bin/setup_panda_token` & `idds-doma-1.3.1/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/bin/setup_panda_token.py` & `idds-doma-1.3.1/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.3.1/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds/doma/workflowv2/domaeventmap.py` & `idds-doma-1.3.1/lib/idds/doma/workflowv2/domaeventmap.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandaeswork.py` & `idds-doma-1.3.1/lib/idds/doma/workflowv2/domapandaeswork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.3.1/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds/doma/workflowv2/domatree.py` & `idds-doma-1.3.1/lib/idds/doma/workflowv2/domatree.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.3.1/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.3.0
+Version: 1.3.1
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.3.0/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.3.1/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.0/setup.py` & `idds-doma-1.3.1/setup.py`

 * *Files identical despite different names*

