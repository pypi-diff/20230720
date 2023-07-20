# Comparing `tmp/requestsbankrko-0.2.4.tar.gz` & `tmp/requestsbankrko-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.4.tar", last modified: Mon Jul 17 11:16:14 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.5.tar", last modified: Thu Jul 20 11:05:09 2023, max compression
```

## Comparing `requestsbankrko-0.2.4.tar` & `requestsbankrko-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    56956 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29207 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56968 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.4/LICENSE` & `requestsbankrko-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.4/PKG-INFO` & `requestsbankrko-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.4
+Version: 0.2.5
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.4/pyproject.toml` & `requestsbankrko-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.4"
+version = "0.2.5"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.4/src/bank_methods.py` & `requestsbankrko-0.2.5/src/bank_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -867,15 +867,18 @@
                 if message is not None:
                     if message in self.invalids:
                         self.success = True
                         return inn_busy
 
 
 class KonturCanCreate(Kontur):
-    invalids = ['Есть такая же потенциальная продажа в запрашиваемом PartnerCode']
+    invalids = [
+        'Есть такая же потенциальная продажа в запрашиваемом PartnerCode',
+        'Есть такая же потенциальная продажа в другом PartnerCode'
+    ]
     def __init__(self, json, test):
         super().__init__(json, test)
         self.endpoint = '/prospectivesales/cancreate/v2'
         self.method = 'post'
 
 
     def suc_resp(self):
```

### Comparing `requestsbankrko-0.2.4/src/open_methods.py` & `requestsbankrko-0.2.5/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.4/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.5/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.4
+Version: 0.2.5
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.4/src/zip_functions.py` & `requestsbankrko-0.2.5/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.4/tests/test_bank_methods.py` & `requestsbankrko-0.2.5/tests/test_bank_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1323,34 +1323,34 @@
         json = {
             # "ProspectiveSaleId": "7cd28409-4c7c-4b55-af5e-f388a3326124",
             "Organization": {
                 "Inn": "7654776644",
                 # "Kpp": "765401001",
                 "IsPhysical": False,
                 "Name": "ООО «Боевые Робоединороги»",
-                "Region": "66",
+                # "Region": "66",
                 "City": "Екатеринбург",
                 "Address": "ул. Малопрудная, д. 5"
             },
             "Contacts": [
                 {
                     "Name": "Кропоткин Василий Павлович",
                     "Position": "Директор",
                     "Phones": [
                         {
                             "Id": "98da9a79-55f2-46a0-bfa8-a50b8cbce3c4",
                             "Number": "+75554440011",
                             "AdditionalNumber": "123"
                         }
                     ],
-                    "Emails": [
-                        {
-                            "Address": "ooo@yandex.ru"
-                        }
-                    ]
+                    # "Emails": [
+                    #     {
+                    #         "Address": "ooo@yandex.ru"
+                    #     }
+                    # ]
                 }
             ],
             "Source": "www.source.ru",
             "CountryCode": "RU",
             "ForeignOrganization": None,
             "ExternalProductId": None,
             "InternalProductId": "Evrika",
```

