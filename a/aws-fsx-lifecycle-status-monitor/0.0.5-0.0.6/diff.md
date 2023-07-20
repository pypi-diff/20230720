# Comparing `tmp/aws-fsx-lifecycle-status-monitor-0.0.5.tar.gz` & `tmp/aws-fsx-lifecycle-status-monitor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.5.tar", last modified: Thu Jul 20 07:58:34 2023, max compression
+gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.6.tar", last modified: Thu Jul 20 08:10:19 2023, max compression
```

## Comparing `aws-fsx-lifecycle-status-monitor-0.0.5.tar` & `aws-fsx-lifecycle-status-monitor-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:58:34.391822 aws-fsx-lifecycle-status-monitor-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 07:58:34.391822 aws-fsx-lifecycle-status-monitor-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 07:58:34.391822 aws-fsx-lifecycle-status-monitor-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:58:34.387822 aws-fsx-lifecycle-status-monitor-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:58:34.387822 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:58:34.387822 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   452433 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:58:22.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:58:34.387822 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 07:58:34.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 07:58:34.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:58:34.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 07:58:34.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 07:58:34.000000 aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   452431 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:10:08.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:10:19.387226 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 08:10:19.000000 aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/LICENSE` & `aws-fsx-lifecycle-status-monitor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.5
+Version: 0.0.6
 Summary: aws_fsx_lifecycle_status_monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
-Project-URL: Source, https://github.com/stefan.freitag/aws_fsx_lifecycle_status_monitor
+Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/setup.py` & `aws-fsx-lifecycle-status-monitor-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-fsx-lifecycle-status-monitor",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "aws_fsx_lifecycle_status_monitor",
     "license": "Apache-2.0",
     "url": "https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
-        "Source": "https://github.com/stefan.freitag/aws_fsx_lifecycle_status_monitor"
+        "Source": "https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "aws_fsx_lifecycle_status_monitor",
         "aws_fsx_lifecycle_status_monitor._jsii"
     ],
     "package_data": {
         "aws_fsx_lifecycle_status_monitor._jsii": [
-            "aws_fsx_lifecycle_status_monitor@0.0.5.jsii.tgz"
+            "aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz"
         ],
         "aws_fsx_lifecycle_status_monitor": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor/__init__.py` & `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.5
+Version: 0.0.6
 Summary: aws_fsx_lifecycle_status_monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
-Project-URL: Source, https://github.com/stefan.freitag/aws_fsx_lifecycle_status_monitor
+Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.5/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt` & `aws-fsx-lifecycle-status-monitor-0.0.6/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_fsx_lifecycle_status_monitor/py.typed
 src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
 src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
 src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
-src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.5.jsii.tgz
+src/aws_fsx_lifecycle_status_monitor/_jsii/aws_fsx_lifecycle_status_monitor@0.0.6.jsii.tgz
```

