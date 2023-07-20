# Comparing `tmp/ltsfit-6.0.1.tar.gz` & `tmp/ltsfit-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltsfit-6.0.1.tar", last modified: Thu Jul 20 11:20:32 2023, max compression
+gzip compressed data, was "ltsfit-6.0.2.tar", last modified: Thu Jul 20 11:26:00 2023, max compression
```

## Comparing `ltsfit-6.0.1.tar` & `ltsfit-6.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/
--rw-rw-rw-   0        0        0    13646 2023-07-20 11:20:32.757317 ltsfit-6.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.726063 ltsfit-6.0.1/ltsfit/
--rw-rw-rw-   0        0        0     3961 2023-07-20 10:55:57.000000 ltsfit-6.0.1/ltsfit/CHANGELOG.rst
--rw-rw-rw-   0        0        0      398 2023-07-07 13:04:21.000000 ltsfit-6.0.1/ltsfit/LICENSE.txt
--rw-rw-rw-   0        0        0     2751 2023-07-07 13:18:09.000000 ltsfit-6.0.1/ltsfit/README.rst
--rw-rw-rw-   0        0        0       23 2023-07-20 10:56:06.000000 ltsfit-6.0.1/ltsfit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/ltsfit/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-6.0.1/ltsfit/examples/__init__.py
--rw-rw-rw-   0        0        0     6416 2023-07-20 11:18:04.000000 ltsfit-6.0.1/ltsfit/examples/ltsfit_examples.py
--rw-rw-rw-   0        0        0     4151 2023-07-20 10:53:10.000000 ltsfit-6.0.1/ltsfit/examples/ltsfit_python_reference_output.txt
--rw-rw-rw-   0        0        0      710 2023-07-18 06:10:19.000000 ltsfit-6.0.1/ltsfit/lts_linefit.py
--rw-rw-rw-   0        0        0      980 2023-07-18 06:12:24.000000 ltsfit-6.0.1/ltsfit/lts_planefit.py
--rw-rw-rw-   0        0        0    21941 2023-07-20 11:19:29.000000 ltsfit-6.0.1/ltsfit/ltsfit.py
-drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/ltsfit.egg-info/
--rw-rw-rw-   0        0        0    13646 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-07-20 11:20:32.757317 ltsfit-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-20 10:57:13.000000 ltsfit-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:26:00.014384 ltsfit-6.0.2/
+-rw-rw-rw-   0        0        0    13646 2023-07-20 11:26:00.014384 ltsfit-6.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 11:25:59.983138 ltsfit-6.0.2/ltsfit/
+-rw-rw-rw-   0        0        0     3961 2023-07-20 10:55:57.000000 ltsfit-6.0.2/ltsfit/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2023-07-07 13:04:21.000000 ltsfit-6.0.2/ltsfit/LICENSE.txt
+-rw-rw-rw-   0        0        0     2751 2023-07-07 13:18:09.000000 ltsfit-6.0.2/ltsfit/README.rst
+-rw-rw-rw-   0        0        0       23 2023-07-20 11:25:42.000000 ltsfit-6.0.2/ltsfit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:26:00.014384 ltsfit-6.0.2/ltsfit/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-6.0.2/ltsfit/examples/__init__.py
+-rw-rw-rw-   0        0        0     6361 2023-07-20 11:25:42.000000 ltsfit-6.0.2/ltsfit/examples/ltsfit_examples.py
+-rw-rw-rw-   0        0        0     4151 2023-07-20 10:53:10.000000 ltsfit-6.0.2/ltsfit/examples/ltsfit_python_reference_output.txt
+-rw-rw-rw-   0        0        0      710 2023-07-18 06:10:19.000000 ltsfit-6.0.2/ltsfit/lts_linefit.py
+-rw-rw-rw-   0        0        0      980 2023-07-18 06:12:24.000000 ltsfit-6.0.2/ltsfit/lts_planefit.py
+-rw-rw-rw-   0        0        0    21941 2023-07-20 11:19:29.000000 ltsfit-6.0.2/ltsfit/ltsfit.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:25:59.998767 ltsfit-6.0.2/ltsfit.egg-info/
+-rw-rw-rw-   0        0        0    13646 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 11:25:59.000000 ltsfit-6.0.2/ltsfit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-20 11:26:00.014384 ltsfit-6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-20 10:57:13.000000 ltsfit-6.0.2/setup.py
```

### Comparing `ltsfit-6.0.1/PKG-INFO` & `ltsfit-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 6.0.1
+Version: 6.0.2
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ltsfit-6.0.1/ltsfit/CHANGELOG.rst` & `ltsfit-6.0.2/ltsfit/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit/README.rst` & `ltsfit-6.0.2/ltsfit/README.rst`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit/examples/ltsfit_examples.py` & `ltsfit-6.0.2/ltsfit/examples/ltsfit_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Usage example for ltsfit() fitting a line in 2-dim.
     In this example I assume that 10% of the values are strong outliers.
 
     """
     print('-'*70 + "\nExample fitting a line in 2-dim\n" + '-'*70 + '\n')
 
     ntot = 300  # Total number of values
-    frac = 0.4  # fraction of outliers
+    frac = 0.1  # fraction of outliers
 
     # Coefficients of the test line
     a = 10.
     b = 1.
 
     n = int(ntot*(1 - frac))  # (1 - frac) good values
     rng = np.random.default_rng(913)
@@ -51,15 +51,14 @@
     #
     x = np.append(x, x1)
     y = np.append(y, y1)
 
     sigx = np.full_like(x, sigx)  # Adopted error in x
     sigy = np.full_like(x, sigy)  # Adopted error in y
 
-    # Important: use the kwyword `pivot` as done below
     plt.clf()
     pivot = np.round(np.median(x))
     p = ltsfit(x, y, sigx, sigy, pivot=pivot)
     plt.pause(1)
 
     # Illustrates how to obtain the best-fitting values from the class
     print(f"The best fitting parameters are: {p.coef}\n")
```

### Comparing `ltsfit-6.0.1/ltsfit/examples/ltsfit_python_reference_output.txt` & `ltsfit-6.0.2/ltsfit/examples/ltsfit_python_reference_output.txt`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit/lts_linefit.py` & `ltsfit-6.0.2/ltsfit/lts_linefit.py`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit/lts_planefit.py` & `ltsfit-6.0.2/ltsfit/lts_planefit.py`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit/ltsfit.py` & `ltsfit-6.0.2/ltsfit/ltsfit.py`

 * *Files identical despite different names*

### Comparing `ltsfit-6.0.1/ltsfit.egg-info/PKG-INFO` & `ltsfit-6.0.2/ltsfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 6.0.1
+Version: 6.0.2
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ltsfit-6.0.1/setup.py` & `ltsfit-6.0.2/setup.py`

 * *Files identical despite different names*

