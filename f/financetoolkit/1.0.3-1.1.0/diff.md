# Comparing `tmp/financetoolkit-1.0.3.tar.gz` & `tmp/financetoolkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.0.3.tar", max compression
+gzip compressed data, was "financetoolkit-1.1.0.tar", max compression
```

## Comparing `financetoolkit-1.0.3.tar` & `financetoolkit-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0    14921 2023-06-11 09:42:00.954941 financetoolkit-1.0.3/README.md
--rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.0.3/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.0.3/financetoolkit/base/__init__.py
--rw-r--r--   0        0        0     2051 2023-06-11 09:35:38.348627 financetoolkit-1.0.3/financetoolkit/base/helpers.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.0.3/financetoolkit/base/models/__init__.py
--rw-r--r--   0        0        0    10797 2023-06-11 09:35:38.349404 financetoolkit-1.0.3/financetoolkit/base/models/fundamentals_model.py
--rw-r--r--   0        0        0     4067 2023-06-11 09:35:38.350197 financetoolkit-1.0.3/financetoolkit/base/models/historical_model.py
--rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.0.3/financetoolkit/base/models/normalization/README.md
--rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.0.3/financetoolkit/base/models/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.0.3/financetoolkit/base/models/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.0.3/financetoolkit/base/models/normalization/income.csv
--rw-r--r--   0        0        0     4119 2023-06-11 09:35:38.350761 financetoolkit-1.0.3/financetoolkit/base/models/normalization_model.py
--rw-r--r--   0        0        0     2751 2023-06-11 09:35:38.350924 financetoolkit-1.0.3/financetoolkit/base/models_controller.py
--rw-r--r--   0        0        0    53898 2023-06-11 09:35:38.351456 financetoolkit-1.0.3/financetoolkit/base/ratios_controller.py
--rw-r--r--   0        0        0    17522 2023-06-11 09:35:38.351715 financetoolkit-1.0.3/financetoolkit/base/toolkit_controller.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.0.3/financetoolkit/historical/__init__.py
--rw-r--r--   0        0        0     2804 2023-06-11 09:35:38.352033 financetoolkit-1.0.3/financetoolkit/historical/price.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.0.3/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     5436 2023-06-11 09:35:38.353239 financetoolkit-1.0.3/financetoolkit/models/dupont.py
--rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.0.3/financetoolkit/portfolio/__init__.py
--rw-r--r--   0        0        0     5958 2023-06-11 09:35:38.354587 financetoolkit-1.0.3/financetoolkit/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.0.3/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9590 2023-06-11 09:35:38.355194 financetoolkit-1.0.3/financetoolkit/ratios/efficiency.py
--rw-r--r--   0        0        0     5236 2023-06-11 09:35:38.355358 financetoolkit-1.0.3/financetoolkit/ratios/liquidity.py
--rw-r--r--   0        0        0    12600 2023-06-11 09:35:38.355636 financetoolkit-1.0.3/financetoolkit/ratios/profitability.py
--rw-r--r--   0        0        0     7090 2023-06-11 09:35:38.355808 financetoolkit-1.0.3/financetoolkit/ratios/solvency.py
--rw-r--r--   0        0        0    15285 2023-06-11 09:35:38.356260 financetoolkit-1.0.3/financetoolkit/ratios/valuation.py
--rw-r--r--   0        0        0     1984 2023-06-11 09:53:44.580260 financetoolkit-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    15770 1970-01-01 00:00:00.000000 financetoolkit-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    15047 2023-07-20 09:08:23.484138 financetoolkit-1.1.0/README.md
+-rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.1.0/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.1.0/financetoolkit/base/__init__.py
+-rw-r--r--   0        0        0     3305 2023-07-20 08:13:34.949877 financetoolkit-1.1.0/financetoolkit/base/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.1.0/financetoolkit/base/models/__init__.py
+-rw-r--r--   0        0        0    12557 2023-07-20 09:07:01.496497 financetoolkit-1.1.0/financetoolkit/base/models/fundamentals_model.py
+-rw-r--r--   0        0        0     5680 2023-07-20 08:02:31.857798 financetoolkit-1.1.0/financetoolkit/base/models/historical_model.py
+-rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.1.0/financetoolkit/base/models/normalization/README.md
+-rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.1.0/financetoolkit/base/models/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.1.0/financetoolkit/base/models/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.1.0/financetoolkit/base/models/normalization/income.csv
+-rw-r--r--   0        0        0     4126 2023-07-20 07:02:40.987492 financetoolkit-1.1.0/financetoolkit/base/models/normalization_model.py
+-rw-r--r--   0        0        0     2751 2023-06-11 10:10:27.009590 financetoolkit-1.1.0/financetoolkit/base/models_controller.py
+-rw-r--r--   0        0        0    53788 2023-07-20 07:14:06.784762 financetoolkit-1.1.0/financetoolkit/base/ratios_controller.py
+-rw-r--r--   0        0        0    23583 2023-07-20 08:09:34.192259 financetoolkit-1.1.0/financetoolkit/base/toolkit_controller.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.1.0/financetoolkit/historical/__init__.py
+-rw-r--r--   0        0        0     2804 2023-06-11 10:10:27.010650 financetoolkit-1.1.0/financetoolkit/historical/price.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.1.0/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     5436 2023-06-11 10:10:27.011152 financetoolkit-1.1.0/financetoolkit/models/dupont.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.1.0/financetoolkit/portfolio/__init__.py
+-rw-r--r--   0        0        0     5958 2023-06-11 10:10:27.011432 financetoolkit-1.1.0/financetoolkit/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.1.0/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9590 2023-06-11 10:10:27.011837 financetoolkit-1.1.0/financetoolkit/ratios/efficiency.py
+-rw-r--r--   0        0        0     5236 2023-06-11 10:10:27.012162 financetoolkit-1.1.0/financetoolkit/ratios/liquidity.py
+-rw-r--r--   0        0        0    12600 2023-06-11 10:10:27.012508 financetoolkit-1.1.0/financetoolkit/ratios/profitability.py
+-rw-r--r--   0        0        0     7090 2023-06-11 10:10:27.012732 financetoolkit-1.1.0/financetoolkit/ratios/solvency.py
+-rw-r--r--   0        0        0    15285 2023-07-20 07:06:05.477276 financetoolkit-1.1.0/financetoolkit/ratios/valuation.py
+-rw-r--r--   0        0        0     1996 2023-07-20 09:08:51.836828 financetoolkit-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15896 1970-01-01 00:00:00.000000 financetoolkit-1.1.0/PKG-INFO
```

### Comparing `financetoolkit-1.0.3/LICENSE.txt` & `financetoolkit-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/README.md` & `financetoolkit-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/financetoolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
@@ -37,17 +38,14 @@
 ````
 
 Then within Python use:
 
 ```python
 from financetoolkit import Toolkit
 ```
