# Comparing `tmp/tap-shopify-1.7.5.tar.gz` & `tmp/tap-shopify-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-shopify-1.7.5.tar", last modified: Wed Jun 21 17:17:00 2023, max compression
+gzip compressed data, was "tap-shopify-1.7.6.tar", last modified: Thu Jul 20 17:46:02 2023, max compression
```

## Comparing `tap-shopify-1.7.5.tar` & `tap-shopify-1.7.6.tar`

### file list

```diff
@@ -1,49 +1,59 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 17:17:00.898779 tap-shopify-1.7.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-06-21 17:17:00.898779 tap-shopify-1.7.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2548 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-21 17:17:00.898779 tap-shopify-1.7.5/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      840 2023-06-21 16:54:58.000000 tap-shopify-1.7.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 17:17:00.874779 tap-shopify-1.7.5/tap_shopify/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1321 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 17:17:00.886779 tap-shopify-1.7.5/tap_shopify/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10539 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/abandoned_checkouts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/collects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/custom_collections.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/customers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27088 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/definitions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1147 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/inventory_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/inventory_levels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/locations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/metafields.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20799 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/order_refunds.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23571 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/orders.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6059 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/schemas/transactions.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 17:17:00.894779 tap-shopify-1.7.5/tap_shopify/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/abandoned_checkouts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13568 2023-06-20 14:20:46.000000 tap-shopify-1.7.5/tap_shopify/streams/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/collects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/custom_collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/customers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/inventory_items.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/inventory_levels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1381 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/locations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/metafields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2583 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/order_refunds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/orders.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-05-25 13:25:31.000000 tap-shopify-1.7.5/tap_shopify/streams/transactions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 17:17:00.874779 tap-shopify-1.7.5/tap_shopify.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-21 17:17:00.000000 tap-shopify-1.7.5/tap_shopify.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.459838 tap-shopify-1.7.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-20 17:46:02.459838 tap-shopify-1.7.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2548 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-20 17:46:02.459838 tap-shopify-1.7.6/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      840 2023-07-20 17:41:59.000000 tap-shopify-1.7.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.451838 tap-shopify-1.7.6/tap_shopify/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1321 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.455838 tap-shopify-1.7.6/tap_shopify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10539 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/abandoned_checkouts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/collects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/custom_collections.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27088 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/definitions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1147 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/inventory_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/inventory_levels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/locations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/metafields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20799 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/order_refunds.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23571 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/orders.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6059 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/schemas/transactions.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.459838 tap-shopify-1.7.6/tap_shopify/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/abandoned_checkouts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13844 2023-07-20 17:41:59.000000 tap-shopify-1.7.6/tap_shopify/streams/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/collects.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/custom_collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/customers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/inventory_items.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/inventory_levels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1381 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/locations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/metafields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2583 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/order_refunds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/orders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tap_shopify/streams/transactions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.451838 tap-shopify-1.7.6/tap_shopify.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1626 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-07-20 17:46:02.000000 tap-shopify-1.7.6/tap_shopify.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 17:46:02.459838 tap-shopify-1.7.6/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4312 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4416 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9626 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11083 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_bookmarks_updated.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9258 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4128 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_full_replication.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5655 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_shop_info_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8192 2023-06-09 08:22:37.000000 tap-shopify-1.7.6/tests/test_start_date.py
```

### Comparing `tap-shopify-1.7.5/LICENSE` & `tap-shopify-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/README.md` & `tap-shopify-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/setup.py` & `tap-shopify-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-shopify",
-    version="1.7.5",
+    version="1.7.6",
     description="Singer.io tap for extracting Shopify data",
     author="Stitch",
     url="http://github.com/singer-io/tap-shopify",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     python_requires='>=3.5.2',
     py_modules=["tap_shopify"],
     install_requires=[
```

### Comparing `tap-shopify-1.7.5/tap_shopify/__init__.py` & `tap-shopify-1.7.6/tap_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/context.py` & `tap-shopify-1.7.6/tap_shopify/context.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/abandoned_checkouts.json` & `tap-shopify-1.7.6/tap_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/collects.json` & `tap-shopify-1.7.6/tap_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/custom_collections.json` & `tap-shopify-1.7.6/tap_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/definitions.json` & `tap-shopify-1.7.6/tap_shopify/schemas/definitions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/events.json` & `tap-shopify-1.7.6/tap_shopify/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/inventory_items.json` & `tap-shopify-1.7.6/tap_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/metafields.json` & `tap-shopify-1.7.6/tap_shopify/schemas/metafields.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/order_refunds.json` & `tap-shopify-1.7.6/tap_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/orders.json` & `tap-shopify-1.7.6/tap_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/products.json` & `tap-shopify-1.7.6/tap_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/schemas/transactions.json` & `tap-shopify-1.7.6/tap_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/__init__.py` & `tap-shopify-1.7.6/tap_shopify/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/base.py` & `tap-shopify-1.7.6/tap_shopify/streams/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,19 @@
                           (pyactiveresource.connection.ServerError,
                            pyactiveresource.formats.Error,
                            simplejson.scanner.JSONDecodeError,
                            URLError),
                           giveup=is_not_status_code_fn(range(500, 599)),
                           on_backoff=retry_handler,
                           max_tries=MAX_RETRIES)
+    @backoff.on_exception(backoff.expo,
+                          pyactiveresource.connection.ResourceNotFound,
+                          giveup=is_not_status_code_fn([404]),
+                          on_backoff=retry_handler,
+                          max_tries=MAX_RETRIES)
     @backoff.on_exception(retry_after_wait_gen,
                           pyactiveresource.connection.ClientError,
                           giveup=is_not_status_code_fn([429]),
                           on_backoff=leaky_bucket_handler,
                           # No jitter as we want a constant value
                           jitter=None)
     @functools.wraps(fnc)
```

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/collects.py` & `tap-shopify-1.7.6/tap_shopify/streams/collects.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/events.py` & `tap-shopify-1.7.6/tap_shopify/streams/events.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/inventory_items.py` & `tap-shopify-1.7.6/tap_shopify/streams/inventory_items.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/inventory_levels.py` & `tap-shopify-1.7.6/tap_shopify/streams/inventory_levels.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/locations.py` & `tap-shopify-1.7.6/tap_shopify/streams/locations.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/metafields.py` & `tap-shopify-1.7.6/tap_shopify/streams/metafields.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/order_refunds.py` & `tap-shopify-1.7.6/tap_shopify/streams/order_refunds.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify/streams/transactions.py` & `tap-shopify-1.7.6/tap_shopify/streams/transactions.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.5/tap_shopify.egg-info/SOURCES.txt` & `tap-shopify-1.7.6/tap_shopify.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -36,8 +36,17 @@
 tap_shopify/streams/inventory_items.py
 tap_shopify/streams/inventory_levels.py
 tap_shopify/streams/locations.py
 tap_shopify/streams/metafields.py
 tap_shopify/streams/order_refunds.py
 tap_shopify/streams/orders.py
 tap_shopify/streams/products.py
-tap_shopify/streams/transactions.py
+tap_shopify/streams/transactions.py
+tests/test_all_fields.py
+tests/test_automatic_fields.py
+tests/test_bookmarks.py
+tests/test_bookmarks_updated.py
+tests/test_discovery.py
+tests/test_full_replication.py
+tests/test_pagination.py
+tests/test_shop_info_fields.py
+tests/test_start_date.py
```

