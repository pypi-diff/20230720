# Comparing `tmp/im_data_manager_metadata-1.0.3-py3-none-any.whl.zip` & `tmp/im_data_manager_metadata-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 18668 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 15:52 data_manager_metadata/__init__.py
--rw-r--r--  2.0 unx     1942 b- defN 23-Jul-20 15:52 data_manager_metadata/annotation_utils.py
--rw-r--r--  2.0 unx    24263 b- defN 23-Jul-20 15:52 data_manager_metadata/data_tier_api.py
--rw-r--r--  2.0 unx     4004 b- defN 23-Jul-20 15:52 data_manager_metadata/exceptions.py
--rw-r--r--  2.0 unx    31629 b- defN 23-Jul-20 15:53 data_manager_metadata/metadata.py
--rw-r--r--  2.0 unx     1080 b- defN 23-Jul-20 15:53 im_data_manager_metadata-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4327 b- defN 23-Jul-20 15:53 im_data_manager_metadata-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 15:53 im_data_manager_metadata-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 15:53 im_data_manager_metadata-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 23-Jul-20 15:53 im_data_manager_metadata-1.0.3.dist-info/RECORD
-10 files, 68294 bytes uncompressed, 17038 bytes compressed:  75.1%
+Zip file size: 18673 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 16:14 data_manager_metadata/__init__.py
+-rw-r--r--  2.0 unx     1942 b- defN 23-Jul-20 16:14 data_manager_metadata/annotation_utils.py
+-rw-r--r--  2.0 unx    24263 b- defN 23-Jul-20 16:14 data_manager_metadata/data_tier_api.py
+-rw-r--r--  2.0 unx     4004 b- defN 23-Jul-20 16:14 data_manager_metadata/exceptions.py
+-rw-r--r--  2.0 unx    31629 b- defN 23-Jul-20 16:14 data_manager_metadata/metadata.py
+-rw-r--r--  2.0 unx     1080 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4328 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      935 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/RECORD
+10 files, 68295 bytes uncompressed, 17043 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: data_manager_metadata/exceptions.py
 Comment: 
 
 Filename: data_manager_metadata/metadata.py
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.3.dist-info/LICENSE
+Filename: im_data_manager_metadata-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.3.dist-info/METADATA
+Filename: im_data_manager_metadata-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.3.dist-info/WHEEL
+Filename: im_data_manager_metadata-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.3.dist-info/top_level.txt
+Filename: im_data_manager_metadata-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.3.dist-info/RECORD
+Filename: im_data_manager_metadata-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `im_data_manager_metadata-1.0.3.dist-info/LICENSE` & `im_data_manager_metadata-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `im_data_manager_metadata-1.0.3.dist-info/METADATA` & `im_data_manager_metadata-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: im-data-manager-metadata
-Version: 1.0.3
+Version: 1.0.4
 Summary: A framework for Informatics Matters dataset metadata
 Home-page: https://github.com/InformaticsMatters/squonk2-data-manager-metadata
 Author: Tim Dudgeon
 Author-email: tdudgeon@informaticsmatters.com
 License: MIT
 Keywords: jenkins
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3, <4
 License-File: LICENSE
 Requires-Dist: PyYAML (<7.0,>=6.0.1)
 Requires-Dist: jsonpickle (<3.0.0,>=2.0.0)
 Requires-Dist: im-data-manager-job-decoder (<2.0.0,>=1.17.2)
```

## Comparing `im_data_manager_metadata-1.0.3.dist-info/RECORD` & `im_data_manager_metadata-1.0.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 data_manager_metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_manager_metadata/annotation_utils.py,sha256=8DbTyMNC4za3bjVj5wb3bUGEh5-E3Plo0i7SgA1bR3c,1942
 data_manager_metadata/data_tier_api.py,sha256=zZBVGPG9UDCb88kdh-f37nm-U9bMAlNvHwW-bmP-xt0,24263
 data_manager_metadata/exceptions.py,sha256=_JsUyYP6uxYodV-0vFUw3ibY-TuxGY7dEIwgwASciew,4004
 data_manager_metadata/metadata.py,sha256=hyJuoHtC64s-LvbgGWHPv5bUAwZXzFm6YfTAhy3fhPE,31629
-im_data_manager_metadata-1.0.3.dist-info/LICENSE,sha256=aPo-a09Zp9KzKrL5Spr6s59gb3b4cro7mJ3igSBbqrQ,1080
-im_data_manager_metadata-1.0.3.dist-info/METADATA,sha256=WLpbiQ6jeiEzhxw7RZo5HNsXbHvhRnbqken5mIZttIU,4327
-im_data_manager_metadata-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-im_data_manager_metadata-1.0.3.dist-info/top_level.txt,sha256=ayBYnZrfzouPELqGB79YSQ0oyvL6RonH4kGerlGt5yk,22
-im_data_manager_metadata-1.0.3.dist-info/RECORD,,
+im_data_manager_metadata-1.0.4.dist-info/LICENSE,sha256=aPo-a09Zp9KzKrL5Spr6s59gb3b4cro7mJ3igSBbqrQ,1080
+im_data_manager_metadata-1.0.4.dist-info/METADATA,sha256=zT1NQm2flg3TpoBH9a9rY4UdDq8dGs50aqJhQ83b5pQ,4328
+im_data_manager_metadata-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+im_data_manager_metadata-1.0.4.dist-info/top_level.txt,sha256=ayBYnZrfzouPELqGB79YSQ0oyvL6RonH4kGerlGt5yk,22
+im_data_manager_metadata-1.0.4.dist-info/RECORD,,
```

