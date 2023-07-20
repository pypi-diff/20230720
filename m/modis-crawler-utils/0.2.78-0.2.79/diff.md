# Comparing `tmp/modis_crawler_utils-0.2.78.tar.gz` & `tmp/modis_crawler_utils-0.2.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.2.78.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.2.79.tar", max compression
```

## Comparing `modis_crawler_utils-0.2.78.tar` & `modis_crawler_utils-0.2.79.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1784 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/README.md
--rw-r--r--   0        0        0     1050 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     5975 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0     1263 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4105 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      703 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/domains.py
--rw-r--r--   0        0        0     1373 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3040 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2177 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1513 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     2882 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    26371 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/files.py
--rw-r--r--   0        0        0     5002 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3083 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/logstash.py
--rw-r--r--   0        0        0      581 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/misc.py
--rw-r--r--   0        0        0     4862 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    25668 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1955 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0     5751 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0      179 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-07-19 15:28:27.424859 modis_crawler_utils-0.2.78/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1480 2023-07-19 15:28:53.533192 modis_crawler_utils-0.2.78/pyproject.toml
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.78/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.79/README.md
+-rw-r--r--   0        0        0     1050 2023-07-10 09:34:47.574239 modis_crawler_utils-0.2.79/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.79/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.79/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-26 14:22:46.892695 modis_crawler_utils-0.2.79/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     5975 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.79/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0     1263 2023-07-12 14:56:04.794699 modis_crawler_utils-0.2.79/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:35:49.617028 modis_crawler_utils-0.2.79/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4105 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      703 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1373 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3040 2023-07-12 14:56:04.814698 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2177 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1513 2023-07-19 15:26:54.867809 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     2882 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    26371 2023-07-19 15:26:54.867809 modis_crawler_utils-0.2.79/crawler_utils/files.py
+-rw-r--r--   0        0        0     5002 2023-07-12 13:48:37.648012 modis_crawler_utils-0.2.79/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3083 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/logstash.py
+-rw-r--r--   0        0        0      581 2023-07-12 14:56:04.818698 modis_crawler_utils-0.2.79/crawler_utils/misc.py
+-rw-r--r--   0        0        0     4862 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:35:49.617028 modis_crawler_utils-0.2.79/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    25908 2023-07-20 16:34:33.892048 modis_crawler_utils-0.2.79/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-06-26 14:22:46.896695 modis_crawler_utils-0.2.79/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1955 2023-07-12 14:56:04.830697 modis_crawler_utils-0.2.79/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-07-11 08:36:53.815987 modis_crawler_utils-0.2.79/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0     5751 2023-07-10 10:32:48.279315 modis_crawler_utils-0.2.79/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0      179 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-06-26 14:22:46.900695 modis_crawler_utils-0.2.79/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1480 2023-07-20 16:36:44.362846 modis_crawler_utils-0.2.79/pyproject.toml
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 modis_crawler_utils-0.2.79/PKG-INFO
```

### Comparing `modis_crawler_utils-0.2.78/README.md` & `modis_crawler_utils-0.2.79/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/__init__.py` & `modis_crawler_utils-0.2.79/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.2.79/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.2.79/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.2.79/crawler_utils/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.2.79/crawler_utils/credentials/store/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.2.79/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.2.79/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.2.79/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.2.79/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/domains.py` & `modis_crawler_utils-0.2.79/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/echo.py` & `modis_crawler_utils-0.2.79/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/request_fingerprint.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/request_fingerprint.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.2.79/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/files.py` & `modis_crawler_utils-0.2.79/crawler_utils/files.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/images.py` & `modis_crawler_utils-0.2.79/crawler_utils/images.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/kafka.py` & `modis_crawler_utils-0.2.79/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/logstash.py` & `modis_crawler_utils-0.2.79/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/misc.py` & `modis_crawler_utils-0.2.79/crawler_utils/misc.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/mongodb.py` & `modis_crawler_utils-0.2.79/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/proxypy.py` & `modis_crawler_utils-0.2.79/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.2.79/crawler_utils/social_media/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from typing import List
-
+from typing import Union
 from dateparser import parse
 
 UnixTimestamp = int  # Имитация типа timestamp
 
 
 def class_output(obj_class: object):
     # Метод, не пропускающий в конечный JSON-файл пустые поля.
@@ -66,14 +66,23 @@
     ACTIVE = "Active"
     DELETED = "Deleted"
     BANNED = "Banned"
     CLOSED = "Closed"
     NOT_SPECIFIED = None
 
 
+class AttachmentType(Enum):
+    DOCUMENT = "document"
+    IMAGE = "image"
+    LINK = "link"
+    VIDEO = "video"
+    AUDIO = "audio"
+    NOT_SPECIFIED = None
+
+
 class Gender(Enum):
     MALE = "Male"
     FEMALE = "Female"
     OTHER = "Other"
     NOT_SPECIFIED = None
 
 
@@ -324,20 +333,21 @@
     value: str
     contact_type: str
 
 
 @dataclass
 class Attachment:
     url: str
-    attachment_type: str = None
+    attachment_type: Union[str, AttachmentType] = None
     title: str = None
     path: str = None
     filename: str = None
     checksum: str = None
     status: str = None
+    to_be_downloaded: bool = True
     # __________Other Fields____________
     attachment_id: str = None  # VK
     owner_id: str = None  # VK
     image_url: str = None  # VK
     duration: float = None  # VK
     artist: str = None  # VK
```

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/socks.py` & `modis_crawler_utils-0.2.79/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/states/__init__.py` & `modis_crawler_utils-0.2.79/crawler_utils/states/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.2.79/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.2.79/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.2.79/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.2.79/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.2.79/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.2.79/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/trust_level.py` & `modis_crawler_utils-0.2.79/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/crawler_utils/validate_input.py` & `modis_crawler_utils-0.2.79/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.2.78/pyproject.toml` & `modis_crawler_utils-0.2.79/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.2.78"
+version = "0.2.79"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
```

### Comparing `modis_crawler_utils-0.2.78/PKG-INFO` & `modis_crawler_utils-0.2.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.2.78
+Version: 0.2.79
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