- 
-The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines and lastly allow for any source to be incorporated to allow for the incorporation of data sources from [OpenBB](https://openbb.co/).
-
 To be able to get started, you need to obtain an API Key from FinancialModelingPrep. Use the following instructions to obtain a _free_ API Key. Note that these keys are limited to 250 requests per day but the premium plans are kept at a low cost in case you do run out of the limit or have a need for access to more data. **It is possible to use your own set of financial statements and not rely on FinancialModelingPrep, please have a look [here](#working-with-other-datasets).**
 
 1. Go to [FinancialModellingPrep's API](https://financialmodelingprep.com/developer/docs/)
 2. Under "Get your Free API Key Today!" click on "Get my API KEY here"
 3. Sign-up to the website and select the Free Plan
 4. Obtain the API Key as found [here](https://financialmodelingprep.com/developer/docs/)
 5. Start using this package.
@@ -70,14 +68,16 @@
 - Market cap and enterprise values (`enterprise`), including every intermediate step (from FinancialModelingPrep)
 - Company ratings (`rating`), based on key indicators like PE and DE ratios (from FinancialModelingPrep)
 - Historical market data (`historical_data`), which can be retrieved on a daily, weekly, monthly and yearly basis (from Yahoo Finance)
 - Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`) and Cash Flow Statements (`cash_flow_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
 - Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements.
 - Models (`models`) like DUPONT analysis that can be used to perform in-depth financial analysis through a single function.
 
+The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines and lastly allow for any source to be incorporated to allow for the incorporation of data sources from [OpenBB](https://openbb.co/).
+
 ## Using the Finance Toolkit
 
 A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%20Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
 
 ````python
 from financetoolkit import Toolkit
 
@@ -145,15 +145,15 @@
 ![Dataset Example](https://github.com/JerBouma/FinanceToolkit/assets/46355364/fe0e3db0-3e88-41d2-a355-5f68110fdcf3)
 
 If you have individual DataFrames for each company, you can do the following which will return the DataFrame structure that is required:
 
 ```python
 from financetoolkit.base import helpers
 
-balance_grouped = helpers.combine_dataframes(['AAPL', 'MSFT'], balance_apple, balance_msft)
+balance_grouped = helpers.combine_dataframes({'AAPL': balance_apple, 'MSFT': balance_msft})
 ```
 
 Once all of this is set-up you can feed this information to the Toolkit and use the Toolkit as normally.
 
 ```python
 
 # Initialize the Toolkit
```

### Comparing `financetoolkit-1.0.3/financetoolkit/base/helpers.py` & `financetoolkit-1.1.0/financetoolkit/base/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 """Helpers Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
 
-def combine_dataframes(tickers: str | list[str], *args) -> pd.DataFrame:
+def combine_dataframes(dataset_dictionary: dict[str, pd.DataFrame]) -> pd.DataFrame:
     """
     Combine the dataframes from different companies of the same financial statement,
     e.g. the balance sheet statement, into a single dataframe.
 
     Args:
-        **args: A dictionary of the same type of financial statement from multiple companies.
+        dataset_dictionary (dict[str, pd.DataFrame]): A dictionary containing the
+        dataframes for each company. It should have the structure key: ticker,
+        value: dataframe.
 
     Returns:
         pd.DataFrame: A pandas DataFrame with the combined financial statements.
     """
-    ticker_list = tickers if isinstance(tickers, list) else [tickers]
-    combined = zip(ticker_list, args)
-    combined_df = pd.concat(dict(combined), axis=0)
+    combined_df = pd.concat(dict(dataset_dictionary), axis=0)
 
     return combined_df.sort_index(level=0, sort_remaining=False)
 
 
+def equal_length(dataset1: pd.Series, dataset2: pd.Series) -> pd.Series:
+    """
+    Equalize the length of two datasets by adding zeros to the beginning of the shorter dataset.
+
+    Args:
+        dataset1 (pd.Series): The first dataset to be equalized.
+        dataset2 (pd.Series): The second dataset to be equalized.
+
+    Returns:
+        pd.Series, pd.Series: The equalized datasets.
+    """
+    if int(dataset1.columns[0]) > int(dataset2.columns[0]):
+        for value in range(
+            int(dataset1.columns[0]) - 1, int(dataset2.columns[0]) - 1, -1
+        ):
+            dataset1.insert(0, value, 0.0)
+        dataset1 = dataset1.sort_index()
+    elif int(dataset1.columns[0]) < int(dataset2.columns[0]):
+        for value in range(
+            int(dataset2.columns[0]) - 1, int(dataset1.columns[0]) - 1, -1
+        ):
+            dataset2.insert(0, value, 0.0)
+        dataset2 = dataset2.sort_index()
+
+    return dataset1, dataset2
+
+
 def handle_errors(func):
     """
     Decorator to handle specific errors that may occur in a function and provide informative messages.
 
     Args:
         func (function): The function to be decorated.
 
@@ -52,9 +79,16 @@
             function_name = func.__name__
             print(
                 f"An error occurred while trying to run the function "
                 f"{function_name}. This is {e}. Usually this is due to incomplete "
                 "financial statements. "
             )
             return pd.Series()
+        except ZeroDivisionError as e:
+            function_name = func.__name__
+            print(
+                f"An error occurred while trying to run the function "
+                f"{function_name}. This is {e}. This is due to a division by zero."
+            )
+            return pd.Series()
 
     return wrapper
```

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/fundamentals_model.py` & `financetoolkit-1.1.0/financetoolkit/base/models/fundamentals_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Fundamentals Module"""
 __docformat__ = "numpy"
 
 
+import numpy as np
 import pandas as pd
 
 from financetoolkit.base.models.normalization_model import (
     convert_financial_statements,
 )
 
 # pylint: disable=no-member
@@ -62,46 +63,72 @@
             "Please enter an API key from FinancialModelingPrep. "
             "For more information, look here: https://site.financialmodelingprep.com/developer/docs/"
         )
 
     period = "quarter" if quarter else "annual"
 
     financial_statement_dict: dict = {}
-
+    invalid_tickers = []
     for ticker in ticker_list:
         try:
             financial_statement = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/{location}/"
                 f"{ticker}?period={period}&apikey={api_key}&limit={limit}"
             )
         except Exception as error:
             raise ValueError(error) from error
 
-        financial_statement = financial_statement.drop("symbol", axis=1)
+        try:
+            financial_statement = financial_statement.drop("symbol", axis=1)
+        except KeyError:
+            print(f"No financial statement data found for {ticker}")
+            invalid_tickers.append(ticker)
+            continue
 
         if quarter:
             financial_statement["date"] = pd.to_datetime(
                 financial_statement["date"]
             ).dt.to_period("M")
         else:
             financial_statement["date"] = pd.to_datetime(
                 financial_statement["date"]
             ).dt.year
 
         financial_statement = financial_statement.set_index("date").T
 
         financial_statement_dict[ticker] = financial_statement
 
-    financial_statement_total = pd.concat(financial_statement_dict, axis=0)
+    if financial_statement_dict:
+        financial_statement_total = pd.concat(financial_statement_dict, axis=0)
 
-    financial_statement_total = convert_financial_statements(
-        financial_statement_total, statement_format, True
-    )
+        financial_statement_total = convert_financial_statements(
+            financial_statement_total, statement_format, True
+        )
 
-    return financial_statement_total
+        try:
+            financial_statement_total = financial_statement_total.astype(np.float64)
+        except ValueError as error:
+            print(
+                f"Not able to convert DataFrame to float64 due to {error}. This could result in"
+                "issues when values are zero and is prodominently relevant for "
+                "ratio calculations."
+            )
+
+        if quarter:
+            financial_statement_total.columns = pd.PeriodIndex(
+                financial_statement_total.columns, freq="M"
+            )
+        else:
+            financial_statement_total.columns = pd.PeriodIndex(
+                financial_statement_total.columns, freq="Y"
+            )
+
+        return financial_statement_total, invalid_tickers
+
+    return pd.DataFrame(), invalid_tickers
 
 
 def get_profile(tickers: list[str] | str, api_key: str):
     """
     Description
     ----
     Gives information about the profile of a company which includes
@@ -122,23 +149,27 @@
     elif isinstance(tickers, list):
         ticker_list = tickers
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
     profile_dataframe: pd.DataFrame = pd.DataFrame()
 
+    invalid_tickers = []
     for ticker in ticker_list:
         try:
             profile_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/profile/{ticker}?apikey={api_key}"
             ).T
+        except ValueError:
+            print(f"No historical data found for {ticker}")
+            invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
-    return profile_dataframe
+    return profile_dataframe, invalid_tickers
 
 
 def get_quote(tickers: list[str] | str, api_key: str):
     """
     Description
     ----
     Gives information about the quote of a company which includes i.a.
@@ -159,23 +190,27 @@
     elif isinstance(tickers, list):
         ticker_list = tickers
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
     quote_dataframe: pd.DataFrame = pd.DataFrame()
 
+    invalid_tickers = []
     for ticker in ticker_list:
         try:
             quote_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/quote/{ticker}?apikey={api_key}"
             ).T
+        except ValueError:
+            print(f"No historical data found for {ticker}")
+            invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
-    return quote_dataframe
+    return quote_dataframe, invalid_tickers
 
 
 def get_enterprise(
     tickers: list[str] | str, api_key: str, quarter: bool = False, limit: int = 100
 ):
     """
     Description
@@ -204,26 +239,33 @@
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
     enterprise_value_dict = {}
 
     period = "quarter" if quarter else "annual"
 
+    invalid_tickers = []
     for ticker in ticker_list:
         try:
             enterprise_values = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/enterprise-values/{ticker}"
                 f"?period={period}&limit={limit}&apikey={api_key}"
             )
         except Exception as error:
             raise ValueError(error) from error
 
-        enterprise_values = enterprise_values.drop("symbol", axis=1).sort_values(
-            by="date", ascending=True
-        )
+        try:
+            enterprise_values = enterprise_values.drop("symbol", axis=1).sort_values(
+                by="date", ascending=True
+            )
+        except KeyError:
+            print(f"No historical data found for {ticker}.")
+            invalid_tickers.append(ticker)
+            continue
+
         enterprise_values["date"] = pd.to_datetime(enterprise_values["date"]).dt.year
         enterprise_values = enterprise_values.set_index("date")
 
         enterprise_values = enterprise_values.rename(
             columns={
                 "stockPrice": "Stock Price",
                 "numberOfShares": "Number of Shares",
@@ -237,15 +279,15 @@
         enterprise_value_dict[ticker] = enterprise_values
 
     enterprise_dataframe = pd.concat(enterprise_value_dict, axis=0).dropna()
 
     if len(ticker_list) == 1:
         enterprise_dataframe = enterprise_dataframe.loc[ticker_list[0]]
 
-    return enterprise_dataframe
+    return enterprise_dataframe, invalid_tickers
 
 
 def get_rating(tickers: list[str] | str, api_key: str, limit: int = 100):
     """
     Description
     ----
     Gives information about the rating of a company which includes i.a. the company
@@ -265,20 +307,23 @@
         ticker_list = [tickers]
     elif isinstance(tickers, list):
         ticker_list = tickers
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
     ratings_dict = {}
-
+    invalid_tickers = []
     for ticker in ticker_list:
         try:
             ratings = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/historical-rating/{ticker}?limit={limit}&apikey={api_key}"
             )
+        except ValueError:
+            print(f"No historical data found for {ticker}")
+            invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
         ratings = ratings.drop("symbol", axis=1).sort_values(by="date", ascending=True)
         ratings = ratings.set_index("date")
 
         ratings = ratings.rename(
@@ -304,8 +349,8 @@
         ratings_dict[ticker] = ratings
 
     ratings_dataframe = pd.concat(ratings_dict, axis=0).dropna()
 
     if len(ticker_list) == 1:
         ratings_dataframe = ratings_dataframe.loc[ticker_list[0]]
 
-    return ratings_dataframe
+    return ratings_dataframe, invalid_tickers
```

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/normalization/README.md` & `financetoolkit-1.1.0/financetoolkit/base/models/normalization/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/normalization/balance.csv` & `financetoolkit-1.1.0/financetoolkit/base/models/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/normalization/cash.csv` & `financetoolkit-1.1.0/financetoolkit/base/models/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/normalization/income.csv` & `financetoolkit-1.1.0/financetoolkit/base/models/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models/normalization_model.py` & `financetoolkit-1.1.0/financetoolkit/base/models/normalization_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         financial_statements = financial_statements[financial_statements.columns[::-1]]
 
     return financial_statements.sort_index(level=0, sort_remaining=False)
 
 
 def copy_normalization_files(
     format_location: str = "",
-    save_location: str = Path(Path.home(), "Downloads"),
+    save_location: str | Path = Path(Path.home(), "Downloads"),
 ):
     """
     This function copies the normalization files as found inside the environment and saves them
     to a custom location defined by the user. This is designed to make it possible to edit these files
     and supply them to the financial statement functions and within the Analyzer class.
 
     Args:
```

### Comparing `financetoolkit-1.0.3/financetoolkit/base/models_controller.py` & `financetoolkit-1.1.0/financetoolkit/base/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/base/ratios_controller.py` & `financetoolkit-1.1.0/financetoolkit/base/ratios_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         tickers: str | list[str],
         historical: pd.DataFrame,
         balance: pd.DataFrame,
         income: pd.DataFrame,
         cash: pd.DataFrame,
     ):
         self._tickers = tickers
-        self._yearly_historical_data = historical
-        self._balance_sheet_statement = balance
-        self._income_statement = income
-        self._cash_flow_statement = cash
+        self._historical_data: pd.DataFrame = historical
+        self._balance_sheet_statement: pd.DataFrame = balance
+        self._income_statement: pd.DataFrame = income
+        self._cash_flow_statement: pd.DataFrame = cash
 
         # Initialization of Fundamentals Variables
         self._all_ratios: pd.DataFrame = pd.DataFrame()
         self._efficiency_ratios: pd.DataFrame = pd.DataFrame()
         self._liquidity_ratios: pd.DataFrame = pd.DataFrame()
         self._profitability_ratios: pd.DataFrame = pd.DataFrame()
         self._solvency_ratios: pd.DataFrame = pd.DataFrame()
@@ -113,15 +113,15 @@
             )
 
         if len(self._tickers) == 1:
             return self._efficiency_ratios.loc[self._tickers[0]]
 
         return self._efficiency_ratios
 
-    def collect_liquidity_ratios(self):
+    def collect_liquidity_ratios(self) -> pd.DataFrame:
         """
         Calculates all Liquidity Ratios based on the data provided.
         """
         if self._liquidity_ratios.empty:
             liquidity_ratios: dict = {}
 
             liquidity_ratios["Current Ratio"] = self.get_current_ratio()
@@ -146,15 +146,15 @@
             )
 
         if len(self._tickers) == 1:
             return self._liquidity_ratios.loc[self._tickers[0]]
 
         return self._liquidity_ratios
 
