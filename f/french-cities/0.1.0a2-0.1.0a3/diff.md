# Comparing `tmp/french_cities-0.1.0a2.tar.gz` & `tmp/french_cities-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a2.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a3.tar", max compression
```

## Comparing `french_cities-0.1.0a2.tar` & `french_cities-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1003 2023-07-20 12:05:49.356617 french_cities-0.1.0a2/french_cities/__init__.py
--rw-r--r--   0        0        0    16645 2023-07-20 11:00:48.287264 french_cities-0.1.0a2/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a2/french_cities/departement_finder.py
--rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a2/french_cities/utils.py
--rw-r--r--   0        0        0     7719 2023-07-17 15:18:15.371670 french_cities-0.1.0a2/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-20 11:44:07.438358 french_cities-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a2/README.fr.md
--rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a2/README.md
--rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-07-20 12:31:33.351032 french_cities-0.1.0a3/french_cities/__init__.py
+-rw-r--r--   0        0        0    16645 2023-07-20 11:00:48.287264 french_cities-0.1.0a3/french_cities/city_finder.py
+-rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a3/french_cities/departement_finder.py
+-rw-r--r--   0        0        0     8996 2023-07-20 08:57:54.526764 french_cities-0.1.0a3/french_cities/test.xlsx
+-rw-r--r--   0        0        0    18534 2023-07-20 12:06:04.703855 french_cities-0.1.0a3/french_cities/test_sample.xlsx
+-rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a3/french_cities/utils.py
+-rw-r--r--   0        0        0     7719 2023-07-17 15:18:15.371670 french_cities-0.1.0a3/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-20 12:31:36.220513 french_cities-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a3/README.fr.md
+-rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a3/README.md
+-rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a3/PKG-INFO
```

### Comparing `french_cities-0.1.0a2/french_cities/__init__.py` & `french_cities-0.1.0a3/french_cities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from french_cities.city_finder import find_city
 from french_cities.departement_finder import find_departements
 from french_cities.vintage import set_vintage
 
 load_dotenv()
 
-__version__ = "0.1.0a1"
+__version__ = "0.1.0a3"
 
 
 __all__ = [
     "find_city",
     "find_departements",
     "set_vintage",
 ]
```

### Comparing `french_cities-0.1.0a2/french_cities/city_finder.py` & `french_cities-0.1.0a3/french_cities/city_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a2/french_cities/departement_finder.py` & `french_cities-0.1.0a3/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a2/french_cities/vintage.py` & `french_cities-0.1.0a3/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a2/pyproject.toml` & `french_cities-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.0a2/README.fr.md` & `french_cities-0.1.0a3/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a2/README.md` & `french_cities-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a2/PKG-INFO` & `french_cities-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
```

