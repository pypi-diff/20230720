# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.24.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.24.tar", last modified: Sat Feb  4 12:39:05 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.25.tar", last modified: Thu Jul 20 08:21:47 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.24.tar` & `basebot22-basebot_JustinGuese-0.3.25.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 12:39:05.862672 basebot22-basebot_JustinGuese-0.3.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-04 12:39:05.862672 basebot22-basebot_JustinGuese-0.3.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-04 12:38:56.000000 basebot22-basebot_JustinGuese-0.3.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 12:39:05.862672 basebot22-basebot_JustinGuese-0.3.24/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 12:38:56.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 12:38:56.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-02-04 12:38:56.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 12:39:05.862672 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-04 12:39:05.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-04 12:39:05.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 12:39:05.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-04 12:39:05.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-04 12:39:05.000000 basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-04 12:38:58.000000 basebot22-basebot_JustinGuese-0.3.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 12:39:05.862672 basebot22-basebot_JustinGuese-0.3.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 08:21:39.000000 basebot22-basebot_JustinGuese-0.3.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.24/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.24
+Version: 0.3.25
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.24/README.md` & `basebot22-basebot_JustinGuese-0.3.25/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.24/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.25/basebot22/basebot.py`

 * *Files 18% similar despite different names*

```diff
@@ -231,14 +231,55 @@
     def getEarningsRatings(self, ticker: str) -> dict:
         response = get(self.backendurl + '/data/earnings/ratings/?ticker=%s' % (ticker) , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting earnings ratings: ", response.text)
         response = response.json()
         response["timestamp"] = pd.to_datetime(response["timestamp"])
         return response
+    
+        
+    def backtest(self, df: pd.DataFrame, signalLookback: int = 0, startMoney: int = 10000):
+        # expects a pandas dataframe containing close column and a signal column
+        assert "close" in df, "close column not in dataframe"
+        assert "signal" in df, "signal column not in dataframe"
+        # assert for signal column that it only contains -1, 0, 1
+        assert df["signal"].isin([-1, 0, 1]).all(), "signal column contains values other than -1, 0, 1"
+
+        # now we can start
+        money = startMoney
+        shares = 0
+        portfolio = []
+        boughtAt = None
+        trades = []
+        backtestNrStocks = startMoney / df.iloc[0]["close"]
+        backtest = []
+
+        for i in range(signalLookback, len(df)):
+            decision = df.iloc[i-signalLookback:i]["signal"].median()
+            if decision == 1 and shares == 0:
+                # buy
+                howMany = money / df.iloc[i]["close"]
+                shares += howMany
+                money -= howMany * df.iloc[i]["close"]
+                boughtAt = df.iloc[i]["close"] * howMany
+            elif decision == -1 and shares > 0:
+                # sell
+                win = shares * df.iloc[i]["close"]
+                money += win
+                shares = 0
+                trades.append(win-boughtAt)
+            portfolio.append(money + shares * df.iloc[i]["close"])
+            backtest.append(backtestNrStocks * df.iloc[i]["close"])
+        # last day sell all
+        if shares > 0:
+            win = shares * df.iloc[i]["close"]
+            money += win
+            shares = 0
+            trades.append(win-boughtAt)
+        return portfolio[-1], backtest[-1], portfolio, backtest, trades
 
 if __name__ == "__main__":
     bot = BaseBot("testbot")
     print(bot.getPortfolio())
     bot.buy("AAPL", 2000, amountInUSD=True)
     print("portfolio after buy")
     print(bot.getPortfolio())
```

### Comparing `basebot22-basebot_JustinGuese-0.3.24/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.24
+Version: 0.3.25
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.24/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.25/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.24"
+version = "0.3.25"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

