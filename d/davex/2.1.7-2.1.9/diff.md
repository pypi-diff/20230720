# Comparing `tmp/davex-2.1.7.tar.gz` & `tmp/davex-2.1.9.tar.gz`

## Comparing `davex-2.1.7.tar` & `davex-2.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 davex-2.1.7/.gitattributes
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/.schemawiz_config2
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/.schemawiz_config3
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/MySQLTableAnalysis.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/PostgresTableAnalysis.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/SimpleAnalysis.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/TableAnalysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/__init__.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/cache_chart_counts.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/help.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_extract.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_extract.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_import.py
--rw-r--r--   0        0        0    16318 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/run.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sp_analyze.sql
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sp_setup.sql
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_extract.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_import.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqliter.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/test.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 davex-2.1.7/tests/.schemawiz_config1
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.7/tests/.schemawiz_config3
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 davex-2.1.7/tests/BasicTest.bat
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 davex-2.1.7/tests/Untitled1.bat
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 davex-2.1.7/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 davex-2.1.7/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 davex-2.1.7/README.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 davex-2.1.7/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 davex-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 davex-2.1.9/.gitattributes
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/.schemawiz_config1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/.schemawiz_config3
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/MySQLTableAnalysis.py
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/PostgresTableAnalysis.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/SimpleAnalysis.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/TableAnalysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/cache_chart_counts.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/help.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/mysql_extract.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/postgres_extract.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/postgres_import.py
+-rw-r--r--   0        0        0    16318 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/run.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sp_analyze.sql
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sp_setup.sql
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sqlite_extract.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sqlite_import.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/sqliter.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 davex-2.1.9/src/davex/test.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 davex-2.1.9/tests/.schemawiz_config1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.9/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 davex-2.1.9/tests/BasicTest.bat
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 davex-2.1.9/tests/Untitled1.bat
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 davex-2.1.9/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 davex-2.1.9/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 davex-2.1.9/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 davex-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 davex-2.1.9/PKG-INFO
```

### Comparing `davex-2.1.7/src/davex/MySQLTableAnalysis.py` & `davex-2.1.9/src/davex/MySQLTableAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/PostgresTableAnalysis.py` & `davex-2.1.9/src/davex/PostgresTableAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 import logging
 import sys
 class runner():
 
 	def __init__(self,cache_prefix='',selected_schema='%',selected_table=''):
 
-		self.cache_schemas_tablename = cache_prefix.lower() +  "schemas"
-		self.cache_tblcounts_tablename = cache_prefix.lower() + "table_counts"
+		self.cache_schemas_tablename = cache_prefix.lower() + "_schemas"
+		self.cache_tblcounts_tablename = cache_prefix.lower() + "_table_counts"
 
 		self.metrics_table_name = cache_prefix.lower() + 'table_metrics'
 		self.metrics_tablehdr_name = cache_prefix.lower() + 'table_comments'
-		self.sqlite = sqlite_db()
-		
-		self.db = postgres_db() 
+
+		self.sqlite = sqlite_db()		
+		self.db = postgres_db(cache_prefix.lower().replace('_','')) 
 
 		self.connect()
 		self.build_metrics_table(self.sqlite)
 		if selected_schema != '':
 			self.sqlite.execute('DELETE FROM ' + self.metrics_table_name + " WHERE schema_name='" + selected_schema + "' and table_name = '" + selected_table + "'")
 		else:
 			self.sqlite.execute('DELETE FROM ' + self.metrics_table_name )
```

### Comparing `davex-2.1.7/src/davex/SimpleAnalysis.py` & `davex-2.1.9/src/davex/SimpleAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/TableAnalysis.py` & `davex-2.1.9/src/davex/TableAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/cache_chart_counts.py` & `davex-2.1.9/src/davex/cache_chart_counts.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/help.py` & `davex-2.1.9/src/davex/help.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/mysql_export.py` & `davex-2.1.9/src/davex/mysql_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/mysql_extract.py` & `davex-2.1.9/src/davex/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/mysql_import.py` & `davex-2.1.9/src/davex/mysql_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/postgres_export.py` & `davex-2.1.9/src/davex/postgres_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/postgres_extract.py` & `davex-2.1.9/src/davex/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/postgres_import.py` & `davex-2.1.9/src/davex/postgres_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/run.py` & `davex-2.1.9/src/davex/run.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sp_analyze.sql` & `davex-2.1.9/src/davex/sp_analyze.sql`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sp_setup.sql` & `davex-2.1.9/src/davex/sp_setup.sql`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sqlite_export.py` & `davex-2.1.9/src/davex/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sqlite_extract.py` & `davex-2.1.9/src/davex/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sqlite_import.py` & `davex-2.1.9/src/davex/sqlite_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/sqliter.py` & `davex-2.1.9/src/davex/sqliter.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/src/davex/test.py` & `davex-2.1.9/src/davex/test.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/LICENSE` & `davex-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `davex-2.1.7/pyproject.toml` & `davex-2.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
-requires = ["hatchling","querychart_package","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package","sqlitedave_package"]
+requires = ["hatchling","readchar","querychart_package","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package","sqlitedave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "davex"
-version = "2.1.7"
+version = "2.1.9"
 dependencies = [
-  'querychart_package >= 2.0.3',
+  'readchar',
+  'querychart_package >= 2.0.4',
   'schemawizard_package >= 2.5.1',
-  'postgresdave_package >= 2.0.3',
+  'postgresdave_package >= 2.0.4',
   'mysqldave_package >= 2.0.3',
   'sqlitedave_package >= 2.0.1',
   'garbledave_package >= 1.0.0 '
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
```

### Comparing `davex-2.1.7/PKG-INFO` & `davex-2.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: davex
-Version: 2.1.7
+Version: 2.1.9
 Summary: Command line Data Profiling for Postgres, MySQL and sqlite.
 Project-URL: Homepage, https://github.com/daveskura/davex
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: garbledave-package>=1.0.0
 Requires-Dist: mysqldave-package>=2.0.3
-Requires-Dist: postgresdave-package>=2.0.3
-Requires-Dist: querychart-package>=2.0.3
+Requires-Dist: postgresdave-package>=2.0.4
+Requires-Dist: querychart-package>=2.0.4
+Requires-Dist: readchar
 Requires-Dist: schemawizard-package>=2.5.1
 Requires-Dist: sqlitedave-package>=2.0.1
 Description-Content-Type: text/markdown
 
 # dbx
```

