# Comparing `tmp/IngeoDash-0.0.25.tar.gz` & `tmp/IngeoDash-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.25.tar", last modified: Thu Jul 20 03:40:50 2023, max compression
+gzip compressed data, was "IngeoDash-0.1.0.tar", last modified: Thu Jul 20 12:27:27 2023, max compression
```

## Comparing `IngeoDash-0.0.25.tar` & `IngeoDash-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:40:50.576442 IngeoDash-0.0.25/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:40:50.572442 IngeoDash-0.0.25/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:40:50.572442 IngeoDash-0.0.25/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:40:50.572442 IngeoDash-0.0.25/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 03:40:50.000000 IngeoDash-0.0.25/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 03:40:50.000000 IngeoDash-0.0.25/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:40:50.000000 IngeoDash-0.0.25/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 03:40:50.000000 IngeoDash-0.0.25/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 03:40:50.000000 IngeoDash-0.0.25/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 03:40:50.576442 IngeoDash-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:40:50.576442 IngeoDash-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 03:38:56.000000 IngeoDash-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/setup.py
```

### Comparing `IngeoDash-0.0.25/IngeoDash/__init__.py` & `IngeoDash-0.1.0/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.25'
+__version__ = '0.1.0'
```

### Comparing `IngeoDash-0.0.25/IngeoDash/__main__.py` & `IngeoDash-0.1.0/IngeoDash/__main__.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/annotate.py` & `IngeoDash-0.1.0/IngeoDash/annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/app.py` & `IngeoDash-0.1.0/IngeoDash/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 
 def table(mem: Config):
     if mem.username in mem:
         data = CONFIG.db[mem[mem.username]][mem.data]
     else:
         data = [{}]
+    data = [{k: f'{v}'for k, v in x.items()} for x in data]
     return dash_table.DataTable(data if len(data) else [{}],
                                 style_data={'whiteSpace': 'normal',
                                             'textAlign': 'left',
                                             'height': 'auto'},
                                 style_header={'fontWeight': 'bold',
                                               'textAlign': 'left'},
                                 id=CONFIG.data)
@@ -125,12 +126,12 @@
     return np.ceil(100 * (tot - ori) / tot)
 
 
 def update_row(mem: Config, table: dict):
     data = flip_label(mem, k=table['row'])
     patch = Patch()
     del patch[table['row']]
-    patch.insert(table['row'], data)
+    patch.insert(table['row'], {k: f'{v}'for k, v in data.items()})
     return patch
```

### Comparing `IngeoDash-0.0.25/IngeoDash/config.py` & `IngeoDash-0.1.0/IngeoDash/config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/download.py` & `IngeoDash-0.1.0/IngeoDash/download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.1.0/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/tests/test_app.py` & `IngeoDash-0.1.0/IngeoDash/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/tests/test_config.py` & `IngeoDash-0.1.0/IngeoDash/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/tests/test_download.py` & `IngeoDash-0.1.0/IngeoDash/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/tests/test_upload.py` & `IngeoDash-0.1.0/IngeoDash/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash/upload.py` & `IngeoDash-0.1.0/IngeoDash/upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.1.0/IngeoDash.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.25
+Version: 0.1.0
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.25/LICENSE` & `IngeoDash-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/PKG-INFO` & `IngeoDash-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.25
+Version: 0.1.0
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.25/README.rst` & `IngeoDash-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.25/setup.py` & `IngeoDash-0.1.0/setup.py`

 * *Files identical despite different names*

