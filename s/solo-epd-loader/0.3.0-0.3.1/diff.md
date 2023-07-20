# Comparing `tmp/solo_epd_loader-0.3.0.tar.gz` & `tmp/solo_epd_loader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-04rue_h5/solo_epd_loader-0.3.0.tar", last modified: Tue Jul 11 13:18:08 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-akki_32u/solo_epd_loader-0.3.1.tar", last modified: Thu Jul 20 14:47:11 2023, max compression
```

## Comparing `solo_epd_loader-0.3.0.tar` & `solo_epd_loader-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.0/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16697 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15749 2023-07-11 13:14:50.000000 solo_epd_loader-0.3.0/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.0/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.261785 solo_epd_loader-0.3.0/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.0/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.265785 solo_epd_loader-0.3.0/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.0/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.0/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.0/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.0/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.269784 solo_epd_loader-0.3.0/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.0/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.0/licenses/SUNPY_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.269784 solo_epd_loader-0.3.0/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    76151 2023-07-11 13:17:01.000000 solo_epd_loader-0.3.0/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16697 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.0/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.1/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.1/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.1/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.860363 solo_epd_loader-0.3.1/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.1/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.860363 solo_epd_loader-0.3.1/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.1/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.1/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.1/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.1/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.1/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.1/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-07-20 14:47:11.868363 solo_epd_loader-0.3.1/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    77138 2023-07-20 13:47:58.000000 solo_epd_loader-0.3.1/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.1/tox.ini
```

### Comparing `solo_epd_loader-0.3.0/LICENSE.rst` & `solo_epd_loader-0.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/PKG-INFO` & `solo_epd_loader-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -88,16 +88,16 @@
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
--  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
-   needed for ``sensor = 'step'``
+-  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'``, ``'omni'`` (string) or ``None``; not
+   needed for ``sensor = 'step'``. ``'omni'`` is just calculated as the average of the other four viewing directions: ``('sun'+'asun'+'north'+'south')/4``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
 
 Return
@@ -183,15 +183,15 @@
 
 Example 1 - low latency data
 ----------------------------
 
 Example code that loads low latency (ll) electron and proton (+alphas)
 fluxes (and errors) for EPT NORTH telescope from Apr 15 2021 to Apr 16
 2021 into two Pandas dataframes (one for protons & alphas, one for
-electrons). In general available are ‘sun’, ‘asun’, ‘north’, and ‘south’
+electrons). In general available are ‘sun’, ‘asun’, ‘north’, ‘south’, and ‘omni’
 viewing directions for ‘ept’ and ‘het’ telescopes of SolO/EPD.
 
 .. code:: python
 
    from matplotlib import pyplot as plt
    from solo_epd_loader import epd_load
```

### Comparing `solo_epd_loader-0.3.0/README.rst` & `solo_epd_loader-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
--  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
-   needed for ``sensor = 'step'``
+-  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'``, ``'omni'`` (string) or ``None``; not
+   needed for ``sensor = 'step'``. ``'omni'`` is just calculated as the average of the other four viewing directions: ``('sun'+'asun'+'north'+'south')/4``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
 
 Return
@@ -158,15 +158,15 @@
 
 Example 1 - low latency data
 ----------------------------
 
 Example code that loads low latency (ll) electron and proton (+alphas)
 fluxes (and errors) for EPT NORTH telescope from Apr 15 2021 to Apr 16
 2021 into two Pandas dataframes (one for protons & alphas, one for
-electrons). In general available are ‘sun’, ‘asun’, ‘north’, and ‘south’
+electrons). In general available are ‘sun’, ‘asun’, ‘north’, ‘south’, and ‘omni’
 viewing directions for ‘ept’ and ‘het’ telescopes of SolO/EPD.
 
 .. code:: python
 
    from matplotlib import pyplot as plt
    from solo_epd_loader import epd_load
```

### Comparing `solo_epd_loader-0.3.0/code_of_conduct.md` & `solo_epd_loader-0.3.1/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/docs/Makefile` & `solo_epd_loader-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/docs/conf.py` & `solo_epd_loader-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/docs/make.bat` & `solo_epd_loader-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.1/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.1/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/gh2021_fig_2.png` & `solo_epd_loader-0.3.1/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/gh2021_fig_2a.png` & `solo_epd_loader-0.3.1/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/licenses/LICENSE.rst` & `solo_epd_loader-0.3.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/licenses/SUNPY_LICENSE.rst` & `solo_epd_loader-0.3.1/licenses/SUNPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/setup.cfg` & `solo_epd_loader-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/setup.py` & `solo_epd_loader-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.1/solo_epd_loader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from packaging.version import Version
 from pathlib import Path
 
 import cdflib
 import numpy as np
 import pandas as pd
 from astropy.io.votable import parse_single_table
+from tqdm import tqdm
 
 if hasattr(sunpy, "__version__") and Version(sunpy.__version__) >= Version("5.0.0"):
     from sunpy.io._cdf import read_cdf, _known_units
 else:
     from sunpy.io.cdf import read_cdf, _known_units
 from sunpy.timeseries import TimeSeries
 
@@ -465,17 +466,18 @@
         or dt.datetime(2021,4,15)). Or a combined integer yyyymmdd with year
         (yyyy), month (mm) and day (dd) with empty positions filled with zeros,
         e.g. 20210415
         (if no enddate is given, 'enddate = startdate' will be set)
     level : {'l2', 'll'}, optional
         Defines level of data product: level 2 ('l2') or low-latency ('ll'). By
         default 'l2'
