# Comparing `tmp/contact_magic-0.5.5.tar.gz` & `tmp/contact_magic-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.5.tar", max compression
+gzip compressed data, was "contact_magic-0.5.6.tar", max compression
```

## Comparing `contact_magic-0.5.5.tar` & `contact_magic-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.5/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.5/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.5/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.5/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5418 2023-07-13 11:03:11.215506 contact_magic-0.5.5/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.5/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.5/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.5/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-13 10:14:40.612229 contact_magic-0.5.5/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.5/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.5/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.5/contact_magic/logger.py
--rw-r--r--   0        0        0    16833 2023-07-17 16:16:08.641976 contact_magic-0.5.5/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.5/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.5/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.5/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.5/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.5/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.5/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.5/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.5/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.5/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-07-17 16:15:47.756172 contact_magic-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.6/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.6/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.6/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.6/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5418 2023-07-20 15:24:39.359080 contact_magic-0.5.6/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2663 2023-07-20 16:08:38.910133 contact_magic-0.5.6/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-20 14:30:01.195479 contact_magic-0.5.6/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.6/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-20 16:08:38.513794 contact_magic-0.5.6/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1784 2023-07-20 14:41:42.621150 contact_magic-0.5.6/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.6/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.6/contact_magic/logger.py
+-rw-r--r--   0        0        0    16920 2023-07-20 15:55:40.352110 contact_magic-0.5.6/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.6/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.6/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.6/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.6/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.6/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.6/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.6/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.6/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.6/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-20 16:00:56.144079 contact_magic-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.6/PKG-INFO
```

### Comparing `contact_magic-0.5.5/README.md` & `contact_magic-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/asyncio.py` & `contact_magic-0.5.6/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/conf/settings.py` & `contact_magic-0.5.6/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/dict_utils.py` & `contact_magic-0.5.6/contact_magic/dict_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """
 Helpers for working with potentially heavily nested pieces of data
 """
 
 
+def get_first_level_items(data: dict) -> dict:
+    """
+    Returns only the top level of data from a dict that is valid.
+    :param data:
+    :return:
+    """
+    return {
+        key: value for key, value in data.items() if not isinstance(value, (dict, list))
+    }
+
+
 def delete_key_in_object(data, target_key):
     """
     Go through original object and delete
     all occurrences of a target key
     """
     if isinstance(data, list):
         for list_item in data:
```

### Comparing `contact_magic-0.5.5/contact_magic/helpers.py` & `contact_magic-0.5.6/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.6/contact_magic/integrations/copyfactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 
 import httpx
 
 from contact_magic.conf.settings import SETTINGS
-from contact_magic.dict_utils import get_values_in_object_by_key
+from contact_magic.dict_utils import get_first_level_items, get_values_in_object_by_key
 from contact_magic.logger import logger
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 endpoint = "https://app.copyfactory.io/api/v2/generate/"
 
@@ -28,17 +28,18 @@
 async def make_copyfactory_request(premise_id: int, variables: dict, max_retries=3):
     if not SETTINGS.COPYFACTORY_API_KEY:
         return None
     headers = {
         "Accept": "application/json",
         "Authorization": SETTINGS.COPYFACTORY_API_KEY,
     }
+    variable_data = get_first_level_items(variables)
     data = {
         "premise_id": premise_id,
-        "variables": variables,
+        "variables": variable_data,
     }
     try:
         session = httpx.AsyncClient(timeout=90)
         retries = 0
         while retries < max_retries:
             res = await session.request(
                 method="POST", url=endpoint, headers=headers, json=data
```

### Comparing `contact_magic-0.5.5/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.6/contact_magic/integrations/sales_scrapers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 
 import httpx
 
 from contact_magic.conf.settings import SETTINGS
+from contact_magic.dict_utils import get_first_level_items
 from contact_magic.logger import logger
 from contact_magic.utils import fix_website
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 base_url = "https://salesscrapers.dev/api/"
 
@@ -20,17 +21,18 @@
         "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY,
     }
 
     url = f"{base_url}{endpoint}"
     try:
         session = httpx.AsyncClient(timeout=120)
         retries = 0
+        params = get_first_level_items(data)
         while retries < max_retries:
             res = await session.request(
-                method="get", url=url, headers=headers, params=data
+                method="get", url=url, headers=headers, params=params
             )
             # authorization error so can break
             if res.status_code == 401:
                 logger.warning("sales_scraper_error", message=res.text)
                 break
             if res.status_code == 400:
                 logger.warning("proxy_error", message=res.text)
```

### Comparing `contact_magic-0.5.5/contact_magic/integrations/sheets.py` & `contact_magic-0.5.6/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/models.py` & `contact_magic-0.5.6/contact_magic/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,16 @@
         # Remove all other scraped data keys
         # from the row from consideration in the event of
         # multiple keys from scraped data having
         # the same name to restrict the passed data to being from
         # this sentence wizard scrape.
         if self.restrict_to_scraped_data:
             for key in keys_to_delete:
-                data = delete_key_in_object(data, key)
+                if not key.startswith(f"{content_col_name}__{self.scraper_name}"):
+                    data = delete_key_in_object(data, key)
 
         if cf := await make_copyfactory_request(self.premise_id, variables=data):
             row.data[content_col_name] = cf["content"]
             source = row.data.get(
                 f"{content_col_name}__{self.scraper_name}__scraper_info", {}
             ).get(f"{SALES_SCRAPER_KEY_PREFIX_NAME}__data_source", "-")
             row.data[source_col_name] = f"{self.scraper_name}, {source}"
```

### Comparing `contact_magic-0.5.5/contact_magic/preprocessors.py` & `contact_magic-0.5.6/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/scripts/agency.py` & `contact_magic-0.5.6/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.5.6/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.6/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.5.6/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.6/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/contact_magic/utils.py` & `contact_magic-0.5.6/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.5/pyproject.toml` & `contact_magic-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.5"
+version = "0.5.6"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.5/PKG-INFO` & `contact_magic-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.5
+Version: 0.5.6
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