-    def collect_profitability_ratios(self):
+    def collect_profitability_ratios(self) -> pd.DataFrame:
         """
         Calculates all Profitability Ratios based on the data provided.
         """
         if self._profitability_ratios.empty:
             profitability_ratios: dict = {}
 
             profitability_ratios["Gross Margin"] = self.get_gross_margin()
@@ -872,17 +872,15 @@
         """
         Calculates the free cash flow yield ratio, which measures the free cash flow
         relative to the market capitalization of the company.
         """
         years = self._balance_sheet_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         average_shares = (
             self._income_statement.loc[:, "Weighted Average Shares Diluted", :]
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
@@ -1001,17 +999,15 @@
         company's stock price to its earnings per share.
         """
         eps = self.get_earnings_per_share(include_dividends, diluted)
 
         years = eps.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         return valuation.get_price_earnings_ratio(share_prices, eps)
 
     @handle_errors
     def get_price_to_earnings_growth_ratio(
         self, include_dividends: bool = False, diluted: bool = True
     ):
@@ -1049,17 +1045,15 @@
         company's market price to its book value per share.
         """
         book_value_per_share = self.get_book_value_per_share(diluted)
 
         years = book_value_per_share.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         return valuation.get_price_to_book_ratio(share_prices, book_value_per_share)
 
     @handle_errors
     def get_interest_debt_per_share(self, diluted: bool = True):
         """
         Calculate the interest debt per share, a valuation ratio that measures the
@@ -1106,17 +1100,15 @@
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
         years = self._cash_flow_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         return valuation.get_dividend_yield(
             abs(self._cash_flow_statement.loc[:, "Dividends Paid", :]),
             average_shares,
             share_prices,
         )
 
@@ -1131,19 +1123,17 @@
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
         years = self._cash_flow_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
-        market_cap = share_prices * average_shares
+        market_cap = valuation.get_market_cap(share_prices, average_shares)
 
         return valuation.get_price_to_cash_flow_ratio(
             market_cap, self._cash_flow_statement.loc[:, "Cash Flow from Operations", :]
         )
 
     @handle_errors
     def get_price_to_free_cash_flow_ratio(self, diluted: bool = True):
@@ -1156,17 +1146,15 @@
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
         years = self._cash_flow_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         market_cap = valuation.get_market_cap(share_prices, average_shares)
 
         return valuation.get_price_to_free_cash_flow_ratio(
             market_cap, self._cash_flow_statement.loc[:, "Free Cash Flow", :]
         )
 
@@ -1182,17 +1170,15 @@
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
         years = self._cash_flow_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         return valuation.get_market_cap(share_prices, average_shares)
 
     @handle_errors
     def get_enterprise_value(self, diluted: bool = True):
         """
         Calculates the Enterprise Value (EV) of a company. The Enterprise Value (EV)
@@ -1208,17 +1194,15 @@
             if diluted
             else self._income_statement.loc[:, "Weighted Average Shares", :]
         )
 
         years = self._cash_flow_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         market_cap = valuation.get_market_cap(share_prices, average_shares)
 
         return valuation.get_enterprise_value(
             market_cap,
             self._balance_sheet_statement.loc[:, "Total Debt", :],
             self._balance_sheet_statement.loc[:, "Minority Interest", :],
@@ -1273,17 +1257,15 @@
         relative to the market price per share.
         """
         eps = self.get_earnings_per_share(include_dividends, diluted)
 
         years = eps.columns
         begin, end = str(years[0]), str(years[-1])
 
-        share_prices = self._yearly_historical_data.loc[
-            begin:end, "Adj Close"
-        ].T.to_numpy()
+        share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         return valuation.get_earnings_yield(eps, share_prices)
 
     @handle_errors
     def get_payout_ratio(self):
         """
         Calculates the (dividend) payout ratio, which measures the proportion of earnings
```

### Comparing `financetoolkit-1.0.3/financetoolkit/base/toolkit_controller.py` & `financetoolkit-1.1.0/financetoolkit/base/toolkit_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     get_enterprise as _get_enterprise,
     get_financial_statements as _get_financial_statements,
     get_profile as _get_profile,
     get_quote as _get_quote,
     get_rating as _get_rating,
 )
 from financetoolkit.base.models.historical_model import (
+    convert_daily_to_quarterly as _convert_daily_to_quarterly,
     convert_daily_to_yearly as _convert_daily_to_yearly,
     get_historical_data as _get_historical_data,
 )
 from financetoolkit.base.models.normalization_model import (
     convert_financial_statements as _convert_financial_statements,
     copy_normalization_files as _copy_normalization_files,
     read_normalization_file as _read_normalization_file,
@@ -41,16 +42,18 @@
         self,
         tickers,
         api_key: str = "",
         historical: pd.DataFrame = pd.DataFrame(),
         balance: pd.DataFrame = pd.DataFrame(),
         income: pd.DataFrame = pd.DataFrame(),
         cash: pd.DataFrame = pd.DataFrame(),
+        quarterly: bool = False,
         format_location: str = "",
         reverse_dates: bool = False,
+        remove_invalid_tickers: bool = True,
     ):
         """
         Initializes an Toolkit object with a ticker or a list of tickers.
 
         Args:
         tickers (str or list): A string or a list of strings containing the company ticker(s).
         api_key (str): An API key from FinancialModelingPrep.
@@ -58,35 +61,43 @@
         balance (pd.DataFrame): A DataFrame containing balance sheet data.
         income (pd.DataFrame): A DataFrame containing income statement data.
         cash (pd.DataFrame): A DataFrame containing cash flow statement data.
         format_location (str): A string containing the location of the normalization files.
         reverse_dates (bool): A boolean indicating whether to reverse the dates in the financial statements.
         """
         if isinstance(tickers, str):
