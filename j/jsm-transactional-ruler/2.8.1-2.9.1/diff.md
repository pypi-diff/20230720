# Comparing `tmp/jsm_transactional_ruler-2.8.1.tar.gz` & `tmp/jsm_transactional_ruler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_transactional_ruler-2.8.1.tar", max compression
+gzip compressed data, was "jsm_transactional_ruler-2.9.1.tar", max compression
```

## Comparing `jsm_transactional_ruler-2.8.1.tar` & `jsm_transactional_ruler-2.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2510 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/README.md
--rw-r--r--   0        0        0     4323 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/enums.py
--rw-r--r--   0        0        0     1131 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/events.py
--rw-r--r--   0        0        0       49 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/exceptions.py
--rw-r--r--   0        0        0      938 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/publisher.py
--rw-r--r--   0        0        0     1545 2023-05-03 21:26:24.559700 jsm_transactional_ruler-2.8.1/pyproject.toml
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 jsm_transactional_ruler-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2510 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/README.md
+-rw-r--r--   0        0        0     4379 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/enums.py
+-rw-r--r--   0        0        0     1131 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/events.py
+-rw-r--r--   0        0        0       49 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/exceptions.py
+-rw-r--r--   0        0        0      938 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/publisher.py
+-rw-r--r--   0        0        0     1545 2023-05-22 17:21:39.181693 jsm_transactional_ruler-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 jsm_transactional_ruler-2.9.1/PKG-INFO
```

### Comparing `jsm_transactional_ruler-2.8.1/README.md` & `jsm_transactional_ruler-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/enums.py` & `jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,11 +51,12 @@
     T_EVENT_COMPLETE_CARD_NEW_PROFISSIONAL_MAIS = "T_EVENT_COMPLETE_CARD_NEW_PROFISSIONAL_MAIS"
     T_EVENT_LAST_30_DAYS_OF_BONUS_NEW_PROFISSIONAL_MAIS = "T_EVENT_LAST_30_DAYS_OF_BONUS_NEW_PROFISSIONAL_MAIS"
     T_EVENT_PURCHASE_TOP_CASHBACK = "T_EVENT_PURCHASE_TOP_CASHBACK"
     T_EVENT_PURCHASE_VOUCHER = "T_EVENT_PURCHASE_VOUCHER"
     T_EVENT_CERTIFICATION = "T_EVENT_CERTIFICATION"
     T_EVENT_NEW_LUCKY_NUMBER_AVAILABLE = "T_EVENT_NEW_LUCKY_NUMBER_AVAILABLE"
     T_EVENT_POINTSBACK_SUCCESSFUL_RECEIVED_POINTS = "T_EVENT_POINTSBACK_SUCCESSFULL_RECEIVED_POINTS"
+    T_EVENT_RECEIPT_NON_TAX = "T_EVENT_RECEIPT_NON_TAX"
 
     @classmethod
     def get_choices(cls):
         return tuple(item.value for item in cls)
```

### Comparing `jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/events.py` & `jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/events.py`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.8.1/jsm_transactional_ruler/publisher.py` & `jsm_transactional_ruler-2.9.1/jsm_transactional_ruler/publisher.py`

 * *Files identical despite different names*

### Comparing `jsm_transactional_ruler-2.8.1/pyproject.toml` & `jsm_transactional_ruler-2.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-transactional-ruler"
-version = "2.8.1"
+version = "2.9.1"
 description = "Lib to post user events on transactional topics"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 maintainers = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 readme = "README.md"
 homepage = "https://juntossomosmais.com.br"
 repository = "https://github.com/juntossomosmais/transactional-ruler"
```

### Comparing `jsm_transactional_ruler-2.8.1/PKG-INFO` & `jsm_transactional_ruler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-transactional-ruler
-Version: 2.8.1
+Version: 2.9.1
 Summary: Lib to post user events on transactional topics
 Home-page: https://juntossomosmais.com.br
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Maintainer: Juntos Somos Mais
 Maintainer-email: labs@juntossomosmais.com.br
 Requires-Python: >=3.7,<4.0
```

