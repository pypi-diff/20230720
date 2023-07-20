# Comparing `tmp/ecallisto_ng-0.2.3.tar.gz` & `tmp/ecallisto_ng-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.3.tar", last modified: Tue Jul 18 20:20:10 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.4.tar", last modified: Wed Jul 19 09:57:36 2023, max compression
```

## Comparing `ecallisto_ng-0.2.3.tar` & `ecallisto_ng-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.3/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.3/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 20:19:56.000000 ecallisto_ng-0.2.3/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.101095 ecallisto_ng-0.2.3/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7760 2023-07-18 20:19:47.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2844 2023-07-18 19:00:07.000000 ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 20:20:10.111928 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 20:20:10.000000 ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.4/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.4/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-19 09:20:12.000000 ecallisto_ng-0.2.4/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8924 2023-07-19 09:20:02.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.640160 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2954 2023-07-19 09:56:22.000000 ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 09:57:36.629327 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-19 09:57:36.000000 ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.3/LICENSE` & `ecallisto_ng-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.3/PKG-INFO` & `ecallisto_ng-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.3/README.md` & `ecallisto_ng-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.3/pyproject.toml` & `ecallisto_ng-0.2.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 def get_data(
     instrument_name,
     start_datetime,
     end_datetime,
     timebucket=None,
     agg_function=None,
     data_folder='ecallisto_ng_cache',
-    verbose=False
+    verbose=False,
+    max_retries=3,
 ):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
     Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
     weeks of data, aggregated in a specific way, can take around 20 seconds.
 
@@ -35,14 +36,16 @@
         "timebucket" function)
     agg_function : str
         The aggregation function to use (see timescaledb "timebucket" function)
     data_folder : str
         Where to save the cached data.
     verbose : bool
         Whether to print the progress or not.
+    max_retries : int
+        The maximum number of retries to download the data.
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the data from the eCallisto API.
     """
     data = {
         "instrument_name": instrument_name,
@@ -76,48 +79,65 @@
             print("Data retrieval started successfully. Waiting for file to be ready...")
         # Get the URL for the parquet file
         parquet_url = response.json()["data_parquet_url"]
         json_url = response.json()["info_json_url"]
         file_id = response.json()["file_id"]
 
         # Now we can start polling the URL until the parquet file is ready for download
+        n_tries = 0
         while True:
-            if verbose:
-                print(f"Trying to download file {file_id}")
-            # Try to download the parquet file
-            file_response = requests.get(BASE_URL + parquet_url)
-            # If the file is available, save it to disk
-            if file_response.status_code == 200:
-                print("File downloaded successfully")
-                with open(file_path, "wb") as f:
-                    f.write(file_response.content)
-                return pd.read_parquet(file_path)
-            elif file_response.status_code == 204:
-                # Check if the file creation causes any errors
-                # This json contains information about the request
-                json_response = requests.get(BASE_URL + json_url)
-                # Check the status of the json 
-                if 'status' in json_response.json():
-                    if json_response.json()['status'] == 'processing':
-                        # If the file is not found, sleep for a short period and try again
-                        if verbose:
-                            print(f"File {file_id} not ready yet, waiting...")
-                        time.sleep(5)
-                    elif json_response.json()['status'] == 'ok':
-                        if verbose:
-                            print(f'File {file_id} succesfully written! Will return file')
+            try:
+                if verbose:
+                    print(f"Trying to download file {file_id}")
+                # Try to download the parquet file
+                file_response = requests.get(BASE_URL + parquet_url)
+                # If the file is available, save it to disk
+                if file_response.status_code == 200:
+                    print("File downloaded successfully")
+                    with open(file_path, "wb") as f:
+                        f.write(file_response.content)
+                    # Check that the file is bigger than 8 bytes (sometimes, the API returns an empty file)
+                    if os.path.getsize(file_path) > 8:
+                        # Return the file as a DataFrame  
+                        return pd.read_parquet(file_path)
                     else:
-                        raise ValueError(f"Error downloading file: {json_response.json()['status']}")
-                elif 'error' in json_response.json():
-                    raise ValueError(f"Error downloading file: {json_response.json()['error']}")
-            else:
-                print(f"Error downloading file: {file_response.status_code}")
-                json_response = requests.get(BASE_URL + json_url)
-                print(json_response.json())
-                break
+                        # Remove file and try again
+                        os.remove(file_path)
+                        raise ValueError(f"Error downloading file: {file_response.status_code}. File is empty.")
+                elif file_response.status_code == 204:
+                    # Check if the file creation causes any errors
+                    json_response = requests.get(BASE_URL + json_url) # This json contains information about your data request (e.g. status)
+                    # Check the status of the json 
+                    if 'status' in json_response.json():
+                        if json_response.json()['status'] == 'processing':
+                            # If the file is not found, sleep for a short period and try again
+                            if verbose:
+                                print(f"File {file_id} not ready yet, waiting...")
+                            time.sleep(3)
+                        elif json_response.json()['status'] == 'ok':
+                            if verbose:
+                                print(f'File {file_id} succesfully written! Will return file.')
+                        else:
+                            raise ValueError(f"Error downloading file: {json_response.json()['status']}")
+                    elif 'error' in json_response.json():
+                        raise ValueError(f"Error downloading file: {json_response.json()['error']}")
+                else:
+                    print(f"Error downloading file: {file_response.status_code}")
+                    json_response = requests.get(BASE_URL + json_url)
+                    print(json_response.json())
+                    break
+            except Exception as e:
+                print(
+                    f"""Error downloading file: {e}. Try {n_tries} of {max_retries}. Retrying in 3 seconds...
+                    """
+                    )
+                n_tries += 1
+                if n_tries > max_retries:
+                    raise ValueError(f"Error downloading file: {file_response.status_code}. Max retries reached.")
+                time.sleep(3)
     else:
         print(f"Error starting data retrieval: {response.status_code}")
 
 
 # Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
 # This function converts the instrument name to the table name.
 def extract_instrument_name(file_path):
```

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.4/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.4/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.4/src/ecallisto_ng/plotting/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18, round_precision=1, color_scale=px.colors.sequential.Plasma):
     # Create a new dataframe with rounded column names
     df_rounded = df.copy()
     df_rounded.columns = [f"{float(col):.{round_precision}f}" for col in df.columns]
 
     # Make datetime prettier
+    if isinstance(start_datetime, str):
+        start_datetime = pd.to_datetime(start_datetime)
+    if isinstance(end_datetime, str):
+        end_datetime = pd.to_datetime(end_datetime)
     sd_str = start_datetime.strftime("%Y-%m-%d %H:%M:%S")
     ed_str = end_datetime.strftime("%Y-%m-%d %H:%M:%S")
 
-    # Trick to make NANs appear black
-    # Replace NaNs with -1
-    df_rounded.fillna(-1, inplace=True)
-    # Add black for NANS
-    color_scale.insert(0, "black")
-
     fig = px.imshow(df_rounded.T, color_continuous_scale=color_scale, zmin=df.min().min(), zmax=df.max().max())
     fig.update_layout(
         title=f"Spectogram of {instrument_name} between {sd_str} and {ed_str}",
         xaxis_title="Datetime",
         yaxis_title="Frequency",
         font=dict(family="Courier New, monospace", size=size, color="#7f7f7f"),
+        plot_bgcolor="black",
+        xaxis_showgrid=False,
+        yaxis_showgrid=False,
     )
     return fig
 
 def fill_missing_timesteps_with_nan(df):
     """
     Fill missing timesteps in a pandas DataFrame with NaN values. Only needed for plotting.
```

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.3/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.4/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

