# Comparing `tmp/easyfrenchtax-0.0.7.tar.gz` & `tmp/easyfrenchtax-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.7.tar", last modified: Mon Jul 10 22:03:01 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.8.tar", last modified: Thu Jul 20 16:54:07 2023, max compression
```

## Comparing `easyfrenchtax-0.0.7.tar` & `easyfrenchtax-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.370544 easyfrenchtax-0.0.7/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.7/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-10 22:03:01.370637 easyfrenchtax-0.0.7/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.7/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.7/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-10 22:03:01.370939 easyfrenchtax-0.0.7/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.365499 easyfrenchtax-0.0.7/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.367038 easyfrenchtax-0.0.7/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    21251 2023-07-10 22:00:39.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.368043 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.370280 easyfrenchtax-0.0.7/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.7/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.7/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.7/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.7/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    12964 2023-07-10 21:59:44.000000 easyfrenchtax-0.0.7/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.354313 easyfrenchtax-0.0.8/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.8/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-20 16:54:07.354391 easyfrenchtax-0.0.8/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.8/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.8/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-20 16:54:07.354672 easyfrenchtax-0.0.8/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.350046 easyfrenchtax-0.0.8/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.351788 easyfrenchtax-0.0.8/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      114 2023-07-16 12:40:46.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    22810 2023-07-20 14:14:29.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.352835 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.354077 easyfrenchtax-0.0.8/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.8/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.8/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.8/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.8/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    14179 2023-07-20 16:51:06.000000 easyfrenchtax-0.0.8/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.7/LICENSE` & `easyfrenchtax-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/PKG-INFO` & `easyfrenchtax-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.7/README.md` & `easyfrenchtax-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/setup.cfg` & `easyfrenchtax-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.7
+version = 0.0.8
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.7/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.8/src/easyfrenchtax/stock_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from enum import Enum
-from typing import Optional
+from typing import Optional, Tuple
 
 from dateutil.relativedelta import relativedelta
 from currency_converter import CurrencyConverter
 from collections import defaultdict
 import csv
 import glob
 
 class RsuTaxScheme(Enum):
-    NONQUALIFIED_RSU = 1
-    QUALIFIED_RSU = 2
-    MACRON_1_RSU = 3
-    MACRON_2_RSU = 4
-    MACRON_3_RSU = 5
+    NONQUALIFIED_RSU = "Non-qualified RSU"
+    QUALIFIED_RSU = "Qualified RSU"
+    MACRON_1_RSU = "Macron I"
+    MACRON_2_RSU = "Macron II"
+    MACRON_3_RSU = "Macron III"
 
 class StockType(Enum):
     RSU = 1
     ESPP = 2
     STOCKOPTIONS = 3
 
 @dataclass
@@ -431,14 +431,36 @@
             total_capital_gain += result
         if total_capital_gain >= 0:
             tax_report["2042C"]["capital_gain_3VG"] = total_capital_gain
         else:
             tax_report["2042C"]["capital_loss_3VH"] = -total_capital_gain
         return tax_report
 
+    def estimate_tax(self, acquisition_gain_info, capital_gain_info, marginal_tax_rate) -> Tuple[int, int]:
+        exercise_gain_1_1TT = acquisition_gain_info.get("exercise_gain_1_1TT", 0)
+        exercise_gain_2_1UT = acquisition_gain_info.get("exercise_gain_2_1UT", 0)
+        acquisition_gain_rebates_1UZ = acquisition_gain_info.get("acquisition_gain_rebates_1UZ", 0)
+        acquisition_gain_50p_rebates_1WZ = acquisition_gain_info.get("acquisition_gain_50p_rebates_1WZ", 0)
+        taxable_acquisition_gain_1TZ = acquisition_gain_info.get("taxable_acquisition_gain_1TZ", 0)
+        capital_gain_3VG = capital_gain_info.get("2042C", {}).get("capital_gain_3VG", 0)
+
+        taxable_income = (exercise_gain_1_1TT + exercise_gain_2_1UT) * 0.9 + taxable_acquisition_gain_1TZ
+        csgcrds_base = taxable_acquisition_gain_1TZ + acquisition_gain_rebates_1UZ + acquisition_gain_50p_rebates_1WZ + capital_gain_3VG
+        activity_income_crds_base = exercise_gain_1_1TT + exercise_gain_2_1UT
+        salary_contrib_10p_base = exercise_gain_1_1TT + exercise_gain_2_1UT
+
+        incremental_income_tax = round(taxable_income * marginal_tax_rate)
+        incremental_capital_tax = round(capital_gain_3VG * 0.128)
+        incremental_social_tax = round(
+            (csgcrds_base + activity_income_crds_base) * 0.097 +
+            csgcrds_base * 0.075 +
+            salary_contrib_10p_base * 0.1
+        )
+        return incremental_income_tax + incremental_capital_tax, incremental_social_tax
+
     @staticmethod
     def helper_capital_gain_tax(tax_report):
         form_2042c = tax_report["2042C"]
         print(f"Form 2042C:")
         if "capital_loss_3VH" in form_2042c:
             print(f" * 3VH: {form_2042c['capital_loss_3VH']}")
             print(f"(no need for form 2074)")
```

### Comparing `easyfrenchtax-0.0.7/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.8/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.7/tests/test_capital_tax.py` & `easyfrenchtax-0.0.8/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.8/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/tests/test_income_tax.py` & `easyfrenchtax-0.0.8/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/tests/test_rental_tax.py` & `easyfrenchtax-0.0.8/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.7/tests/test_stock_helper.py` & `easyfrenchtax-0.0.8/tests/test_stock_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -236,7 +236,37 @@
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
     stock_helper_with_plan.reset(symbols=["BUD"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
+
+def test_estimate_tax_rsu_acquisition_gain():
+    agi = {
+        "acquisition_gain_rebates_1UZ": 16000,
+        "acquisition_gain_50p_rebates_1WZ": 32000,
+        "taxable_acquisition_gain_1TZ": 8000
+    }
+    stock_helper = StockHelper()
+    marginal_rate = 0.15
+    income_tax, social_tax = stock_helper.estimate_tax(agi, {}, marginal_rate)
+    assert income_tax == 8000 * marginal_rate
+    assert social_tax == (32000+16000+8000) * (0.097+0.075)  # CSG / CRDS / Solidarité
+
+def test_estimate_tax_capital_gain():
+    cgi = {"2042C" : {"capital_gain_3VG": 1000}}
+    stock_helper = StockHelper()
+    income_tax, social_tax = stock_helper.estimate_tax({}, cgi, 0)
+    assert income_tax == 1000 * 0.128
+    assert social_tax == 1000 * (0.097+0.075)  # CSG / CRDS / Solidarité
+
+def test_estimate_stock_options_exercise():
+    agi = {
+        "exercise_gain_1_1TT": 16000,
+        "exercise_gain_2_1UT": 32000,
+    }
+    stock_helper = StockHelper()
+    marginal_rate = 0.15
+    income_tax, social_tax = stock_helper.estimate_tax(agi, {}, marginal_rate)
+    assert income_tax == (16000 + 32000) * 0.9 * marginal_rate
+    assert social_tax == (16000 + 32000) * (0.097 + 0.1)  # CSG / CRDS / 10% Salary contribution
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

