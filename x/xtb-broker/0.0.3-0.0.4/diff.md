# Comparing `tmp/xtb_broker-0.0.3.tar.gz` & `tmp/xtb_broker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.3.tar", last modified: Thu Jul 20 21:23:59 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.4.tar", last modified: Thu Jul 20 21:31:31 2023, max compression
```

## Comparing `xtb_broker-0.0.3.tar` & `xtb_broker-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1073 2023-07-20 20:49:36.000000 xtb_broker-0.0.3/LICENSE
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      485 2023-07-20 21:18:13.000000 xtb_broker-0.0.3/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:23:18.000000 xtb_broker-0.0.3/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/setup.cfg
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/client.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.3/src/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker/xtb_config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.500331 xtb_broker-0.0.3/src/xtb_broker/xtb_models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.3/src/xtb_broker/xtb_models/transaction.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:23:59.496331 xtb_broker-0.0.3/src/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      695 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-20 21:23:59.000000 xtb_broker-0.0.3/src/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1073 2023-07-20 20:49:36.000000 xtb_broker-0.0.4/LICENSE
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      485 2023-07-20 21:18:13.000000 xtb_broker-0.0.4/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:31:01.000000 xtb_broker-0.0.4/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/setup.cfg
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/src/
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/src/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/client.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/src/xtb_broker/config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.4/src/xtb_broker/config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/src/xtb_broker/models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/models/transaction.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.4/src/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.4/src/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:31:31.028777 xtb_broker-0.0.4/src/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:31:31.000000 xtb_broker-0.0.4/src/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      651 2023-07-20 21:31:31.000000 xtb_broker-0.0.4/src/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-20 21:31:31.000000 xtb_broker-0.0.4/src/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-20 21:31:31.000000 xtb_broker-0.0.4/src/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.3/LICENSE` & `xtb_broker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/PKG-INFO` & `xtb_broker-0.0.4/src/xtb_broker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xtb_broker
-Version: 0.0.3
+Name: xtb-broker
+Version: 0.0.4
 Summary: XTB broker models, methods and tools
 Author-email: Arrubo <author@example.com>
 Project-URL: Homepage, https://pypi.org/project/xtb-broker/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xtb_broker-0.0.3/pyproject.toml` & `xtb_broker-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xtb_broker"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Arrubo", email="author@example.com" },
 ]
 description = "XTB broker models, methods and tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xtb_broker-0.0.3/src/xtb_broker/client.py` & `xtb_broker-0.0.4/src/xtb_broker/client.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/utils.py` & `xtb_broker-0.0.4/src/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb.py` & `xtb_broker-0.0.4/src/xtb_broker/xtb.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_config/constants.py` & `xtb_broker-0.0.4/src/xtb_broker/config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_config/exception.py` & `xtb_broker-0.0.4/src/xtb_broker/config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_config/frozen.py` & `xtb_broker-0.0.4/src/xtb_broker/config/frozen.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/arbitrage.py` & `xtb_broker-0.0.4/src/xtb_broker/models/arbitrage.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/position.py` & `xtb_broker-0.0.4/src/xtb_broker/models/position.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/shift.py` & `xtb_broker-0.0.4/src/xtb_broker/models/shift.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/symbol.py` & `xtb_broker-0.0.4/src/xtb_broker/models/symbol.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/timetable.py` & `xtb_broker-0.0.4/src/xtb_broker/models/timetable.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/trade.py` & `xtb_broker-0.0.4/src/xtb_broker/models/trade.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker/xtb_models/transaction.py` & `xtb_broker-0.0.4/src/xtb_broker/models/transaction.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.3/src/xtb_broker.egg-info/PKG-INFO` & `xtb_broker-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xtb-broker
-Version: 0.0.3
+Name: xtb_broker
+Version: 0.0.4
 Summary: XTB broker models, methods and tools
 Author-email: Arrubo <author@example.com>
 Project-URL: Homepage, https://pypi.org/project/xtb-broker/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

