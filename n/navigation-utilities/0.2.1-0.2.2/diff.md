# Comparing `tmp/navigation-utilities-0.2.1.tar.gz` & `tmp/navigation-utilities-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigation-utilities-0.2.1.tar", last modified: Wed May  3 17:00:28 2023, max compression
+gzip compressed data, was "navigation-utilities-0.2.2.tar", last modified: Thu Jul 20 10:46:34 2023, max compression
```

## Comparing `navigation-utilities-0.2.1.tar` & `navigation-utilities-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1073 2023-05-03 16:59:00.000000 navigation-utilities-0.2.1/LICENSE
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)      522 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/README.md
--rw-r--r--   0 pablo     (1000) pablo     (1000)      715 2023-05-03 16:59:24.000000 navigation-utilities-0.2.1/pyproject.toml
--rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/setup.cfg
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities/
--rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/__init__.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1455 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/coordinate.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     4187 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/gngga.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1936 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/nmea.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     2749 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/oxts.py
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities/utils/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     2515 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/utils/time.py
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)      486 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       14 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/requires.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       21 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1073 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1099 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      492 2023-05-14 17:47:33.000000 navigation-utilities-0.2.2/README.md
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      714 2023-07-20 10:46:02.000000 navigation-utilities-0.2.2/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/setup.cfg
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/src/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/src/navigation_utilities/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/src/navigation_utilities/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1455 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/src/navigation_utilities/coordinate.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4187 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/src/navigation_utilities/gngga.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1936 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/src/navigation_utilities/nmea.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2749 2023-05-04 18:23:35.000000 navigation-utilities-0.2.2/src/navigation_utilities/oxts.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/src/navigation_utilities/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:24:11.000000 navigation-utilities-0.2.2/src/navigation_utilities/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2567 2023-05-04 18:46:52.000000 navigation-utilities-0.2.2/src/navigation_utilities/utils/time.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-07-20 10:46:34.362678 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1099 2023-07-20 10:46:34.000000 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      529 2023-07-20 10:46:34.000000 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-07-20 10:46:34.000000 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       14 2023-07-20 10:46:34.000000 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       21 2023-07-20 10:46:34.000000 navigation-utilities-0.2.2/src/navigation_utilities.egg-info/top_level.txt
```

### Comparing `navigation-utilities-0.2.1/LICENSE` & `navigation-utilities-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.1/PKG-INFO` & `navigation-utilities-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: navigation-utilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: Collection of utilities for driverless navigation systems and gnss tools
 Author-email: Pablo Dorrio Vazquez <pablo.dorrio.vazquez@gmail.com>
 Project-URL: Homepage, https://github.com/pablodorrio/navigation-utilities
 Project-URL: Bug Tracker, https://github.com/pablodorrio/navigation-utilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Navigation Utilities
 
 Navigation Utilities is a Python library for dealing with driverless navigation systems, it is focused on gnss coordinates.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install navigation-utilities.
 
 ```bash
-python -m pip install navigation-utilities -r requirements.txt
+pip install navigation-utilities
 ```
 
 ## Usage
 
 ```python
 import navigation_utilities
 ```
```

### Comparing `navigation-utilities-0.2.1/pyproject.toml` & `navigation-utilities-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = [
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "navigation-utilities"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Pablo Dorrio Vazquez", email="pablo.dorrio.vazquez@gmail.com" },
 ]
 description = "Collection of utilities for driverless navigation systems and gnss tools"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy>=1.24.1"
```

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities/coordinate.py` & `navigation-utilities-0.2.2/src/navigation_utilities/coordinate.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities/gngga.py` & `navigation-utilities-0.2.2/src/navigation_utilities/gngga.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities/nmea.py` & `navigation-utilities-0.2.2/src/navigation_utilities/nmea.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities/oxts.py` & `navigation-utilities-0.2.2/src/navigation_utilities/oxts.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities/utils/time.py` & `navigation-utilities-0.2.2/src/navigation_utilities/utils/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,28 @@
     ) -> None:
         """Initialize the time sentence.
 
         Args:
             hours (int): Hours.
             minutes (int): Minutes.
             seconds (int): Seconds.
+            miliseconds (int): Miliseconds.
         """
         self.__hours = hours
         self.__minutes = minutes
         self.__seconds = seconds
         self.__miliseconds = miliseconds
 
     @property
     def hours(self) -> int:
         """Get the hours of the time.
 
         Returns:
-            int: Hours."""
+            int: Hours.
+        """
         return self.__hours
 
     @hours.setter
     def hours(self, hours: int) -> None:
         """Set the hours of the time.
 
         Args:
@@ -67,15 +69,15 @@
 
     @property
     def seconds(self) -> int:
         """Get the seconds of the time.
 
         Returns:
             int: Seconds.
-        ."""
+        """
         return self.__seconds
 
     @seconds.setter
     def seconds(self, seconds: int) -> None:
         """Set the seconds of the time.
 
         Args:
```

### Comparing `navigation-utilities-0.2.1/src/navigation_utilities.egg-info/PKG-INFO` & `navigation-utilities-0.2.2/src/navigation_utilities.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: navigation-utilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: Collection of utilities for driverless navigation systems and gnss tools
 Author-email: Pablo Dorrio Vazquez <pablo.dorrio.vazquez@gmail.com>
 Project-URL: Homepage, https://github.com/pablodorrio/navigation-utilities
 Project-URL: Bug Tracker, https://github.com/pablodorrio/navigation-utilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Navigation Utilities
 
 Navigation Utilities is a Python library for dealing with driverless navigation systems, it is focused on gnss coordinates.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install navigation-utilities.
 
 ```bash
-python -m pip install navigation-utilities -r requirements.txt
+pip install navigation-utilities
 ```
 
 ## Usage
 
 ```python
 import navigation_utilities
 ```
```

