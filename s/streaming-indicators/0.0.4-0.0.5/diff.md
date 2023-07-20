# Comparing `tmp/streaming_indicators-0.0.4.tar.gz` & `tmp/streaming_indicators-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.4.tar", last modified: Fri Jun 23 06:27:14 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.5.tar", last modified: Thu Jul 20 13:43:51 2023, max compression
```

## Comparing `streaming_indicators-0.0.4.tar` & `streaming_indicators-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.084177 streaming_indicators-0.0.4/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3279 2023-06-23 06:27:14.084177 streaming_indicators-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2023-06-20 14:02:39.000000 streaming_indicators-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      847 2023-06-23 06:27:14.091168 streaming_indicators-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.010775 streaming_indicators-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.025770 streaming_indicators-0.0.4/src/streaming_indicators/
--rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.4/src/streaming_indicators/__init__.py
--rw-rw-rw-   0        0        0     7719 2023-06-20 15:46:51.000000 streaming_indicators-0.0.4/src/streaming_indicators/streaming_indicators.py
-drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.083158 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     3279 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 13:43:51.334892 streaming_indicators-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4296 2023-07-20 13:43:51.334892 streaming_indicators-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2539 2023-06-28 05:34:16.000000 streaming_indicators-0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      847 2023-07-20 13:43:51.334892 streaming_indicators-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 13:43:51.303639 streaming_indicators-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 13:43:51.303639 streaming_indicators-0.0.5/src/streaming_indicators/
+-rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.5/src/streaming_indicators/__init__.py
+-rw-rw-rw-   0        0        0     9872 2023-07-20 13:40:11.000000 streaming_indicators-0.0.5/src/streaming_indicators/streaming_indicators.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:43:51.334892 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     4296 2023-07-20 13:43:51.000000 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-20 13:43:51.000000 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:43:51.000000 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 13:43:51.000000 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-20 13:43:51.000000 streaming_indicators-0.0.5/src/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.4/LICENSE.txt` & `streaming_indicators-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.4/PKG-INFO` & `streaming_indicators-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
@@ -28,36 +28,76 @@
 
 ## Usage
 Each indicator is a class, and is statefull. It will have 3 main functions:
 1. Constructor: initialise all parameters such as period.
 2. update: To add new data point in the indicator computation. Returns the new value of the indicator.
 3. compute: Compute indicator value with a new data point, but don't update it's state. This is useful in some cases, for example, compute indictor on ltp, but don't update it.
 
-## Example
+## List of indicators (and usage)
+- Simple Moving Average (SMA)
 ```
-from streaming_indicators import SMA
+import streaming_indicators as si
 
-sma = SMA(10)
-for i in range(20):
-    print(i, sma.update(i))
+period = 14
+SMA = si.SMA(period)
+for idx, candle in candles.iterrows():
+    sma = SMA.update(candle['close'])
+    print(sma)
 ```
-
-## List of indicators
-- Simple Moving Average (SMA)
 - Exponential Moving Average (EMA)
+```
+period = 14
+EMA = si.EMA(period)
+for idx, candle in candles.iterrows():
+    ema = EMA.update(candle['close'])
+    print(ema)
+```
 - Relative Strength Index (RSI)
+```
+period = 14
+RSI = si.RSI(period)
+for idx, candle in candles.iterrows():
+    rsi = RSI.update(candle['close'])
+    print(rsi)
+```
 - True Range (TR)
 - Average True Range (ATR)
+```
+atr_period = 20
+ATR = si.ATR(atr_period)
+for idx, candle in candles.iterrows():
+    atr = ATR.update(candle)  # Assumes candle to have 'open',high','low','close' - TODO: give multiple inputs to update.
+    print(atr)
+```
 - Heikin Ashi Candlesticks (HeikinAshi)
 - Renko Bricks (Renko)
+```
+# For fixed brick size
+brick_size = 20
+Renko = si.Renko()
+for idx, candle in candles.iterrows():
+    bricks = Renko.update(candle['close'], brick_size)
+    print(bricks)
+```
+```
+# For brick size using ATR
+atr_period = 20
+ATR = si.ATR(atr_period)
+Renko = si.Renko()
+for idx, candle in candles.iterrows():
+    atr = ATR.update(candle)
+    print(atr)
+    bricks = Renko.update(candle['close'], atr)
+    print(bricks)
+```
 
 ## TODO
 - Not all indicators current support compute method.
 - Add documentation.
-- HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
+- HeikinAshi,ATR depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
 - Implement more indicators.
 MIT License
 
 Copyright (c) [2023] [Rishabh Gupta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `streaming_indicators-0.0.4/setup.cfg` & `streaming_indicators-0.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e34 0d0a 6175 7468 6f72   = 0.0.4..author
+00000030: 203d 2030 2e30 2e35 0d0a 6175 7468 6f72   = 0.0.5..author
 00000040: 203d 2052 6973 6861 6268 2047 7570 7461   = Rishabh Gupta
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2072 6973 6861 6268 6731 3939 3740 676d   rishabhg1997@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 6c69 6272 6172 7920 666f 7220 636f 6d70  library for comp
 000000a0: 7574 696e 6720 7465 6368 6e69 6361 6c20  uting technical
```

