# Comparing `tmp/crypto-screening-7.2.0.tar.gz` & `tmp/crypto-screening-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.2.0.tar", last modified: Thu Jul 20 08:35:05 2023, max compression
+gzip compressed data, was "crypto-screening-7.3.0.tar", last modified: Thu Jul 20 16:11:04 2023, max compression
```

## Comparing `crypto-screening-7.2.0.tar` & `crypto-screening-7.3.0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/
--rw-rw-rw-   0        0        0       98 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.2.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.875692 crypto-screening-7.2.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.893697 crypto-screening-7.2.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.2.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.2.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.896696 crypto-screening-7.2.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.2.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.2.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.2.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.2.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.899698 crypto-screening-7.2.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.2.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16701 2023-07-19 10:06:31.000000 crypto-screening-7.2.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.2.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.2.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.2.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.2.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.900722 crypto-screening-7.2.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-7.2.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.903698 crypto-screening-7.2.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.911696 crypto-screening-7.2.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-19 09:07:33.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11400 2023-07-19 10:06:31.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13883 2023-07-20 08:20:28.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/callbacks.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     7002 2023-07-19 18:46:12.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/sockets.py
--rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.2.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.2.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.2.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.2.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.890697 crypto-screening-7.2.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-20 08:34:57.000000 crypto-screening-7.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.918616 crypto-screening-7.3.0/
+-rw-rw-rw-   0        0        0       98 2023-07-20 16:11:03.000000 crypto-screening-7.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-20 16:11:04.917616 crypto-screening-7.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.3.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.3.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.714790 crypto-screening-7.3.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.751794 crypto-screening-7.3.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.3.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.3.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.779794 crypto-screening-7.3.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.3.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.3.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.3.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.3.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.802360 crypto-screening-7.3.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.3.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.3.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-20 15:18:05.000000 crypto-screening-7.3.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.3.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.3.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.3.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.3.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.3.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.3.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.3.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.813364 crypto-screening-7.3.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    21478 2023-07-20 14:19:49.000000 crypto-screening-7.3.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.837009 crypto-screening-7.3.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.3.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.3.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.3.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.3.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.896647 crypto-screening-7.3.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11649 2023-07-20 15:46:53.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.916617 crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3645 2023-07-20 15:49:53.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4109 2023-07-20 15:57:21.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    19750 2023-07-20 15:10:58.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10926 2023-07-20 15:55:41.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.3.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.3.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.3.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.3.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.3.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:11:04.729791 crypto-screening-7.3.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-20 16:11:04.000000 crypto-screening-7.3.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1989 2023-07-20 16:11:04.000000 crypto-screening-7.3.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 16:11:04.000000 crypto-screening-7.3.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-20 16:11:04.000000 crypto-screening-7.3.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 16:11:04.000000 crypto-screening-7.3.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-20 16:11:03.000000 crypto-screening-7.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.3.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 16:11:04.918616 crypto-screening-7.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-20 16:10:43.000000 crypto-screening-7.3.0/setup.py
```

### Comparing `crypto-screening-7.2.0/PKG-INFO` & `crypto-screening-7.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.2.0
+Version: 7.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.2.0/README.md` & `crypto-screening-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/build.py` & `crypto-screening-7.3.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/assets.py` & `crypto-screening-7.3.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/exchanges.py` & `crypto-screening-7.3.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/orders.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/state/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # base.py
 
 from abc import ABCMeta
 import datetime as dt
 from typing import (
     Iterable, Dict, Optional, Reversible,
-    Any, ClassVar, List, Tuple, TypeVar, Type
+    Any, ClassVar, List, Tuple, TypeVar
 )
 
 from attrs import define
 
 from represent import represent, Modifiers
 
 import pandas as pd
@@ -445,33 +445,39 @@
             else:
                 screener.market.loc[index] = row
             # end if
         # end for
     # end for
 # end add_data_to_screeners
 
-def index_to_datetime(index: Any) -> dt.datetime:
+def index_to_datetime(index: Any, adjust: Optional[bool] = True) -> dt.datetime:
     """
     Converts the index into a datetime object.
 
     :param index: The value to convert.
+    :param adjust: The value to adjust the process for errors.
 
     :return: The datetime object.
     """
 
     try:
         if isinstance(index, str):
             index = dt.datetime.fromisoformat(index)
 
