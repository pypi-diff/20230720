# Comparing `tmp/indico_plugin_storage_s3-3.2.1-py3-none-any.whl.zip` & `tmp/indico_plugin_storage_s3-3.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20071 bytes, number of entries: 13
--rw-r--r--  2.0 unx      484 b- defN 23-Jan-08 16:35 indico_storage_s3/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jan-08 16:35 indico_storage_s3/blueprint.py
--rw-r--r--  2.0 unx     2717 b- defN 23-Apr-18 21:21 indico_storage_s3/controllers.py
--rw-r--r--  2.0 unx    22823 b- defN 23-Jan-08 16:35 indico_storage_s3/migrate.py
--rw-r--r--  2.0 unx     4568 b- defN 23-Jan-08 16:35 indico_storage_s3/plugin.py
--rw-r--r--  2.0 unx    11348 b- defN 23-May-02 13:41 indico_storage_s3/storage.py
--rw-r--r--  2.0 unx     1710 b- defN 23-Jan-08 16:35 indico_storage_s3/task.py
--rw-r--r--  2.0 unx      722 b- defN 23-May-02 13:41 indico_storage_s3/util.py
--rw-r--r--  2.0 unx     7665 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1157 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/RECORD
-13 files, 53871 bytes uncompressed, 18107 bytes compressed:  66.4%
+Zip file size: 20093 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      484 b- defN 23-Jun-01 10:35 indico_storage_s3/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-01 10:35 indico_storage_s3/blueprint.py
+-rw-r--r--  2.0 unx     2717 b- defN 23-Jun-01 10:35 indico_storage_s3/controllers.py
+-rw-r--r--  2.0 unx    22823 b- defN 23-Jun-01 10:35 indico_storage_s3/migrate.py
+-rw-r--r--  2.0 unx     4568 b- defN 23-Jun-01 10:35 indico_storage_s3/plugin.py
+-rw-r--r--  2.0 unx    11348 b- defN 23-Jun-01 10:35 indico_storage_s3/storage.py
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-01 10:35 indico_storage_s3/task.py
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-01 10:35 indico_storage_s3/util.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-Jul-20 19:36 indico_plugin_storage_s3-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:36 indico_plugin_storage_s3-3.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-20 19:36 indico_plugin_storage_s3-3.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-20 19:36 indico_plugin_storage_s3-3.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1157 b- defN 23-Jul-20 19:36 indico_plugin_storage_s3-3.2.2.dist-info/RECORD
+13 files, 53956 bytes uncompressed, 18129 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: indico_storage_s3/task.py
 Comment: 
 
 Filename: indico_storage_s3/util.py
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.1.dist-info/METADATA
+Filename: indico_plugin_storage_s3-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.1.dist-info/WHEEL
+Filename: indico_plugin_storage_s3-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt
+Filename: indico_plugin_storage_s3-3.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt
+Filename: indico_plugin_storage_s3-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.1.dist-info/RECORD
+Filename: indico_plugin_storage_s3-3.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `indico_plugin_storage_s3-3.2.1.dist-info/METADATA` & `indico_plugin_storage_s3-3.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: indico-plugin-storage-s3
-Version: 3.2.1
+Version: 3.2.2
 Summary: S3 storage backend for Indico
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.9.0
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: indico (>=3.2)
 Requires-Dist: boto3 (<2.0,>=1.20.51)
 
 # S3 Storage Plugin
 
 The S3 storage plugin allows Indico to store materials etc. on [Amazon S3][amazon-s3] or
@@ -29,14 +30,18 @@
 
 It is currently used in production on multiple Indico instances, so we believe it is
 stable, but please be advised that we do not provide a way to move files back from S3
 to local storage (but it would of course be possible to write a script for this).
 
 ## Changelog
 
+### 3.2.2
+
+- Support Python 3.11
+
 ### 3.2.1
 
 - Stop using deprecated URL utils from werkzeug
 
 ### 3.2
 
 - Update translations
```

## Comparing `indico_plugin_storage_s3-3.2.1.dist-info/RECORD` & `indico_plugin_storage_s3-3.2.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 indico_storage_s3/blueprint.py,sha256=EqIG8VcrnABsds3PNVybE0mY6rwSHjDh02f0UihMbkY,496
 indico_storage_s3/controllers.py,sha256=nYxqHsJESuVzXzPupBPQb7bofek1mZ7OfDj5pMpNmsg,2717
 indico_storage_s3/migrate.py,sha256=Izla22EGd40_BF8Du_U0PnA6z33WqtWNDznY31gSOWA,22823
 indico_storage_s3/plugin.py,sha256=-Mk44tiQpjbOZSH-Q-xdAYR5YeubgeLhxsH_1emHhBg,4568
 indico_storage_s3/storage.py,sha256=VNuMxPD7kAiCoGQIkCxDvX02qVCmhCuE7FN9GTC-Dto,11348
 indico_storage_s3/task.py,sha256=O7o1-072NVl0JETMALehQ-PkTQF80y11gUaLyYfDnxY,1710
 indico_storage_s3/util.py,sha256=JwSbpGqwj-ownX9t2YYh17xk-KyjTIrFnpyjDS6-8vA,722
-indico_plugin_storage_s3-3.2.1.dist-info/METADATA,sha256=GLxX0YF8jDzBot2qdP9DVB1fuJLpWHXly6ePLMkR7KI,7665
-indico_plugin_storage_s3-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt,sha256=rts2AI5QEK9cu2WcFujOUCUtP9YMiABEMTQ-dkafx4Y,71
-indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt,sha256=wMajir5p9AELlngQV8mOHyzu5xWvybvbG0rJg-YsQpM,18
-indico_plugin_storage_s3-3.2.1.dist-info/RECORD,,
+indico_plugin_storage_s3-3.2.2.dist-info/METADATA,sha256=NbZZ-Dqn6KucMI9o6JWDKL9sFagcmpUi9pYmG5oBqC4,7750
+indico_plugin_storage_s3-3.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_storage_s3-3.2.2.dist-info/entry_points.txt,sha256=rts2AI5QEK9cu2WcFujOUCUtP9YMiABEMTQ-dkafx4Y,71
+indico_plugin_storage_s3-3.2.2.dist-info/top_level.txt,sha256=wMajir5p9AELlngQV8mOHyzu5xWvybvbG0rJg-YsQpM,18
+indico_plugin_storage_s3-3.2.2.dist-info/RECORD,,
```

