# Comparing `tmp/estyp-0.2.2.tar.gz` & `tmp/estyp-0.2.3.tar.gz`

## Comparing `estyp-0.2.2.tar` & `estyp-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.2/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 estyp-0.2.2/estyp/linear_model/stepwise.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 estyp-0.2.2/estyp/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 estyp-0.2.2/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.2/LICENSE
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 estyp-0.2.2/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 estyp-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 estyp-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.3/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 estyp-0.2.3/estyp/linear_model/stepwise.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 estyp-0.2.3/estyp/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 estyp-0.2.3/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 estyp-0.2.3/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 estyp-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 estyp-0.2.3/PKG-INFO
```

### Comparing `estyp-0.2.2/estyp/linear_model/__init__.py` & `estyp-0.2.3/estyp/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.2.2/estyp/linear_model/stepwise.py` & `estyp-0.2.3/estyp/linear_model/stepwise.py`

 * *Files identical despite different names*

### Comparing `estyp-0.2.2/estyp/testing/__init__.py` & `estyp-0.2.3/estyp/testing/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ratio=1,
     alternative: Literal["two-sided", "less", "greater"] = "two-sided",
     conf_level=0.95,
 ) -> TestResults:
     """
 # F-ratio Test
 
-Performs an F-ratio test to compare the variances of two samples.
+Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
 
 ## Arguments
 
 * `x`: The first sample.
 * `y`: The second sample.
 * `ratio`: The ratio of the two variances under the null hypothesis.
 * `alternative`: The alternative hypothesis. Can be one of "two-sided", "less", or "greater".
```

### Comparing `estyp-0.2.2/estyp/testing/__base/__init__.py` & `estyp-0.2.3/estyp/testing/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.2.2/.gitignore` & `estyp-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.2.2/LICENSE` & `estyp-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.2.2/README.md` & `estyp-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
 ## Description
 
 This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
 
-Actually the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
+Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
 ## Functions
 
-`linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
-`linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-`testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
+* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
+* `testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

### Comparing `estyp-0.2.2/pyproject.toml` & `estyp-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Paquete con algunas necesidades que he tenido en python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
```

### Comparing `estyp-0.2.2/PKG-INFO` & `estyp-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.2.2
+Version: 0.2.3
 Summary: Paquete con algunas necesidades que he tenido en python
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -41,21 +41,21 @@
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
 ## Description
 
 This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
 
-Actually the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
+Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
 ## Functions
 
-`linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
-`linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-`testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
+* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
+* `testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

