# Comparing `tmp/investos-0.1.3.tar.gz` & `tmp/investos-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.3.tar", max compression
+gzip compressed data, was "investos-0.1.4.tar", max compression
```

## Comparing `investos-0.1.3.tar` & `investos-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.3/LICENSE
--rw-r--r--   0        0        0      806 2023-06-23 19:47:27.617845 investos-0.1.3/README.md
--rw-r--r--   0        0        0       48 2023-06-22 23:44:52.403440 investos-0.1.3/investos/__init__.py
--rw-r--r--   0        0        0      237 2023-06-22 23:46:12.605021 investos-0.1.3/investos/portfolio/__init__.py
--rw-r--r--   0        0        0      336 2023-06-22 23:46:19.538745 investos-0.1.3/investos/portfolio/constraint_model/__init__.py
--rw-r--r--   0        0        0      554 2023-06-23 07:08:21.486031 investos-0.1.3/investos/portfolio/constraint_model/base_constraint.py
--rw-r--r--   0        0        0     1377 2023-06-22 23:46:19.540939 investos-0.1.3/investos/portfolio/constraint_model/leverage_constraint.py
--rw-r--r--   0        0        0     2673 2023-06-22 23:46:19.542231 investos-0.1.3/investos/portfolio/constraint_model/long_constraint.py
--rw-r--r--   0        0        0     1366 2023-06-22 23:46:19.542979 investos-0.1.3/investos/portfolio/constraint_model/trade_constraint.py
--rw-r--r--   0        0        0     2400 2023-06-22 23:46:19.543696 investos-0.1.3/investos/portfolio/constraint_model/weight_constraint.py
--rw-r--r--   0        0        0    12997 2023-06-23 17:09:46.339230 investos-0.1.3/investos/portfolio/controller.py
--rw-r--r--   0        0        0      167 2023-06-22 23:46:24.228466 investos-0.1.3/investos/portfolio/cost_model/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-23 07:07:49.043269 investos-0.1.3/investos/portfolio/cost_model/base_cost.py
--rw-r--r--   0        0        0     2151 2023-06-23 06:37:22.698101 investos-0.1.3/investos/portfolio/cost_model/holding_cost.py
--rw-r--r--   0        0        0     4085 2023-06-23 07:07:33.965063 investos-0.1.3/investos/portfolio/cost_model/trading_cost.py
--rw-r--r--   0        0        0       51 2023-06-23 07:06:43.880398 investos-0.1.3/investos/portfolio/result/__init__.py
--rw-r--r--   0        0        0     7515 2023-06-23 17:13:07.013409 investos-0.1.3/investos/portfolio/result/base_result.py
--rw-r--r--   0        0        0      297 2023-06-23 17:05:36.524816 investos-0.1.3/investos/portfolio/result/forecast_result.py
--rw-r--r--   0        0        0      116 2023-06-22 23:46:36.366559 investos-0.1.3/investos/portfolio/risk_model/__init__.py
--rw-r--r--   0        0        0     1314 2023-06-23 07:01:34.207139 investos-0.1.3/investos/portfolio/risk_model/base_risk.py
--rw-r--r--   0        0        0     2648 2023-06-23 07:00:56.552682 investos-0.1.3/investos/portfolio/risk_model/stat_factor_risk.py
--rw-r--r--   0        0        0      159 2023-06-22 23:46:41.515323 investos-0.1.3/investos/portfolio/strategy/__init__.py
--rw-r--r--   0        0        0     1278 2023-06-23 07:02:51.365518 investos-0.1.3/investos/portfolio/strategy/base_strategy.py
--rw-r--r--   0        0        0     3937 2023-06-23 07:03:19.040651 investos-0.1.3/investos/portfolio/strategy/rank_long_short.py
--rw-r--r--   0        0        0     3848 2023-06-23 07:04:39.977541 investos-0.1.3/investos/portfolio/strategy/spo.py
--rw-r--r--   0        0        0     1896 2023-06-22 23:44:52.404096 investos-0.1.3/investos/util.py
--rw-r--r--   0        0        0      726 2023-06-23 21:10:22.552461 investos-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 investos-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.4/LICENSE
+-rw-r--r--   0        0        0      803 2023-07-18 21:12:06.647068 investos-0.1.4/README.md
+-rw-r--r--   0        0        0       49 2023-07-20 19:36:40.097745 investos-0.1.4/investos/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-19 05:16:44.131001 investos-0.1.4/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-19 05:16:44.131177 investos-0.1.4/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-19 05:16:44.131684 investos-0.1.4/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1372 2023-07-19 05:16:44.131849 investos-0.1.4/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2660 2023-07-19 05:16:44.132122 investos-0.1.4/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1411 2023-07-19 05:16:44.132321 investos-0.1.4/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2402 2023-07-19 05:16:44.132629 investos-0.1.4/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    13341 2023-07-19 05:16:44.132867 investos-0.1.4/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      168 2023-07-19 05:16:44.133026 investos-0.1.4/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     1850 2023-07-19 05:16:44.133180 investos-0.1.4/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2120 2023-07-19 05:16:44.133467 investos-0.1.4/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4075 2023-07-19 05:16:44.133639 investos-0.1.4/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0      104 2023-07-19 05:16:44.133795 investos-0.1.4/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0    12614 2023-07-19 05:16:44.133970 investos-0.1.4/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      300 2023-07-19 05:16:44.134415 investos-0.1.4/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0     4532 2023-07-19 05:16:44.134575 investos-0.1.4/investos/portfolio/result/save_result.py
+-rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.4/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1306 2023-07-19 05:16:44.135169 investos-0.1.4/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2599 2023-07-19 05:16:44.135446 investos-0.1.4/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.4/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-19 05:16:44.136176 investos-0.1.4/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3990 2023-07-19 05:16:44.136619 investos-0.1.4/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     3887 2023-07-19 05:16:44.136789 investos-0.1.4/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     2249 2023-07-19 05:16:44.137255 investos-0.1.4/investos/util.py
+-rw-r--r--   0        0        0     1908 2023-07-20 19:36:12.954666 investos-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 investos-0.1.4/PKG-INFO
```

### Comparing `investos-0.1.3/LICENSE` & `investos-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.3/README.md` & `investos-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
 # InvestOS
 
 **InvestOS** (/InvEst əʊˈes/) is a Python library for investors who want to focus on generating alpha. As it stands today, it provides reliable backtesting and portfolio optimization software for investors... but we have bigger ambitions!
 
