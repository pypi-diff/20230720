# Comparing `tmp/robotframework-databaselibrary-1.3.0.tar.gz` & `tmp/robotframework-databaselibrary-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-databaselibrary-1.3.0.tar", last modified: Mon Jul 17 17:25:52 2023, max compression
+gzip compressed data, was "robotframework-databaselibrary-1.3.1.tar", last modified: Thu Jul 20 19:36:12 2023, max compression
```

## Comparing `robotframework-databaselibrary-1.3.0.tar` & `robotframework-databaselibrary-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.982480 robotframework-databaselibrary-1.3.0/
--rw-r--r--   0 andremochinin   (501) staff       (20)      570 2023-07-11 18:41:08.000000 robotframework-databaselibrary-1.3.0/LICENSE
--rw-r--r--   0 andremochinin   (501) staff       (20)     4195 2023-07-17 17:25:52.982344 robotframework-databaselibrary-1.3.0/PKG-INFO
--rw-r--r--   0 andremochinin   (501) staff       (20)     2900 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/README.md
--rw-r--r--   0 andremochinin   (501) staff       (20)      913 2023-07-17 17:25:42.000000 robotframework-databaselibrary-1.3.0/pyproject.toml
--rw-r--r--   0 andremochinin   (501) staff       (20)       38 2023-07-17 17:25:52.982522 robotframework-databaselibrary-1.3.0/setup.cfg
-drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.979577 robotframework-databaselibrary-1.3.0/src/
-drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.981253 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/
--rw-r--r--   0 andremochinin   (501) staff       (20)     2955 2023-07-17 17:15:49.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/__init__.py
--rw-r--r--   0 andremochinin   (501) staff       (20)    14306 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/assertion.py
--rw-r--r--   0 andremochinin   (501) staff       (20)    13763 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/connection_manager.py
--rw-r--r--   0 andremochinin   (501) staff       (20)    22829 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/query.py
--rw-r--r--   0 andremochinin   (501) staff       (20)       18 2023-07-17 17:14:02.000000 robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/version.py
-drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-17 17:25:52.982133 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/
--rw-r--r--   0 andremochinin   (501) staff       (20)     4195 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/PKG-INFO
--rw-r--r--   0 andremochinin   (501) staff       (20)      488 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/SOURCES.txt
--rw-r--r--   0 andremochinin   (501) staff       (20)        1 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/dependency_links.txt
--rw-r--r--   0 andremochinin   (501) staff       (20)       39 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/requires.txt
--rw-r--r--   0 andremochinin   (501) staff       (20)       16 2023-07-17 17:25:52.000000 robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/top_level.txt
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-20 19:36:12.110339 robotframework-databaselibrary-1.3.1/
+-rw-r--r--   0 andremochinin   (501) staff       (20)      570 2023-07-11 18:41:08.000000 robotframework-databaselibrary-1.3.1/LICENSE
+-rw-r--r--   0 andremochinin   (501) staff       (20)     3531 2023-07-20 19:36:12.110210 robotframework-databaselibrary-1.3.1/PKG-INFO
+-rw-r--r--   0 andremochinin   (501) staff       (20)     2900 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.1/README.md
+-rw-r--r--   0 andremochinin   (501) staff       (20)      893 2023-07-18 19:26:15.000000 robotframework-databaselibrary-1.3.1/pyproject.toml
+-rw-r--r--   0 andremochinin   (501) staff       (20)       38 2023-07-20 19:36:12.110386 robotframework-databaselibrary-1.3.1/setup.cfg
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-20 19:36:12.108092 robotframework-databaselibrary-1.3.1/src/
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-20 19:36:12.109201 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/
+-rw-r--r--   0 andremochinin   (501) staff       (20)     2955 2023-07-17 17:15:49.000000 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/__init__.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    14306 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/assertion.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    13895 2023-07-20 19:27:57.000000 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/connection_manager.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)    22829 2023-07-17 14:48:37.000000 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/query.py
+-rw-r--r--   0 andremochinin   (501) staff       (20)       18 2023-07-18 19:18:02.000000 robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/version.py
+drwxr-xr-x   0 andremochinin   (501) staff       (20)        0 2023-07-20 19:36:12.109992 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/
+-rw-r--r--   0 andremochinin   (501) staff       (20)     3531 2023-07-20 19:36:12.000000 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/PKG-INFO
+-rw-r--r--   0 andremochinin   (501) staff       (20)      488 2023-07-20 19:36:12.000000 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)        1 2023-07-20 19:36:12.000000 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)       39 2023-07-20 19:36:12.000000 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/requires.txt
+-rw-r--r--   0 andremochinin   (501) staff       (20)       16 2023-07-20 19:36:12.000000 robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/top_level.txt
```

### Comparing `robotframework-databaselibrary-1.3.0/LICENSE` & `robotframework-databaselibrary-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-databaselibrary-1.3.0/PKG-INFO` & `robotframework-databaselibrary-1.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-databaselibrary
-Version: 1.3.0
+Version: 1.3.1
 Summary: Database Library for Robot Framework
 Author-email: Franz Allan Valencia See <franz.see@gmail.com>
