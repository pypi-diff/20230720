# Comparing `tmp/idbadapter-1.9.1.tar.gz` & `tmp/idbadapter-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.1.tar", last modified: Wed Jul 19 12:49:53 2023, max compression
+gzip compressed data, was "idbadapter-1.9.2.tar", last modified: Wed Jul 19 12:59:25 2023, max compression
```

## Comparing `idbadapter-1.9.1.tar` & `idbadapter-1.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.165595 idbadapter-1.9.1/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.1/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-19 12:49:53.165595 idbadapter-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.148597 idbadapter-1.9.1/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.1/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    11816 2023-07-19 12:47:26.000000 idbadapter-1.9.1/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:49:53.163596 idbadapter-1.9.1/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 12:49:53.000000 idbadapter-1.9.1/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 12:49:53.166595 idbadapter-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-19 12:49:49.000000 idbadapter-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:59:25.552217 idbadapter-1.9.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-19 12:59:25.553214 idbadapter-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 12:59:25.536247 idbadapter-1.9.2/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.2/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11823 2023-07-19 12:58:54.000000 idbadapter-1.9.2/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:59:25.551212 idbadapter-1.9.2/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-19 12:59:25.000000 idbadapter-1.9.2/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-19 12:59:25.000000 idbadapter-1.9.2/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:59:25.000000 idbadapter-1.9.2/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 12:59:25.000000 idbadapter-1.9.2/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 12:59:25.000000 idbadapter-1.9.2/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:59:25.554212 idbadapter-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-19 12:59:08.000000 idbadapter-1.9.2/setup.py
```

### Comparing `idbadapter-1.9.1/LICENSE` & `idbadapter-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.1/PKG-INFO` & `idbadapter-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.1
+Version: 1.9.2
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.1/idbadapter/schedule_loader.py` & `idbadapter-1.9.2/idbadapter/schedule_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import requests
 import json
 from urllib.parse import urljoin
 
 GRANULARY = {"column": "granulary_name", "table": "granulary_works", "id": "id_granulary_work", "res_table": "granulary_resources"}
 
-PROCESSED = {"column": "processed_name", "table": "processed_works", "id": "id_processed_work", "res_table": "processed_resourcesobje"}
+PROCESSED = {"column": "processed_name", "table": "processed_works", "id": "id_processed_work", "res_table": "processed_resources"}
 
 TYPEDLVL2 = {"column": "typed_lvl2_name", "table": "typed_lvl2_works", "id": "id_typed_lvl2_work", "res_table": "typed_lvl2_resources"}
 
 ALL = "all"
 
 
 class Schedules:
@@ -182,15 +182,15 @@
                 select false as is_work, * from resource_names_mv rnm
                 join date_cte on date_cte.object_id = rnm.object_id
                 and rnm.date >= date_cte.date
                 where rnm.object_id = date_cte.object_id"""
 
                 
             if len(resource_list) != 0:
-                query += f""" and rnm.name in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
+                query += f""" and rnm.{key["column"]} in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
                 print("jsondecodeerror occurred", pull)
                 continue 
 
             if df.empty:
```

### Comparing `idbadapter-1.9.1/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.2/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.1
+Version: 1.9.2
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.1/setup.py` & `idbadapter-1.9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.1'
+version = '1.9.2'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.1',
+      version='1.9.2',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

