# Comparing `tmp/ecallisto_ng-0.2.4.tar.gz` & `tmp/ecallisto_ng-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.4.tar", last modified: Wed Jul 19 09:57:36 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.5.tar", last modified: Wed Jul 19 13:09:25 2023, max compression
```

## Comparing `ecallisto_ng-0.2.4.tar` & `ecallisto_ng-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.4/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.4/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-19 09:20:12.000000 ecallisto_ng-0.2.4/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8924 2023-07-19 09:20:02.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2954 2023-07-19 09:56:22.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.5/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3525 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2945 2023-07-19 13:07:49.000000 ecallisto_ng-0.2.5/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-19 13:09:17.000000 ecallisto_ng-0.2.5/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-19 13:09:25.385265 ecallisto_ng-0.2.5/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.363598 ecallisto_ng-0.2.5/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.363598 ecallisto_ng-0.2.5/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8924 2023-07-19 09:20:02.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5646 2023-07-19 13:08:15.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2954 2023-07-19 09:56:22.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3525 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.4/LICENSE` & `ecallisto_ng-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.4/PKG-INFO` & `ecallisto_ng-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,8 +79,7 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.2.4/README.md` & `ecallisto_ng-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,8 +65,7 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.2.4/pyproject.toml` & `ecallisto_ng-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.4"
+version = "0.2.5"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 from skimage import filters
 
 
-def elimwrongchannels(df, channel_std_mult=5, jump_std_mult=2):
+def elimwrongchannels(df, channel_std_mult=5, jump_std_mult=2, nan_interpolation_method='pchip'):
     """
     Remove Radio Frequency Interference (RFI) from a spectrogram represented by a pandas DataFrame.
-    This function currently does not work when there is missing data. So it should be used before the function
-    `fill_missing_timesteps_with_nan`.
+    This function works even when there is missing data thanks to interpolation of missing values.
+    However, it could lead to some false or different results.
     Parameters
     ----------
     df : pandas.DataFrame
         Input DataFrame where the index represents time and the columns represent frequency channels.
     channel_std_mult : float, optional
         Multiplicative factor for the standard deviation threshold used in the first RFI elimination step.
         Channels with standard deviation less than this threshold times the mean standard deviation across all channels are retained.
@@ -24,14 +24,22 @@
     Returns
     -------
     pandas.DataFrame
         DataFrame with RFI removed. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
 
     """
     df = df.copy()
+
+    # Store original NaN positions
+    nan_positions = df.isna()
+
+    # Fill missing data with interpolation
+    df.interpolate(method=nan_interpolation_method, inplace=True)
+    df.fillna(method='bfill', inplace=True)  # for cases where NaNs are at the start of a series
+
     # Transpose df so that rows represent channels and columns represent time
     df = df.T
 
     # Calculate standard deviation for each channel and scale it to 0-255
     std = df.std(axis=1).fillna(0)
     std = ((std - std.min()) * 255) / (std.max() - std.min())
     std = std.clip(upper=255).astype(int)
@@ -57,14 +65,18 @@
         df = df[positions]
     else:
         print("Sorry, all channels are bad ...")
         df = pd.DataFrame()
 
     # Transpose df back to original orientation
     df = df.T
+
+    # Bring back original NaN values
+    df[nan_positions] = np.nan
+
     return df
 
 
 def subtract_constant_background(df, n=30):
     """
     Subtract a constant background from a spectrogram represented by a pandas DataFrame.
```

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,8 +79,7 @@
 df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-Be careful when using `elimwrongchannels` after `fill_missing_timesteps_with_nan`.
```

### Comparing `ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