-            self._tickers = [tickers]
+            self._tickers = [tickers.upper()]
         elif isinstance(tickers, list):
-            self._tickers = tickers
+            self._tickers = [ticker.upper() for ticker in tickers]
         else:
             raise TypeError("Tickers must be a string or a list of strings.")
 
         self._api_key = api_key
+        self._quarterly = quarterly
+        self._remove_invalid_tickers = remove_invalid_tickers
+        self._invalid_tickers: list = []
 
         if self._api_key:
             # Initialization of FinancialModelingPrep Variables
             self._profile: pd.DataFrame = pd.DataFrame()
             self._quote: pd.DataFrame = pd.DataFrame()
             self._enterprise: pd.DataFrame = pd.DataFrame()
             self._rating: pd.DataFrame = pd.DataFrame()
 
         # Initialization of Historical Variables
         self._daily_historical_data: pd.DataFrame = (
             historical if not historical.empty else pd.DataFrame()
         )
         self._weekly_historical_data: pd.DataFrame = pd.DataFrame()
         self._monthly_historical_data: pd.DataFrame = pd.DataFrame()
+        self._quarterly_historical_data: pd.DataFrame = (
+            _convert_daily_to_quarterly(self._daily_historical_data)
+            if not historical.empty
+            else pd.DataFrame()
+        )
         self._yearly_historical_data: pd.DataFrame = (
             _convert_daily_to_yearly(self._daily_historical_data)
             if not historical.empty
             else pd.DataFrame()
         )
 
         # Initialization of Normalization Variables
