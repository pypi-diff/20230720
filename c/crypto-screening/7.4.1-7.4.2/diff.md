# Comparing `tmp/crypto-screening-7.4.1.tar.gz` & `tmp/crypto-screening-7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.4.1.tar", last modified: Thu Jul 20 16:49:01 2023, max compression
+gzip compressed data, was "crypto-screening-7.4.2.tar", last modified: Thu Jul 20 19:14:32 2023, max compression
```

## Comparing `crypto-screening-7.4.1.tar` & `crypto-screening-7.4.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.279782 crypto-screening-7.4.1/
--rw-rw-rw-   0        0        0       98 2023-07-20 16:49:00.000000 crypto-screening-7.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-20 16:49:01.279782 crypto-screening-7.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.4.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.4.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.245782 crypto-screening-7.4.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.258782 crypto-screening-7.4.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.4.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.4.1/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.261783 crypto-screening-7.4.1/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.4.1/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.4.1/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.4.1/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.4.1/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.264782 crypto-screening-7.4.1/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.4.1/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.4.1/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-20 15:18:05.000000 crypto-screening-7.4.1/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.4.1/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.4.1/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.4.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.4.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.4.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.4.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.4.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.265782 crypto-screening-7.4.1/crypto_screening/market/
--rw-rw-rw-   0        0        0    21478 2023-07-20 14:19:49.000000 crypto-screening-7.4.1/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.268783 crypto-screening-7.4.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.4.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.4.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.4.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.4.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.275782 crypto-screening-7.4.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11649 2023-07-20 15:46:53.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.278782 crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-20 15:49:53.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4109 2023-07-20 15:57:21.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    20299 2023-07-20 16:48:21.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10926 2023-07-20 15:55:41.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.4.1/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.4.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.4.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.4.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.4.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:49:01.255782 crypto-screening-7.4.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-20 16:49:01.000000 crypto-screening-7.4.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1989 2023-07-20 16:49:01.000000 crypto-screening-7.4.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 16:49:01.000000 crypto-screening-7.4.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-20 16:49:01.000000 crypto-screening-7.4.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 16:49:01.000000 crypto-screening-7.4.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-20 16:49:00.000000 crypto-screening-7.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.4.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 16:49:01.279782 crypto-screening-7.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-20 16:48:53.000000 crypto-screening-7.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.042902 crypto-screening-7.4.2/
+-rw-rw-rw-   0        0        0       98 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-20 19:14:32.042902 crypto-screening-7.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.4.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.4.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.001896 crypto-screening-7.4.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.021896 crypto-screening-7.4.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.4.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.4.2/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.024896 crypto-screening-7.4.2/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.4.2/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.4.2/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.4.2/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.4.2/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.027896 crypto-screening-7.4.2/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-20 15:18:05.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.4.2/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.4.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.4.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.4.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.4.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.4.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.028897 crypto-screening-7.4.2/crypto_screening/market/
+-rw-rw-rw-   0        0        0    21478 2023-07-20 14:19:49.000000 crypto-screening-7.4.2/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.031896 crypto-screening-7.4.2/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.039900 crypto-screening-7.4.2/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    11649 2023-07-20 15:46:53.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.041900 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3645 2023-07-20 15:49:53.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4109 2023-07-20 15:57:21.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    20745 2023-07-20 19:14:02.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10926 2023-07-20 15:55:41.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.4.2/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.4.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.4.2/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.4.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.018927 crypto-screening-7.4.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1989 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.4.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:14:32.043900 crypto-screening-7.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-20 19:14:15.000000 crypto-screening-7.4.2/setup.py
```

### Comparing `crypto-screening-7.4.1/PKG-INFO` & `crypto-screening-7.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.4.1
+Version: 7.4.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.4.1/README.md` & `crypto-screening-7.4.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/build.py` & `crypto-screening-7.4.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/assets.py` & `crypto-screening-7.4.2/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/exchanges.py` & `crypto-screening-7.4.2/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/orders.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/market/trades.py` & `crypto-screening-7.4.2/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/screeners.py` & `crypto-screening-7.4.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/collect/symbols.py` & `crypto-screening-7.4.2/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/dataset.py` & `crypto-screening-7.4.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/interval.py` & `crypto-screening-7.4.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/dynamic.py` & `crypto-screening-7.4.2/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/foundation/data.py` & `crypto-screening-7.4.2/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.4.2/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/foundation/state.py` & `crypto-screening-7.4.2/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.4.2/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/base.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/container.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,15 +498,15 @@
         :return: The data.
         """
 
         screeners = []
 
         for screener in self.screeners:
             if (
-                ((screener.exchange == exchange) or exchange is None) and
+                ((screener.exchange == exchange) or (exchange is None)) and
                 ((screener.symbol == symbol) or (symbol is None)) and
                 isinstance(screener, base or BaseScreener) and
                 (
                     (screener.interval == interval) if (
                         isinstance(screener, OHLCVScreener) and
                         (interval is not None)
                     ) else True
@@ -548,78 +548,85 @@
     for screener in screeners:
         interval = (
             screener.interval
             if isinstance(screener, OHLCVScreener) else
             None
         )
 
-        (
-            table.
-            setdefault(type(screener), {}).
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table.
-            setdefault(type(screener), {}).
-            setdefault(screener.exchange, {}).
-            setdefault(None, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table.
-            setdefault(type(screener), {}).
-            setdefault(None, {}).
-            setdefault(screener.symbol, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table[type(screener)].
-            setdefault(None, {}).
-            setdefault(None, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
+        lists = [
+            (
+                table.
+                setdefault(type(screener), {}).
+                setdefault(screener.exchange, {}).
+                setdefault(screener.symbol, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(type(screener), {}).
+                setdefault(screener.exchange, {}).
+                setdefault(None, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(type(screener), {}).
+                setdefault(None, {}).
+                setdefault(screener.symbol, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(type(screener), {}).
+                setdefault(None, {}).
+                setdefault(None, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(type(screener), {}).
+                setdefault(None, {}).
+                setdefault(None, {}).
+                setdefault(None, [])
+            ),
+            (
+                table.
+                setdefault(None, {}).
+                setdefault(screener.exchange, {}).
+                setdefault(screener.symbol, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(None, {}).
+                setdefault(screener.exchange, {}).
+                setdefault(None, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(None, {}).
+                setdefault(None, {}).
+                setdefault(screener.symbol, {}).
+                setdefault(interval, [])
+            ),
+            (
+                table.
+                setdefault(None, {}).
+                setdefault(None, {}).
+                setdefault(None, {}).
+                setdefault(interval, [])
+            )
+        ]
 
-        (
-            table.
-            setdefault(None, {}).
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table.
-            setdefault(None, {}).
-            setdefault(screener.exchange, {}).
-            setdefault(None, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table.
-            setdefault(None, {}).
-            setdefault(None, {}).
-            setdefault(screener.symbol, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
-        (
-            table.
-            setdefault(None, {}).
-            setdefault(None, {}).
-            setdefault(None, {}).
-            setdefault(interval, []).
-            append(screener)
-        )
+        for screeners_list in lists:
+            if screener not in screeners_list:
+                screeners_list.append(screener)
+            # end if
+        # end for
     # end for
 
     return table
 # end screeners_table
 
 class FixedScreenersContainer(ScreenersContainer):
     """
@@ -684,15 +691,15 @@
         :param symbol: The ticker name.
         :param interval: The interval for the search.
 
         :return: The data.
         """
 
         try:
-            return self._table[base][exchange][symbol][interval]
+            return list(self._table[base][exchange][symbol][interval])
 
         except KeyError:
             raise ValueError(
                 f"Cannot find screeners  matching to "
                 f"type - {base}, exchange - {exchange}, "
                 f"symbol - {symbol}, interval - {interval} "
                 f"inside {repr(self)}"
```

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/database.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.4.2/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/market/waiting.py` & `crypto-screening-7.4.2/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/process.py` & `crypto-screening-7.4.2/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/symbols.py` & `crypto-screening-7.4.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening/validate.py` & `crypto-screening-7.4.2/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.4.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.4.1
+Version: 7.4.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.4.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.4.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.1/pyproject.toml` & `crypto-screening-7.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.4.1'
+version = '7.4.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.4.1/setup.py` & `crypto-screening-7.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.4.1',
+        version='7.4.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

