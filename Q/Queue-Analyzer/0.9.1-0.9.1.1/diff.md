# Comparing `tmp/Queue_Analyzer-0.9.1.tar.gz` & `tmp/Queue_Analyzer-0.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Queue_Analyzer-0.9.1.tar", last modified: Thu Jul 20 13:41:55 2023, max compression
+gzip compressed data, was "Queue_Analyzer-0.9.1.1.tar", last modified: Thu Jul 20 13:46:28 2023, max compression
```

## Comparing `Queue_Analyzer-0.9.1.tar` & `Queue_Analyzer-0.9.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35148 2023-07-20 13:32:52.000000 Queue_Analyzer-0.9.1/LICENSE.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6740 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6281 2023-07-20 13:29:06.000000 Queue_Analyzer-0.9.1/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/setup.cfg
--rwxrwxrwx   0 dipson    (1000) dipson    (1000)     1009 2023-07-20 13:41:32.000000 Queue_Analyzer-0.9.1/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.024579 Queue_Analyzer-0.9.1/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/src/Queue_Analyzer/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-19 18:01:22.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6740 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-20 13:41:55.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       98 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35148 2023-07-20 13:32:52.000000 Queue_Analyzer-0.9.1.1/LICENSE.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6749 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6288 2023-07-20 13:45:52.000000 Queue_Analyzer-0.9.1.1/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/setup.cfg
+-rwxrwxrwx   0 dipson    (1000) dipson    (1000)     1011 2023-07-20 13:46:02.000000 Queue_Analyzer-0.9.1.1/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.317335 Queue_Analyzer-0.9.1.1/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.317335 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-19 18:01:22.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6749 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       98 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/top_level.txt
```

### Comparing `Queue_Analyzer-0.9.1/LICENSE.txt` & `Queue_Analyzer-0.9.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Queue_Analyzer-0.9.1/PKG-INFO` & `Queue_Analyzer-0.9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Queue_Analyzer
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Queue Analyzer
 
-This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival and analyse the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
+This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival objects and analyze the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [How it works](#how-it-works)
 - [Contributing](#contributing)
@@ -33,23 +33,23 @@
 
 The App can be run/installed in following ways.
 
 **Install**
 
 Prerequisites are following
 
-- matplotlib==3.7.2
+- matplotlib>=3.5.1
 
-- numpy==1.25.1
+- numpy>=1.21.5
 
-- pycairo==1.24.0
+- pycairo>=1.20.1
 
-- PyGObject==3.44.1
+- PyGObject>3.42.0
 
-- pandas==2.0.1
+- pandas>=2.0.1
 
   **Prerequistic for PyGObject**
 
   
 
   On **Ubuntu** or debian based OS :
```

### Comparing `Queue_Analyzer-0.9.1/README.md` & `Queue_Analyzer-0.9.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Queue Analyzer
 
-This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival and analyse the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
+This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival objects and analyze the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [How it works](#how-it-works)
 - [Contributing](#contributing)
@@ -15,23 +15,23 @@
 
 The App can be run/installed in following ways.
 
 **Install**
 
 Prerequisites are following
 
-- matplotlib==3.7.2
+- matplotlib>=3.5.1
 
-- numpy==1.25.1
+- numpy>=1.21.5
 
-- pycairo==1.24.0
+- pycairo>=1.20.1
 
-- PyGObject==3.44.1
+- PyGObject>3.42.0
 
-- pandas==2.0.1
+- pandas>=2.0.1
 
   **Prerequistic for PyGObject**
 
   
 
   On **Ubuntu** or debian based OS :
```

### Comparing `Queue_Analyzer-0.9.1/setup.py` & `Queue_Analyzer-0.9.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup 
 with open("README.md", "r") as f:
 	long_description = f.read()
 setup(
 name="Queue_Analyzer",
-version="0.9.1",
+version="0.9.1.1",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/Queue-Analyzer",
 author="Dipson",
```

### Comparing `Queue_Analyzer-0.9.1/src/Queue_Analyzer/__init__.py` & `Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/PKG-INFO` & `Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Queue-Analyzer
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Queue Analyzer
 
-This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival and analyse the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
+This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival objects and analyze the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [How it works](#how-it-works)
 - [Contributing](#contributing)
@@ -33,23 +33,23 @@
 
 The App can be run/installed in following ways.
 
 **Install**
 
 Prerequisites are following
 
-- matplotlib==3.7.2
+- matplotlib>=3.5.1
 
-- numpy==1.25.1
+- numpy>=1.21.5
 
-- pycairo==1.24.0
+- pycairo>=1.20.1
 
-- PyGObject==3.44.1
+- PyGObject>3.42.0
 
-- pandas==2.0.1
+- pandas>=2.0.1
 
   **Prerequistic for PyGObject**
 
   
 
   On **Ubuntu** or debian based OS :
```

