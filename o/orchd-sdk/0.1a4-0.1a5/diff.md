# Comparing `tmp/orchd-sdk-0.1a4.tar.gz` & `tmp/orchd-sdk-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchd-sdk-0.1a4.tar", last modified: Mon Apr 17 15:14:56 2023, max compression
+gzip compressed data, was "orchd-sdk-0.1a5.tar", last modified: Thu Jul 20 10:48:05 2023, max compression
```

## Comparing `orchd-sdk-0.1a4.tar` & `orchd-sdk-0.1a5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.720550 orchd-sdk-0.1a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2264 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/reactions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/sinks.py
--rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/logger.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    12001 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13919 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     9526 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/reaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     6912 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3436 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/sink.py
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:48:05.878630 orchd-sdk-0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-20 10:48:05.878630 orchd-sdk-0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:48:05.878630 orchd-sdk-0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:48:05.874630 orchd-sdk-0.1a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:48:05.874630 orchd-sdk-0.1a5/src/orchd_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:48:05.874630 orchd-sdk-0.1a5/src/orchd_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2264 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/api/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/api/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/api/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/logger.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12006 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13919 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9526 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6912 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3436 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/sink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-07-20 10:47:13.000000 orchd-sdk-0.1a5/src/orchd_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:48:05.874630 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 10:48:05.000000 orchd-sdk-0.1a5/src/orchd_sdk.egg-info/top_level.txt
```

### Comparing `orchd-sdk-0.1a4/LICENSE.md` & `orchd-sdk-0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/PKG-INFO` & `orchd-sdk-0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a4
+Version: 0.1a5
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
```

### Comparing `orchd-sdk-0.1a4/README.md` & `orchd-sdk-0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/setup.py` & `orchd-sdk-0.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/__init__.py` & `orchd-sdk-0.1a5/src/orchd_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/api/__init__.py` & `orchd-sdk-0.1a5/src/orchd_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/api/events.py` & `orchd-sdk-0.1a5/src/orchd_sdk/api/events.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/api/reactions.py` & `orchd-sdk-0.1a5/src/orchd_sdk/api/reactions.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/api/sensors.py` & `orchd-sdk-0.1a5/src/orchd_sdk/api/sensors.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/api/sinks.py` & `orchd-sdk-0.1a5/src/orchd_sdk/api/sinks.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/cli.py` & `orchd-sdk-0.1a5/src/orchd_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/common.py` & `orchd-sdk-0.1a5/src/orchd_sdk/common.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/errors.py` & `orchd-sdk-0.1a5/src/orchd_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/logger.ini` & `orchd-sdk-0.1a5/src/orchd_sdk/logger.ini`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/logging.py` & `orchd-sdk-0.1a5/src/orchd_sdk/logging.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/models.py` & `orchd-sdk-0.1a5/src/orchd_sdk/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     An event have a name and data associated. Each event have
     an unique ID. They are propagated into the Orchd System usually
     by Sensors and captured by Reactions that can react to it.
     """
     event_name: str = Field(
         title='Event Name',
         description='A unique/namespaced name for the event.',
-        regex=r'^\w[\w\._\-]+$',
+        pattern=r'^\w[\w\._\-]+$',
         example='io.orchd.events.system.Test'
     )
     data: Dict[str, Any] = Field(
         default_factory=dict,
         title='Event Data',
         description='Data attached to the event in the form of key/value pairs.'
     )
@@ -153,15 +153,15 @@
     - Service Discovered
     - USB Device Attached
     - Service Down
     """
     name: str = Field(
         title='Reaction Template Name',
         description='A unique/namespaced name for the Reaction Template',
-        regex=r'^\w[\w\._\-]+$',
+        pattern=r'^\w[\w\._\-]+$',
         example='io.orchd.reaction_template.DummyTemplate'
     )
     version: str = Field(
         title='Template Version',
         description='Version of this reaction template.',
         example='1.0'
     )
@@ -224,15 +224,15 @@
         example='0ba3376f-64b8-4ecf-a579-66c353100e1c',
         default_factory=uuid_str_factory
     )
 
     name: str = Field(
         title='Sensor\'s Name',
         description='The namespaced name of the Sensor',
-        regex=r'^\w[\w\._\-]+$',
+        patter=r'^\w[\w\._\-]+$',
         example='io.orchd.sensor.template.DummySensorTemplate'
     )
 
     version: str = Field(
         title='Version',
         description='Sensor\'s version',
         example='1.0'
```

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/project.py` & `orchd-sdk-0.1a5/src/orchd_sdk/project.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/reaction.py` & `orchd-sdk-0.1a5/src/orchd_sdk/reaction.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/sensor.py` & `orchd-sdk-0.1a5/src/orchd_sdk/sensor.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/sink.py` & `orchd-sdk-0.1a5/src/orchd_sdk/sink.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk/util.py` & `orchd-sdk-0.1a5/src/orchd_sdk/util.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk.egg-info/PKG-INFO` & `orchd-sdk-0.1a5/src/orchd_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a4
+Version: 0.1a5
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
```

### Comparing `orchd-sdk-0.1a4/src/orchd_sdk.egg-info/SOURCES.txt` & `orchd-sdk-0.1a5/src/orchd_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

