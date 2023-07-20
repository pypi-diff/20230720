# Comparing `tmp/XoxoDay-0.0.28.tar.gz` & `tmp/XoxoDay-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.28.tar", last modified: Thu Jul 13 10:07:37 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.29.tar", last modified: Thu Jul 20 21:45:40 2023, max compression
```

## Comparing `XoxoDay-0.0.28.tar` & `XoxoDay-0.0.29.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-13 10:07:37.256394 XoxoDay-0.0.28/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.28/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-13 10:07:37.256217 XoxoDay-0.0.28/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.28/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-13 10:07:37.250948 XoxoDay-0.0.28/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-13 10:07:28.000000 XoxoDay-0.0.28/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.28/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-13 10:07:37.251947 XoxoDay-0.0.28/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.28/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      700 2023-07-13 10:07:14.000000 XoxoDay-0.0.28/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      626 2023-07-13 10:07:14.000000 XoxoDay-0.0.28/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-13 10:07:37.255879 XoxoDay-0.0.28/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.28/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.28/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.28/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1892 2023-07-13 10:07:14.000000 XoxoDay-0.0.28/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.28/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.28/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-13 10:07:37.251695 XoxoDay-0.0.28/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-13 10:07:37.000000 XoxoDay-0.0.28/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      483 2023-07-13 10:07:37.000000 XoxoDay-0.0.28/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-13 10:07:37.000000 XoxoDay-0.0.28/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-13 10:07:37.000000 XoxoDay-0.0.28/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-13 10:07:37.000000 XoxoDay-0.0.28/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-13 10:07:37.256462 XoxoDay-0.0.28/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-13 10:07:25.000000 XoxoDay-0.0.28/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-20 21:45:40.657034 XoxoDay-0.0.29/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.29/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-20 21:45:40.656887 XoxoDay-0.0.29/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.29/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-20 21:45:40.653576 XoxoDay-0.0.29/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-20 21:45:21.000000 XoxoDay-0.0.29/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.29/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-20 21:45:40.654848 XoxoDay-0.0.29/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.29/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      700 2023-07-13 10:07:14.000000 XoxoDay-0.0.29/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      626 2023-07-13 10:07:14.000000 XoxoDay-0.0.29/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-20 21:45:40.656528 XoxoDay-0.0.29/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.29/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.29/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.29/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1892 2023-07-13 10:07:14.000000 XoxoDay-0.0.29/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.29/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4637 2023-07-20 21:44:57.000000 XoxoDay-0.0.29/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-20 21:45:40.654600 XoxoDay-0.0.29/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-20 21:45:40.000000 XoxoDay-0.0.29/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      483 2023-07-20 21:45:40.000000 XoxoDay-0.0.29/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-20 21:45:40.000000 XoxoDay-0.0.29/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-20 21:45:40.000000 XoxoDay-0.0.29/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-20 21:45:40.000000 XoxoDay-0.0.29/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-20 21:45:40.657079 XoxoDay-0.0.29/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-20 21:45:16.000000 XoxoDay-0.0.29/setup.py
```

### Comparing `XoxoDay-0.0.28/LICENSE` & `XoxoDay-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/PKG-INFO` & `XoxoDay-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.28
+Version: 0.0.29
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.28/README.md` & `XoxoDay-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/exception.py` & `XoxoDay-0.0.29/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/helper/token.py` & `XoxoDay-0.0.29/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/serializer.py` & `XoxoDay-0.0.29/XoxoDay/serializer.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/service/http_service.py` & `XoxoDay-0.0.29/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/service/token_service.py` & `XoxoDay-0.0.29/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.28/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.29/XoxoDay/service/xoxoday_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         file = open(payload_file_path)
         payload = json.load(file)
         product = self.getVouchers(includeProducts=productId)
         if len(product) == 0:
             raise XoxoDayException(ErrorCodes.INVALID_ATTRIBUTE)
         denominations = product[0]['denominations'].split(',')
         denominations = list(map(int, denominations))
-        if int(denomination) not in denominations:
+        if int(denomination) not in denominations and self.environment == 'dev':
             raise XoxoDayException(ErrorCodes.INVALID_DENOMINATION)
         if poNumber is None:
             poNumber = str(uuid.uuid4())
         payload['variables']['data']['productId'] = productId
         payload['variables']['data']['denomination'] = denomination
         payload['variables']['data']['email'] = email
         payload['variables']['data']['poNumber'] = poNumber
```

### Comparing `XoxoDay-0.0.28/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.29/XoxoDay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.28
+Version: 0.0.29
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.28/setup.py` & `XoxoDay-0.0.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.28",
+    version="0.0.29",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

