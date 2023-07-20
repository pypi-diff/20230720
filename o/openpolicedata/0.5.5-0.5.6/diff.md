# Comparing `tmp/openpolicedata-0.5.5.tar.gz` & `tmp/openpolicedata-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.5.5.tar", last modified: Wed Jun 21 00:37:17 2023, max compression
+gzip compressed data, was "openpolicedata-0.5.6.tar", last modified: Thu Jul 20 19:53:58 2023, max compression
```

## Comparing `openpolicedata-0.5.5.tar` & `openpolicedata-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.897311 openpolicedata-0.5.5/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.5/LICENSE
--rw-rw-rw-   0        0        0    14967 2023-06-21 00:37:17.897311 openpolicedata-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    13825 2023-06-21 00:05:22.000000 openpolicedata-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.851312 openpolicedata-0.5.5/openpolicedata/
--rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.5/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-21 00:04:59.000000 openpolicedata-0.5.5/openpolicedata/_version.py
--rw-rw-rw-   0        0        0    30791 2023-06-16 21:55:53.000000 openpolicedata-0.5.5/openpolicedata/data.py
--rw-rw-rw-   0        0        0    77576 2023-06-19 21:11:56.000000 openpolicedata-0.5.5/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    11480 2023-06-19 21:25:39.000000 openpolicedata-0.5.5/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0     8688 2023-06-03 12:50:40.000000 openpolicedata-0.5.5/openpolicedata/defs.py
--rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.5/openpolicedata/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.887314 openpolicedata-0.5.5/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0    14967 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0     1377 2023-06-21 00:37:17.898312 openpolicedata-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.896312 openpolicedata-0.5.5/tests/
--rw-rw-rw-   0        0        0    21379 2023-05-17 22:48:02.000000 openpolicedata-0.5.5/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0     9438 2023-06-20 11:16:04.000000 openpolicedata-0.5.5/tests/test_datasets.py
--rw-rw-rw-   0        0        0    11536 2023-06-21 00:35:42.000000 openpolicedata-0.5.5/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     7998 2023-06-16 21:56:15.000000 openpolicedata-0.5.5/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    11429 2023-06-15 23:29:48.000000 openpolicedata-0.5.5/tests/test_opd_data3.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:53:58.631318 openpolicedata-0.5.6/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0    15360 2023-07-20 19:53:58.632320 openpolicedata-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    14218 2023-07-20 01:47:08.000000 openpolicedata-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:53:58.611347 openpolicedata-0.5.6/openpolicedata/
+-rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.6/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-19 00:47:32.000000 openpolicedata-0.5.6/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0    30791 2023-07-18 22:52:28.000000 openpolicedata-0.5.6/openpolicedata/data.py
+-rw-rw-rw-   0        0        0    78085 2023-07-19 00:10:49.000000 openpolicedata-0.5.6/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    11499 2023-07-19 23:44:21.000000 openpolicedata-0.5.6/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0     8688 2023-07-18 22:52:28.000000 openpolicedata-0.5.6/openpolicedata/defs.py
+-rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.6/openpolicedata/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:53:58.624305 openpolicedata-0.5.6/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0    15360 2023-07-20 19:53:58.000000 openpolicedata-0.5.6/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-07-20 19:53:58.000000 openpolicedata-0.5.6/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:53:58.000000 openpolicedata-0.5.6/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-07-20 19:53:58.000000 openpolicedata-0.5.6/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-20 19:53:58.000000 openpolicedata-0.5.6/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2023-06-26 23:09:08.000000 openpolicedata-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1377 2023-07-20 19:53:58.633319 openpolicedata-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:53:58.630313 openpolicedata-0.5.6/tests/
+-rw-rw-rw-   0        0        0    21379 2023-06-26 23:09:08.000000 openpolicedata-0.5.6/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9438 2023-06-26 23:09:22.000000 openpolicedata-0.5.6/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    11173 2023-07-20 19:49:31.000000 openpolicedata-0.5.6/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     7998 2023-07-19 00:07:38.000000 openpolicedata-0.5.6/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    11429 2023-07-18 22:52:28.000000 openpolicedata-0.5.6/tests/test_opd_data3.py
```

### Comparing `openpolicedata-0.5.5/LICENSE` & `openpolicedata-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/PKG-INFO` & `openpolicedata-0.5.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -20,15 +20,15 @@
 Provides-Extra: optional
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets for over 4000 police agencies around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -47,15 +47,17 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-**[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
+**Not ready to code or only looking for a single dataset? Checkout our [OPD Explorer Streamlit App](https://openpolicedata.streamlit.app/)!**
+
+**You can try out OpenPoliceData and run examples online on [Binder](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD).**
 
 Basic usage of OpenPoliceData simply involves:
 1. Finding datasets
 2. Loading datasets
 
 The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
 ```
@@ -126,16 +128,19 @@
 | California | California     | MULTI            | STOPS         | 2019     |
 | California | California     | MULTI            | STOPS         | 2020     |
 
 (only 1st 5 columns shown above)
 
 datasets is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). The first 5 datasets available from California include traffic stops data from multiples years from Anaheim and Bakersfield and data from every agency in California for all types of police stops for years 2018, 2019, and 2020.
 
-### opd.datasets.num_unique()
-Returns the number of unique datasets in OpenPoliceData. This counts the number of datasets from distinct sources AND table types (stops, use of force, etc.).
+### opd.datasets.summary_by_table_type(by_year=False)
+Returns a pandas DataFrame with the number of datasets available for each type of table (stops, use of force, etc.). Setting `by_year` to True also returns a breakdown of table types by year.
+
+### opd.datasets.get_table_types(contains=None)
+Returns types of tables available in OpenPoliceData. If `contains` is not None, only table types containing `contains` are returned.
 
 ### opd.datasets.num_sources(full_states_only=False)
 Returns the number of sources (police departments and states) that provide the data available in OpenPoliceData. Setting `full_states_only` to True returns only the number of states that share data for all agencies in the state.
 
 ### opd.datasets.summary_by_state(by=None)
 Returns a pandas DataFrame with the number of datasets available for each state. The optional input `by` can be used to further breakdown by "year" or "table".
```

### Comparing `openpolicedata-0.5.5/README.md` & `openpolicedata-0.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets for over 4000 police agencies around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -25,15 +25,17 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-**[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
+**Not ready to code or only looking for a single dataset? Checkout our [OPD Explorer Streamlit App](https://openpolicedata.streamlit.app/)!**
+
+**You can try out OpenPoliceData and run examples online on [Binder](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD).**
 
 Basic usage of OpenPoliceData simply involves:
 1. Finding datasets
 2. Loading datasets
 
 The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
 ```
@@ -104,16 +106,19 @@
 | California | California     | MULTI            | STOPS         | 2019     |
 | California | California     | MULTI            | STOPS         | 2020     |
 
 (only 1st 5 columns shown above)
 
 datasets is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). The first 5 datasets available from California include traffic stops data from multiples years from Anaheim and Bakersfield and data from every agency in California for all types of police stops for years 2018, 2019, and 2020.
 
-### opd.datasets.num_unique()
-Returns the number of unique datasets in OpenPoliceData. This counts the number of datasets from distinct sources AND table types (stops, use of force, etc.).
+### opd.datasets.summary_by_table_type(by_year=False)
+Returns a pandas DataFrame with the number of datasets available for each type of table (stops, use of force, etc.). Setting `by_year` to True also returns a breakdown of table types by year.
+
+### opd.datasets.get_table_types(contains=None)
+Returns types of tables available in OpenPoliceData. If `contains` is not None, only table types containing `contains` are returned.
 
 ### opd.datasets.num_sources(full_states_only=False)
 Returns the number of sources (police departments and states) that provide the data available in OpenPoliceData. Setting `full_states_only` to True returns only the number of states that share data for all agencies in the state.
 
 ### opd.datasets.summary_by_state(by=None)
 Returns a pandas DataFrame with the number of datasets available for each state. The optional input `by` can be used to further breakdown by "year" or "table".
```

### Comparing `openpolicedata-0.5.5/openpolicedata/__init__.py` & `openpolicedata-0.5.6/openpolicedata/__init__.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/openpolicedata/data.py` & `openpolicedata-0.5.6/openpolicedata/data.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/openpolicedata/data_loaders.py` & `openpolicedata-0.5.6/openpolicedata/data_loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,16 +360,19 @@
             raise ValueError("Extracting the years of a CSV file requires reading the whole file in. In most cases, "+
                 "running load() with no arguments to load in the whole CSV file and manually finding the years will be more "
                 "efficient. If running get_years is still desired, set force=True")
         else:
             if self.date_field==None:
                 raise ValueError("No date field provided to access year information")
             df = self.load()
-            date_col = pd.to_datetime(df[self.date_field])
-            years = list(date_col.dt.year.dropna().unique())
+            if self.date_field.lower()=="year":
+                years = df[self.date_field].unique()
+            else:
+                date_col = pd.to_datetime(df[self.date_field])
+                years = list(date_col.dt.year.dropna().unique())
             years.sort()
             return [int(x) for x in years]
 
 
 class Excel(Data_Loader):
     """
     A class for accessing data from Excel download URLs
@@ -973,14 +976,17 @@
         
         where_query = ""
         zero_found = False
         if self._date_format in [0,1] or self._date_format==None:
             start_date, stop_date = _process_date(year)
             
             for k in range(0,2):
+                if self._date_format is not None and self._date_format!=k:
+                    continue
+
                 if k==0:
                     where_query = f"{self.date_field} >= '{start_date}' AND  {self.date_field} < '{stop_date}'"
                 else:
                     # break
                     # Dataset (San Jose crash data) that required this does not function well so removing its functionality for now to speed up this function.
                     # This is the recommended way but it has been found to not work sometimes. One dataset was found that requires this.
                     # https://gis.stackexchange.com/questions/451107/arcgis-rest-api-unable-to-complete-operation-on-esrifieldtypedate-in-query
@@ -1019,15 +1025,16 @@
                     raise
 
 
         where_formats = [
             "{} LIKE '%[0-9][0-9]/[0-9][0-9]/{}%'",   # mm/dd/yyyy
             double_format("{} LIKE '{}/[0-9][0-9]' OR {} LIKE '{}/[0-9]'"),                # yyyy/mm
             "{} = {}",                # yyyy
-            double_format("{} LIKE '[0-9][0-9]-{}' OR {} LIKE '[0-9]-{}'")   # mm-yyyy or m-yyyy
+            double_format("{} LIKE '[0-9][0-9]-{}' OR {} LIKE '[0-9]-{}'"),   # mm-yyyy or m-yyyy
+            "{} = '{}'",                # 'yyyy'
         ]
         # Make year iterable
         year = [year] if isinstance(year, numbers.Number) else year
 
         if self._date_format not in [None, 0, 1] and any([isinstance(x,str) and len(x)!=4 for x in year]):
             # Currently can only handle years
             raise ValueError("Currently unable to handle non-year inputs")
@@ -1775,18 +1782,23 @@
             # To retain the old behavior, use either `df[df.columns[i]] = newvals` or, if columns are non-unique, `df.isetitem(i, newvals)`
             warnings.simplefilter("ignore", category=FutureWarning)
             if date_field.lower()!="year":
                 df[date_field] = pd.to_datetime(df[date_field])
     
     if year_filter != None and date_field != None:
         if isinstance(year_filter, list):
-            df = df[(df[date_field].dt.year >= year_filter[0]) & (df[date_field].dt.year <= year_filter[1])]
-        else:
+            if date_field.lower()!="year":
+                df = df[(df[date_field].dt.year >= year_filter[0]) & (df[date_field].dt.year <= year_filter[1])]
+            else:
+                df = df[df[date_field].isin(year_filter)]
+        elif date_field.lower()!="year":
             date_col = pd.to_datetime(df[date_field])
             df = df[date_col.dt.year == year_filter]
+        else:
+            df = df[df[date_field] == year_filter]
 
     if agency != None and agency_field != None:
         df = df.query(agency_field + " = '" + agency + "'")
 
     return df
```

### Comparing `openpolicedata-0.5.5/openpolicedata/datasets.py` & `openpolicedata-0.5.6/openpolicedata/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # Ensure that all states are correctly spelled
     not_state = df["State"].apply(lambda x: x not in defs.states)
     if not_state.any():
         misspelled = df["State"][not_state]
         raise ValueError(f"{len(misspelled)} states are misspelled in the data sources table including {misspelled.iloc[0]} at index {misspelled.index[0]}")
 
     key_vals = ['State', 'SourceName', 'Agency', 'TableType','Year']
-    df.drop_duplicates(subset=key_vals, inplace=True)
+    df.drop_duplicates(subset=key_vals, inplace=True, ignore_index=True)
 
     if "coverage_start" in df:
         p = re.compile(r"\d{1,2}/\d{1,2}/\d{4}")
         df["coverage_start"] = df["coverage_start"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
         df["coverage_end"] = df["coverage_end"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
 
     return df
```

### Comparing `openpolicedata-0.5.5/openpolicedata/defs.py` & `openpolicedata-0.5.6/openpolicedata/defs.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/openpolicedata/exceptions.py` & `openpolicedata-0.5.6/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.5.6/openpolicedata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -20,15 +20,15 @@
 Provides-Extra: optional
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets for over 4000 police agencies around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -47,15 +47,17 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-**[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
+**Not ready to code or only looking for a single dataset? Checkout our [OPD Explorer Streamlit App](https://openpolicedata.streamlit.app/)!**
+
+**You can try out OpenPoliceData and run examples online on [Binder](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD).**
 
 Basic usage of OpenPoliceData simply involves:
 1. Finding datasets
 2. Loading datasets
 
 The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
 ```
@@ -126,16 +128,19 @@
 | California | California     | MULTI            | STOPS         | 2019     |
 | California | California     | MULTI            | STOPS         | 2020     |
 
 (only 1st 5 columns shown above)
 
 datasets is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). The first 5 datasets available from California include traffic stops data from multiples years from Anaheim and Bakersfield and data from every agency in California for all types of police stops for years 2018, 2019, and 2020.
 
-### opd.datasets.num_unique()
-Returns the number of unique datasets in OpenPoliceData. This counts the number of datasets from distinct sources AND table types (stops, use of force, etc.).
+### opd.datasets.summary_by_table_type(by_year=False)
+Returns a pandas DataFrame with the number of datasets available for each type of table (stops, use of force, etc.). Setting `by_year` to True also returns a breakdown of table types by year.
+
+### opd.datasets.get_table_types(contains=None)
+Returns types of tables available in OpenPoliceData. If `contains` is not None, only table types containing `contains` are returned.
 
 ### opd.datasets.num_sources(full_states_only=False)
 Returns the number of sources (police departments and states) that provide the data available in OpenPoliceData. Setting `full_states_only` to True returns only the number of states that share data for all agencies in the state.
 
 ### opd.datasets.summary_by_state(by=None)
 Returns a pandas DataFrame with the number of datasets available for each state. The optional input `by` can be used to further breakdown by "year" or "table".
```

### Comparing `openpolicedata-0.5.5/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.5.6/openpolicedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/setup.cfg` & `openpolicedata-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/tests/test_data_loaders.py` & `openpolicedata-0.5.6/tests/test_data_loaders.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/tests/test_datasets.py` & `openpolicedata-0.5.6/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/tests/test_opd_data1.py` & `openpolicedata-0.5.6/tests/test_opd_data1.py`

 * *Files 7% similar despite different names*

```diff
@@ -286,29 +286,20 @@
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
 	csvfile = r"..\opd-data\opd_source_table.csv"
 	last = None
-	# last = 875-1+1
+	last = 873-290+1
 	skip = None
-	skip = "Beloit"
+	skip = "Bloomington"
 	source = None
 	# source = "Mesa"
-	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
-	# tp.test_check_version(csvfile, None, last, skip, None) #
+	tp.check_table_type_warning(csvfile, source, last, skip, None) 
+	tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	tp.test_check_version(csvfile, None, last, skip, None) #
 	tp.test_source_download_limitable(csvfile, source, last, skip, None) 
 	
-	# tp.test_get_count(csvfile, None, last, skip, None)
-	# tp.test_load_gen(csvfile, source, last, skip, None) 
-
-	last = None
-	import test_opd_data2
-	tp = test_opd_data2.TestData()
-	tp.test_get_years(csvfile, source, last, skip, None)
-	tp.test_get_agencies(csvfile, None, None, skip, None)
-	tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
-	tp.test_agency_filter(csvfile, None, None, skip, None)
-	tp.test_to_csv(csvfile, None, None, skip, None)
+	tp.test_get_count(csvfile, None, last, skip, None)
+	tp.test_load_gen(csvfile, source, last, skip, None)
```

### Comparing `openpolicedata-0.5.5/tests/test_opd_data2.py` & `openpolicedata-0.5.6/tests/test_opd_data2.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.5/tests/test_opd_data3.py` & `openpolicedata-0.5.6/tests/test_opd_data3.py`

 * *Files identical despite different names*

