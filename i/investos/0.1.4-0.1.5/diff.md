# Comparing `tmp/investos-0.1.4.tar.gz` & `tmp/investos-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.4.tar", max compression
+gzip compressed data, was "investos-0.1.5.tar", max compression
```

## Comparing `investos-0.1.4.tar` & `investos-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.4/LICENSE
--rw-r--r--   0        0        0      803 2023-07-18 21:12:06.647068 investos-0.1.4/README.md
--rw-r--r--   0        0        0       49 2023-07-20 19:36:40.097745 investos-0.1.4/investos/__init__.py
--rw-r--r--   0        0        0      238 2023-07-19 05:16:44.131001 investos-0.1.4/investos/portfolio/__init__.py
--rw-r--r--   0        0        0      337 2023-07-19 05:16:44.131177 investos-0.1.4/investos/portfolio/constraint_model/__init__.py
--rw-r--r--   0        0        0      557 2023-07-19 05:16:44.131684 investos-0.1.4/investos/portfolio/constraint_model/base_constraint.py
--rw-r--r--   0        0        0     1372 2023-07-19 05:16:44.131849 investos-0.1.4/investos/portfolio/constraint_model/leverage_constraint.py
--rw-r--r--   0        0        0     2660 2023-07-19 05:16:44.132122 investos-0.1.4/investos/portfolio/constraint_model/long_constraint.py
--rw-r--r--   0        0        0     1411 2023-07-19 05:16:44.132321 investos-0.1.4/investos/portfolio/constraint_model/trade_constraint.py
--rw-r--r--   0        0        0     2402 2023-07-19 05:16:44.132629 investos-0.1.4/investos/portfolio/constraint_model/weight_constraint.py
--rw-r--r--   0        0        0    13341 2023-07-19 05:16:44.132867 investos-0.1.4/investos/portfolio/controller.py
--rw-r--r--   0        0        0      168 2023-07-19 05:16:44.133026 investos-0.1.4/investos/portfolio/cost_model/__init__.py
--rw-r--r--   0        0        0     1850 2023-07-19 05:16:44.133180 investos-0.1.4/investos/portfolio/cost_model/base_cost.py
--rw-r--r--   0        0        0     2120 2023-07-19 05:16:44.133467 investos-0.1.4/investos/portfolio/cost_model/holding_cost.py
--rw-r--r--   0        0        0     4075 2023-07-19 05:16:44.133639 investos-0.1.4/investos/portfolio/cost_model/trading_cost.py
--rw-r--r--   0        0        0      104 2023-07-19 05:16:44.133795 investos-0.1.4/investos/portfolio/result/__init__.py
--rw-r--r--   0        0        0    12614 2023-07-19 05:16:44.133970 investos-0.1.4/investos/portfolio/result/base_result.py
--rw-r--r--   0        0        0      300 2023-07-19 05:16:44.134415 investos-0.1.4/investos/portfolio/result/forecast_result.py
--rw-r--r--   0        0        0     4532 2023-07-19 05:16:44.134575 investos-0.1.4/investos/portfolio/result/save_result.py
--rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.4/investos/portfolio/risk_model/__init__.py
--rw-r--r--   0        0        0     1306 2023-07-19 05:16:44.135169 investos-0.1.4/investos/portfolio/risk_model/base_risk.py
--rw-r--r--   0        0        0     2599 2023-07-19 05:16:44.135446 investos-0.1.4/investos/portfolio/risk_model/stat_factor_risk.py
--rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.4/investos/portfolio/strategy/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-19 05:16:44.136176 investos-0.1.4/investos/portfolio/strategy/base_strategy.py
--rw-r--r--   0        0        0     3990 2023-07-19 05:16:44.136619 investos-0.1.4/investos/portfolio/strategy/rank_long_short.py
--rw-r--r--   0        0        0     3887 2023-07-19 05:16:44.136789 investos-0.1.4/investos/portfolio/strategy/spo.py
--rw-r--r--   0        0        0     2249 2023-07-19 05:16:44.137255 investos-0.1.4/investos/util.py
--rw-r--r--   0        0        0     1908 2023-07-20 19:36:12.954666 investos-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 investos-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.5/LICENSE
+-rw-r--r--   0        0        0      803 2023-07-18 21:12:06.647068 investos-0.1.5/README.md
+-rw-r--r--   0        0        0       49 2023-07-20 19:52:49.628775 investos-0.1.5/investos/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-19 05:16:44.131001 investos-0.1.5/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-19 05:16:44.131177 investos-0.1.5/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-19 05:16:44.131684 investos-0.1.5/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1372 2023-07-19 05:16:44.131849 investos-0.1.5/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2660 2023-07-19 05:16:44.132122 investos-0.1.5/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1411 2023-07-19 05:16:44.132321 investos-0.1.5/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2402 2023-07-19 05:16:44.132629 investos-0.1.5/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    13341 2023-07-19 05:16:44.132867 investos-0.1.5/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      168 2023-07-19 05:16:44.133026 investos-0.1.5/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     1850 2023-07-19 05:16:44.133180 investos-0.1.5/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2120 2023-07-19 05:16:44.133467 investos-0.1.5/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4075 2023-07-19 05:16:44.133639 investos-0.1.5/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0      104 2023-07-19 05:16:44.133795 investos-0.1.5/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0    12614 2023-07-19 05:16:44.133970 investos-0.1.5/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      300 2023-07-19 05:16:44.134415 investos-0.1.5/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0     4532 2023-07-19 05:16:44.134575 investos-0.1.5/investos/portfolio/result/save_result.py
+-rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.5/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1306 2023-07-19 05:16:44.135169 investos-0.1.5/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2599 2023-07-19 05:16:44.135446 investos-0.1.5/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.5/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-19 05:16:44.136176 investos-0.1.5/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3990 2023-07-19 05:16:44.136619 investos-0.1.5/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     3887 2023-07-19 05:16:44.136789 investos-0.1.5/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     2249 2023-07-19 05:16:44.137255 investos-0.1.5/investos/util.py
+-rw-r--r--   0        0        0     1908 2023-07-20 19:52:38.569220 investos-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 investos-0.1.5/PKG-INFO
```

### Comparing `investos-0.1.4/LICENSE` & `investos-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/README.md` & `investos-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/constraint_model/base_constraint.py` & `investos-0.1.5/investos/portfolio/constraint_model/base_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/constraint_model/leverage_constraint.py` & `investos-0.1.5/investos/portfolio/constraint_model/leverage_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/constraint_model/long_constraint.py` & `investos-0.1.5/investos/portfolio/constraint_model/long_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/constraint_model/trade_constraint.py` & `investos-0.1.5/investos/portfolio/constraint_model/trade_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/constraint_model/weight_constraint.py` & `investos-0.1.5/investos/portfolio/constraint_model/weight_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/controller.py` & `investos-0.1.5/investos/portfolio/controller.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/cost_model/base_cost.py` & `investos-0.1.5/investos/portfolio/cost_model/base_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/cost_model/holding_cost.py` & `investos-0.1.5/investos/portfolio/cost_model/holding_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/cost_model/trading_cost.py` & `investos-0.1.5/investos/portfolio/cost_model/trading_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/result/base_result.py` & `investos-0.1.5/investos/portfolio/result/base_result.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/result/save_result.py` & `investos-0.1.5/investos/portfolio/result/save_result.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/risk_model/base_risk.py` & `investos-0.1.5/investos/portfolio/risk_model/base_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/risk_model/stat_factor_risk.py` & `investos-0.1.5/investos/portfolio/risk_model/stat_factor_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/strategy/base_strategy.py` & `investos-0.1.5/investos/portfolio/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/strategy/rank_long_short.py` & `investos-0.1.5/investos/portfolio/strategy/rank_long_short.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/portfolio/strategy/spo.py` & `investos-0.1.5/investos/portfolio/strategy/spo.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/investos/util.py` & `investos-0.1.5/investos/util.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.4/pyproject.toml` & `investos-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investos"
-version = "0.1.4"
+version = "0.1.5"
 description = "For investors who want to focus on generating alpha"
 authors = ["Charlie Reese"]
 license = "Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)"
 readme = "README.md"
 packages = [{include = "investos"}]
 homepage = "https://investos.io/"
 repository = "https://github.com/charliereese/investos"
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.9",
     "Topic :: Office/Business :: Financial :: Investment",
     "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 cvxpy = "^1.3.1"
 requests = "^2.31.0"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `investos-0.1.4/PKG-INFO` & `investos-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: investos
-Version: 0.1.4
+Version: 0.1.5
 Summary: For investors who want to focus on generating alpha
 Home-page: https://investos.io/
 License: Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)
 Keywords: investing,alpha,backtesting,portfolio,optimization
 Author: Charlie Reese
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
```