-As mentioned in our [first blog article](https://blog.investos.io/why-we-created-investos/): _“From the start, our goal has been to support all possible optimization strategies and backtesting requirements through flexible, extensible code, while prioritizing reliability and ease-of-use. Once we feel we’ve achieved that goal as it pertains to portfolio optimization and backtesting, we plan to begin productizing other (non-IP) parts of investors’ alpha-generation process.”_
+As mentioned in our [first blog article](https://blog.investos.io/why-we-created-investos/):
+
+> From the start, our goal has been to support all possible optimization strategies and backtesting requirements through flexible, extensible code, while prioritizing reliability and ease-of-use.
+> Once we feel we’ve achieved that goal as it pertains to portfolio optimization and backtesting, we plan to begin productizing other (non-IP) parts of investors’ alpha-generation process.
 
 For more information, visit [investos.io](https://investos.io).
```

### Comparing `investos-0.1.3/investos/portfolio/constraint_model/base_constraint.py` & `investos-0.1.4/investos/portfolio/constraint_model/base_constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from investos.util import values_in_time
 
 import cvxpy as cvx
 import numpy as np
 
+
 # http://web.cvxr.com/cvx/doc/basics.html#constraints
 class BaseConstraint(object):
     """
     Base class for constraint objects used in convex portfolio optimization strategies.
 
     Subclass `BaseConstraint`, and create your own `weight_expr` method to create custom constraints.
     """
-    def __init__(self, **kwargs):
-        self.optimizer = None # Set during Optimizer initialization
 
+    def __init__(self, **kwargs):
+        self.optimizer = None  # Set during Optimizer initialization
 
     def weight_expr(self, t, w_plus, z, v):
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `investos-0.1.3/investos/portfolio/constraint_model/leverage_constraint.py` & `investos-0.1.4/investos/portfolio/constraint_model/leverage_constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import cvxpy as cvx
 
 from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
+
 class MaxLeverageConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the (absolute) leverage of the portfolio.
 
-    E.g. For leverage of 2.0x, a portfolio with 100MM net value 
-    (i.e. the portfolio value if it were converted into cash, 
-    ignoring liquidation / trading costs) 
+    E.g. For leverage of 2.0x, a portfolio with 100MM net value
+    (i.e. the portfolio value if it were converted into cash,
+    ignoring liquidation / trading costs)
     could have 200MM of (combined long and short) exposure.
 
     Parameters
     ----------
     limit : float, optional
         The minimum weight of each asset in the portfolio. Defaults to -0.05.
 
     **kwargs :
         Additional keyword arguments.
     """
-    
+
     def __init__(self, limit: float = 2.0, **kwargs):
         self.limit = limit
 
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
@@ -43,8 +44,8 @@
             Value of portfolio at period t
 
         Returns
         -------
         series
             The holding constraints based on the portfolio leverage after trades.
         """
-        return cvx.sum(cvx.abs(w_plus[:-1])) <= self.limit
+        return cvx.sum(cvx.abs(w_plus[:-1])) <= self.limit
```

### Comparing `investos-0.1.3/investos/portfolio/constraint_model/long_constraint.py` & `investos-0.1.4/investos/portfolio/constraint_model/long_constraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 import cvxpy as cvx
 
 from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
+
 class LongOnlyConstraint(BaseConstraint):
     """
     A constraint that enforces no short positions. Including no short cash position.
 
     Parameters
     ----------
     **kwargs :
         Additional keyword arguments.
     """
-    
+
     def __init__(self, **kwargs):
         pass
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -49,19 +49,18 @@
     A constraint that enforces no short cash positions.
 
     Parameters
     ----------
     **kwargs :
         Additional keyword arguments.
     """
-    
+
     def __init__(self, **kwargs):
         pass
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -89,19 +88,18 @@
     A constraint that enforces equal long and short exposure.
 
     Parameters
     ----------
     **kwargs :
         Additional keyword arguments.
     """
-    
+
     def __init__(self, **kwargs):
         pass
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -117,8 +115,8 @@
             Value of portfolio at period t
 
         Returns
         -------
         series
             The holding constraints based on the equal long and short exposure constraint.
         """
-        return sum(w_plus[:-1]) == 0.0
+        return sum(w_plus[:-1]) == 0.0
```

### Comparing `investos-0.1.3/investos/portfolio/constraint_model/trade_constraint.py` & `investos-0.1.4/investos/portfolio/constraint_model/trade_constraint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import numpy as np
 import cvxpy as cvx
 
 from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
+
 class MaxTradeConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the (absolute) max trade size (as a weight, or fraction, of daily volume).
 
     Parameters
     ----------
     limit : float, optional
         The limit on the (absolute) max trade size (as a weight, or fraction, of volume for period `t`).
 
     **kwargs :
         Additional keyword arguments.
     """
-    
+
     def __init__(self, limit: float = 1.0, **kwargs):
         self.limit = limit
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -40,11 +40,15 @@
             Value of portfolio at period t
 
         Returns
         -------
         series
             The holding constraints based on the max trade constraint.
         """
-        return cvx.abs(z[:-1]) * v <= np.array(
-                values_in_time(self.optimizer.forecast['volume'], t) *
-                values_in_time(self.optimizer.forecast['price'], t)
-            ) * self.limit
+        return (
+            cvx.abs(z[:-1]) * v
+            <= np.array(
+                values_in_time(self.optimizer.forecast["volume"], t)
+                * values_in_time(self.optimizer.forecast["price"], t)
+            )
+            * self.limit
+        )
```

### Comparing `investos-0.1.3/investos/portfolio/constraint_model/weight_constraint.py` & `investos-0.1.4/investos/portfolio/constraint_model/weight_constraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
+
 class MaxWeightConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the weight of each asset in a portfolio.
 
     Parameters
     ----------
     limit : float, optional
@@ -15,18 +16,18 @@
 
     Methods
     -------
     weight_expr(self, t, w_plus, z, v):
         Returns a series of holding constraints based on the portfolio weights after trades.
 
     """
+
     def __init__(self, limit: float = 0.025, **kwargs):
         self.limit = limit
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -63,18 +64,18 @@
 
     Methods
     -------
     weight_expr(self, t, w_plus, z, v):
         Returns a series of holding constraints based on the portfolio weights after trades.
 
     """
+
     def __init__(self, limit: float = -0.025, **kwargs):
         self.limit = limit
 
-
     def weight_expr(self, t, w_plus, z, v):
         """
         Returns a series of holding constraints.
 
         Parameters
         ----------
         t : datetime
@@ -90,8 +91,8 @@
             Value of portfolio at period t
 
         Returns
         -------
         series
             The holding constraints based on the portfolio weights after trades.
         """
-        return w_plus[:-1] >= self.limit
+        return w_plus[:-1] >= self.limit
```

### Comparing `investos-0.1.3/investos/portfolio/controller.py` & `investos-0.1.4/investos/portfolio/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,42 @@
 from typing import Callable
 
 import investos.portfolio.strategy as strategy
 from investos.portfolio.strategy import BaseStrategy, RankLongShort
 import investos.portfolio.result as result
 import investos.util as util
 
-class Controller():
+
+class Controller:
     """Container class that runs backtests using passed-in portfolio optimization `strategy` (see :py:class:`~investos.portfolio.strategy.base_strategy.BaseStrategy`), then saves results into passed-in `result` (see :py:class:`~investos.backtest.result.Result`) class.
-    
+
     Parameters
     ----------
     df_forecast : pd.DataFrame
         DataFrame of forecast asset returns for backtest period.
 
-        Expected columns: 
-        asset (unique ID/ticker), 
-        date (datetime), 
+        Expected columns:
+        asset (unique ID/ticker),
+        date (datetime),
         return (float)
-    
+
     df_actual : pd.DataFrame
         DataFrame of actual asset returns for backtest period. Used to create forecasts for std_dev, spread, and volume if forecasts not given.
 
-        Expected columns: 
-        asset (unique ID/ticker), 
-        date (datetime), 
-        price (float), 
-        return (float), 
-        volume (of shares traded, float), 
+        Expected columns:
+        asset (unique ID/ticker),
+        date (datetime),
+        price (float),
+        return (float),
+        volume (of shares traded, float),
         spread (float)
 
     strategy : :py:class:`~investos.portfolio.strategy.base_strategy.BaseStrategy`
         Optimization strategy used by backtester. Used to determine what trades to make at each forecast time period.
-    
+
     backtest_model : :py:class:`~investos.portfolio.result.BaseResult`
         Stores result from simulated backtest, and contains convenience properties and methods for reporting.
 
     initial_portfolio : pd.DataFrame, optional
         Initial portfolio values in dollars (or other currency), not in weights.
 
     aum : float, optional
@@ -47,15 +48,15 @@
 
     df_categories : pd.DataFrame, optional
         Additional category data for assets. Used by certain optimization strategies.
 
     config : dict, optional
         Configuration parameters.
 
-    **kwargs : 
+    **kwargs :
         Additional keyword arguments.
 
     Attributes
     ----------
     config : dict
         Configuration parameters after merging with base configuration.
 
@@ -77,15 +78,15 @@
     after_step : [Callable]
         Callable objects, that are passed a reference to Controller (i.e. self), that run at end of each step through time
 
     Methods
     -------
     generate_positions(self):
         Optimizes the portfolio and backtests it. Returns :py:class:`~investos.portfolio.result.BaseResult` object.
-    
+
     pivot_and_fill(self, df: pd.DataFrame, values: str, columns='asset', index='date', fill_method='bfill'):
         Pivots and fills the DataFrame based on the provided values, columns, and index.
 
     create_forecast(self, df_forecast: pd.DataFrame, col_name: str = 'std_dev'):
         Creates a forecast DataFrame based on the provided df_forecast and col_name.
 
     create_price(self, df_return: pd.DataFrame):
@@ -105,231 +106,248 @@
         Returns:
             h_next: pandas Series portfolio after returns propagation (for t to t+1 period)
             u: pandas Series trades vector with simulated cash balance
 
     get_initial_t(self):
         Gets the initial time period for the backtest.
     """
-    
+
     BASE_CONFIG = {
         "forecast": {
             "std_dev": {
-                "calc_from_n_prev_periods": 100, # Calc from actual_df if not passed in
+                "calc_from_n_prev_periods": 100,  # Calc from actual_df if not passed in
             },
             "half_spread": {
-                "calc_from_n_prev_periods": 100, # Calc from actual_df if not passed in
+                "calc_from_n_prev_periods": 100,  # Calc from actual_df if not passed in
             },
             "volume": {
-                "calc_from_n_prev_periods": 100, # Calc from actual_df if not passed in
+                "calc_from_n_prev_periods": 100,  # Calc from actual_df if not passed in
             },
         },
-        "borrowing": {
-            "interest_rate": 0.005,
-            "short_rate": 0.005
-        },
+        "borrowing": {"interest_rate": 0.005, "short_rate": 0.005},
     }
 
     def __init__(
-        self, 
+        self,
         df_forecast: pd.DataFrame,
         df_actual: pd.DataFrame = None,
         strategy: BaseStrategy = RankLongShort,
         backtest_model: result.BaseResult = None,
-        initial_portfolio: pd.DataFrame = None, # In dollars (or other currency), not in weights
+        initial_portfolio: pd.DataFrame = None,  # In dollars (or other currency), not in weights
         aum: float = 100_000_000,
-        df_categories: pd.DataFrame = None, 
-        start_date = None,
-        end_date = None,
+        df_categories: pd.DataFrame = None,
+        start_date=None,
+        end_date=None,
         after_step: [Callable] = [],
         config: dict = {},
-        **kwargs):
-        
+        **kwargs,
+    ):
         self.config = util.deep_dict_merge(self.BASE_CONFIG, config)
 
         self._init_strategy(strategy)
         self._init_backtest_model(backtest_model, df_actual)
 
         self.forecast = {}
-        df_forecast = self._clip_forecast_df_for_dates(start_date, end_date, df_forecast)
-        
+        df_forecast = self._clip_forecast_df_for_dates(
+            start_date, end_date, df_forecast
+        )
+
         self._init_df_actual(df_actual)
         self._init_df_forecast(df_forecast)
 
-        self._set_cash_return_for_each_period(self.forecast['return'])
+        self._set_cash_return_for_each_period(self.forecast["return"])
         self.create_initial_portfolio(initial_portfolio, aum)
         self._set_references_back_to_optimizer()
 
-        self.after_step = after_step # Hook for callables at end of each step in t
-
-
-    def pivot_and_fill(self, df, values, columns='asset', index='date', fill_method='bfill'):
-        return pd.pivot(
-            df, values=values, columns=columns, index=index
-        ).fillna(method=fill_method)
+        self.after_step = after_step  # Hook for callables at end of each step in t
 
+    def pivot_and_fill(
+        self, df, values, columns="asset", index="date", fill_method="bfill"
+    ):
+        return pd.pivot(df, values=values, columns=columns, index=index).fillna(
+            method=fill_method
+        )
 
-    def create_forecast(self, df_forecast, col_name='std_dev'):
+    def create_forecast(self, df_forecast, col_name="std_dev"):
         if col_name in df_forecast.columns:
             return df_forecast
-        elif col_name == 'std_dev':
-            return df_forecast[['date', 'asset']].merge(
-                self.actual['return'][self.actual['return'].index < self.forecast['date']['start']].tail(
-                    self.config['forecast'][col_name]['calc_from_n_prev_periods']
-                ).std().rename(col_name).reset_index(), 
-                how='left', 
-                on='asset'
+        elif col_name == "std_dev":
+            return df_forecast[["date", "asset"]].merge(
+                self.actual["return"][
+                    self.actual["return"].index < self.forecast["date"]["start"]
+                ]
+                .tail(self.config["forecast"][col_name]["calc_from_n_prev_periods"])
+                .std()
+                .rename(col_name)
+                .reset_index(),
+                how="left",
+                on="asset",
             )
         else:
-            return df_forecast[['date', 'asset']].merge(
-                 self.actual[col_name][self.actual[col_name].index < self.forecast['date']['start']].tail(
-                    self.config['forecast'][col_name]['calc_from_n_prev_periods']
-                ).mean().rename(col_name).reset_index(), 
-                how='left', 
-                on='asset'
+            return df_forecast[["date", "asset"]].merge(
+                self.actual[col_name][
+                    self.actual[col_name].index < self.forecast["date"]["start"]
+                ]
+                .tail(self.config["forecast"][col_name]["calc_from_n_prev_periods"])
+                .mean()
+                .rename(col_name)
+                .reset_index(),
+                how="left",
+                on="asset",
             )
 
-
     def create_price(self, df_return):
-        last_historical_prices = (
-            self.actual['price']
-                .loc[self.actual['price'][self.actual['price'].index < self.forecast['date']['start']].index.max()]
-            )
-        
+        last_historical_prices = self.actual["price"].loc[
+            self.actual["price"][
+                self.actual["price"].index < self.forecast["date"]["start"]
+            ].index.max()
+        ]
+
         # Make geometric - add 1
         df = df_return + 1
-        
+
         # Geometric cumulative mean
         df = df.cumprod()
-        
+
         # Multiply geometric return factors by last historical value
         return df * last_historical_prices
-       
 
     def create_initial_portfolio(self, initial_portfolio, aum):
         if initial_portfolio is None:
-            initial_portfolio = pd.Series(index=self.forecast['return'].columns, data=0)
+            initial_portfolio = pd.Series(index=self.forecast["return"].columns, data=0)
             initial_portfolio["cash"] = aum
 
         self.initial_portfolio = initial_portfolio
 
-
     def generate_positions(self):
         print("Optimizing...")
 
-        self.backtest = self.backtest_model()
+        self.backtest = self.backtest_model(
+            start_date=self.forecast["date"]["start"],
+            end_date=self.forecast["date"]["end"],
+        )
 
         # Submit initial position
         t = self.get_initial_t()
-        u = pd.Series(index=self.initial_portfolio.index, data=0) # No trades at time 0
-        h_next = self.initial_portfolio # Includes cash
+        u = pd.Series(index=self.initial_portfolio.index, data=0)  # No trades at time 0
+        h_next = self.initial_portfolio  # Includes cash
         self.backtest.save_position(t, u, h_next)
 
         # Walk through time and calculate future trades, estimated and actual costs and returns, and resulting positions
-        for t in self.forecast['return'].index:
+        for t in self.forecast["return"].index:
             u = self.strategy.generate_trade_list(h_next, t)
             h_next, u = self.get_actual_positions_for_t(h_next, u, t)
             self.backtest.save_position(t, u, h_next)
-            
-            for func in self.after_step: # Run after_step hooks
+
+            for func in self.after_step:  # Run after_step hooks
                 func(self, t, u, h_next)
 
         print("Done simulating.")
-        
-        return self.backtest
 
+        return self.backtest
 
-    def get_actual_positions_for_t(self, h, u, t):        
+    def get_actual_positions_for_t(self, h, u, t):
         h_plus = h + u
-        
-        costs = [cost.actual_cost(t, h_plus=h_plus, u=u) for cost in self.strategy.costs]
+
+        costs = [
+            cost.actual_cost(t, h_plus=h_plus, u=u) for cost in self.strategy.costs
+        ]
 
         u["cash"] = -sum(u[u.index != "cash"]) - sum(costs)
         h_plus["cash"] = h["cash"] + u["cash"]
 
-        h_next = self.actual['return'].loc[t] * h_plus + h_plus
+        h_next = self.actual["return"].loc[t] * h_plus + h_plus
 
         zero_threshold = 0.00001
         h_next[np.abs(h_next) < zero_threshold] = 0
         u[np.abs(u) < zero_threshold] = 0
-        
-        return h_next, u
 
+        return h_next, u
 
     def get_initial_t(self):
         median_time_delta = statistics.median(
-            self.forecast['return'].index[1:5] - self.forecast['return'].index[0:4]
+            self.forecast["return"].index[1:5] - self.forecast["return"].index[0:4]
         )
 
-        return self.forecast['return'].index[0] - median_time_delta
-
-
-    def _set_cash_return_for_each_period(self, df): 
-        df['cash'] = self.config['borrowing']['interest_rate']
+        return self.forecast["return"].index[0] - median_time_delta
 
-        df['tmp_date'] = df.index
-        df['tmp_date_lagged'] = df['tmp_date'].shift(1)
-        df['tmp_date_delta'] = df['tmp_date'] - df['tmp_date_lagged']
-        df['tmp_date_delta_fraction_of_year'] = df['tmp_date_delta'] / dt.timedelta(365,0,0,0)
-        df['cash'] = (1 + df['cash']) ** df['tmp_date_delta_fraction_of_year'] - 1
-        df['cash'] = df['cash'].fillna(method='bfill')
+    def _set_cash_return_for_each_period(self, df):
+        df["cash"] = self.config["borrowing"]["interest_rate"]
 
-        df.drop(columns=['tmp_date', 'tmp_date_lagged', 'tmp_date_delta', 'tmp_date_delta_fraction_of_year'], inplace=True)
+        df["tmp_date"] = df.index
+        df["tmp_date_lagged"] = df["tmp_date"].shift(1)
+        df["tmp_date_delta"] = df["tmp_date"] - df["tmp_date_lagged"]
+        df["tmp_date_delta_fraction_of_year"] = df["tmp_date_delta"] / dt.timedelta(
+            365, 0, 0, 0
+        )
+        df["cash"] = (1 + df["cash"]) ** df["tmp_date_delta_fraction_of_year"] - 1
+        df["cash"] = df["cash"].fillna(method="bfill")
 
+        df.drop(
+            columns=[
+                "tmp_date",
+                "tmp_date_lagged",
+                "tmp_date_delta",
+                "tmp_date_delta_fraction_of_year",
+            ],
+            inplace=True,
+        )
 
     def _set_references_back_to_optimizer(self):
-        self.strategy.forecast_returns = self.forecast['return']
+        self.strategy.forecast_returns = self.forecast["return"]
         self.strategy.optimizer = self
-        
+
         for c in self.strategy.costs + (self.strategy.constraints or []):
             c.optimizer = self
 
-
     def _init_df_actual(self, df_actual):
         if df_actual is not None:
             self.actual = {}
-            self.actual['return'] = self.pivot_and_fill(df_actual, values='return')
-            self.actual['price'] = self.pivot_and_fill(df_actual, values='price')
-            self.actual['volume'] = self.pivot_and_fill(df_actual, values='volume')
-            self.actual['half_spread'] = (
-                self.pivot_and_fill(df_actual, values='spread') / 2
-            ).rename(
-                columns={'spread': 'half_spread'}
+            self.actual["return"] = self.pivot_and_fill(df_actual, values="return")
+            self.actual["price"] = self.pivot_and_fill(df_actual, values="price")
+            self.actual["volume"] = self.pivot_and_fill(df_actual, values="volume")
+            self.actual["half_spread"] = (
+                self.pivot_and_fill(df_actual, values="spread") / 2
+            ).rename(columns={"spread": "half_spread"})
+            self.actual["std_dev"] = self.pivot_and_fill(
+                self.create_forecast(df_actual, "std_dev"), values="std_dev"
             )
-            self.actual['std_dev'] = self.pivot_and_fill(self.create_forecast(df_actual, 'std_dev'), values='std_dev')
-            self._set_cash_return_for_each_period(self.actual['return'])
-
+            self._set_cash_return_for_each_period(self.actual["return"])
 
     def _init_backtest_model(self, backtest_model, df_actual):
         if backtest_model is None:
             if df_actual is not None:
                 self.backtest_model = result.BaseResult
             else:
                 self.backtest_model = result.ForecastResult
-        else:   
-            self.backtest_model = backtest_model # Not initialized when passed in
+        else:
+            self.backtest_model = backtest_model  # Not initialized when passed in
 
         self.backtest_model.optimizer = self
 
-
     def _clip_forecast_df_for_dates(self, start_date, end_date, df_forecast):
-        self.forecast['date'] = {
+        self.forecast["date"] = {
             "start": start_date or df_forecast.date.min(),
             "end": end_date or df_forecast.date.max(),
         }
         return df_forecast[
-            (df_forecast['date'] >= self.forecast['date']['start']) & 
-            (df_forecast['date'] <= self.forecast['date']['end'])
+            (df_forecast["date"] >= self.forecast["date"]["start"])
+            & (df_forecast["date"] <= self.forecast["date"]["end"])
         ]
 
-
     def _init_df_forecast(self, df_forecast):
-        self.forecast['return'] = self.pivot_and_fill(df_forecast, values='return')
-        self.forecast['std_dev'] = self.pivot_and_fill(self.create_forecast(df_forecast, 'std_dev'), values='std_dev')
-        self.forecast['volume'] = self.pivot_and_fill(self.create_forecast(df_forecast, 'volume'), values='volume')
-        self.forecast['half_spread'] = self.pivot_and_fill(self.create_forecast(df_forecast, 'half_spread'), values='half_spread')
-        self.forecast['price'] = self.create_price(self.forecast['return'])
-
+        self.forecast["return"] = self.pivot_and_fill(df_forecast, values="return")
+        self.forecast["std_dev"] = self.pivot_and_fill(
+            self.create_forecast(df_forecast, "std_dev"), values="std_dev"
+        )
+        self.forecast["volume"] = self.pivot_and_fill(
+            self.create_forecast(df_forecast, "volume"), values="volume"
+        )
+        self.forecast["half_spread"] = self.pivot_and_fill(
+            self.create_forecast(df_forecast, "half_spread"), values="half_spread"
+        )
+        self.forecast["price"] = self.create_price(self.forecast["return"])
 
     def _init_strategy(self, strategy):
-        self.strategy = strategy # Must be initialized first
-        if getattr(self.strategy, 'risk_model', None):
+        self.strategy = strategy  # Must be initialized first
+        if getattr(self.strategy, "risk_model", None):
             self.strategy.costs += [self.strategy.risk_model]
```

### Comparing `investos-0.1.3/investos/portfolio/cost_model/base_cost.py` & `investos-0.1.4/investos/portfolio/cost_model/base_cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import pandas as pd
 import datetime as dt
 import copy
 
-class BaseCost():
-    """Base cost model for InvestOS. 
-    Other cost models should subclass BaseCost. 
+
+class BaseCost:
+    """Base cost model for InvestOS.
+    Other cost models should subclass BaseCost.
     The only requirement of custom cost models is that they (re)implement :py:meth:`~investos.portfolio.cost_model.base_cost.BaseCost.value_expr`.
     """
-    
+
     def __init__(self):
-        self.optimizer = None # Set during Optimizer initialization
+        self.optimizer = None  # Set during Optimizer initialization
         self.gamma = 1  # Can change without setting directly as: gamma * BaseCost(). Note that gamma doesn't impact actual costs in backtester / simulated performance, just trades in optimization strategy.
 
-    
     def weight_expr(self, t, w_plus, z, value):
         cost, constraints = self._estimated_cost_for_optimization(t, w_plus, z, value)
         return self.gamma * cost, constraints
 
-
     def actual_cost(self, t: dt.datetime, h_plus: pd.Series, u: pd.Series) -> pd.Series:
         """Method that calculates per-period costs given period `t` holdings and trades.
 
         Parameters
         ----------
         t : datetime.datetime
             The datetime for associated trades `u` and holdings plus trades `h_plus`.
         h_plus : pandas.Series
             Holdings at beginning of period t, plus trades for period `t` (`u`). Same as `u` + `h` for `t`.
         u : pandas.Series
             Trades (as values) for period `t`.
         """
         raise NotImplementedError
-    
 
     def __mul__(self, other):
         """Read the gamma parameter as a multiplication; so you can change self.gamma without setting it directly as: gamma * BaseCost()"""
         newobj = copy.copy(self)
         newobj.gamma *= other
         return newobj
 
     def __rmul__(self, other):
         """Read the gamma parameter as a multiplication; so you can change self.gamma without setting it directly as: gamma * BaseCost()"""
-        return self.__mul__(other)
+        return self.__mul__(other)
```

### Comparing `investos-0.1.3/investos/portfolio/cost_model/holding_cost.py` & `investos-0.1.4/investos/portfolio/cost_model/holding_cost.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 import numpy as np
 import datetime as dt
 import cvxpy as cvx
 
 from investos.portfolio.cost_model import BaseCost
 from investos.util import values_in_time
 
+
 class HoldingCost(BaseCost):
-    """Calculates cost for holding short positions, given customizable short_rate.
-    """
+    """Calculates cost for holding short positions, given customizable short_rate."""
 
     def __init__(self):
-        self.optimizer = None # Set during Optimizer initialization
+        self.optimizer = None  # Set during Optimizer initialization
 
         super().__init__()
 
-
     def _estimated_cost_for_optimization(self, t, w_plus, z, value):
         """Estimated holding costs.
 
-        Used by optimization strategy to determine trades. 
+        Used by optimization strategy to determine trades.
 
         Not used to calculate simulated holding costs for backtest performance.
         """
         w_plus = w_plus[:-1]
 
-        self.expression = self._get_short_rate(t) * cvx.neg(w_plus) # Borrowing rate for period * negative values
+        self.expression = self._get_short_rate(t) * cvx.neg(
+            w_plus
+        )  # Borrowing rate for period * negative values
 
         return cvx.sum(self.expression), []
 
-
     def actual_cost(self, t: dt.datetime, h_plus: pd.Series, u: pd.Series) -> pd.Series:
         """Method that calculates per-period (short position) holding costs given period `t` holdings and trades.
 
         Parameters
         ----------
         t : datetime.datetime
             The datetime for associated trades `u` and holdings plus trades `h_plus`.
@@ -43,23 +43,19 @@
             Trades (as values) for period `t`.
         """
         short_rate = self._get_short_rate(t)
         self.last_cost = -np.minimum(0, h_plus.iloc[:-1]) * short_rate
 
         return sum(self.last_cost)
 
-
     def _get_short_rate(self, t):
         # Check if t is period 0
-        idx_t = self.optimizer.forecast['return'].index.get_loc(t)
+        idx_t = self.optimizer.forecast["return"].index.get_loc(t)
         if idx_t == 0:
-            idx_t = 1 # If it is, use first period as proxy
+            idx_t = 1  # If it is, use first period as proxy
+
+        t_minus_1 = self.optimizer.forecast["return"].index[idx_t - 1]
+        fraction_of_year = (t - t_minus_1) / dt.timedelta(365, 0, 0, 0)
 
-        t_minus_1 = self.optimizer.forecast['return'].index[idx_t - 1]
-        fraction_of_year = (t - t_minus_1) / dt.timedelta(365,0,0,0)
-        
         return (
-            (1 + values_in_time(
-                self.optimizer.config['borrowing']['short_rate'], t
-            )) ** (fraction_of_year)
-            - 1
-        )
+            1 + values_in_time(self.optimizer.config["borrowing"]["short_rate"], t)
+        ) ** (fraction_of_year) - 1
```

### Comparing `investos-0.1.3/investos/portfolio/cost_model/trading_cost.py` & `investos-0.1.4/investos/portfolio/cost_model/trading_cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,103 +2,104 @@
 import numpy as np
 import datetime as dt
 import cvxpy as cvx
 
 from investos.portfolio.cost_model import BaseCost
 from investos.util import values_in_time
 
+
 class TradingCost(BaseCost):
     """Calculates per period cost for trades `u`, based on spread, standard deviation, volume, and price.
-    
+
     Attributes
     ----------
     sensitivity_coeff : float
         For scaling transaction cost; 1 assumes 1 period's volume moves price by 1 std_dev in vol
     """
 
     def __init__(self, price_movement_sensitivity=1):
-        self.optimizer = None # Set during Optimizer initialization
+        self.optimizer = None  # Set during Optimizer initialization
         # For scaling realized transaction cost; 1 assumes 1 day's volume moves price by 1 day's vol
         # --> Eventually support DF for this
         self.sensitivity_coeff = price_movement_sensitivity
 
         super().__init__()
 
-    
     def _estimated_cost_for_optimization(self, t, w_plus, z, value):
         """Estimated trading costs.
 
-        Used by optimization strategy to determine trades. 
+        Used by optimization strategy to determine trades.
         """
         z = z[:-1]
         constraints = []
 
         # Calculate terms for estimated trading cost
-        std_dev = values_in_time(self.optimizer.forecast['std_dev'], t)
-        volume_dollars = (
-            values_in_time(self.optimizer.forecast['volume'], t) *
-            values_in_time(self.optimizer.forecast['price'], t)
-        )
-        percent_volume_traded_pre_trade_weight = np.abs(value) / volume_dollars # Multiplied (using cvx) by trade weight (z) below!
+        std_dev = values_in_time(self.optimizer.forecast["std_dev"], t)
+        volume_dollars = values_in_time(
+            self.optimizer.forecast["volume"], t
+        ) * values_in_time(self.optimizer.forecast["price"], t)
+        percent_volume_traded_pre_trade_weight = (
+            np.abs(value) / volume_dollars
+        )  # Multiplied (using cvx) by trade weight (z) below!
 
         price_movement_term = (
-            self.sensitivity_coeff * 
-            std_dev * 
-            percent_volume_traded_pre_trade_weight
+            self.sensitivity_coeff * std_dev * percent_volume_traded_pre_trade_weight
         )
         # END calculate terms for estimated trading cost
 
         # Create estimated cost expression
-        try: # Spread (estimated) costs
+        try:  # Spread (estimated) costs
             self.estimate_expression = cvx.multiply(
-                values_in_time(self.optimizer.forecast['half_spread'], t), cvx.abs(z))
+                values_in_time(self.optimizer.forecast["half_spread"], t), cvx.abs(z)
+            )
         except TypeError:
             self.estimate_expression = cvx.multiply(
-                values_in_time(self.optimizer.forecast['half_spread'], t).values, cvx.abs(z))
-        
-        try: # Price movement due to volume (estimated) costs
-            self.estimate_expression += cvx.multiply(price_movement_term, cvx.abs(z) ** 2)
+                values_in_time(self.optimizer.forecast["half_spread"], t).values,
+                cvx.abs(z),
+            )
+
+        try:  # Price movement due to volume (estimated) costs
+            self.estimate_expression += cvx.multiply(
+                price_movement_term, cvx.abs(z) ** 2
+            )
         except TypeError:
-            self.estimate_expression += cvx.multiply(price_movement_term.values, cvx.abs(z) ** 2)
+            self.estimate_expression += cvx.multiply(
+                price_movement_term.values, cvx.abs(z) ** 2
+            )
         # END create estimated cost expression
 
         return cvx.sum(self.estimate_expression), constraints
 
-
     def actual_cost(self, t: dt.datetime, h_plus: pd.Series, u: pd.Series) -> pd.Series:
         """Method that calculates `t` period cost for trades `u`.
 
-        Trading cost (per asset) is assumed to be half of bid-ask spread, plus (per asset) standard deviation * % of period volume traded. 
-        Assumption is trading 100% of period volume moves price by 1 (default value for `self.sensitivity_coeff`) standard deviation. 
+        Trading cost (per asset) is assumed to be half of bid-ask spread, plus (per asset) standard deviation * % of period volume traded.
+        Assumption is trading 100% of period volume moves price by 1 (default value for `self.sensitivity_coeff`) standard deviation.
 
         Parameters
         ----------
         t : datetime.datetime
             The datetime for associated trades `u` and holdings plus trades `h_plus`.
         h_plus : pandas.Series
             Holdings at beginning of period t, plus trades for period `t` (`u`). Same as `u` + `h` for `t`.
         u : pandas.Series
             Trades (as values) for period `t`.
         """
 
         u_no_cash = u.iloc[:-1]