-License: Copyright (c) 2010 Franz Allan Valencia See
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        
-            http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
+License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MarketSquare/Robotframework-Database-Library
 Project-URL: Keyword docs, http://marketsquare.github.io/Robotframework-Database-Library/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `robotframework-databaselibrary-1.3.0/README.md` & `robotframework-databaselibrary-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-databaselibrary-1.3.0/pyproject.toml` & `robotframework-databaselibrary-1.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [build-system]
 requires = [
     "setuptools>=61.0",
-    "robotframework",
-    "robotframework-excellib"
+    "robotframework"
     ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robotframework-databaselibrary"
 authors = [{name="Franz Allan Valencia See", email="franz.see@gmail.com"},
 ]
@@ -18,15 +17,15 @@
     "robotframework-excellib"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
-license = {file = "LICENSE"}
+license = {text = "Apache License 2.0"}
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/MarketSquare/Robotframework-Database-Library"
 "Keyword docs" = "http://marketsquare.github.io/Robotframework-Database-Library/"
 
 [tool.setuptools.dynamic]
```

### Comparing `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/__init__.py` & `robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/assertion.py` & `robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/assertion.py`

 * *Files identical despite different names*

### Comparing `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/connection_manager.py` & `robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/connection_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,23 @@
             self._dbconnection = db_api_2.connect(db=dbName, user=dbUsername, passwd=dbPassword, host=dbHost, port=dbPort, charset='utf8mb4' or dbCharset)
         elif dbapiModuleName in ["psycopg2"]:
             dbPort = dbPort or 5432
             logger.info('Connecting using : %s.connect(database=%s, user=%s, password=***, host=%s, port=%s) ' % (dbapiModuleName, dbName, dbUsername, dbHost, dbPort))
             self._dbconnection = db_api_2.connect(database=dbName, user=dbUsername, password=dbPassword, host=dbHost, port=dbPort)
         elif dbapiModuleName in ["pyodbc", "pypyodbc"]:
             dbPort = dbPort or 1433
+            dbCharset = dbCharset or 'utf8mb4'
             dbDriver = dbDriver or "{SQL Server}"
-            logger.info('Connecting using : %s.connect(DRIVER=%s;SERVER=%s:%s;DATABASE=%s;UID=%s;PWD=***)' % (dbapiModuleName, dbDriver,  dbHost, dbPort, dbName, dbUsername))
-            self._dbconnection = db_api_2.connect('DRIVER=%s;SERVER=%s:%s;DATABASE=%s;UID=%s;PWD=%s;charset=%s' % (dbDriver, dbHost, dbPort, dbName, dbUsername, dbPassword, 'utf8mb4' or dbCharset))
+            con_str = f"DRIVER={dbDriver};DATABASE={dbName};UID={dbUsername};PWD={dbPassword};charset={dbCharset};"
+            if "mysql" in dbDriver.lower():
+                con_str += f"SERVER={dbHost}:{dbPort}"
+            else:
+                con_str += f"SERVER={dbHost},{dbPort}"
+            logger.info(f'Connecting using : {dbapiModuleName}.connect({con_str.replace(dbPassword, "***")})')
+            self._dbconnection = db_api_2.connect(con_str)
         elif dbapiModuleName in ["excel"]:
             logger.info(
                 'Connecting using : %s.connect(DRIVER={Microsoft Excel Driver (*.xls, *.xlsx, *.xlsm, *.xlsb)};DBQ=%s;ReadOnly=1;Extended Properties="Excel 8.0;HDR=YES";)' % (
                 dbapiModuleName, dbName))
             self._dbconnection = db_api_2.connect(
                 'DRIVER={Microsoft Excel Driver (*.xls, *.xlsx, *.xlsm, *.xlsb)};DBQ=%s;ReadOnly=1;Extended Properties="Excel 8.0;HDR=YES";)' % (
                     dbName), autocommit=True)
```

### Comparing `robotframework-databaselibrary-1.3.0/src/DatabaseLibrary/query.py` & `robotframework-databaselibrary-1.3.1/src/DatabaseLibrary/query.py`

 * *Files identical despite different names*

### Comparing `robotframework-databaselibrary-1.3.0/src/robotframework_databaselibrary.egg-info/PKG-INFO` & `robotframework-databaselibrary-1.3.1/src/robotframework_databaselibrary.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-databaselibrary
-Version: 1.3.0
+Version: 1.3.1
 Summary: Database Library for Robot Framework
 Author-email: Franz Allan Valencia See <franz.see@gmail.com>
-License: Copyright (c) 2010 Franz Allan Valencia See
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        
-            http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
+License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MarketSquare/Robotframework-Database-Library
 Project-URL: Keyword docs, http://marketsquare.github.io/Robotframework-Database-Library/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