@@ -120,15 +131,15 @@
                 cash, self._cash_flow_statement_generic, reverse_dates
             )
             if not cash.empty
             else pd.DataFrame()
         )
 
     @property
-    def ratios(self):
+    def ratios(self) -> Ratios:
         """
         Gives access to financial ratios.
         """
         empty_data: list = []
 
         if not self._api_key and (
             self._balance_sheet_statement.empty
@@ -136,42 +147,69 @@
             or self._cash_flow_statement.empty
         ):
             raise ValueError(
                 "The ratios property requires manual addition of balance, income "
                 "and cash flow statements or an API key from FinancialModelPrep "
                 "within the Toolkit class."
             )
-        if self._yearly_historical_data.empty:
-            self.get_historical_data(period="yearly")
         if self._balance_sheet_statement.empty:
             empty_data.append("Balance Sheet Statement")
             self.get_balance_sheet_statement()
         if self._income_statement.empty:
             empty_data.append("Income Statement")
             self.get_income_statement()
         if self._cash_flow_statement.empty:
             empty_data.append("Cash Flow Statement")
             self.get_cash_flow_statement()
 
+        if (
+            self._balance_sheet_statement.empty
+            and self._income_statement.empty
+            and self._cash_flow_statement.empty
+        ):
+            raise ValueError(
+                "The datasets could not be populated and therefore the Ratios class cannot be initialized."
+            )
+
+        start = f"{self._balance_sheet_statement.columns[0].year - 5}-01-01"
+        end = f"{self._balance_sheet_statement.columns[-1].year + 5}-01-01"
+
+        if self._quarterly:
+            if (
+                self._quarterly_historical_data.empty
+                and not self._balance_sheet_statement.empty
+            ):
+                self.get_historical_data(period="quarterly", start=start, end=end)
+        elif not self._quarterly:
+            if (
+                self._yearly_historical_data.empty
+                and not self._balance_sheet_statement.empty
+            ):
+                self.get_historical_data(period="yearly", start=start, end=end)
+        else:
+            raise ValueError("Invalid value for the quarterly parameter.")
+
         if empty_data:
             print(
                 "The following data was not provided within the Toolkit class and "
                 f"thus was retrieved from FinancialModelingPrep: {', '.join(empty_data)}."
             )
 
         return Ratios(
             self._tickers,
-            self._yearly_historical_data,
+            self._quarterly_historical_data
+            if self._quarterly
+            else self._yearly_historical_data,
             self._balance_sheet_statement,
             self._income_statement,
             self._cash_flow_statement,
         )
 
     @property
