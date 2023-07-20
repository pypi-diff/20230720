# Comparing `tmp/cdk-rds-dump-1.2.5.tar.gz` & `tmp/cdk-rds-dump-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.2.5.tar", last modified: Wed Jul 19 01:04:04 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.6.tar", last modified: Thu Jul 20 09:26:03 2023, max compression
```

## Comparing `cdk-rds-dump-1.2.5.tar` & `cdk-rds-dump-1.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:04:04.224904 cdk-rds-dump-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-19 01:04:04.224904 cdk-rds-dump-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 01:04:04.224904 cdk-rds-dump-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:04:04.220904 cdk-rds-dump-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:04:04.220904 cdk-rds-dump-1.2.5/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:04:04.220904 cdk-rds-dump-1.2.5/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2576430 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 01:03:49.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:04:04.220904 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-19 01:04:04.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-19 01:04:04.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 01:04:04.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 01:04:04.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 01:04:04.000000 cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2575769 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.2.5/LICENSE` & `cdk-rds-dump-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.5/PKG-INFO` & `cdk-rds-dump-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.5
+Version: 1.2.6
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-1.2.5/README.md` & `cdk-rds-dump-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.5/setup.py` & `cdk-rds-dump-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.2.5",
+    "version": "1.2.6",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@1.2.5.jsii.tgz"
+            "cdk-rds-dump@1.2.6.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.2.5/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-1.2.6/src/cdk_rds_dump/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.5/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.5
+Version: 1.2.6
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

