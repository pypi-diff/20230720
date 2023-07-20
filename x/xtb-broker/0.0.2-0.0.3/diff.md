# Comparing `tmp/xtb_broker-0.0.2.tar.gz` & `tmp/xtb_broker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.2.tar", last modified: Thu Jul 20 21:20:03 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.3.tar", last modified: Thu Jul 20 21:23:59 2023, max compression
```

## Comparing `xtb_broker-0.0.2.tar` & `xtb_broker-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1073 2023-07-20 20:49:36.000000 xtb_broker-0.0.2/LICENSE
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      485 2023-07-20 21:18:13.000000 xtb_broker-0.0.2/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:19:25.000000 xtb_broker-0.0.2/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/setup.cfg
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/src/
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/src/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/client.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.2/src/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/src/xtb_broker/xtb_config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/src/xtb_broker/xtb_models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.2/src/xtb_broker/xtb_models/transaction.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:20:03.480195 xtb_broker-0.0.2/src/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:20:03.000000 xtb_broker-0.0.2/src/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      695 2023-07-20 21:20:03.000000 xtb_broker-0.0.2/src/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-20 21:20:03.000000 xtb_broker-0.0.2/src/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-20 21:20:03.000000 xtb_broker-0.0.2/src/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1073 2023-07-20 20:49:36.000000 xtb_broker-0.0.3/LICENSE
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      485 2023-07-20 21:18:13.000000 xtb_broker-0.0.3/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:23:18.000000 xtb_broker-0.0.3/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/setup.cfg
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/client.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.3/src/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker/xtb_config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/src/xtb_broker/xtb_models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/transaction.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      695 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.2/LICENSE` & `xtb_broker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/PKG-INFO` & `xtb_broker-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtb_broker
-Version: 0.0.2
+Version: 0.0.3
 Summary: XTB broker models, methods and tools
 Author-email: Arrubo <author@example.com>
 Project-URL: Homepage, https://pypi.org/project/xtb-broker/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xtb_broker-0.0.2/pyproject.toml` & `xtb_broker-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xtb_broker"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Arrubo", email="author@example.com" },
 ]
 description = "XTB broker models, methods and tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xtb_broker-0.0.2/src/xtb_broker/client.py` & `xtb_broker-0.0.3/src/xtb_broker/client.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/utils.py` & `xtb_broker-0.0.3/src/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_config/constants.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_config/exception.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_config/frozen.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_config/frozen.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/arbitrage.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/arbitrage.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/position.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/position.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/shift.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/shift.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/symbol.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/symbol.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/timetable.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/timetable.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/trade.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/trade.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker/xtb_models/transaction.py` & `xtb_broker-0.0.3/src/xtb_broker/xtb_models/transaction.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.2/src/xtb_broker.egg-info/PKG-INFO` & `xtb_broker-0.0.3/src/xtb_broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtb-broker
-Version: 0.0.2
+Version: 0.0.3
 Summary: XTB broker models, methods and tools
 Author-email: Arrubo <author@example.com>
 Project-URL: Homepage, https://pypi.org/project/xtb-broker/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xtb_broker-0.0.2/src/xtb_broker.egg-info/SOURCES.txt` & `xtb_broker-0.0.3/src/xtb_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