-    def models(self):
+    def models(self) -> Models:
         """
         Gives access to financial models.
         """
         empty_data: list = []
 
         if not self._api_key and (
             self._balance_sheet_statement.empty
@@ -190,14 +228,23 @@
         if self._income_statement.empty:
             empty_data.append("Income Statement")
             self.get_income_statement()
         if self._cash_flow_statement.empty:
             empty_data.append("Cash Flow Statement")
             self.get_cash_flow_statement()
 
+        if (
+            self._balance_sheet_statement.empty
+            and self._income_statement.empty
+            and self._cash_flow_statement.empty
+        ):
+            raise ValueError(
+                "The datasets could not be populated and therefore the Models class cannot be initialized."
+            )
+
         if empty_data:
             print(
                 "The following data was not provided within the Toolkit class and "
                 f"thus was retrieved from FinancialModelingPrep: {', '.join(empty_data)}."
             )
 
         return Models(
@@ -219,15 +266,24 @@
         """
         if not self._api_key:
             return print(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._profile.empty:
-            self._profile = _get_profile(self._tickers, self._api_key)
+            self._profile, self._invalid_tickers = _get_profile(
+                self._tickers, self._api_key
+            )
+
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
 
         return self._profile
 
     def get_quote(self):
         """
         Returns a pandas dataframe containing the stock quote information for the specified tickers.
 
@@ -239,19 +295,28 @@
         """
         if not self._api_key:
             return print(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._quote.empty:
-            self._quote = _get_quote(self._tickers, self._api_key)
+            self._quote, self._invalid_tickers = _get_quote(
+                self._tickers, self._api_key
+            )
+
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
 
         return self._quote
 
-    def get_enterprise(self, quarter: str = False, limit: str = 100):
+    def get_enterprise(self, limit: int = 100):
         """
         Returns a pandas dataframe containing the enterprise value information for the specified tickers.
 
         Args:
             quarter (str): The quarter for which the enterprise value is required. Defaults to False.
             limit (str): The number of results to return. Defaults to 100.
 
@@ -263,18 +328,25 @@
         """
         if not self._api_key:
             return print(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._enterprise.empty:
-            self._enterprise = _get_enterprise(
-                self._tickers, self._api_key, quarter, limit
+            self._enterprise, self._invalid_tickers = _get_enterprise(
+                self._tickers, self._api_key, self._quarterly, limit
             )
 
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
+
         return self._enterprise
 
     def get_rating(self, limit: int = 100):
         """
         Returns a pandas dataframe containing the stock rating information for the specified tickers.
 
         Args:
@@ -288,15 +360,24 @@
         """
         if not self._api_key:
             return print(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._rating.empty:
-            self._rating = _get_rating(self._tickers, self._api_key, limit)
+            self._rating, self._invalid_tickers = _get_rating(
+                self._tickers, self._api_key, limit
+            )
+
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
 
         return self._rating
 
     def get_historical_data(self, start=None, end=None, period: str = "daily"):
         """
         Returns a pandas dataframe containing the historical data for the specified tickers.
 
@@ -309,73 +390,138 @@
         Raises:
             ValueError: If an invalid value is specified for period.
 
         Returns:
             pandas.DataFrame: The historical data for the specified tickers.
         """
         if period == "daily":
-            self._daily_historical_data = _get_historical_data(
+            self._daily_historical_data, self._invalid_tickers = _get_historical_data(
                 self._tickers, start, end, interval="1d"
             )
 
+            if self._remove_invalid_tickers:
+                self._tickers = [
+                    ticker
+                    for ticker in self._tickers
+                    if ticker not in self._invalid_tickers
+                ]
+
+            self._daily_historical_data = self._daily_historical_data.sort_index()
+
             if len(self._tickers) == 1:
                 return self._daily_historical_data.xs(
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._daily_historical_data
 
         if period == "weekly":
-            self._weekly_historical_data = _get_historical_data(
+            self._weekly_historical_data, self._invalid_tickers = _get_historical_data(
                 self._tickers, start, end, interval="1wk"
             )
 
+            if self._remove_invalid_tickers:
+                self._tickers = [
+                    ticker
+                    for ticker in self._tickers
+                    if ticker not in self._invalid_tickers
+                ]
+
+            self._weekly_historical_data = self._weekly_historical_data.sort_index()
+
             if len(self._tickers) == 1:
                 return self._weekly_historical_data.xs(
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._weekly_historical_data
 
         if period == "monthly":
-            self._monthly_historical_data = _get_historical_data(
+            self._monthly_historical_data, self._invalid_tickers = _get_historical_data(
                 self._tickers, start, end, interval="1mo"
             )
 
+            if self._remove_invalid_tickers:
+                self._tickers = [
+                    ticker
+                    for ticker in self._tickers
+                    if ticker not in self._invalid_tickers
+                ]
+
+            self._monthly_historical_data = self._monthly_historical_data.sort_index()
+
             if len(self._tickers) == 1:
                 return self._monthly_historical_data.xs(
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._monthly_historical_data
 
-        if period == "yearly":
+        if period == "quarterly":
             if self._daily_historical_data.empty:
-                self._daily_historical_data = _get_historical_data(
-                    self._tickers, start, end, interval="1d"
+                (
+                    self._daily_historical_data,
+                    self._invalid_tickers,
+                ) = _get_historical_data(self._tickers, start, end, interval="1d")
+
+            self._quarterly_historical_data = _convert_daily_to_quarterly(
+                self._daily_historical_data
+            )
+
+            if self._remove_invalid_tickers:
+                self._tickers = [
+                    ticker
+                    for ticker in self._tickers
+                    if ticker not in self._invalid_tickers
+                ]
+
+            self._quarterly_historical_data = (
+                self._quarterly_historical_data.sort_index()
+            )
+
+            if len(self._tickers) == 1:
+                return self._quarterly_historical_data.xs(
+                    self._tickers[0], level=1, axis="columns"
                 )
 
+            return self._quarterly_historical_data
+
+        if period == "yearly":
+            if self._daily_historical_data.empty:
+                (
+                    self._daily_historical_data,
+                    self._invalid_tickers,
+                ) = _get_historical_data(self._tickers, start, end, interval="1d")
+
             self._yearly_historical_data = _convert_daily_to_yearly(
                 self._daily_historical_data
             )
 
+            if self._remove_invalid_tickers:
+                self._tickers = [
+                    ticker
+                    for ticker in self._tickers
+                    if ticker not in self._invalid_tickers
+                ]
+
+            self._yearly_historical_data = self._yearly_historical_data.sort_index()
+
             if len(self._tickers) == 1:
                 return self._yearly_historical_data.xs(
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._yearly_historical_data
 
         raise ValueError(
-            "Please choose from daily, weekly, monthly or yearly as period."
+            "Please choose from daily, weekly, monthly, quarterly or yearly as period."
         )
 
     def get_balance_sheet_statement(
         self,
-        quarter=False,
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the balance sheet statement financial data for the company(s) from the specified source.
 
         Args:
@@ -386,31 +532,40 @@
         """
         if not self._api_key and self._balance_sheet_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._balance_sheet_statement.empty or overwrite:
-            self._balance_sheet_statement = _get_financial_statements(
+            (
+                self._balance_sheet_statement,
+                self._invalid_tickers,
+            ) = _get_financial_statements(
                 self._tickers,
                 "balance",
                 self._api_key,
-                quarter,
+                self._quarterly,
                 limit,
                 self._balance_sheet_statement_generic,
             )
 
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
+
         if len(self._tickers) == 1:
             return self._balance_sheet_statement.loc[self._tickers[0]]
 
         return self._balance_sheet_statement
 
     def get_income_statement(
         self,
-        quarter=False,
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the income statement financial data for the company(s) from the specified source.
 
         Args:
@@ -421,31 +576,37 @@
         """
         if not self._api_key and self._income_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._income_statement.empty or overwrite:
-            self._income_statement = _get_financial_statements(
+            self._income_statement, self._invalid_tickers = _get_financial_statements(
                 self._tickers,
                 "income",
                 self._api_key,
-                quarter,
+                self._quarterly,
                 limit,
                 self._income_statement_generic,
             )
 
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
+
         if len(self._tickers) == 1:
             return self._income_statement.loc[self._tickers[0]]
 
         return self._income_statement
 
     def get_cash_flow_statement(
         self,
-        quarter=False,
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the cash flow statement financial data for the company(s) from the specified source.
 
         Args:
@@ -456,23 +617,33 @@
         """
         if not self._api_key and self._cash_flow_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._cash_flow_statement.empty or overwrite:
-            self._cash_flow_statement = _get_financial_statements(
+            (
+                self._cash_flow_statement,
+                self._invalid_tickers,
+            ) = _get_financial_statements(
                 self._tickers,
                 "cashflow",
                 self._api_key,
-                quarter,
+                self._quarterly,
                 limit,
                 self._cash_flow_statement_generic,
             )
 
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
+
         if len(self._tickers) == 1:
             return self._cash_flow_statement.loc[self._tickers[0]]
 
         return self._cash_flow_statement
 
     def get_normalization_files(self, path: str = ""):
         """
```

### Comparing `financetoolkit-1.0.3/financetoolkit/historical/price.py` & `financetoolkit-1.1.0/financetoolkit/historical/price.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/models/dupont.py` & `financetoolkit-1.1.0/financetoolkit/models/dupont.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/portfolio/portfolio.py` & `financetoolkit-1.1.0/financetoolkit/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/ratios/efficiency.py` & `financetoolkit-1.1.0/financetoolkit/ratios/efficiency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/ratios/liquidity.py` & `financetoolkit-1.1.0/financetoolkit/ratios/liquidity.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/ratios/profitability.py` & `financetoolkit-1.1.0/financetoolkit/ratios/profitability.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/ratios/solvency.py` & `financetoolkit-1.1.0/financetoolkit/ratios/solvency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/financetoolkit/ratios/valuation.py` & `financetoolkit-1.1.0/financetoolkit/ratios/valuation.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.3/pyproject.toml` & `financetoolkit-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.0.3"
+version = "1.1.0"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
@@ -61,13 +61,13 @@
 profile = "black"
 line_length = 122
 skip_gitignore = true
 combine_as_imports = true
 
 [tool.codespell]
 ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo'
-skip = '*.json,./.git,pyproject.toml'
+skip = '*.json,./.git,pyproject.toml,poetry.lock'
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::pytest.PytestAssertRewriteWarning:",
 ]
```

### Comparing `financetoolkit-1.0.3/PKG-INFO` & `financetoolkit-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.0.3
+Version: 1.1.0
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/
 License: MIT
 Author: Jeroen Bouma
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -19,14 +19,15 @@
 Project-URL: Repository, https://github.com/JerBouma/FinanceToolkit
 Description-Content-Type: text/markdown
 
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/financetoolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
@@ -58,17 +59,14 @@
 ````
 
 Then within Python use:
 
 ```python
 from financetoolkit import Toolkit
 ```
- 
-The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines and lastly allow for any source to be incorporated to allow for the incorporation of data sources from [OpenBB](https://openbb.co/).
-
 To be able to get started, you need to obtain an API Key from FinancialModelingPrep. Use the following instructions to obtain a _free_ API Key. Note that these keys are limited to 250 requests per day but the premium plans are kept at a low cost in case you do run out of the limit or have a need for access to more data. **It is possible to use your own set of financial statements and not rely on FinancialModelingPrep, please have a look [here](#working-with-other-datasets).**
 
 1. Go to [FinancialModellingPrep's API](https://financialmodelingprep.com/developer/docs/)
 2. Under "Get your Free API Key Today!" click on "Get my API KEY here"
 3. Sign-up to the website and select the Free Plan
 4. Obtain the API Key as found [here](https://financialmodelingprep.com/developer/docs/)
 5. Start using this package.
@@ -91,14 +89,16 @@
 - Market cap and enterprise values (`enterprise`), including every intermediate step (from FinancialModelingPrep)
 - Company ratings (`rating`), based on key indicators like PE and DE ratios (from FinancialModelingPrep)
 - Historical market data (`historical_data`), which can be retrieved on a daily, weekly, monthly and yearly basis (from Yahoo Finance)
 - Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`) and Cash Flow Statements (`cash_flow_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
 - Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements.
 - Models (`models`) like DUPONT analysis that can be used to perform in-depth financial analysis through a single function.
 
+The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines and lastly allow for any source to be incorporated to allow for the incorporation of data sources from [OpenBB](https://openbb.co/).
+
 ## Using the Finance Toolkit
 
 A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%20Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
 
 ````python
 from financetoolkit import Toolkit
 
@@ -166,15 +166,15 @@
 ![Dataset Example](https://github.com/JerBouma/FinanceToolkit/assets/46355364/fe0e3db0-3e88-41d2-a355-5f68110fdcf3)
 
 If you have individual DataFrames for each company, you can do the following which will return the DataFrame structure that is required:
 
 ```python
 from financetoolkit.base import helpers
 
-balance_grouped = helpers.combine_dataframes(['AAPL', 'MSFT'], balance_apple, balance_msft)
+balance_grouped = helpers.combine_dataframes({'AAPL': balance_apple, 'MSFT': balance_msft})
 ```
 
 Once all of this is set-up you can feed this information to the Toolkit and use the Toolkit as normally.
 
 ```python
 
 # Initialize the Toolkit
```