-        elif isinstance(index, int):
+        elif isinstance(index, (int, float)):
             index = dt.datetime.fromtimestamp(index)
         # end if
 
-    except (Type, ValueError):
-        pass
+    except (TypeError, ValueError) as e:
+        if adjust:
+            pass
+
+        else:
+            raise e
+        # end if
     # end try
 
     return index
 # end index_to_datetime
 
 def screener_dataset(
         columns: Dict[str, str], screener: BaseScreener
```

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/market/trades.py` & `crypto-screening-7.3.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/screeners.py` & `crypto-screening-7.3.0/crypto_screening/collect/screeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,31 +225,33 @@
         ).append(screener)
     # end for
 
     return structure
 # end structure_screeners
 
 def find_screeners(
-        screeners: Iterable[BaseScreener], exchange: str, symbol: str
+        screeners: Iterable[BaseScreener],
+        exchange: Optional[str] = None,
+        symbol: Optional[str] = None
 ) -> List[BaseScreener]:
     """
     Finds all the screeners with the matching exchange and symbol key.
 
     :param screeners: The screeners to process.
     :param exchange: The exchange key for the symbol.
     :param symbol: The pair symbol to search its screeners.
 
     :return: The matching screeners.
     """
 
     return [
         screener for screener in screeners
         if (
-            (screener.symbol.lower() == symbol.lower()) and
-            (exchange.lower() == screener.exchange.lower())
+            ((symbol is None) or (screener.symbol.lower() == symbol.lower())) and
+            ((exchange is None) or (exchange.lower() == screener.exchange.lower()))
         )
     ]
 # end find_screeners
 
 def remove_empty_screeners(screeners: Iterable[BaseScreener]) -> List[BaseScreener]:
     """
     Removes the empty screeners.
```

### Comparing `crypto-screening-7.2.0/crypto_screening/collect/symbols.py` & `crypto-screening-7.3.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/dataset.py` & `crypto-screening-7.3.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/interval.py` & `crypto-screening-7.3.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/dynamic.py` & `crypto-screening-7.3.0/crypto_screening/market/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # dynamic.py
 
+from abc import ABCMeta
 from typing import Optional, Iterable, List, Union, Dict
 
-from represent import Modifiers
-
 import pandas as pd
 
 from crypto_screening.collect.screeners import exchanges_symbols_screeners
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.collect.market.orderbook import (
     assets_orderbook_market_state, symbols_orderbook_market_state,
     SymbolsOrderbookMarketState, AssetsOrderbookMarketState
 )
 from crypto_screening.collect.market.ohlcv import (
     assets_ohlcv_market_state, symbols_ohlcv_market_state,
     SymbolsOHLCVMarketState, AssetsOHLCVMarketState
@@ -20,156 +18,165 @@
     assets_orders_market_state, symbols_orders_market_state,
     SymbolsOrdersMarketState, AssetsOrdersMarketState
 )
 from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
-from crypto_screening.market.screeners.container import ScreenersContainer
+from crypto_screening.market.screeners.container import (
+    DynamicScreenersContainer, FixedScreenersContainer, ScreenersContainer
+)
 
 __all__ = [
-    "DynamicScreenerContainer"
+    "ScreenersData",
+    "DynamicScreenersData",
+    "FixedScreenersData"
 ]
 
-class DynamicScreenerContainer(ScreenersContainer):
+class ScreenersData(ScreenersContainer, metaclass=ABCMeta):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects.
 
-    >>> from crypto_screening.market.dynamic import DynamicScreenerContainer
+    >>> from crypto_screening.market.dynamic import ScreenersData
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> dynamic_screener = DynamicScreenerContainer(
+    >>> data = ScreenersData(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
-    >>> dynamic_screener.find_screener(exchange="binance", symbol="BTC/USDT"))
-    >>> dynamic_screener.data(exchange="binance", symbol="BTC/USDT", length=10))
+    >>> data.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
 
-    __modifiers__ = Modifiers(**ScreenersContainer.__modifiers__)
-    __modifiers__.excluded.append("exchanges")
-
     def find_ohlcv_dataset(
             self,
             exchange: str,
             symbol: str,
-            interval: str,
-            length: Optional[int] = None
+            interval: Optional[str] = None,
+            length: Optional[int] = None,
+            index: Optional[int] = None
     ) -> pd.DataFrame:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
         :param interval: The interval for the dataset.
         :param length: The length of the data.
+        :param index: The index for the screener.
 
         :return: The data.
         """
 
         screener = self.find_ohlcv_screener(
-            exchange=exchange, symbol=symbol, interval=interval
+            exchange=exchange, symbol=symbol,
+            interval=interval, index=index
         )
 
         length = min(length or 0, len(screener.market))
 
         return screener.market.iloc[-length:]
     # end find_ohlcv_dataset
 
     def find_orderbook_dataset(
             self,
             exchange: str,
             symbol: str,
-            length: Optional[int] = None
+            length: Optional[int] = None,
+            index: Optional[int] = None
     ) -> pd.DataFrame:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
         :param length: The length of the data.
+        :param index: The index for the screener.
 
         :return: The data.
         """
 
         try:
             screener = self.find_orderbook_screener(
-                exchange=exchange, symbol=symbol
+                exchange=exchange, symbol=symbol, index=index
             )
 
             market = screener.market
 
-        except ValueError:
-            screener = self.find_screeners(
-                exchange=exchange, symbol=symbol
-            )[0]
+        except ValueError as e:
+            try:
+                screener = self.find_ohlcv_screener(
+                    exchange=exchange, symbol=symbol, index=index
+                )
 
-            if isinstance(screener, OHLCVScreener):
                 market = screener.orderbook_market
 
-            else:
-                market = screener.market
-            # end if
+            except ValueError:
+                raise e
+            # end try
         # end try
 
         length = min(length or 0, len(market))
 
         return market.iloc[-length:]
     # end find_orderbook_dataset
 
     def find_orders_dataset(
             self,
             exchange: str,
             symbol: str,
-            length: Optional[int] = None
+            length: Optional[int] = None,
+            index: Optional[int] = None
     ) -> pd.DataFrame:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
         :param length: The length of the data.
+        :param index: The index for the screener.
 
         :return: The data.
         """
 
         screener = self.find_orders_screener(
-            exchange=exchange, symbol=symbol
+            exchange=exchange, symbol=symbol, index=index
         )
 
         length = min(length or 0, len(screener.market))
 
         return screener.market.iloc[-length:]
     # end find_orders_dataset
 
     def find_trades_dataset(
             self,
             exchange: str,
             symbol: str,
-            length: Optional[int] = None
+            length: Optional[int] = None,
+            index: Optional[int] = None
     ) -> pd.DataFrame:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
         :param length: The length of the data.
+        :param index: The index for the screener.
 
         :return: The data.
         """
 
         screener = self.find_trades_screener(
-            exchange=exchange, symbol=symbol
+            exchange=exchange, symbol=symbol, index=index
         )
 
         length = min(length or 0, len(screener.market))
 
         return screener.market.iloc[-length:]
     # end find_trades_dataset
 
@@ -508,8 +515,52 @@
             included=included, excluded=excluded, adjust=adjust
         )
 
         return symbols_orders_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
     # end symbols_orders_market_state
