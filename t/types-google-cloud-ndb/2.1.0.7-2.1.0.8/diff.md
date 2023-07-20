# Comparing `tmp/types-google-cloud-ndb-2.1.0.7.tar.gz` & `tmp/types-google-cloud-ndb-2.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-google-cloud-ndb-2.1.0.7.tar", last modified: Wed May 10 15:22:36 2023, max compression
+gzip compressed data, was "types-google-cloud-ndb-2.1.0.8.tar", last modified: Thu Jul 20 15:20:25 2023, max compression
```

## Comparing `types-google-cloud-ndb-2.1.0.7.tar` & `types-google-cloud-ndb-2.1.0.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.677130 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_batch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_eventloop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_options.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/blobstore.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/django_middleware.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/global_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/msgprop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/polymodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/tasklets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.700237 types-google-cloud-ndb-2.1.0.8/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.700237 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.704238 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_eventloop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/blobstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/django_middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/global_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/msgprop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/polymodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/tasklets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.704238 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/top_level.txt
```

### Comparing `types-google-cloud-ndb-2.1.0.7/CHANGELOG.md` & `types-google-cloud-ndb-2.1.0.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.1.0.8 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.1.0.7 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 2.1.0.6 (2023-04-04)
 
 `google-cloud-ndb`, `paramiko`, `setuptools`: remove unnecessary `= ...`s (#10011)
```

### Comparing `types-google-cloud-ndb-2.1.0.7/PKG-INFO` & `types-google-cloud-ndb-2.1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.7
+Version: 2.1.0.8
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/__init__.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_cache.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_query.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_query.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_eventloop.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_eventloop.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_transaction.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/blobstore.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/blobstore.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/client.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/context.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/context.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/exceptions.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/global_cache.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/global_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/key.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/key.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/metadata.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/metadata.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/model.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/model.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/query.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/query.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/stats.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/stats.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/tasklets.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/tasklets.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/utils.pyi` & `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.7/setup.py` & `types-google-cloud-ndb-2.1.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.0.7",
+      version="2.1.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['google-stubs'],
-      package_data={'google-stubs': ['cloud/ndb/__init__.pyi', 'cloud/ndb/_batch.pyi', 'cloud/ndb/_cache.pyi', 'cloud/ndb/_datastore_api.pyi', 'cloud/ndb/_datastore_query.pyi', 'cloud/ndb/_eventloop.pyi', 'cloud/ndb/_options.pyi', 'cloud/ndb/_transaction.pyi', 'cloud/ndb/blobstore.pyi', 'cloud/ndb/client.pyi', 'cloud/ndb/context.pyi', 'cloud/ndb/django_middleware.pyi', 'cloud/ndb/exceptions.pyi', 'cloud/ndb/global_cache.pyi', 'cloud/ndb/key.pyi', 'cloud/ndb/metadata.pyi', 'cloud/ndb/model.pyi', 'cloud/ndb/msgprop.pyi', 'cloud/ndb/polymodel.pyi', 'cloud/ndb/query.pyi', 'cloud/ndb/stats.pyi', 'cloud/ndb/tasklets.pyi', 'cloud/ndb/utils.pyi', 'METADATA.toml']},
+      package_data={'google-stubs': ['cloud/ndb/__init__.pyi', 'cloud/ndb/_batch.pyi', 'cloud/ndb/_cache.pyi', 'cloud/ndb/_datastore_api.pyi', 'cloud/ndb/_datastore_query.pyi', 'cloud/ndb/_eventloop.pyi', 'cloud/ndb/_options.pyi', 'cloud/ndb/_transaction.pyi', 'cloud/ndb/blobstore.pyi', 'cloud/ndb/client.pyi', 'cloud/ndb/context.pyi', 'cloud/ndb/django_middleware.pyi', 'cloud/ndb/exceptions.pyi', 'cloud/ndb/global_cache.pyi', 'cloud/ndb/key.pyi', 'cloud/ndb/metadata.pyi', 'cloud/ndb/model.pyi', 'cloud/ndb/msgprop.pyi', 'cloud/ndb/polymodel.pyi', 'cloud/ndb/query.pyi', 'cloud/ndb/stats.pyi', 'cloud/ndb/tasklets.pyi', 'cloud/ndb/utils.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/PKG-INFO` & `types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.7
+Version: 2.1.0.8
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/SOURCES.txt` & `types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

