# Comparing `tmp/indico_plugins-3.2.1-py3-none-any.whl.zip` & `tmp/indico_plugins-3.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1713 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2084 b- defN 23-May-26 14:23 indico_plugins-3.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:23 indico_plugins-3.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 14:23 indico_plugins-3.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      325 b- defN 23-May-26 14:23 indico_plugins-3.2.1.dist-info/RECORD
-4 files, 2502 bytes uncompressed, 1075 bytes compressed:  57.0%
+Zip file size: 1730 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2155 b- defN 23-Jul-20 19:35 indico_plugins-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:35 indico_plugins-3.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-20 19:35 indico_plugins-3.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      325 b- defN 23-Jul-20 19:35 indico_plugins-3.2.2.dist-info/RECORD
+4 files, 2573 bytes uncompressed, 1092 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: indico_plugins-3.2.1.dist-info/METADATA
+Filename: indico_plugins-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugins-3.2.1.dist-info/WHEEL
+Filename: indico_plugins-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugins-3.2.1.dist-info/top_level.txt
+Filename: indico_plugins-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugins-3.2.1.dist-info/RECORD
+Filename: indico_plugins-3.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `indico_plugins-3.2.1.dist-info/METADATA` & `indico_plugins-3.2.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: indico-plugins
-Version: 3.2.1
+Version: 3.2.2
 Summary: A meta-package containing the official Indico plugins
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
-Requires-Dist: indico (>=3.2)
-Requires-Dist: indico-plugin-citadel (<3.3.dev0,>=3.2.1)
-Requires-Dist: indico-plugin-cloud-captchas (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-livesync (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-owncloud (<3.3.dev0,>=3.2.1)
-Requires-Dist: indico-plugin-payment-manual (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-payment-paypal (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-payment-sixpay (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-piwik (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-previewer-code (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-previewer-jupyter (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-prometheus (<3.3.dev0,>=3.2)
-Requires-Dist: indico-plugin-storage-s3 (<3.3.dev0,>=3.2.1)
-Requires-Dist: indico-plugin-ursh (<3.3.dev0,>=3.2.1)
-Requires-Dist: indico-plugin-vc-zoom (<3.3.dev0,>=3.2.2)
+Requires-Dist: indico (>=3.2.6)
+Requires-Dist: indico-plugin-citadel (<3.3.dev0,>=3.2.2)
+Requires-Dist: indico-plugin-cloud-captchas (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-livesync (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-owncloud (<3.3.dev0,>=3.2.2)
+Requires-Dist: indico-plugin-payment-manual (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-payment-paypal (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-payment-sixpay (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-piwik (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-previewer-code (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-previewer-jupyter (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-prometheus (<3.3.dev0,>=3.2.1)
+Requires-Dist: indico-plugin-storage-s3 (<3.3.dev0,>=3.2.2)
+Requires-Dist: indico-plugin-ursh (<3.3.dev0,>=3.2.2)
+Requires-Dist: indico-plugin-vc-zoom (<3.3.dev0,>=3.2.4)
 
 # Official Indico Plugins
 
 This package is a meta-package that installs the most common Indico plugins
 that are developed by the core Indico development team.
 
 It does not have any functionality by itself; its sole purpose is to provide
```