-        
-        spread_cost = np.abs(u_no_cash) * values_in_time(self.optimizer.actual['half_spread'], t)
-        std_dev = values_in_time(self.optimizer.actual['std_dev'], t)
-        volume_dollars = (
-            values_in_time(self.optimizer.actual['volume'], t) *
-            values_in_time(self.optimizer.actual['price'], t)
+
+        spread_cost = np.abs(u_no_cash) * values_in_time(
+            self.optimizer.actual["half_spread"], t
         )
+        std_dev = values_in_time(self.optimizer.actual["std_dev"], t)
+        volume_dollars = values_in_time(
+            self.optimizer.actual["volume"], t
+        ) * values_in_time(self.optimizer.actual["price"], t)
         percent_volume_traded = np.abs(u_no_cash) / volume_dollars
 
-        trading_costs = (
-            spread_cost + (
-                self.sensitivity_coeff * 
-                std_dev * 
-                np.abs(u_no_cash) *
-                percent_volume_traded
-            )
+        trading_costs = spread_cost + (
+            self.sensitivity_coeff * std_dev * np.abs(u_no_cash) * percent_volume_traded
         )
 
-        self.optimizer.backtest.save_data('costs_trading', t, trading_costs)
+        self.optimizer.backtest.save_data("costs_trading", t, trading_costs)
 
-        return trading_costs.sum()
+        return trading_costs.sum()
```

### Comparing `investos-0.1.3/investos/portfolio/result/base_result.py` & `investos-0.1.4/investos/portfolio/result/base_result.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pandas as pd
 import numpy as np
 
 import datetime as dt
 import collections
+from investos.util import clip_for_dates
+from investos.portfolio.result import SaveResult
 
-class BaseResult():
+
+class BaseResult(SaveResult):
     """The `Result` class captures portfolio data and performance for each asset and period over time.
 
     Instances of this object are called by the :py:meth:`investos.portfolio.controller.Controller.generate_positions` method.
     """
 
-    def __init__(self):
-        pass
+    def __init__(self, start_date, end_date):
+        self.start_date = start_date
+        self.end_date = end_date
 
     def save_data(self, name: str, t: dt.datetime, entry: pd.Series) -> None:
         """Save `entry` on `Result` object, a (pandas) Series of data as `name` for datetime `t`.
 
         Parameters
         ----------
         name : str
@@ -24,18 +28,21 @@
             The datetime `entry` is saved under in this `Result` object.
         entry : pandas.Series
             A series of values - for a collection of assets / stocks / tickers at a specific point in time.
         """
         try:
             getattr(self, name).loc[t] = entry
         except AttributeError:
-            setattr(self, name,
-                    (pd.Series if np.isscalar(entry) else
-                     pd.DataFrame)(index=[t], data=[entry]))
-
+            setattr(
+                self,
+                name,
+                (pd.Series if np.isscalar(entry) else pd.DataFrame)(
+                    index=[t], data=[entry]
+                ),
+            )
 
     def save_position(self, t: dt.datetime, u: pd.Series, h_next: pd.Series) -> None:
         """
         Save data `u` and `h_next` related to position for datetime `t` on `Result` object.
 
         Parameters
         ----------
@@ -45,150 +52,246 @@
             Trades (as values) for period `t`.
         h_next : pandas.Series
             Holdings at beginning of period t + 1, after trades `u` and returns for period `t`.
         """
         self.save_data("u", t, u)
         self.save_data("h_next", t, h_next)
 
-
     @property
     def summary(self) -> None:
-        """Outputs a string summary of backtest result properties and performance 
+        """Outputs a string summary of backtest result properties and performance
         (e.g. :py:attr:`~investos.portfolio.result.base_result.BaseResult.num_periods`, :py:attr:`~investos.portfolio.result.base_result.BaseResult.sharpe_ratio`, :py:attr:`~investos.portfolio.result.base_result.BaseResult.max_drawdown`, etc.).
         """
         print(self._summary_string())
 
     def _summary_string(self) -> str:
-        """Returns a string summary of backtest result properties and performance 
+        """Returns a string summary of backtest result properties and performance
         (e.g. :py:attr:`~investos.portfolio.result.base_result.BaseResult.num_periods`, :py:attr:`~investos.portfolio.result.base_result.BaseResult.sharpe_ratio`, :py:attr:`~investos.portfolio.result.base_result.BaseResult.max_drawdown`, etc.).
 
         Do not call directly; call :py:attr:`~investos.portfolio.result.base_result.BaseResult.summary` instead.
         """
-        data = collections.OrderedDict({
-            'Number of periods':
-                self.num_periods,
-            'Initial timestamp':
-                self.h.index[0],
-            'Final timestamp':
-                self.h.index[-1],
-            'Annualized portfolio return (%)':
-                str(round(self.annualized_return * 100, 2)) + '%',
-            'Total portfolio return (%)':
-                str(round(self.total_return * 100, 2)) + '%',
-            'Sharpe ratio':
-                self.sharpe_ratio,
-            'Max drawdown':
-                f"{round(self.max_drawdown, 2)}%",
-            'Annual turnover (x)':
-                str(round(self.turnover.mean() * self.ppy, 2)) + 'x',
-        })
-
-        return (pd.Series(data=data).
-                to_string(float_format='{:,.3f}'.format))
+        data = collections.OrderedDict(
+            {
+                "Initial timestamp": self.h.index[0],
+                "Final timestamp": self.h.index[-1],
+                "Total portfolio return (%)": str(round(self.total_return * 100, 2))
+                + "%",
+                "Annualized portfolio return (%)": str(
+                    round(self.annualized_return * 100, 2)
+                )
+                + "%",
+                "Annualized excess portfolio return (%)": str(
+                    round(self.annualized_excess_return * 100, 2)
+                )
+                + "%",
+                "Annualized excess risk (%)": str(round(self.excess_risk_annualized, 2))
+                + "%",
+                "Information ratio (calc. from per period returns and risk)": str(
+                    round(self.information_ratio, 2)
+                )
+                + "x",
+                "Annualized risk over risk-free (%)": str(
+                    round(self.risk_over_cash_annualized, 2)
+                )
+                + "%",
+                "Sharpe ratio (calc. from per period returns and risk)": str(
+                    round(self.sharpe_ratio, 2)
+                )
+                + "x",
+                "Max drawdown": f"{round(self.max_drawdown, 2)}%",
+                "Annual turnover (x)": str(round(self.annual_turnover, 2)) + "x",
+            }
+        )
 
+        return pd.Series(data=data).to_string(float_format="{:,.3f}".format)
 
     @property
+    @clip_for_dates
     def h(self) -> pd.DataFrame:
-        """Returns a pandas Dataframe of asset holdings (`h`) at the beginning of each datetime period.
-        """
+        """Returns a pandas Dataframe of asset holdings (`h`) at the beginning of each datetime period."""
         tmp = self.h_next.copy()
-        tmp = self.h_next.shift(1) # Shift h_next to h timing
+        tmp = self.h_next.shift(1)  # Shift h_next to h timing
         return tmp[1:]
 
+    @property
+    @clip_for_dates
+    def trades(self) -> pd.DataFrame:
+        "Returns a pandas Series of trades (u)."
+        return self.u
 
     @property
     def num_periods(self) -> int:
         """Number of periods in backtest. Note that the starting position (at t=0) does not count as a period."""
         return self.h.shape[0]
 
-
     @property
     def v(self) -> pd.Series:
-        """Returns a pandas Series for the value (`v`) of the portfolio for each datetime period.
-        """
+        """Returns a pandas Series for the value (`v`) of the portfolio for each datetime period."""
         return self.h.sum(axis=1)
 
+    @property
+    def v_with_benchmark(self) -> pd.Series:
+        """Returns a pandas Dataframe with simulated portfolio and benchmark values."""
+        return pd.DataFrame({"portfolio": self.v, "benchmark": self.benchmark_v})
 
     @property
     def returns(self) -> pd.Series:
         """Returns a pandas Series of the returns for each datetime period (vs the previous period)."""
         val = self.v
-        return pd.Series(data=val.values[1:] / val.values[:-1] - 1,
-                         index=val.index[1:]).dropna()
-
+        return pd.Series(
+            data=val.values[1:] / val.values[:-1] - 1, index=val.index[1:]
+        ).dropna()
 
     @property
     def total_return(self) -> float:
-        """Returns a float representing the total return for the entire period under review.
-        """
+        """Returns a float representing the total return for the entire period under review."""
         return self.v[-1] / self.v[0] - 1
-    
+
+    @property
+    def total_benchmark_return(self) -> float:
+        """Returns a float representing the total return for the entire period under review."""
+        return self.benchmark_v[-1] / self.benchmark_v[0] - 1
+
+    @property
+    def total_excess_return(self) -> float:
+        """Returns a float representing the total return for the entire period under review."""
+        return self.total_return - self.total_benchmark_return
 
     @property
     def annualized_return(self) -> float:
-        """Returns a float representing the annualized return of the entire period under review. Uses beginning and ending portfolio values for the calculation (value @ t[-1] and value @ t[0]), as well as the number of years in the forecast.
-        """
-        return (
-            ( (self.total_return + 1) ** (1 / self.years_forecast) ) - 1
-        )
+        """Returns a float representing the annualized return of the entire period under review. Uses beginning and ending portfolio values for the calculation (value @ t[-1] and value @ t[0]), as well as the number of years in the forecast."""
+        return ((self.total_return + 1) ** (1 / self.years_forecast)) - 1
 
+    @property
+    def annualized_benchmark_return(self) -> float:
+        """Returns a float representing the annualized benchmark return of the entire period under review. Uses beginning and ending portfolio values for the calculation (value @ t[-1] and value @ t[0]), as well as the number of years in the forecast."""
+        return ((self.total_benchmark_return + 1) ** (1 / self.years_forecast)) - 1
 
     @property
     def excess_returns(self) -> pd.Series:
-        """Returns a pandas Series of returns in excess of the (cash) benchmark.
-        """
-        return (self.returns - self.optimizer.actual['return']['cash']).dropna()
+        """Returns a pandas Series of returns in excess of the benchmark."""
+        return (self.returns - self.benchmark_returns).dropna()
 
+    @property
+    def returns_over_cash(self) -> pd.Series:
+        """Returns a pandas Series of returns in excess of risk free returns."""
+        return (self.returns - self.risk_free_returns).dropna()
+
+    @property
+    def annualized_excess_return(self) -> float:
+        """Returns a float representing the annualized excess return of the entire period under review. Uses beginning and ending portfolio values for the calculation (value @ t[-1] and value @ t[0]), as well as the number of years in the forecast."""
+        return self.annualized_return - self.annualized_benchmark_return
+
+    @property
+    def excess_risk_annualized(self) -> pd.Series:
+        """Returns a pandas Series of risk in excess of the benchmark."""
+        return self.excess_returns.std() * 100 * np.sqrt(self.ppy)
+
+    @property
+    def risk_over_cash_annualized(self) -> pd.Series:
+        """Returns a pandas Series of risk in excess of the risk free rate."""
+        return self.returns_over_cash.std() * 100 * np.sqrt(self.ppy)
+
+    @property
+    @clip_for_dates
+    def benchmark_returns(self) -> pd.Series:
+        if not hasattr(self, "benchmark"):
+            self.benchmark = self.optimizer.actual["return"]["cash"]
+
+        return self.benchmark
+
+    @property
+    @clip_for_dates
+    def risk_free_returns(self) -> pd.Series:
+        if not hasattr(self, "risk_free"):
+            self.risk_free = self.optimizer.actual["return"]["cash"]
+
+        return self.risk_free
+
+    @property
+    def benchmark_v(self) -> pd.Series:
+        """Returns series of simulated portfolio values, if portfolio was invested 100% in benchmark at time 0"""
+        benchmark_factors = self.benchmark_returns + 1
+        benchmark_factors[0] = 1  # No returns for period 0
+
+        return (
+            benchmark_factors.cumprod() * self.v[0]
+        )  # Calculate values if initial portfolio value was invested 100% in benchmark
 
     @property
     def years_forecast(self) -> float:
         """Returns a float representing the number of years in the backtest period.
         Calculated as (datetime @ t[-1] - datetime @ t[0]) / datetime.timedelta(365,0,0,0)
         """
-        return (self.v.index[-1] - self.v.index[0]) / dt.timedelta(365,0,0,0)
-
+        return (self.v.index[-1] - self.v.index[0]) / dt.timedelta(365, 0, 0, 0)
 
     @property
     def ppy(self) -> float:
         """Returns a float representing the number of periods per year in the backtest period.
         Calculated as :py:attr:`~investos.portfolio.result.base_result.BaseResult.num_periods` / :py:attr:`~investos.portfolio.result.base_result.BaseResult.years_forecast`
         """
         return self.num_periods / self.years_forecast
 
+    @property
+    def information_ratio(self) -> float:
+        """Returns a float representing the (annualized) Information Ratio of the portfolio.
+
+        Ratio is calculated as mean of :py:attr:`~investos.portfolio.result.base_result.base_result.BaseResult.excess_returns` / standard deviation of :py:attr:`~investos.portfolio.result.base_result.BaseResult.excess_returns`. Annualized by multiplying ratio by square root of periods per year (:py:attr:`~investos.portfolio.result.base_result.BaseResult.ppy`).
+        """
+        return (
+            np.sqrt(self.ppy)
+            * np.mean(self.excess_returns)
+            / np.std(self.excess_returns)
+        )
 
     @property
     def sharpe_ratio(self) -> float:
-        """Returns a float representing the (annualized) 
-        `Sharpe Ratio <https://en.wikipedia.org/wiki/Sharpe_ratio>`_ 
-        of the portfolio.
+        """Returns a float representing the (annualized) Sharpe Ratio of the portfolio.
 
         Ratio is calculated as mean of :py:attr:`~investos.portfolio.result.base_result.base_result.BaseResult.excess_returns` / standard deviation of :py:attr:`~investos.portfolio.result.base_result.BaseResult.excess_returns`. Annualized by multiplying ratio by square root of periods per year (:py:attr:`~investos.portfolio.result.base_result.BaseResult.ppy`).
-        
-        TBU: accept benchmark for long-only portfolios / portfolios tracking benchmark
         """
         return (
-            np.sqrt(self.ppy) * np.mean(self.excess_returns) /
-            np.std(self.excess_returns)
+            np.sqrt(self.ppy)
+            * np.mean(self.returns_over_cash)
+            / np.std(self.returns_over_cash)
         )
 
-
     @property
     def turnover(self):
-        """Turnover ||u_t||_1/v_t
-        """
-        noncash_trades = self.u.drop(['cash'], axis=1)
+        """Turnover ||u_t||_1/v_t"""
+        noncash_trades = self.trades.drop(["cash"], axis=1)
         return np.abs(noncash_trades).sum(axis=1) / self.v
 
+    @property
+    def leverage(self):
+        """Turnover ||u_t||_1/v_t"""
+        noncash_h = self.h.drop(["cash"], axis=1)
+        return np.abs(noncash_h).sum(axis=1) / self.v
+
+    @property
+    def long_leverage(self):
+        """Turnover ||u_t||_1/v_t"""
+        noncash_h = self.h.drop(["cash"], axis=1)
+        return np.abs(noncash_h[noncash_h > 0]).sum(axis=1) / self.v
+
+    @property
+    def short_leverage(self):
+        """Turnover ||u_t||_1/v_t"""
+        noncash_h = self.h.drop(["cash"], axis=1)
+        return np.abs(noncash_h[noncash_h < 0]).sum(axis=1) / self.v
+
+    @property
+    def annual_turnover(self):
+        return self.turnover.mean() * self.ppy
 
     @property
     def max_drawdown(self):
-        """The maximum peak to trough drawdown in percent.
-        """
+        """The maximum peak to trough drawdown in percent."""
         val_arr = self.v.values
         max_dd_so_far = 0
         cur_max = val_arr[0]
         for val in val_arr[1:]:
             if val >= cur_max:
                 cur_max = val
-            elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
-                max_dd_so_far = 100 * (cur_max - val) / cur_max
-        return max_dd_so_far
+            elif (cur_max - val) / cur_max > max_dd_so_far:
+                max_dd_so_far = (cur_max - val) / cur_max
+        return max_dd_so_far
```

### Comparing `investos-0.1.3/investos/portfolio/risk_model/base_risk.py` & `investos-0.1.4/investos/portfolio/risk_model/base_risk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import pandas as pd
 import datetime as dt
 
 from investos.portfolio.cost_model import BaseCost
 
+
 class BaseRisk(BaseCost):
-    """Base risk model for InvestOS. 
+    """Base risk model for InvestOS.
 
     The only requirement of custom risk models is that they implement a `_estimated_cost_for_optimization` method.
 
     Note: risk models are like cost models, except they return 0 for their `value_expr` method (because they only influence optimization weights, not actual cash costs).
     """
 
     def __init__(self):
-        self.optimizer = None # Set during Controller initialization
+        self.optimizer = None  # Set during Controller initialization
 
         super().__init__()
-        
 
     def actual_cost(self, t: dt.datetime, h_plus: pd.Series, u: pd.Series) -> pd.Series:
         """Method that calculates per-period costs given period `t` holdings and trades.
 
         ALWAYS 0 FOR RISK MODELS; DO NOT OVERRIDE. RISK DOESN'T HAVE A CASH COST, IT ONLY AFFECTS OPTIMIZED ASSET WEIGHTS GIVEN `_estimated_cost_for_optimization` RISK (UTILITY) PENALTY.
         """
         return 0
 
     def _estimated_cost_for_optimization(self, t, w_plus, z, value):
         """Optimization (non-cash) cost penalty for assuming associated asset risk.
 
-        Used by optimization strategy to determine trades. 
+        Used by optimization strategy to determine trades.
 
         Not used to calculate simulated costs for backtest performance.
         """
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `investos-0.1.3/investos/portfolio/risk_model/stat_factor_risk.py` & `investos-0.1.4/investos/portfolio/risk_model/stat_factor_risk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,76 @@
 import pandas as pd
 import numpy as np
 import cvxpy as cvx
 
 from investos.portfolio.risk_model import BaseRisk
 
+
 class StatFactorRisk(BaseRisk):
     """PCA-factor based risk model.
 
     The only requirement of custom risk models is that they implement a `_estimated_cost_for_optimization` method.
 
     Note: risk models are like cost models, except they return 0 for their `value_expr` method (because they only influence optimization weights, not actual cash costs).
     """
 
     def __init__(self, n_factors=5):
         self.n = n_factors
 
-        self.optimizer = None # Set during Controller initialization
+        self.optimizer = None  # Set during Controller initialization
 
         self.factor_variance = None
         self.factor_loadings = None
         self.idiosyncratic_variance = None
 
         super().__init__()
 
-
     def _estimated_cost_for_optimization(self, t, w_plus, z, value):
         """Optimization (non-cash) cost penalty for assuming associated asset risk.
 
-        Used by optimization strategy to determine trades. 
+        Used by optimization strategy to determine trades.
 
         Not used to calculate simulated costs for backtest performance.
         """
-        if self.factor_variance is None or self.factor_loadings is None or self.idiosyncratic_variance is None:
+        if (
+            self.factor_variance is None
+            or self.factor_loadings is None
+            or self.idiosyncratic_variance is None
+        ):
             self.create_risk_model()
 
         self.expression = cvx.sum(
-            cvx.multiply(
-                self.idiosyncratic_variance, 
-                cvx.square(w_plus)
-            )
-        ) + cvx.sum(
-            cvx.multiply(
-                w_plus.T @ self.factor_loadings,
-                self.factor_variance
-            )
-        )
-        
-        return self.expression, []
+            cvx.multiply(self.idiosyncratic_variance, cvx.square(w_plus))
+        ) + cvx.sum(cvx.multiply(w_plus.T @ self.factor_loadings, self.factor_variance))
 
+        return self.expression, []
 
     def create_risk_model(self):
-        df = self.optimizer.actual['return']
-        forecast_start_d = self.optimizer.forecast['date']['start']
-        df = df[(
-            df.index < forecast_start_d) & (
-            df.index >= pd.to_datetime(forecast_start_d) - pd.Timedelta("730 days") # 2 years
-        )]
+        df = self.optimizer.actual["return"]
+        forecast_start_d = self.optimizer.forecast["date"]["start"]
+        df = df[
+            (df.index < forecast_start_d)
+            & (
+                df.index
+                >= pd.to_datetime(forecast_start_d)
+                - pd.Timedelta("730 days")  # 2 years
+            )
+        ]
 
         covariance_matrix = df.cov().dropna().values
         eigenvalue, eigenvector = np.linalg.eigh(covariance_matrix)
-        
-        self.factor_variance = eigenvalue[-self.n:]
+
+        self.factor_variance = eigenvalue[-self.n :]
         self.factor_loadings = pd.DataFrame(
-            data=eigenvector[:,-self.n:], 
-            index=df.columns
+            data=eigenvector[:, -self.n :], index=df.columns
         )
-        self.factor_loadings.iloc[-1] = 0 # For cash
+        self.factor_loadings.iloc[-1] = 0  # For cash
         self.idiosyncratic_variance = pd.Series(
             data=np.diag(
-                eigenvector[:, :-self.n] @ 
-                np.diag(
-                    eigenvalue[:-self.n]
-                ) @ eigenvector[:, :-self.n].T
+                eigenvector[:, : -self.n]
+                @ np.diag(eigenvalue[: -self.n])
+                @ eigenvector[:, : -self.n].T
             ),
-            index=df.columns
+            index=df.columns,
         )
         self.idiosyncratic_variance = self.idiosyncratic_variance.copy()
-        self.idiosyncratic_variance.iloc[-1] = 0
+        self.idiosyncratic_variance.iloc[-1] = 0
```

### Comparing `investos-0.1.3/investos/portfolio/strategy/base_strategy.py` & `investos-0.1.4/investos/portfolio/strategy/base_strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import pandas as pd
 import datetime as dt
 
-class BaseStrategy():
+
+class BaseStrategy:
     """Base class for an optimization strategy.
 
     Must implement :py:meth:`~investos.portfolio.strategy.base_strategy.BaseStrategy.generate_trade_list` as per below.
 
     Attributes
     ----------
     costs : list
         Cost models evaluated during optimization strategy. Defaults to empty list. See :py:class:`~investos.portfolio.cost_model.base_cost.BaseCost` for cost model base class.
     constraints : list
         Constraints applied for optimization strategy. Defaults to empty list. See [TBU] for optimization model base class.
     """
+
     def __init__(self):
         self.costs = []
         self.constraints = []
         self.risk_model = None
 
-    
     def _zerotrade(self, holdings):
-        return pd.Series(index=holdings.index, data=0.)
-
+        return pd.Series(index=holdings.index, data=0.0)
 
     def generate_trade_list(self, holdings: pd.Series, t: dt.datetime) -> pd.Series:
         """Calculates and returns trade list (in units of currency passed in), given (added) optimization logic.
 
         Parameters
         ----------
         holdings : pandas.Series
             Holdings at beginning of period `t`.
         t : datetime.datetime
             The datetime for associated holdings `holdings`.
         """
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `investos-0.1.3/investos/portfolio/strategy/rank_long_short.py` & `investos-0.1.4/investos/portfolio/strategy/rank_long_short.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import datetime as dt
 
 from investos.portfolio.strategy import BaseStrategy
 from investos.portfolio.cost_model import TradingCost, HoldingCost, BaseCost
 from investos.util import values_in_time
 
+
 class RankLongShort(BaseStrategy):
     """Optimization strategy that builds trade list by going long assets with best return forecasts and short stocks with worst return forecasts.
 
 
     Attributes
     ----------
     costs : list[:py:class:`~investos.portfolio.cost_model.base_cost.BaseCost`]
@@ -21,75 +22,81 @@
         Percent of assets in forecast returns to go long.
     leverage : float
         Absolute value of exposure / AUM. Used to calculate holdings.
     n_periods_held : integer
         Number of periods positions held. After n number of periods, positions unwound.
     """
 
-    def __init__(self, n_periods_held: int = 1, leverage: float = 1, percent_short: float = 0.25, percent_long: float = 0.25, costs: list[BaseCost] = []):
-        self.forecast_returns = None # Set by Controller in init
-        self.optimizer = None # Set by Controller in init
+    def __init__(
+        self,
+        n_periods_held: int = 1,
+        leverage: float = 1,
+        percent_short: float = 0.25,
+        percent_long: float = 0.25,
+        costs: list[BaseCost] = [],
+    ):
+        self.forecast_returns = None  # Set by Controller in init
+        self.optimizer = None  # Set by Controller in init
 
         self.costs = costs
         if not self.costs:
             self.costs = [TradingCost(), HoldingCost()]
 
         self.constraints = []
         self.risk_model = None
 
         self.percent_short = percent_short
         self.percent_long = percent_long
         self.n_periods_held = n_periods_held
         self.leverage_per_trade = leverage / n_periods_held
 
-
     def generate_trade_list(self, holdings: pd.Series, t: dt.datetime) -> pd.Series:
         """Calculates and returns trade list (in units of currency passed in) by going long top :py:attr:`~investos.portfolio.strategy.rank_long_short.RankLongShort.percent_long` assets and short bottom :py:attr:`~investos.portfolio.strategy.rank_long_short.RankLongShort.percent_short` assets.
 
         Parameters
         ----------
         holdings : pandas.Series
             Holdings at beginning of period `t`.
         t : datetime.datetime
             The datetime for associated holdings `holdings`.
         """
         w = self._get_trade_weights_for_t(holdings, t)
         u = sum(holdings) * w * self.leverage_per_trade
-        
+
         idx_t = self.forecast_returns.index.get_loc(t)
         if idx_t - self.n_periods_held >= 0:
             # Use holdings_unwind, t_unwind, w_unwind, u_unwind, u_unwind_scaled
             t_unwind = self.forecast_returns.index[idx_t - self.n_periods_held]
             holdings_unwind = self.optimizer.backtest.h.loc[t_unwind]
             w_unwind = self._get_trade_weights_for_t(holdings_unwind, t_unwind)
             u_unwind_pre = sum(holdings_unwind) * w_unwind * self.leverage_per_trade
-            u_unwind_scaled = u_unwind_pre * self._cum_returns_to_scale_unwind(t_unwind, t)
-            
+            u_unwind_scaled = u_unwind_pre * self._cum_returns_to_scale_unwind(
+                t_unwind, t
+            )
+
             u -= u_unwind_scaled
 
         return u
 
-
     def _get_trade_weights_for_t(self, holdings: pd.Series, t: dt.datetime):
         n_short = round(self.forecast_returns.shape[1] * self.percent_short)
         n_long = round(self.forecast_returns.shape[1] * self.percent_long)
 
         prediction = values_in_time(self.forecast_returns, t)
         prediction_sorted = prediction.sort_values()
 
         short_trades = prediction_sorted.index[:n_short]
         long_trades = prediction_sorted.index[-n_long:]
-        
-        w = pd.Series(0., index=prediction.index)
-        w[short_trades] = -1.
-        w[long_trades] = 1.
+
+        w = pd.Series(0.0, index=prediction.index)
+        w[short_trades] = -1.0
+        w[long_trades] = 1.0
 
         w /= sum(abs(w))
 
         return w
 
-
-    def _cum_returns_to_scale_unwind(self, t_unwind: dt.datetime, t: dt.datetime):        
-        df = self.optimizer.actual['return'] + 1
+    def _cum_returns_to_scale_unwind(self, t_unwind: dt.datetime, t: dt.datetime):
+        df = self.optimizer.actual["return"] + 1
         df = df[(df.index >= t_unwind) & (df.index < t)]
 
-        return df.cumprod().iloc[-1]
+        return df.cumprod().iloc[-1]
```

### Comparing `investos-0.1.3/investos/portfolio/strategy/spo.py` & `investos-0.1.4/investos/portfolio/strategy/spo.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,41 +5,48 @@
 from investos.portfolio.constraint_model import *
 from investos.portfolio.risk_model import *
 from investos.portfolio.strategy import BaseStrategy
 from investos.portfolio.cost_model import TradingCost, HoldingCost, BaseCost
 from investos.util import values_in_time
 import investos.util as util
 
+
 class SPO(BaseStrategy):
-    """Optimization strategy that builds trade list using single period optimization.
-    """
+    """Optimization strategy that builds trade list using single period optimization."""
 
     BASE_SOLVER_OPTS = {
-        'max_iter': 50_000,
-        'eps_rel': 0.0000000001,
-        'eps_abs': 0.0000000001,
+        "max_iter": 50_000,
+        "eps_rel": 0.0000000001,
+        "eps_abs": 0.0000000001,
     }
-    
-    
-    def __init__(self, 
-                costs: [BaseCost] = [TradingCost(), HoldingCost()], 
-                constraints: [BaseConstraint] = [MinWeightConstraint(), MaxWeightConstraint(), MaxLeverageConstraint(), EqualLongShortConstraint()], 
-                risk_model: BaseRisk = StatFactorRisk(),
-                solver=cvx.OSQP,
-                solver_opts=None):
-        self.forecast_returns = None # Set by Backtester in init
-        self.optimizer = None # Set by Backtester in init
+
+    def __init__(
+        self,
+        costs: [BaseCost] = [TradingCost(), HoldingCost()],
+        constraints: [BaseConstraint] = [
+            MinWeightConstraint(),
+            MaxWeightConstraint(),
+            MaxLeverageConstraint(),
+            EqualLongShortConstraint(),
+        ],
+        risk_model: BaseRisk = StatFactorRisk(),
+        solver=cvx.OSQP,
+        solver_opts=None,
+    ):
+        self.forecast_returns = None  # Set by Backtester in init
+        self.optimizer = None  # Set by Backtester in init
 
         self.costs = costs
         self.risk_model = risk_model
         self.constraints = constraints
         self.solver = solver
-        self.solver_opts = util.deep_dict_merge(self.BASE_SOLVER_OPTS, solver_opts or {})
+        self.solver_opts = util.deep_dict_merge(
+            self.BASE_SOLVER_OPTS, solver_opts or {}
+        )
 
-    
     def generate_trade_list(self, holdings: pd.Series, t: dt.datetime) -> pd.Series:
         """Calculates and returns trade list (in units of currency passed in) using convex (single period) optimization.
 
         Parameters
         ----------
         holdings : pandas.Series
             Holdings at beginning of period `t`.
@@ -47,62 +54,68 @@
             The datetime for associated holdings `holdings`.
         """
 
         if t is None:
             t = dt.datetime.today()
 
         value = sum(holdings)
-        w = holdings / value # Portfolio weights
+        w = holdings / value  # Portfolio weights
         z = cvx.Variable(w.size)  # Portfolio trades
-        wplus = w.values + z # Portfolio weights after trades
+        wplus = w.values + z  # Portfolio weights after trades
 
-        alpha_term = cvx.sum(cvx.multiply(
-            values_in_time(self.forecast_returns, t).values,
-            wplus))
+        alpha_term = cvx.sum(
+            cvx.multiply(values_in_time(self.forecast_returns, t).values, wplus)
+        )
 
-        assert(alpha_term.is_concave())
+        assert alpha_term.is_concave()
 
         costs, constraints = [], []
 
         for cost in self.costs:
             cost_expr, const_expr = cost.weight_expr(t, wplus, z, value)
             costs.append(cost_expr)
             constraints += const_expr
 
-        constraints += [item for item in (con.weight_expr(t, wplus, z, value)
-                                          for con in self.constraints)]
+        constraints += [
+            item
+            for item in (
+                con.weight_expr(t, wplus, z, value) for con in self.constraints
+            )
+        ]
+
+        # For help debugging:
 
-        # For help debugging: 
-        
         # for el in costs:
         #     if not el.is_convex():
         #         print(t, el, "is not convex")
-            # assert (el.is_convex())
+        # assert (el.is_convex())
 
         # for el in constraints:
-            # if not el.is_dcp():
-            #     print(t, el, "is not dcp")
-            # assert (el.is_dcp())
+        # if not el.is_dcp():
+        #     print(t, el, "is not dcp")
+        # assert (el.is_dcp())
 
         objective = cvx.Maximize(alpha_term - cvx.sum(costs))
         constraints += [cvx.sum(z) == 0]
-        self.prob = cvx.Problem(objective, constraints) # Trades need to 0 out, i.e. cash account must adjust to make everything net to 0
-        
+        self.prob = cvx.Problem(
+            objective, constraints
+        )  # Trades need to 0 out, i.e. cash account must adjust to make everything net to 0
+
         try:
             self.prob.solve(solver=self.solver, **self.solver_opts)
 
-            if self.prob.status == 'unbounded':
+            if self.prob.status == "unbounded":
                 print(f"The problem is unbounded at {t}.")
                 return self._zerotrade(holdings)
 
-            if self.prob.status == 'infeasible':
+            if self.prob.status == "infeasible":
                 print(f"The problem is infeasible at {t}.")
                 return self._zerotrade(holdings)
 
             # print("CVX problem at ", t, self.prob)
             u = pd.Series(index=holdings.index, data=(z.value * value))
 
             return u
-        
+
         except (cvx.SolverError, cvx.DCPError, TypeError):
             print(f"The solver failed for {t}.")
             return self._zerotrade(holdings)
```

### Comparing `investos-0.1.3/investos/util.py` & `investos-0.1.4/investos/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import copy
+from functools import wraps
 
 import numpy as np
 import pandas as pd
 
+
 def deep_dict_merge(default_d, update_d):
     "Deep copies update_d onto default_d recursively"
-    
+
     default_d = copy.deepcopy(default_d)
     update_d = copy.deepcopy(update_d)
 
     def deep_dict_merge_inner(default_d, update_d):
         for k, v in update_d.items():
-            if (k in default_d and isinstance(default_d[k], dict) and isinstance(update_d[k], dict)):
+            if (
+                k in default_d
+                and isinstance(default_d[k], dict)
+                and isinstance(update_d[k], dict)
+            ):
                 deep_dict_merge_inner(default_d[k], update_d[k])
             else:
                 default_d[k] = update_d[k]
 
     deep_dict_merge_inner(default_d, update_d)
-    return default_d # With update_d values copied onto it
+    return default_d  # With update_d values copied onto it
+
 
 def values_in_time(obj, t, tau=None):
     """
     From CVXPortfolio:
 
     Obtain value(s) of object at time t, or right before.
 
@@ -45,20 +52,31 @@
     tau: np.Timestamp (or similar), or None. Time tau >= t
         of the prediction,  e.g., tau could be tomorrow, t
         today, and we ask for prediction of market volume tomorrow,
         made today. If None, then it is assumed tau = t.
 
     """
 
-    if hasattr(obj, '__call__'):
+    if hasattr(obj, "__call__"):
         return obj(t, tau)
 
     if isinstance(obj, pd.Series) or isinstance(obj, pd.DataFrame):
         try:
             if isinstance(obj.index, pd.MultiIndex):
                 return obj.loc[(t, tau)]
             else:
                 return obj.loc[t]
         except KeyError:
             return obj
 
-    return obj
+    return obj
+
+
+def clip_for_dates(func):
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        pd_obj = func(self, *args, **kwargs)
+        return pd_obj[
+            (pd_obj.index >= self.start_date) & (pd_obj.index <= self.end_date)
+        ]
+
+    return wrapper
```

### Comparing `investos-0.1.3/PKG-INFO` & `investos-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 Metadata-Version: 2.1
 Name: investos
-Version: 0.1.3
+Version: 0.1.4
 Summary: For investors who want to focus on generating alpha
 Home-page: https://investos.io/
 License: Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)
+Keywords: investing,alpha,backtesting,portfolio,optimization
 Author: Charlie Reese
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Software Development :: Testing
 Requires-Dist: cvxpy (>=1.3.1,<2.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://investos.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/charliereese/investos
 Description-Content-Type: text/markdown
 
 # InvestOS
 
 **InvestOS** (/InvEst əʊˈes/) is a Python library for investors who want to focus on generating alpha. As it stands today, it provides reliable backtesting and portfolio optimization software for investors... but we have bigger ambitions!
 
-As mentioned in our [first blog article](https://blog.investos.io/why-we-created-investos/): _“From the start, our goal has been to support all possible optimization strategies and backtesting requirements through flexible, extensible code, while prioritizing reliability and ease-of-use. Once we feel we’ve achieved that goal as it pertains to portfolio optimization and backtesting, we plan to begin productizing other (non-IP) parts of investors’ alpha-generation process.”_
+As mentioned in our [first blog article](https://blog.investos.io/why-we-created-investos/):
+
+> From the start, our goal has been to support all possible optimization strategies and backtesting requirements through flexible, extensible code, while prioritizing reliability and ease-of-use.
+> Once we feel we’ve achieved that goal as it pertains to portfolio optimization and backtesting, we plan to begin productizing other (non-IP) parts of investors’ alpha-generation process.
 
 For more information, visit [investos.io](https://investos.io).
```

