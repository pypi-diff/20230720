# Comparing `tmp/spelunker-0.5.4.tar.gz` & `tmp/spelunker-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spelunker-0.5.4.tar", last modified: Thu Jul 20 03:59:04 2023, max compression
+gzip compressed data, was "spelunker-0.5.5.tar", last modified: Thu Jul 20 14:48:33 2023, max compression
```

## Comparing `spelunker-0.5.4.tar` & `spelunker-0.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 03:59:04.606035 spelunker-0.5.4/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-0.5.4/LICENSE
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4050 2023-07-20 03:59:04.606254 spelunker-0.5.4/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     3668 2023-07-20 01:37:44.000000 spelunker-0.5.4/README.md
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-07-20 03:59:04.607308 spelunker-0.5.4/setup.cfg
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      929 2023-07-20 02:43:12.000000 spelunker-0.5.4/setup.py
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 03:59:04.602579 spelunker-0.5.4/spelunker.egg-info/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4050 2023-07-20 03:59:04.000000 spelunker-0.5.4/spelunker.egg-info/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-07-20 03:59:04.000000 spelunker-0.5.4/spelunker.egg-info/SOURCES.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 03:59:04.000000 spelunker-0.5.4/spelunker.egg-info/dependency_links.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 02:44:16.000000 spelunker-0.5.4/spelunker.egg-info/not-zip-safe
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       68 2023-07-20 03:59:04.000000 spelunker-0.5.4/spelunker.egg-info/requires.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-07-20 03:59:04.000000 spelunker-0.5.4/spelunker.egg-info/top_level.txt
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 03:59:04.605436 spelunker-0.5.4/src/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-0.5.4/src/__init__.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-07-20 03:58:18.000000 spelunker-0.5.4/src/_version.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 03:46:26.000000 spelunker-0.5.4/src/dashboard.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    42777 2023-07-20 03:38:07.000000 spelunker-0.5.4/src/spelunker.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.457543 spelunker-0.5.5/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-0.5.5/LICENSE
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4213 2023-07-20 14:48:33.457916 spelunker-0.5.5/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     3673 2023-07-20 14:27:18.000000 spelunker-0.5.5/README.md
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-07-20 14:48:33.459364 spelunker-0.5.5/setup.cfg
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1047 2023-07-20 14:43:56.000000 spelunker-0.5.5/setup.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.453137 spelunker-0.5.5/spelunker.egg-info/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4213 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/SOURCES.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/dependency_links.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/not-zip-safe
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       74 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/requires.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/top_level.txt
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.456449 spelunker-0.5.5/src/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-0.5.5/src/__init__.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-07-20 14:46:06.000000 spelunker-0.5.5/src/_version.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 03:46:26.000000 spelunker-0.5.5/src/dashboard.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    42777 2023-07-20 03:38:07.000000 spelunker-0.5.5/src/spelunker.py
```

### Comparing `spelunker-0.5.4/LICENSE` & `spelunker-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spelunker-0.5.4/PKG-INFO` & `spelunker-0.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 0.5.4
+Version: 0.5.5
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
+Requires: numpy
+Requires: scipy
+Requires: pandas
+Requires: jwst
+Requires: astroquery
+Requires: astropy
+Requires: astroplan
+Requires: matplotlib
+Requires: ray
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spelunker — NIRISS FGS quicklook pipeline 
 
 ![](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/spelunker.png)
@@ -47,15 +56,15 @@
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or the FGS tracks a new guidestar.
+We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
```

### Comparing `spelunker-0.5.4/README.md` & `spelunker-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or the FGS tracks a new guidestar.
+We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
```

### Comparing `spelunker-0.5.4/setup.py` & `spelunker-0.5.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,11 +16,12 @@
       description='spelunker: a library to extract guidestar data and observe technical and stellar events',
       url='https://github.com/GalagaBits/JWST-FGS-Spelunker',
       author='Derod Deal',
       author_email='dealderod@ufl.edu',
       license='MIT',
       packages=['spelunker'],
       package_dir={'spelunker': 'src'},
-      install_requires=['numpy','scipy', 'pandas', 'jwst', 'astroquery', 'astropy','astroplan','matplotlib', 'ray'],
+      requires=['numpy','scipy', 'pandas', 'jwst', 'astroquery', 'astropy','astroplan','matplotlib', 'ray'],
+      install_requires=['numpy','scipy', 'pandas', 'jwst', 'astroquery', 'astropy','astroplan','matplotlib', 'ray', 'wheel'],
       keywords='guidestars',
       python_requires='>=3.0',
       zip_safe=False)
```

### Comparing `spelunker-0.5.4/spelunker.egg-info/PKG-INFO` & `spelunker-0.5.5/spelunker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 0.5.4
+Version: 0.5.5
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
+Requires: numpy
+Requires: scipy
+Requires: pandas
+Requires: jwst
+Requires: astroquery
+Requires: astropy
+Requires: astroplan
+Requires: matplotlib
+Requires: ray
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spelunker — NIRISS FGS quicklook pipeline 
 
 ![](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/spelunker.png)
@@ -47,15 +56,15 @@
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or the FGS tracks a new guidestar.
+We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
```

### Comparing `spelunker-0.5.4/src/spelunker.py` & `spelunker-0.5.5/src/spelunker.py`

 * *Files identical despite different names*

