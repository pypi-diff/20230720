# Comparing `tmp/cloudimized-1.3.5rc1.tar.gz` & `tmp/cloudimized-1.3.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudimized-1.3.5rc1.tar", last modified: Tue Jun 13 09:57:34 2023, max compression
+gzip compressed data, was "cloudimized-1.3.6rc1.tar", last modified: Thu Jul 20 09:09:08 2023, max compression
```

## Comparing `cloudimized-1.3.5rc1.tar` & `cloudimized-1.3.6rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.224938 cloudimized-1.3.5rc1/cloudimized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/cloudimized/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/changeprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/jiranotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/core/slacknotifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/cloudimized/gcpcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gcpcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpchangelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpservicequery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/cloudimized/gitcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gitcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gitcore/gitchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/gitcore/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/cloudimized/tfcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/tfcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/tfcore/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/cloudimized/tfcore/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:57:34.224938 cloudimized-1.3.5rc1/cloudimized.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:57:34.000000 cloudimized-1.3.5rc1/cloudimized.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 09:57:34.228938 cloudimized-1.3.5rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-13 09:57:29.000000 cloudimized-1.3.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/changeprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/jiranotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/slacknotifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/gcpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpchangelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpservicequery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/gitcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/gitchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/tfcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/setup.py
```

### Comparing `cloudimized-1.3.5rc1/LICENSE` & `cloudimized-1.3.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/PKG-INFO` & `cloudimized-1.3.6rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudimized
-Version: 1.3.5rc1
+Version: 1.3.6rc1
 Summary: Google Cloud Platform (GCP) configuration scanning tool
 Home-page: https://github.com/egnyte/cloudimized
 Author: Egnyte and Contributors
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudimized-1.3.5rc1/README.md` & `cloudimized-1.3.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/core/changeprocessor.py` & `cloudimized-1.3.6rc1/cloudimized/core/changeprocessor.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/core/core.py` & `cloudimized-1.3.6rc1/cloudimized/core/core.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/core/jiranotifier.py` & `cloudimized-1.3.6rc1/cloudimized/core/jiranotifier.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/core/result.py` & `cloudimized-1.3.6rc1/cloudimized/core/result.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/core/slacknotifier.py` & `cloudimized-1.3.6rc1/cloudimized/core/slacknotifier.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpchangelog.py` & `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpchangelog.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpquery.py` & `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpquery.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/gcpcore/gcpservicequery.py` & `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpservicequery.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/gitcore/gitchange.py` & `cloudimized-1.3.6rc1/cloudimized/gitcore/gitchange.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/gitcore/repo.py` & `cloudimized-1.3.6rc1/cloudimized/gitcore/repo.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/tfcore/query.py` & `cloudimized-1.3.6rc1/cloudimized/tfcore/query.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized/tfcore/run.py` & `cloudimized-1.3.6rc1/cloudimized/tfcore/run.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized.egg-info/PKG-INFO` & `cloudimized-1.3.6rc1/cloudimized.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudimized
-Version: 1.3.5rc1
+Version: 1.3.6rc1
 Summary: Google Cloud Platform (GCP) configuration scanning tool
 Home-page: https://github.com/egnyte/cloudimized
 Author: Egnyte and Contributors
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudimized-1.3.5rc1/cloudimized.egg-info/SOURCES.txt` & `cloudimized-1.3.6rc1/cloudimized.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.5rc1/cloudimized.egg-info/requires.txt` & `cloudimized-1.3.6rc1/cloudimized.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 cachetools==4.2.4
 certifi==2022.12.7
 cffi==1.15.0
 charset-normalizer==2.0.9
-cryptography==41.0.0
+cryptography==41.0.2
 defusedxml==0.7.1
 flatdict==4.0.1
 gitdb==4.0.9
 GitPython==3.1.30
 google-api-core==2.3.2
 google-api-python-client==2.33.0
 google-auth==2.3.3
 google-auth-httplib2==0.1.0
 google-cloud-appengine-logging==1.1.0
 google-cloud-audit-log==0.2.0
 google-cloud-core==2.2.1
 google-cloud-logging==2.7.0
 googleapis-common-protos==1.54.0
 grpc-google-iam-v1==0.12.3
-grpcio==1.43.0
+grpcio==1.53.0
 grpcio-status==1.43.0
 httplib2==0.20.2
 idna==3.3
 importlib-metadata==4.11.2
 jeepney==0.7.1
 jira==3.1.1
 keyring==23.5.0
```

### Comparing `cloudimized-1.3.5rc1/setup.py` & `cloudimized-1.3.6rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with codecs.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="cloudimized",
-    version="1.3.5rc1",
+    version="1.3.6rc1",
     description='Google Cloud Platform (GCP) configuration scanning tool',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/egnyte/cloudimized",
     author="Egnyte and Contributors",
     classifiers=[
         "Programming Language :: Python :: 3.7",
@@ -32,30 +32,30 @@
     },
     include_package_data=True,
     install_requires=[
         'cachetools==4.2.4',
         'certifi==2022.12.7',
         'cffi==1.15.0',
         'charset-normalizer==2.0.9',
-        'cryptography==41.0.0',
+        'cryptography==41.0.2',
         'defusedxml==0.7.1',
         'flatdict==4.0.1',
         'gitdb==4.0.9',
         'GitPython==3.1.30',
         'google-api-core==2.3.2',
         'google-api-python-client==2.33.0',
         'google-auth==2.3.3',
         'google-auth-httplib2==0.1.0',
         'google-cloud-appengine-logging==1.1.0',
         'google-cloud-audit-log==0.2.0',
         'google-cloud-core==2.2.1',
         'google-cloud-logging==2.7.0',
         'googleapis-common-protos==1.54.0',
         'grpc-google-iam-v1==0.12.3',
-        'grpcio==1.43.0',
+        'grpcio==1.53.0',
         'grpcio-status==1.43.0',
         'httplib2==0.20.2',
         'idna==3.3',
         'importlib-metadata==4.11.2',
         'jeepney==0.7.1',
         'jira==3.1.1',
         'keyring==23.5.0',
```

