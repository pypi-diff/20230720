# Comparing `tmp/advanced-ta-0.1.0.tar.gz` & `tmp/advanced-ta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced-ta-0.1.0.tar", max compression
+gzip compressed data, was "advanced-ta-0.1.1.tar", max compression
```

## Comparing `advanced-ta-0.1.0.tar` & `advanced-ta-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,9 @@
--rw-r--r--   0        0        0      562 2023-07-20 18:32:34.878723 advanced-ta-0.1.0/README.md
--rw-r--r--   0        0        0    26037 2023-07-20 17:13:04.487663 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/Classifier.py
--rw-r--r--   0        0        0     2689 2023-07-20 17:14:25.348338 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/KernelFunctions.py
--rw-r--r--   0        0        0     7252 2023-07-20 17:16:02.641151 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/MLExtensions.py
--rw-r--r--   0        0        0     1891 2023-07-20 15:20:39.939402 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/Types.py
--rw-r--r--   0        0        0     8886 2023-07-20 17:13:05.343670 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/__pycache__/Classifier.cpython-310.pyc
--rw-r--r--   0        0        0     1050 2023-07-20 17:14:26.476348 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/__pycache__/KernelFunctions.cpython-310.pyc
--rw-r--r--   0        0        0     8705 2023-07-19 21:40:31.705946 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/__pycache__/LorentzianClassification.cpython-310.pyc
--rw-r--r--   0        0        0     3986 2023-07-20 17:16:03.453157 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/__pycache__/MLExtensions.cpython-310.pyc
--rw-r--r--   0        0        0     1906 2023-07-20 15:20:39.947402 advanced-ta-0.1.0/advanced_ta/LorentzianClassification/__pycache__/Types.cpython-310.pyc
--rw-r--r--   0        0        0       73 2023-07-20 15:29:10.313143 advanced-ta-0.1.0/advanced_ta/__init__.py
--rw-r--r--   0        0        0      523 2023-07-20 18:35:22.560123 advanced-ta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1411 2023-07-20 18:35:39.567394 advanced-ta-0.1.0/setup.py
--rw-r--r--   0        0        0     1177 2023-07-20 18:35:39.567587 advanced-ta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      562 2023-07-20 18:32:34.878723 advanced-ta-0.1.1/README.md
+-rw-r--r--   0        0        0    26037 2023-07-20 19:33:10.956673 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Classifier.py
+-rw-r--r--   0        0        0     2689 2023-07-20 17:14:25.348338 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/KernelFunctions.py
+-rw-r--r--   0        0        0     7252 2023-07-20 17:16:02.641151 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/MLExtensions.py
+-rw-r--r--   0        0        0     1891 2023-07-20 15:20:39.939402 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Types.py
+-rw-r--r--   0        0        0       73 2023-07-20 15:29:10.313143 advanced-ta-0.1.1/advanced_ta/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-20 19:33:50.072998 advanced-ta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1451 2023-07-20 19:34:16.618661 advanced-ta-0.1.1/setup.py
+-rw-r--r--   0        0        0     1299 2023-07-20 19:34:16.618857 advanced-ta-0.1.1/PKG-INFO
```

### Comparing `advanced-ta-0.1.0/README.md` & `advanced-ta-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.0/advanced_ta/LorentzianClassification/Classifier.py` & `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Classifier.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.0/advanced_ta/LorentzianClassification/KernelFunctions.py` & `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/KernelFunctions.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.0/advanced_ta/LorentzianClassification/MLExtensions.py` & `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/MLExtensions.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.0/advanced_ta/LorentzianClassification/Types.py` & `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Types.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.0/pyproject.toml` & `advanced-ta-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "advanced-ta"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python implementation of Lorentzian Classification algorithm."
 authors = ["Loki Arya <loki.arya+osdev@gmail.com>"]
 readme = "README.md"
+repository = "https://bitbucket.org/lokiarya/advanced-ta"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.25.1"
 pandas = "^2.0.3"
 TA-Lib = "^0.4.27"
 python-dotenv = "^1.0.0"
```

### Comparing `advanced-ta-0.1.0/setup.py` & `advanced-ta-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
  'numpy>=1.25.1,<2.0.0',
  'pandas>=2.0.3,<3.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'scikit-learn>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'advanced-ta',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python implementation of Lorentzian Classification algorithm.',
     'long_description': 'This module is a python implementation of Lorentzian Classification algorithm developed by @jdehorty in pinescript. The original work can be found here - https://www.tradingview.com/script/WhBzgfDu-Machine-Learning-Lorentzian-Classification/\n\n## Prerequisites\n> Ensure that [TA-Lib](https://ta-lib.org/hdr_dw.html) is downloaded and built for your platform. Set `TA_INCLUDE_PATH` and `TA_LIBRARY_PATH` as mentioned in [ta-lib-python](https://github.com/TA-Lib/ta-lib-python#installation). TA-Lib package itself will be installed as a dependency of `advanced-ta`.',
     'author': 'Loki Arya',
     'author_email': 'loki.arya+osdev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
-    'url': None,
+    'url': 'https://bitbucket.org/lokiarya/advanced-ta',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `advanced-ta-0.1.0/PKG-INFO` & `advanced-ta-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: advanced-ta
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of Lorentzian Classification algorithm.
+Home-page: https://bitbucket.org/lokiarya/advanced-ta
 Author: Loki Arya
 Author-email: loki.arya+osdev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: TA-Lib (>=0.4.27,<0.5.0)
 Requires-Dist: mplfinance (>=0.12.9-beta.7,<0.13.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
+Project-URL: Repository, https://bitbucket.org/lokiarya/advanced-ta
 Description-Content-Type: text/markdown
 
 This module is a python implementation of Lorentzian Classification algorithm developed by @jdehorty in pinescript. The original work can be found here - https://www.tradingview.com/script/WhBzgfDu-Machine-Learning-Lorentzian-Classification/
 
 ## Prerequisites
 > Ensure that [TA-Lib](https://ta-lib.org/hdr_dw.html) is downloaded and built for your platform. Set `TA_INCLUDE_PATH` and `TA_LIBRARY_PATH` as mentioned in [ta-lib-python](https://github.com/TA-Lib/ta-lib-python#installation). TA-Lib package itself will be installed as a dependency of `advanced-ta`.
```

