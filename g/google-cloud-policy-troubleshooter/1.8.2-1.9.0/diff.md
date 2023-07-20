# Comparing `tmp/google-cloud-policy-troubleshooter-1.8.2.tar.gz` & `tmp/google-cloud-policy-troubleshooter-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-policy-troubleshooter-1.8.2.tar", last modified: Wed Jul  5 15:54:36 2023, max compression
+gzip compressed data, was "google-cloud-policy-troubleshooter-1.9.0.tar", last modified: Thu Jul 20 19:30:50 2023, max compression
```

## Comparing `google-cloud-policy-troubleshooter-1.8.2.tar` & `google-cloud-policy-troubleshooter-1.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5226 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4277 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.655893 google-cloud-policy-troubleshooter-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.655893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/
--rw-rw-r--   0 root         (0)     1003     1506 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/
--rw-rw-r--   0 root         (0)     1003     1281 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1083 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/
--rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py
--rw-rw-r--   0 root         (0)     1003    12307 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py
--rw-rw-r--   0 root         (0)     1003    20942 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.659893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6117 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12044 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12254 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12240 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/
--rw-rw-r--   0 root         (0)     1003     1015 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3071 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/checker.py
--rw-rw-r--   0 root         (0)     1003    14093 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/explanations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/
--rw-r--r--   0 root         (0)     1003     5226 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1827 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:54:36.000000 google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3020 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:54:36.663893 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    59589 2023-07-05 15:46:59.000000 google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5226 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4277 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.395976 google-cloud-policy-troubleshooter-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.395976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter/
+-rw-rw-r--   0 root         (0)     1003     1506 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/
+-rw-rw-r--   0 root         (0)     1003     1281 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1083 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12367 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21002 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6117 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12050 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12260 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12240 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.399976 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1015 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3432 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/checker.py
+-rw-rw-r--   0 root         (0)     1003    14373 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/explanations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/
+-rw-r--r--   0 root         (0)     1003     5226 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1827 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-20 19:30:50.000000 google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3020 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:50.403975 google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/policytroubleshooter_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/policytroubleshooter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    59639 2023-07-20 19:27:31.000000 google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/LICENSE` & `google-cloud-policy-troubleshooter-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.2/MANIFEST.in` & `google-cloud-policy-troubleshooter-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.2/PKG-INFO` & `google-cloud-policy-troubleshooter-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-policy-troubleshooter
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Policy Troubleshooter API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/README.rst` & `google-cloud-policy-troubleshooter-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter/gapic_version.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_metadata.json` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/gapic_version.py` & `google-cloud-policy-troubleshooter-1.9.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -38,14 +38,16 @@
 from google.cloud.policytroubleshooter_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.rpc import status_pb2  # type: ignore
+
 from google.cloud.policytroubleshooter_v1.types import checker, explanations
 
 from .client import IamCheckerClient
 from .transports.base import DEFAULT_CLIENT_INFO, IamCheckerTransport
 from .transports.grpc_asyncio import IamCheckerGrpcAsyncIOTransport
 
 
@@ -212,17 +214,17 @@
         self,
         request: Optional[Union[checker.TroubleshootIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> checker.TroubleshootIamPolicyResponse:
-        r"""Checks whether a member has a specific permission for
-        a specific resource, and explains why the member does or
-        does not have that permission.
+        r"""Checks whether a principal has a specific permission
+        for a specific resource, and explains why the principal
+        does or does not have that permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -254,15 +256,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.policytroubleshooter_v1.types.TroubleshootIamPolicyResponse:
                 Response for
-                [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
+                   [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
 
         """
         # Create or coerce a protobuf request object.
         request = checker.TroubleshootIamPolicyRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,14 +42,16 @@
 from google.cloud.policytroubleshooter_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
+from google.rpc import status_pb2  # type: ignore
+
 from google.cloud.policytroubleshooter_v1.types import checker, explanations
 
 from .transports.base import DEFAULT_CLIENT_INFO, IamCheckerTransport
 from .transports.grpc import IamCheckerGrpcTransport
 from .transports.grpc_asyncio import IamCheckerGrpcAsyncIOTransport
 from .transports.rest import IamCheckerRestTransport
 
@@ -425,17 +427,17 @@
         self,
         request: Optional[Union[checker.TroubleshootIamPolicyRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> checker.TroubleshootIamPolicyResponse:
-        r"""Checks whether a member has a specific permission for
-        a specific resource, and explains why the member does or
-        does not have that permission.
+        r"""Checks whether a principal has a specific permission
+        for a specific resource, and explains why the principal
+        does or does not have that permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -467,15 +469,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.policytroubleshooter_v1.types.TroubleshootIamPolicyResponse:
                 Response for
-                [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
+                   [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a checker.TroubleshootIamPolicyRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -234,17 +234,17 @@
     def troubleshoot_iam_policy(
         self,
     ) -> Callable[
         [checker.TroubleshootIamPolicyRequest], checker.TroubleshootIamPolicyResponse
     ]:
         r"""Return a callable for the troubleshoot iam policy method over gRPC.
 
-        Checks whether a member has a specific permission for
-        a specific resource, and explains why the member does or
-        does not have that permission.
+        Checks whether a principal has a specific permission
+        for a specific resource, and explains why the principal
+        does or does not have that permission.
 
         Returns:
             Callable[[~.TroubleshootIamPolicyRequest],
                     ~.TroubleshootIamPolicyResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -238,17 +238,17 @@
         self,
     ) -> Callable[
         [checker.TroubleshootIamPolicyRequest],
         Awaitable[checker.TroubleshootIamPolicyResponse],
     ]:
         r"""Return a callable for the troubleshoot iam policy method over gRPC.
 
-        Checks whether a member has a specific permission for
-        a specific resource, and explains why the member does or
-        does not have that permission.
+        Checks whether a principal has a specific permission
+        for a specific resource, and explains why the principal
+        does or does not have that permission.
 
         Returns:
             Callable[[~.TroubleshootIamPolicyRequest],
                     Awaitable[~.TroubleshootIamPolicyResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/services/iam_checker/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/checker.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
+from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.policytroubleshooter_v1.types import explanations
 
 __protobuf__ = proto.module(
     package="google.cloud.policytroubleshooter.v1",
     manifest={
@@ -33,15 +34,15 @@
 class TroubleshootIamPolicyRequest(proto.Message):
     r"""Request for
     [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
 
     Attributes:
         access_tuple (google.cloud.policytroubleshooter_v1.types.AccessTuple):
             The information to use for checking whether a
-            member has a permission for a resource.
+            principal has a permission for a resource.
     """
 
     access_tuple: explanations.AccessTuple = proto.Field(
         proto.MESSAGE,
         number=1,
         message=explanations.AccessTuple,
     )
@@ -49,41 +50,49 @@
 
 class TroubleshootIamPolicyResponse(proto.Message):
     r"""Response for
     [TroubleshootIamPolicy][google.cloud.policytroubleshooter.v1.IamChecker.TroubleshootIamPolicy].
 
     Attributes:
         access (google.cloud.policytroubleshooter_v1.types.AccessState):
-            Indicates whether the member has the
+            Indicates whether the principal has the
             specified permission for the specified resource,
             based on evaluating all of the applicable IAM
             policies.
         explained_policies (MutableSequence[google.cloud.policytroubleshooter_v1.types.ExplainedPolicy]):
             List of IAM policies that were evaluated to
-            check the member's permissions, with annotations
-            to indicate how each policy contributed to the
-            final result.
+            check the principal's permissions, with
+            annotations to indicate how each policy
+            contributed to the final result.
 
             The list of policies can include the policy for
             the resource itself. It can also include
             policies that are inherited from higher levels
             of the resource hierarchy, including the
             organization, the folder, and the project.
             To learn more about the resource hierarchy, see
             https://cloud.google.com/iam/help/resource-hierarchy.
+        errors (MutableSequence[google.rpc.status_pb2.Status]):
+            The general errors contained in the
+            troubleshooting response.
     """
 
     access: explanations.AccessState = proto.Field(
         proto.ENUM,
         number=1,
         enum=explanations.AccessState,
     )
     explained_policies: MutableSequence[
         explanations.ExplainedPolicy
     ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=explanations.ExplainedPolicy,
     )
+    errors: MutableSequence[status_pb2.Status] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=3,
+        message=status_pb2.Status,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google/cloud/policytroubleshooter_v1/types/explanations.py` & `google-cloud-policy-troubleshooter-1.9.0/google/cloud/policytroubleshooter_v1/types/explanations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,45 +30,46 @@
         "ExplainedPolicy",
         "BindingExplanation",
     },
 )
 
 
 class AccessState(proto.Enum):
-    r"""Whether a member has a permission for a resource.
+    r"""Whether a principal has a permission for a resource.
 
     Values:
         ACCESS_STATE_UNSPECIFIED (0):
-            Reserved for future use.
+            Default value. This value is unused.
         GRANTED (1):
-            The member has the permission.
+            The principal has the permission.
         NOT_GRANTED (2):
-            The member does not have the permission.
+            The principal does not have the permission.
         UNKNOWN_CONDITIONAL (3):
-            The member has the permission only if a condition expression
-            evaluates to ``true``.
+            The principal has the permission only if a condition
+            expression evaluates to ``true``.
         UNKNOWN_INFO_DENIED (4):
             The sender of the request does not have
             access to all of the policies that Policy
             Troubleshooter needs to evaluate.
     """
     ACCESS_STATE_UNSPECIFIED = 0
     GRANTED = 1
     NOT_GRANTED = 2
     UNKNOWN_CONDITIONAL = 3
     UNKNOWN_INFO_DENIED = 4
 
 
 class HeuristicRelevance(proto.Enum):
-    r"""The extent to which a single data point contributes to an
-    overall determination.
+    r"""The extent to which a single data point, such as the
+    existence of a binding or whether a binding includes a specific
+    principal, contributes to an overall determination.
 
     Values:
         HEURISTIC_RELEVANCE_UNSPECIFIED (0):
-            Reserved for future use.
+            Default value. This value is unused.
         NORMAL (1):
             The data point has a limited effect on the
             result. Changing the data point is unlikely to
             affect the overall determination.
         HIGH (2):
             The data point has a strong effect on the
             result. Changing the data point is likely to
@@ -76,37 +77,38 @@
     """
     HEURISTIC_RELEVANCE_UNSPECIFIED = 0
     NORMAL = 1
     HIGH = 2
 
 
 class AccessTuple(proto.Message):
-    r"""Information about the member, resource, and permission to
+    r"""Information about the principal, resource, and permission to
     check.
 
     Attributes:
         principal (str):
-            Required. The member, or principal, whose access you want to
-            check, in the form of the email address that represents that
-            member. For example, ``alice@example.com`` or
+            Required. The principal whose access you want to check, in
+            the form of the email address that represents that
+            principal. For example, ``alice@example.com`` or
             ``my-service-account@my-project.iam.gserviceaccount.com``.
 
-            The member must be a Google Account or a service account.
-            Other types of members are not supported.
+            The principal must be a Google Account or a service account.
+            Other types of principals are not supported.
         full_resource_name (str):
             Required. The full resource name that identifies the
             resource. For example,
             ``//compute.googleapis.com/projects/my-project/zones/us-central1-a/instances/my-instance``.
 
             For examples of full resource names for Google Cloud
             services, see
             https://cloud.google.com/iam/help/troubleshooter/full-resource-names.
         permission (str):
             Required. The IAM permission to check for the
-            specified member and resource.
+            specified principal and resource.
+
             For a complete list of IAM permissions, see
             https://cloud.google.com/iam/help/permissions/reference.
             For a complete list of predefined IAM roles and
             the permissions in each role, see
             https://cloud.google.com/iam/help/roles/reference.
     """
 
@@ -127,22 +129,22 @@
 class ExplainedPolicy(proto.Message):
     r"""Details about how a specific IAM [Policy][google.iam.v1.Policy]
     contributed to the access check.
 
     Attributes:
         access (google.cloud.policytroubleshooter_v1.types.AccessState):
             Indicates whether *this policy* provides the specified
-            permission to the specified member for the specified
+            permission to the specified principal for the specified
             resource.
 
-            This field does *not* indicate whether the member actually
-            has the permission for the resource. There might be another
-            policy that overrides this policy. To determine whether the
-            member actually has the permission, use the ``access`` field
-            in the
+            This field does *not* indicate whether the principal
+            actually has the permission for the resource. There might be
+            another policy that overrides this policy. To determine
+            whether the principal actually has the permission, use the
+            ``access`` field in the
             [TroubleshootIamPolicyResponse][IamChecker.TroubleshootIamPolicyResponse].
         full_resource_name (str):
             The full resource name that identifies the resource. For
             example,
             ``//compute.googleapis.com/projects/my-project/zones/us-central1-a/instances/my-instance``.
 
             If the sender of the request does not have access to the
@@ -153,16 +155,16 @@
             https://cloud.google.com/iam/help/troubleshooter/full-resource-names.
         policy (google.iam.v1.policy_pb2.Policy):
             The IAM policy attached to the resource.
             If the sender of the request does not have
             access to the policy, this field is empty.
         binding_explanations (MutableSequence[google.cloud.policytroubleshooter_v1.types.BindingExplanation]):
             Details about how each binding in the policy
-            affects the member's ability, or inability, to
-            use the permission for the resource.
+            affects the principal's ability, or inability,
+            to use the permission for the resource.
             If the sender of the request does not have
             access to the policy, this field is omitted.
         relevance (google.cloud.policytroubleshooter_v1.types.HeuristicRelevance):
             The relevance of this policy to the overall determination in
             the
             [TroubleshootIamPolicyResponse][IamChecker.TroubleshootIamPolicyResponse].
 
@@ -193,28 +195,28 @@
         proto.ENUM,
         number=5,
         enum="HeuristicRelevance",
     )
 
 
 class BindingExplanation(proto.Message):
-    r"""Details about how a binding in a policy affects a member's
+    r"""Details about how a binding in a policy affects a principal's
     ability to use a permission.
 
     Attributes:
         access (google.cloud.policytroubleshooter_v1.types.AccessState):
             Required. Indicates whether *this binding* provides the
-            specified permission to the specified member for the
+            specified permission to the specified principal for the
             specified resource.
 
-            This field does *not* indicate whether the member actually
-            has the permission for the resource. There might be another
-            binding that overrides this binding. To determine whether
-            the member actually has the permission, use the ``access``
-            field in the
+            This field does *not* indicate whether the principal
+            actually has the permission for the resource. There might be
+            another binding that overrides this binding. To determine
+            whether the principal actually has the permission, use the
+            ``access`` field in the
             [TroubleshootIamPolicyResponse][IamChecker.TroubleshootIamPolicyResponse].
         role (str):
             The role that this binding grants. For example,
             ``roles/compute.serviceAgent``.
 
             For a complete list of predefined IAM roles, as well as the
             permissions in each role, see
@@ -223,108 +225,108 @@
             Indicates whether the role granted by this
             binding contains the specified permission.
         role_permission_relevance (google.cloud.policytroubleshooter_v1.types.HeuristicRelevance):
             The relevance of the permission's existence,
             or nonexistence, in the role to the overall
             determination for the entire policy.
         memberships (MutableMapping[str, google.cloud.policytroubleshooter_v1.types.BindingExplanation.AnnotatedMembership]):
-            Indicates whether each member in the binding includes the
-            member specified in the request, either directly or
-            indirectly. Each key identifies a member in the binding, and
-            each value indicates whether the member in the binding
-            includes the member in the request.
+            Indicates whether each principal in the binding includes the
+            principal specified in the request, either directly or
+            indirectly. Each key identifies a principal in the binding,
+            and each value indicates whether the principal in the
+            binding includes the principal in the request.
 
             For example, suppose that a binding includes the following
-            members:
+            principals:
 
             -  ``user:alice@example.com``
             -  ``group:product-eng@example.com``
 
             You want to troubleshoot access for
-            ``user:bob@example.com``. This user is a member of the group
-            ``group:product-eng@example.com``.
+            ``user:bob@example.com``. This user is a principal of the
+            group ``group:product-eng@example.com``.
 
-            For the first member in the binding, the key is
+            For the first principal in the binding, the key is
             ``user:alice@example.com``, and the ``membership`` field in
             the value is set to ``MEMBERSHIP_NOT_INCLUDED``.
 
-            For the second member in the binding, the key is
+            For the second principal in the binding, the key is
             ``group:product-eng@example.com``, and the ``membership``
             field in the value is set to ``MEMBERSHIP_INCLUDED``.
         relevance (google.cloud.policytroubleshooter_v1.types.HeuristicRelevance):
             The relevance of this binding to the overall
             determination for the entire policy.
         condition (google.type.expr_pb2.Expr):
-            A condition expression that prevents access unless the
-            expression evaluates to ``true``.
+            A condition expression that prevents this binding from
+            granting access unless the expression evaluates to ``true``.
 
             To learn about IAM Conditions, see
-            http://cloud.google.com/iam/help/conditions/overview.
+            https://cloud.google.com/iam/help/conditions/overview.
     """
 
     class RolePermission(proto.Enum):
         r"""Whether a role includes a specific permission.
 
         Values:
             ROLE_PERMISSION_UNSPECIFIED (0):
-                Reserved for future use.
+                Default value. This value is unused.
             ROLE_PERMISSION_INCLUDED (1):
                 The permission is included in the role.
             ROLE_PERMISSION_NOT_INCLUDED (2):
                 The permission is not included in the role.
             ROLE_PERMISSION_UNKNOWN_INFO_DENIED (3):
                 The sender of the request is not allowed to
                 access the binding.
         """
         ROLE_PERMISSION_UNSPECIFIED = 0
         ROLE_PERMISSION_INCLUDED = 1
         ROLE_PERMISSION_NOT_INCLUDED = 2
         ROLE_PERMISSION_UNKNOWN_INFO_DENIED = 3
 
     class Membership(proto.Enum):
-        r"""Whether the binding includes the member.
+        r"""Whether the binding includes the principal.
 
         Values:
             MEMBERSHIP_UNSPECIFIED (0):
-                Reserved for future use.
+                Default value. This value is unused.
             MEMBERSHIP_INCLUDED (1):
-                The binding includes the member. The member can be included
-                directly or indirectly. For example:
+                The binding includes the principal. The principal can be
+                included directly or indirectly. For example:
 
-                -  A member is included directly if that member is listed in
-                   the binding.
-                -  A member is included indirectly if that member is in a
-                   Google group or G Suite domain that is listed in the
-                   binding.
+                -  A principal is included directly if that principal is
+                   listed in the binding.
+                -  A principal is included indirectly if that principal is
+                   in a Google group or Google Workspace domain that is
+                   listed in the binding.
             MEMBERSHIP_NOT_INCLUDED (2):
-                The binding does not include the member.
+                The binding does not include the principal.
             MEMBERSHIP_UNKNOWN_INFO_DENIED (3):
                 The sender of the request is not allowed to
                 access the binding.
             MEMBERSHIP_UNKNOWN_UNSUPPORTED (4):
-                The member is an unsupported type. Only
+                The principal is an unsupported type. Only
                 Google Accounts and service accounts are
                 supported.
         """
         MEMBERSHIP_UNSPECIFIED = 0
         MEMBERSHIP_INCLUDED = 1
         MEMBERSHIP_NOT_INCLUDED = 2
         MEMBERSHIP_UNKNOWN_INFO_DENIED = 3
         MEMBERSHIP_UNKNOWN_UNSUPPORTED = 4
 
     class AnnotatedMembership(proto.Message):
-        r"""Details about whether the binding includes the member.
+        r"""Details about whether the binding includes the principal.
 
         Attributes:
             membership (google.cloud.policytroubleshooter_v1.types.BindingExplanation.Membership):
                 Indicates whether the binding includes the
-                member.
+                principal.
             relevance (google.cloud.policytroubleshooter_v1.types.HeuristicRelevance):
-                The relevance of the member's status to the
-                overall determination for the binding.
+                The relevance of the principal's status to
+                the overall determination for the binding.
         """
 
         membership: "BindingExplanation.Membership" = proto.Field(
             proto.ENUM,
             number=1,
             enum="BindingExplanation.Membership",
         )
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/PKG-INFO` & `google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-policy-troubleshooter
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Policy Troubleshooter API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt` & `google-cloud-policy-troubleshooter-1.9.0/google_cloud_policy_troubleshooter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-policy-troubleshooter-1.8.2/setup.py` & `google-cloud-policy-troubleshooter-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/tests/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/tests/unit/__init__.py` & `google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/policytroubleshooter_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-policy-troubleshooter-1.8.2/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py` & `google-cloud-policy-troubleshooter-1.9.0/tests/unit/gapic/policytroubleshooter_v1/test_iam_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,14 +30,15 @@
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.oauth2 import service_account
 from google.protobuf import json_format
+from google.rpc import status_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
```