-# end DynamicScreenerContainer
+# end DynamicScreenerContainer
+
+class FixedScreenersData(FixedScreenersContainer, ScreenersData):
+    """
+    A class to represent a multi-exchange multi-pairs crypto data screener.
+    Using this class enables extracting screener objects and screeners
+    data by the exchange name and the symbol of the pair.
+
+    parameters:
+
+    - screeners:
+        The screener objects.
+
+    >>> from crypto_screening.market.dynamic import FixedScreenersData
+    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>>
+    >>> fixed_data = FixedScreenersData(
+    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
+    >>> )
+    >>>
+    >>> fixed_data.find_screener(exchange="binance", symbol="BTC/USDT"))
+    """
+# end FixedScreenersData
+
+class DynamicScreenersData(DynamicScreenersContainer, ScreenersData):
+    """
+    A class to represent a multi-exchange multi-pairs crypto data screener.
+    Using this class enables extracting screener objects and screeners
+    data by the exchange name and the symbol of the pair.
+
+    parameters:
+
+    - screeners:
+        The screener objects.
+
+    >>> from crypto_screening.market.dynamic import DynamicScreenersData
+    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>>
+    >>> dynamic_data = DynamicScreenersData(
+    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
+    >>> )
+    >>>
+    >>> dynamic_data.find_screener(exchange="binance", symbol="BTC/USDT"))
+    """
+# end DynamicScreenersData
```

### Comparing `crypto-screening-7.2.0/crypto_screening/market/foundation/data.py` & `crypto-screening-7.3.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.3.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/foundation/state.py` & `crypto-screening-7.3.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.3.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/base.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # base.py
 
 import datetime as dt
 import time
 from typing import (
-    Optional, Union, Iterable, Any, List
+    Optional, Union, Iterable, Any, List, Dict
 )
 
 import pandas as pd
 
 from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
