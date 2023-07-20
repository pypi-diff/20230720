# Comparing `tmp/kappe-0.8.0.tar.gz` & `tmp/kappe-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappe-0.8.0.tar", last modified: Thu Jul 20 13:41:54 2023, max compression
+gzip compressed data, was "kappe-0.8.1.tar", last modified: Thu Jul 20 14:50:39 2023, max compression
```

## Comparing `kappe-0.8.0.tar` & `kappe-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.199529 kappe-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 13:41:44.000000 kappe-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 13:41:54.195529 kappe-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 13:41:44.000000 kappe-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-20 13:41:44.000000 kappe-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:41:54.199529 kappe-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.191529 kappe-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/kappe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/qos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/msg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/pointcloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:50:30.000000 kappe-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 14:50:39.818515 kappe-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 14:50:30.000000 kappe-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 14:50:30.000000 kappe-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:50:39.818515 kappe-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.814515 kappe-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/kappe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/msg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/top_level.txt
```

### Comparing `kappe-0.8.0/PKG-INFO` & `kappe-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.8.0
+Version: 0.8.1
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `kappe-0.8.0/README.md` & `kappe-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/pyproject.toml` & `kappe-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 dependencies = [
     "mcap>=0.3.0",
     "mcap-ros1-support>=0.6.0",
     "mcap-ros2-support>=0.3.0",
     "numpy",
-    "pydantic>=1.0.0,<=2.0.0",
+    "pydantic>=1.0.0,<2.0.0",
     "strictyaml",
     "scipy",
     "tqdm",
     "pyyaml>=6.0.1",
 ]
 
 dynamic = ["version"]
```

### Comparing `kappe-0.8.0/src/kappe/convert.py` & `kappe-0.8.1/src/kappe/convert.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/cut.py` & `kappe-0.8.1/src/kappe/cut.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/kappe.py` & `kappe-0.8.1/src/kappe/kappe.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/module/pointcloud.py` & `kappe-0.8.1/src/kappe/module/pointcloud.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/module/qos.py` & `kappe-0.8.1/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/module/tf.py` & `kappe-0.8.1/src/kappe/module/tf.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/module/timing.py` & `kappe-0.8.1/src/kappe/module/timing.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/plugin.py` & `kappe-0.8.1/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/plugins/image.py` & `kappe-0.8.1/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/settings.py` & `kappe-0.8.1/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/utils/msg_def.py` & `kappe-0.8.1/src/kappe/utils/msg_def.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/utils/pointcloud2.py` & `kappe-0.8.1/src/kappe/utils/pointcloud2.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe/utils/settings.py` & `kappe-0.8.1/src/kappe/utils/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.0/src/kappe.egg-info/PKG-INFO` & `kappe-0.8.1/src/kappe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.8.0
+Version: 0.8.1
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `kappe-0.8.0/src/kappe.egg-info/SOURCES.txt` & `kappe-0.8.1/src/kappe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