-    viewing : {'sun', 'asun', 'north', 'south' or None}, optional
-        Viewing direction of sensor. Required for 'ept' or 'het'; for 'step'
-        should be None. By default None
+    viewing : {'sun', 'asun', 'north', 'south', 'omni' or None}, optional
+        Viewing direction of sensor. 'omni' is just calculated as the average of
+        the other four viewing directions: ('sun'+'asun'+'north'+'south')/4
+        Required for 'ept' or 'het'; for 'step' should be None. By default None
     path : str, optional
         User-specified directory in which Solar Orbiter data is/should be
         organized; e.g. '/home/userxyz/solo/data/', by default None
     autodownload : bool, optional
         If True, will try to download missing data files from SOAR, by default
         False.
     only_averages : bool, optional
@@ -549,26 +551,38 @@
     if sensor.lower() == 'ept' or sensor.lower() == 'het':
         if viewing is None:
             raise Exception("EPT and HET need a telescope 'viewing' " +
                             "direction! No data read!")
             df_epd_p = []
             df_epd_e = []
             energies_dict = []
+        elif viewing is 'omni':
+            all_df_epd_p = {}
+            all_df_epd_e = {}
+            for view in ['sun', 'asun', 'north', 'south']:
+                df_epd_p, df_epd_e, energies_dict = \
+                    _read_epd_cdf(sensor=sensor, viewing=view, level=level, startdate=startdate, enddate=enddate,
+                                  path=path, autodownload=autodownload)
+                all_df_epd_p[view] = df_epd_p
+                all_df_epd_e[view] = df_epd_e
+            # sum fluxes from all four sectors and divide by 4
+            df_epd_p = (all_df_epd_p['sun'] + all_df_epd_p['asun'] + all_df_epd_p['north'] + all_df_epd_p['south'])/4
+            df_epd_e = (all_df_epd_e['sun'] + all_df_epd_e['asun'] + all_df_epd_e['north'] + all_df_epd_e['south'])/4
         else:
             df_epd_p, df_epd_e, energies_dict = \
                 _read_epd_cdf(sensor=sensor, viewing=viewing, level=level, startdate=startdate, enddate=enddate,
                               path=path, autodownload=autodownload)
         return df_epd_p, df_epd_e, energies_dict
 
 
 def _read_epd_cdf(sensor, viewing, level, startdate, enddate=None, path=None, autodownload=False):
     """
     INPUT:
         sensor: 'ept' or 'het' (string)
-        viewing: 'sun', 'asun', 'north', or 'south' (string)
+        viewing: 'sun', 'asun', 'north', 'south', or 'omni' (string)
         level: 'll' or 'l2' (string)
         startdate,
         enddate:    YYYYMMDD, e.g., 20210415 (integer)
                     (if no enddate is given, 'enddate = startdate' will be set)
         path: directory in which Solar Orbiter data is/should be organized;
               e.g. '/home/userxyz/uni/solo/data/' (string)
         autodownload: if True will try to download missing data files from SOAR
@@ -970,15 +984,16 @@
                 #     print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
             else:
                 datadf, energies_dict = _read_new_step_cdf(filelist, only_averages)
         elif product == 'main':
             datadf, energies_dict = _read_new_step_cdf(filelist, only_averages)
 
     # rename index column (instead of e.g. 'EPOCH' or 'EPOCH_1')
-    datadf.index.names = ['Time']
+    if type(datadf) is pd.DataFrame:
+        datadf.index.names = ['Time']
 
     '''
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return datadf, energies_dict
@@ -1190,15 +1205,15 @@
     df = df.copy()
 
     Electron_Flux_Mult = meta['Electron_Flux_Mult']
 
     if resample:
         # for all Integral and Magnet Uncertainties:
         col_uncertainties = df.filter(like=f'_Uncertainty_').columns.tolist()
-        for delta_flux in col_uncertainties:
+        for delta_flux in tqdm(col_uncertainties):
             # overwrite x_Uncertainty with temp. variable x_Uncertainty**2 * dt**2 that is summed in the resampling
             df[delta_flux] = df[delta_flux]**2 * df['DELTA_EPOCH']**2
 
         # select columns that should be summed in the resampling process (instead of calculating the mean)
         col_sum = col_uncertainties.copy()
         col_sum.insert(0, 'DELTA_EPOCH')  # same as append, but puts it to the start of the list (not really necessary)
```

### Comparing `solo_epd_loader-0.3.0/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.1/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -88,16 +88,16 @@
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
 -  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
--  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
-   needed for ``sensor = 'step'``
+-  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'``, ``'omni'`` (string) or ``None``; not
+   needed for ``sensor = 'step'``. ``'omni'`` is just calculated as the average of the other four viewing directions: ``('sun'+'asun'+'north'+'south')/4``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
 -  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
 - ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
 
 Return
@@ -183,15 +183,15 @@
 
 Example 1 - low latency data
 ----------------------------
 
 Example code that loads low latency (ll) electron and proton (+alphas)
 fluxes (and errors) for EPT NORTH telescope from Apr 15 2021 to Apr 16
 2021 into two Pandas dataframes (one for protons & alphas, one for
-electrons). In general available are ‘sun’, ‘asun’, ‘north’, and ‘south’
+electrons). In general available are ‘sun’, ‘asun’, ‘north’, ‘south’, and ‘omni’
 viewing directions for ‘ept’ and ‘het’ telescopes of SolO/EPD.
 
 .. code:: python
 
    from matplotlib import pyplot as plt
    from solo_epd_loader import epd_load
```

### Comparing `solo_epd_loader-0.3.0/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.3.1/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.0/tox.ini` & `solo_epd_loader-0.3.1/tox.ini`

 * *Files identical despite different names*