@@ -59,18 +59,21 @@
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
     MINIMUM_DELAY = 1
 
-    NAME = "BASE"
+    NAME: Optional[str] = "BASE"
 
     __slots__ = "symbol", "exchange", "market"
 
+    SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
+    SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
+
     def __init__(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
@@ -85,14 +88,17 @@
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param market: The data for the market.
         """
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
+        self.SCREENER_NAME_TYPE_MATCHES.setdefault(self.NAME, type(self))
+        self.SCREENER_TYPE_NAME_MATCHES.setdefault(type(self), self.NAME)
+
         self.exchange = self.validate_exchange(exchange=exchange)
         self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
 
         self.market = market
     # end __init__
 
     def await_initialization(
@@ -271,16 +277,14 @@
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("screeners")
 
     screeners: List[BaseScreener]
 
-    __slots__ = 'screeners',
-
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
```

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # callbacks.py
 
 import warnings
 import json
 import datetime as dt
-import os
 from typing import Optional, Any, Union, Dict, Callable, List, Tuple
 import asyncio
 from textwrap import wrap
 
 from cryptofeed.backends.socket import UDPProtocol
 
-from sqlalchemy import Engine, create_engine, text, inspect
+from sqlalchemy import Engine, text, inspect
 from sqlalchemy.orm import sessionmaker
 
 from crypto_screening.dataset import DATE_TIME
 from crypto_screening.market.screeners.database import (
-    database_file_path, parts_database_table_name
+    create_engine, parts_to_database_table_name
 )
 
 __all__ = [
     "Callback",
     "SocketCallback",
     "DatabaseCallback",
     "callback_data"
@@ -385,15 +384,16 @@
             database: str,
             engine: Optional[Engine] = None,
             key: Optional[Any] = None
     ) -> None:
         """
         Defines the class attributes.
 
-
+        :param database: The path to the database.
+        :param engine: The engine for the database.
         :param key: The key od the data.
         """
 
         super().__init__(key=key)
 
         self.database = database
 
@@ -435,15 +435,15 @@
         for index, row in data[self.DATA]:
             key, exchange, symbol, interval = (
                 key or self.key, data[self.EXCHANGE],
                 data[self.SYMBOL], data.get(self.INTERVAL, None)
             )
 
             if (key, exchange, symbol, interval) not in self.tables:
-                table = parts_database_table_name(
+                table = parts_to_database_table_name(
                     name=key, exchange=exchange,
                     symbol=symbol, interval=interval
                 )
 
                 self.tables[(key, exchange, symbol, interval)] = table
 
                 if table not in self.table_names:
@@ -460,15 +460,15 @@
                         )
                     )
                 # end if
 
             else:
                 table = self.tables.setdefault(
                     (key, exchange, symbol, interval),
-                    parts_database_table_name(
+                    parts_to_database_table_name(
                         name=key, exchange=exchange,
                         symbol=symbol, interval=interval
                     )
                 )
             # end if
 
             index = dt.datetime.fromtimestamp(index)
@@ -492,16 +492,10 @@
             return False
         # end if
     # end process
 
     async def start(self) -> None:
         """Connects to the socket service."""
 
-        location = os.path.split(database_file_path(self.database))[0]
-
-        if location:
-            os.makedirs(location, exist_ok=True)
-        # end if
-
         self.engine = self.engine or create_engine(self.database)
     # end start
 # end DatabaseCallback
```

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/database.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # data.py
 
 import os
 import time
 import datetime as dt
-from typing import (
-    Optional, Dict, Any, List,
-    Iterable, Union, Tuple
-)
+from typing import Dict, Any, Optional, Union, Iterable, List, Tuple
 
 import pandas as pd
 
-from sqlalchemy import create_engine, Engine, inspect, text
+from sqlalchemy import create_engine as _create_engine, Engine, inspect, text
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import DATE_TIME
 from crypto_screening.symbols import (
     symbol_to_parts, adjust_symbol, parts_to_symbol
 )
 from crypto_screening.market.screeners.base import BaseScreener
 
 __all__ = [
     "insert_database_record",
     "extract_database_record",
     "validate_database_engines",
-    "parts_database_table_name",
+    "parts_to_database_table_name",
     "database_table_name_to_parts",
     "extract_database_tables",
     "database_file_path",
     "await_database_creation",
     "await_all_databases_creation",
     "extract_data_into_screener_dataset",
-    "extract_database_length"
+    "extract_database_length",
+    "extract_database_table_record",
+    "create_engine",
+    "screeners_tables_names"
 ]
 
-def parts_database_table_name(
+def parts_to_database_table_name(
         name: str, exchange: str, symbol: str, interval: Optional[str] = None
 ) -> str:
     """
     Creates the database table name.
 
     :param name: The name for the data.
     :param exchange: The exchange name of the data.
@@ -50,15 +50,15 @@
 
     return (
         f"{name}__"
         f"{exchange}__"
         f"{'_'.join(symbol_to_parts(adjust_symbol(symbol)))}__"
         f"{interval or ''}"
     )
-# end parts_database_table_name
+# end parts_to_database_table_name
 
 def database_table_name_to_parts(table: str) -> Tuple[str, str, str, Optional[str]]:
     """
     Converts the table name to the naming parts.
 
     :param table: The table name.
 
@@ -139,15 +139,15 @@
     :param exchange: The exchange name of the data.
     :param symbol: The symbol of the data.
     :param dataset: The dataframe of the symbol.
     :param databases: The database engines.
     :param interval: The interval.
     """
 
-    table = parts_database_table_name(
+    table = parts_to_database_table_name(
         name=name, exchange=exchange, symbol=symbol, interval=interval
     )
 
     for path, engine in databases.items():
         location = os.path.split(database_file_path(path))[0]
 
         if location:
@@ -173,15 +173,15 @@
     :param symbol: The symbol of the data.
     :param databases: The database engines.
     :param interval: The interval.
 
     :return: The returned database lengths.
     """
 
-    table = parts_database_table_name(
+    table = parts_to_database_table_name(
         name=name, exchange=exchange,
         symbol=symbol, interval=interval
     )
 
     query = 'SELECT COUNT(' + DATE_TIME + ') FROM ' + table
 
     results: Dict[str, int] = {}
@@ -193,42 +193,31 @@
 
         connection.close()
     # end for
 
     return results
 # end extract_database_length
 
-def extract_database_record(
-        name: str,
-        exchange: str,
-        symbol: str,
+def extract_database_table_record(
+        table: str,
         databases: Dict[str, Engine],
-        interval: Optional[str] = None,
         length: Optional[int] = None,
         start: Optional[dt.datetime] = None
 ) -> Dict[str, pd.DataFrame]:
     """
     Extracts the data from the databases.
 
-    :param name: The name for the data.
-    :param exchange: The exchange name of the data.
-    :param symbol: The symbol of the data.
+    :param table: The table name.
     :param databases: The database engines.
     :param length: Yne length of the dataset to extract.
-    :param interval: The interval.
     :param start: The starting row.
 
     :return: The returned databases.
     """
 
-    table = parts_database_table_name(
-        name=name, exchange=exchange,
-        symbol=symbol, interval=interval
-    )
-
     query = 'SELECT * FROM ' + table
 
     if length is not None:
         if isinstance(start, int) and (start > 0):
             length_query = f" WHERE DateTime > {start}"
 
         else:
@@ -240,18 +229,60 @@
             f'(SELECT {length_query} FROM  ' + table + ')'
         )
 
     elif isinstance(start, int) and (start > 0):
         query += f' WHERE DateTime > {start}'
     # end if
 
-    return {
-        path: pd.read_sql(query, engine)
-        for path, engine in databases.items()
-    }
+    results: Dict[str, pd.DataFrame] = {}
+
+    for path, engine in databases.items():
+        dataset: pd.DataFrame = pd.read_sql(query, engine)
+
+        dataset.index = pd.DatetimeIndex(dataset[DATE_TIME])
+        del dataset[DATE_TIME]
+        dataset.index.name = DATE_TIME
+
+        results[path] = dataset
+    # end for
+
+    return results
+# end extract_database_record
+
+def extract_database_record(
+        name: str,
+        exchange: str,
+        symbol: str,
+        databases: Dict[str, Engine],
+        interval: Optional[str] = None,
+        length: Optional[int] = None,
+        start: Optional[dt.datetime] = None
+) -> Dict[str, pd.DataFrame]:
+    """
+    Extracts the data from the databases.
+
+    :param name: The name for the data.
+    :param exchange: The exchange name of the data.
+    :param symbol: The symbol of the data.
+    :param databases: The database engines.
+    :param length: Yne length of the dataset to extract.
+    :param interval: The interval.
+    :param start: The starting row.
+
+    :return: The returned databases.
+    """
+
+    table = parts_to_database_table_name(
+        name=name, exchange=exchange,
+        symbol=symbol, interval=interval
+    )
+
+    return extract_database_table_record(
+        table=table, databases=databases, length=length, start=start
+    )
 # end extract_database_record
 
 def extract_data_into_screener_dataset(
         screener: BaseScreener,
         path: str,
         engine: Engine,
         length: Optional[int] = None,
@@ -309,14 +340,32 @@
     # end for
 
     return tables
 # end extract_database_tables
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
+def create_engine(database: str) -> Engine:
+    """
+    Creates the engine for the database.
+
+    :param database: The path to the database.
+
+    :return: The engine.
+    """
+
+    location = os.path.split(database_file_path(database))[0]
+
+    if location:
+        os.makedirs(location, exist_ok=True)
+    # end if
+
+    return _create_engine(database)
+# end create_engine
+
 def validate_database_engines(data: Any) -> Dict[str, Engine]:
     """
     Validates the databases.
 
     :param data: The databases to validate.
 
     :return: The database engines.
@@ -332,8 +381,27 @@
         isinstance(path, str) and isinstance(engine, Engine)
         for path, engine in data.items()
     ):
         raise ValueError(f"databases must be: {Databases}, not: {data}")
     # end if
 
     return data
-# end validate_database_engines
+# end validate_database_engines
+
+def screeners_tables_names(screeners: Iterable[BaseScreener]) -> Dict[BaseScreener, str]:
+    """
+    Finds the table names for the screeners.
+
+    :param screeners: The screener objects
+
+    :return: The table names in the database for the screeners.
+    """
+
+    return {
+        screener: parts_to_database_table_name(
+            name=screener.NAME, exchange=screener.exchange,
+            symbol=screener.symbol, interval=(
+                screener.interval if (screener.NAME == "OHLCV") else None
+            )
+        ) for screener in screeners
+    }
+# end screeners_tables_names
```

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/sockets.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # sockets.py
 
 import json
 import asyncio
-import warnings
-import threading
 import datetime as dt
 from typing import Dict, Any, Optional, Union, Iterable, List, Tuple
 
-from crypto_screening.market.screeners.callbacks import SocketCallback
-from crypto_screening.market.screeners.base import BaseMarketScreener, BaseScreener
-from crypto_screening.collect.screeners import find_screeners
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
+from crypto_screening.market.screeners.callbacks import SocketCallback, Callback
+from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.market.screeners.collectors.base import ScreenersDataCollector
 
 __all__ = [
-    "SocketMarketScreener"
+    "SocketScreenersDataCollector",
+    "SocketCallback"
 ]
 
-class SocketMarketScreener(BaseMarketScreener):
+ScreenersTable = Dict[str, Dict[str, Dict[str, Dict[Optional[str], List[BaseScreener]]]]]
+
+class SocketScreenersDataCollector(ScreenersDataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
     Parameters:
 
+    - screeners:
+        The screener object to control and fill with data.
+
     - location:
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
@@ -53,14 +56,16 @@
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
+        :param address: The address for the socket.
+        :param port: The port for the socket.
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         """
 
         super().__init__(
             screeners=screeners, location=location,
@@ -99,31 +104,41 @@
                     (payload[SocketCallback.PROTOCOL] == SocketCallback.UDP_PROTOCOL) and
                     (payload[SocketCallback.FORMAT] == SocketCallback.CHUNKED_FORMAT)
                 ):
                     key = payload[SocketCallback.TIMESTAMP]
 
                     chunks = self.chunks.setdefault(key, [])
 
-                    chunks.append(payload[SocketCallback.DATA])
+                    chunks.append(payload[Callback.DATA])
 
                     if len(chunks) == payload[SocketCallback.CHUNKS]:
                         payload = json.loads(''.join(chunks[key]))
 
                         chunks.pop(key)
 
+                        packet = payload[Callback.DATA]
+
                         self.handle(
-                            payload[SocketCallback.DATA],
-                            name=payload[SocketCallback.KEY]
+                            name=payload[SocketCallback.KEY],
+                            data=packet[Callback.DATA],
+                            exchange=packet[Callback.EXCHANGE],
+                            symbol=packet[Callback.SYMBOL],
+                            interval=packet[Callback.INTERVAL]
                         )
                     # end if
 
                 else:
+                    packet = payload[Callback.DATA]
+
                     self.handle(
-                        payload[SocketCallback.DATA],
-                        name=payload[SocketCallback.KEY]
+                        name=payload[SocketCallback.KEY],
+                        data=packet[Callback.DATA],
+                        exchange=packet[Callback.EXCHANGE],
+                        symbol=packet[Callback.SYMBOL],
+                        interval=packet[Callback.INTERVAL]
                     )
                 # end for
             # end for
 
         except Exception as e:
             self.fail_record.setdefault(
                 writer.get_extra_info('peername'), []
@@ -142,53 +157,14 @@
         """
 
         while self.screening:
             await self.receive(reader=reader, writer=writer)
         # end while
     # end receiving_loop
 
-    def handle(self, data: Dict[str, Any], name: str) -> None:
-        """
-        Handles the data received from the connection.
-
-        :param data: The data to handle.
-        :param name: The name of the data.
-        """
-
-        screeners = find_screeners(
-            self.screeners,
-            exchange=data[SocketCallback.EXCHANGE],
-            symbol=data[SocketCallback.SYMBOL]
-        )
-
-        screeners = [
-            screener for screener in screeners
-            if screener.NAME == name
-        ]
-
-        if (
-            (SocketCallback.INTERVAL in data) and
-            isinstance(data[SocketCallback.INTERVAL], str)
-        ):
-            screeners = [
-                screener for screener in screeners
-                if (
-                    isinstance(screener, OHLCVScreener) and
-                    (screener.interval == data[SocketCallback.INTERVAL])
-                )
-            ]
-        # end if
-
-        for screener in screeners:
-            for index, row in data[SocketCallback.DATA]:
-                screener.market.loc[dt.datetime.fromtimestamp(index)] = row
-            # end for
-        # end for
-    # end handle
-
     def screening_loop(
             self,
             loop: Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
         """
         Runs the process of the price screening.
 
@@ -213,30 +189,8 @@
             await server.serve_forever()
         # end run
 
         self._screening = True
 
         asyncio.run(run())
     # end screening_loop
-
-    def start_screening(
-            self, loop: Optional[asyncio.AbstractEventLoop] = None
-    ) -> None:
-        """
-        Starts the screening process.
-
-        :param loop: The event loop.
-        """
-
-        if self.screening:
-            warnings.warn(f"Timeout screening of {self} is already running.")
-
-            return
-        # end if
-
-        self._screening_process = threading.Thread(
-            target=lambda: self.screening_loop(loop=loop)
-        )
-
-        self._screening_process.start()
-    # end start_screening
-# end SocketMarketScreener
+# end SocketScreenersDataCollector
```

### Comparing `crypto-screening-7.2.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.3.0/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/market/waiting.py` & `crypto-screening-7.3.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/process.py` & `crypto-screening-7.3.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/symbols.py` & `crypto-screening-7.3.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening/validate.py` & `crypto-screening-7.3.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.2.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.3.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.2.0
+Version: 7.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.2.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.3.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,9 +41,12 @@
 crypto_screening/market/screeners/combined.py
 crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/database.py
 crypto_screening/market/screeners/ohlcv.py
 crypto_screening/market/screeners/orderbook.py
 crypto_screening/market/screeners/orders.py
 crypto_screening/market/screeners/recorder.py
-crypto_screening/market/screeners/sockets.py
-crypto_screening/market/screeners/trades.py
+crypto_screening/market/screeners/trades.py
+crypto_screening/market/screeners/collectors/__init__.py
+crypto_screening/market/screeners/collectors/base.py
+crypto_screening/market/screeners/collectors/database.py
+crypto_screening/market/screeners/collectors/sockets.py
```

### Comparing `crypto-screening-7.2.0/pyproject.toml` & `crypto-screening-7.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.2.0'
+version = '7.3.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.2.0/setup.py` & `crypto-screening-7.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.2.0',
+        version='7.3.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

