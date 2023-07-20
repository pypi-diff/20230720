# Comparing `tmp/estyp-0.1.0.tar.gz` & `tmp/estyp-0.2.4.tar.gz`

## Comparing `estyp-0.1.0.tar` & `estyp-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.1.0/estyp/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.1.0/estyp/LICENSE
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 estyp-0.1.0/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 estyp-0.1.0/estyp/linear_model/stepwise.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.1.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.1.0/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 estyp-0.1.0/README.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 estyp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 estyp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/linear_model/stepwise.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 estyp-0.2.4/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 estyp-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 estyp-0.2.4/PKG-INFO
```

### Comparing `estyp-0.1.0/estyp/.gitignore` & `estyp-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.1.0/estyp/LICENSE` & `estyp-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.1.0/PKG-INFO` & `estyp-0.2.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.1.0
-Summary: Paquete con algunas necesidades que he tenido en python
+Version: 0.2.4
+Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
         
@@ -28,13 +28,43 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
 
-# estyp
+# ESTYP: Extended Statistical Toolkit Yet Practical
+
+## Description
+
+This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
+
+Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
+
+## Functions
+
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
+* `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
+* `testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
+
+# Installation
+
+To install this library, you can use pip:
+
+```bash
+pip install estyp
+```
+
+## License
+
+This library is under the MIT license.
+
+## Contact
+
+If you have any questions about this library, you can contact me at [errucan@gmail.com](mailto:errucan@gmail.com).
```

