# Comparing `tmp/crypto-screening-7.1.0.tar.gz` & `tmp/crypto-screening-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.1.0.tar", last modified: Thu Jul 20 08:09:16 2023, max compression
+gzip compressed data, was "crypto-screening-7.2.0.tar", last modified: Thu Jul 20 08:35:05 2023, max compression
```

## Comparing `crypto-screening-7.1.0.tar` & `crypto-screening-7.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.445438 crypto-screening-7.1.0/
--rw-rw-rw-   0        0        0       98 2023-07-20 08:09:15.000000 crypto-screening-7.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-20 08:09:16.445438 crypto-screening-7.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.1.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.284560 crypto-screening-7.1.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.325564 crypto-screening-7.1.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.1.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.1.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.355769 crypto-screening-7.1.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.1.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.1.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.1.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.1.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.368734 crypto-screening-7.1.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.1.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.1.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-7.1.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.1.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.1.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16701 2023-07-19 10:06:31.000000 crypto-screening-7.1.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.1.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.1.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.1.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.1.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.382911 crypto-screening-7.1.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-7.1.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.408913 crypto-screening-7.1.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.1.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.1.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.1.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.1.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.444438 crypto-screening-7.1.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-19 09:07:33.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11400 2023-07-19 10:06:31.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13822 2023-07-20 07:45:03.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/callbacks.py
--rw-rw-rw-   0        0        0    12819 2023-07-19 16:50:13.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    37568 2023-07-20 08:03:27.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19549 2023-07-20 08:03:27.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19048 2023-07-20 08:03:27.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     7002 2023-07-19 18:46:12.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/sockets.py
--rw-rw-rw-   0        0        0    19122 2023-07-20 08:03:27.000000 crypto-screening-7.1.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.1.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.1.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.1.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.1.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:09:16.299561 crypto-screening-7.1.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-20 08:09:16.000000 crypto-screening-7.1.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2023-07-20 08:09:16.000000 crypto-screening-7.1.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:09:16.000000 crypto-screening-7.1.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-20 08:09:16.000000 crypto-screening-7.1.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 08:09:16.000000 crypto-screening-7.1.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-20 08:09:15.000000 crypto-screening-7.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 08:09:16.445438 crypto-screening-7.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-20 08:09:10.000000 crypto-screening-7.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/
+-rw-rw-rw-   0        0        0       98 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.2.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.875692 crypto-screening-7.2.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.893697 crypto-screening-7.2.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.2.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.2.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.896696 crypto-screening-7.2.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.2.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.2.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.2.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.2.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.899698 crypto-screening-7.2.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16153 2023-07-18 21:23:25.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.2.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.2.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16701 2023-07-19 10:06:31.000000 crypto-screening-7.2.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.2.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.2.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.2.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.2.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.900722 crypto-screening-7.2.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19703 2023-07-18 21:44:11.000000 crypto-screening-7.2.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.903698 crypto-screening-7.2.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.2.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.911696 crypto-screening-7.2.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-19 09:07:33.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11400 2023-07-19 10:06:31.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13883 2023-07-20 08:20:28.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/callbacks.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12206 2023-07-18 21:43:26.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0     8925 2023-07-18 21:47:33.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     7002 2023-07-19 18:46:12.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/sockets.py
+-rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.2.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.2.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.2.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.2.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.2.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:35:05.890697 crypto-screening-7.2.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-20 08:35:05.000000 crypto-screening-7.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:35:05.912698 crypto-screening-7.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-20 08:34:57.000000 crypto-screening-7.2.0/setup.py
```

### Comparing `crypto-screening-7.1.0/PKG-INFO` & `crypto-screening-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.1.0
+Version: 7.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.1.0/README.md` & `crypto-screening-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/build.py` & `crypto-screening-7.2.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/assets.py` & `crypto-screening-7.2.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/exchanges.py` & `crypto-screening-7.2.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/orders.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/market/trades.py` & `crypto-screening-7.2.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/screeners.py` & `crypto-screening-7.2.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/collect/symbols.py` & `crypto-screening-7.2.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/dataset.py` & `crypto-screening-7.2.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/interval.py` & `crypto-screening-7.2.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/dynamic.py` & `crypto-screening-7.2.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/foundation/data.py` & `crypto-screening-7.2.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.2.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/foundation/state.py` & `crypto-screening-7.2.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.2.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/base.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,15 +451,16 @@
                         f"{column} {self.DATATYPES[type(value)]}"
                         for column, value in row.items()
                     )
 
                     self._session.execute(
                         text(
                             "CREATE TABLE " + table +
-                            f" ({DATE_TIME} TEXT, {creation})"
+                            f" ({DATE_TIME} TEXT, {creation}, "
+                            f"PRIMARY KEY ({DATE_TIME}));"
                         )
                     )
                 # end if
 
             else:
                 table = self.tables.setdefault(
                     (key, exchange, symbol, interval),
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/combined.py`

 * *Files 3% similar despite different names*

```diff
@@ -363,14 +363,29 @@
     def connect_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         for market in self.markets:
             market.connect_screeners()
         # end for
     # end connect_screeners
+
+    def merge_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
+        for ohlcv_screener in self.ohlcv_screeners:
+            for orderbook_screener in self.orderbook_screeners:
+                if (
+                    (ohlcv_screener.exchange == orderbook_screener.exchange) and
+                    (ohlcv_screener.symbol == orderbook_screener.symbol)
+                ):
+                    orderbook_screener.market = ohlcv_screener.orderbook_market
+                # end if
+            # end for
+        # end for
+    # end merge_screeners
 # end CombinedMarketScreener
 
 CATEGORY_RECORDER_CONSTRUCTOR_MATCHES = {
     OrderbookCategory: orderbook_market_screener,
     OHLCVCategory: ohlcv_market_screener,
     TradesCategory: trades_market_screener,
     OrdersCategory: orders_market_screener
@@ -429,14 +444,15 @@
     screener = CombinedMarketScreener(
         markets=markets, recorder=recorder or CombinedMarketRecorder(
             recorders=[market.recorder for market in markets]
         ), handler=handler, location=location, amount=amount, cancel=cancel,
         delay=delay, limited=limited, refresh=refresh
     )
 
+    screener.merge_screeners()
     screener.add_feeds(
         data=screener.recorder.structure(),
         fixed=fixed, parameters=parameters
     )
 
     return screener
 # end combined_market_screener
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/container.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/database.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,16 +532,15 @@
     :param timestamp: The time of the request.
     :param callbacks: The callbacks for the service.
 
     :return: The validation value.
     """
 
     if not await record_orderbook(
-        market=market, data=data, timestamp=timestamp,
-        callbacks=callbacks
+        market=market, data=data, timestamp=timestamp
     ):
         return False
     # end if
 
     exchange = find_string_value(
         value=data.exchange, values=market.keys()
     )
@@ -956,14 +955,29 @@
 
         return [
             screener for screener in self.screeners
             if isinstance(screener, OHLCVScreener)
         ]
     # end ohlcv_screeners
 
+    def merge_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
+        for ohlcv_screener in self.ohlcv_screeners:
+            for orderbook_screener in self.orderbook_screeners:
+                if (
+                    (ohlcv_screener.exchange == orderbook_screener.exchange) and
+                    (ohlcv_screener.symbol == orderbook_screener.symbol)
+                ):
+                    orderbook_screener.market = ohlcv_screener.orderbook_market
+                # end if
+            # end for
+        # end for
+    # end merge_screeners
+
     def connect_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         super().connect_screeners()
 
         for screener in self.screeners:
             if isinstance(screener, OHLCVScreener):
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,26 +199,32 @@
 
     dataset = (
         market.
         setdefault(exchange, {}).
         setdefault(symbol, create_orderbook_market_dataset())
     )
 
-    bids = data.book.bids.to_list()
-    asks = data.book.asks.to_list()
-
     try:
+        index = dt.datetime.fromtimestamp(timestamp)
+
+        if index in dataset.index:
+            return False
+        # end if
+
+        bids = data.book.bids.to_list()
+        asks = data.book.asks.to_list()
+
         data = {
             BIDS: float(bids[0][0]),
             ASKS: float(asks[0][0]),
             BIDS_VOLUME: float(bids[0][1]),
             ASKS_VOLUME: float(asks[0][1])
         }
 
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+        dataset.loc[index] = data
 
         for callback in callbacks or []:
             payload = callback_data(
                 data=[(timestamp, data)], exchange=exchange, symbol=symbol
             )
 
             await callback.record(payload, timestamp, key=OrderbookScreener.NAME)
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,20 +200,26 @@
     dataset = (
         market.
         setdefault(exchange, {}).
         setdefault(symbol, create_orders_market_dataset())
     )
 
     try:
+        index = dt.datetime.fromtimestamp(timestamp)
+
+        if index in dataset.index:
+            return False
+        # end if
+
         data = {
             BIDS: float(data.bid),
             ASKS: float(data.ask)
         }
 
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+        dataset.loc[index] = data
 
         for callback in callbacks or []:
             payload = callback_data(
                 data=[(timestamp, data)], exchange=exchange, symbol=symbol
             )
 
             await callback.record(payload, timestamp, key=OrdersScreener.NAME)
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/sockets.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.2.0/crypto_screening/market/screeners/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,21 +200,27 @@
     dataset = (
         market.
         setdefault(exchange, {}).
         setdefault(symbol, create_trades_market_dataset())
     )
 
     try:
+        index = dt.datetime.fromtimestamp(timestamp)
+
+        if index in dataset.index:
+            return False
+        # end if
+
         data = {
             AMOUNT: float(data.amount),
             PRICE: float(data.price),
             SIDE: data.side
         }
 
-        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = data
+        dataset.loc[index] = data
 
         for callback in callbacks or []:
             payload = callback_data(
                 data=[(timestamp, data)], exchange=exchange, symbol=symbol
             )
 
             await callback.record(payload, timestamp, key=TradesScreener.NAME)
```

### Comparing `crypto-screening-7.1.0/crypto_screening/market/waiting.py` & `crypto-screening-7.2.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/process.py` & `crypto-screening-7.2.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/symbols.py` & `crypto-screening-7.2.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening/validate.py` & `crypto-screening-7.2.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.2.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.1.0
+Version: 7.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.1.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.2.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.1.0/pyproject.toml` & `crypto-screening-7.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.1.0'
+version = '7.2.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.1.0/setup.py` & `crypto-screening-7.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.1.0',
+        version='7.2.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

