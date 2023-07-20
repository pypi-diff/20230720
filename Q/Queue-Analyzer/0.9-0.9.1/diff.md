# Comparing `tmp/Queue_Analyzer-0.9.tar.gz` & `tmp/Queue_Analyzer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Queue_Analyzer-0.9.tar", last modified: Wed Jul 19 19:21:06 2023, max compression
+gzip compressed data, was "Queue_Analyzer-0.9.1.tar", last modified: Thu Jul 20 13:41:55 2023, max compression
```

## Comparing `Queue_Analyzer-0.9.tar` & `Queue_Analyzer-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35149 2023-05-05 10:22:34.000000 Queue_Analyzer-0.9/LICENSE.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6557 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6185 2023-07-19 19:18:01.000000 Queue_Analyzer-0.9/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      926 2023-07-19 17:08:46.000000 Queue_Analyzer-0.9/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/src/Queue_Analyzer/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-19 18:01:22.000000 Queue_Analyzer-0.9/src/Queue_Analyzer/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-19 19:21:06.972514 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6557 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       99 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-19 19:21:06.000000 Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35148 2023-07-20 13:32:52.000000 Queue_Analyzer-0.9.1/LICENSE.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6740 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6281 2023-07-20 13:29:06.000000 Queue_Analyzer-0.9.1/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/setup.cfg
+-rwxrwxrwx   0 dipson    (1000) dipson    (1000)     1009 2023-07-20 13:41:32.000000 Queue_Analyzer-0.9.1/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.024579 Queue_Analyzer-0.9.1/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/src/Queue_Analyzer/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-19 18:01:22.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:41:55.028580 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6740 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-20 13:41:55.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       98 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-20 13:41:54.000000 Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/top_level.txt
```

### Comparing `Queue_Analyzer-0.9/LICENSE.txt` & `Queue_Analyzer-0.9.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -627,16 +627,16 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
+    To generate a distribution for arrival objects and  analyze the queue from the results.
+    Copyright (C) <year>  Dipson
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) <year>  <name of author>
+    Queue Analyzer  Copyright (C) 2023  Dipson
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `Queue_Analyzer-0.9/PKG-INFO` & `Queue_Analyzer-0.9.1/src/Queue_Analyzer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: Queue_Analyzer
-Version: 0.9
+Name: Queue-Analyzer
+Version: 0.9.1
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Queue Analyzer
 
 This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival and analyse the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
@@ -74,21 +76,21 @@
   ```
 
 **Install using pip**
 
 From **GitHub**
 
 ```
-pip install 
+pip install git+https://github.com/dipson94/Queue-Analyzer.git@main#subdirectory=singlepyfile 
 ```
 
 From **pypi**
 
 ```
-pip install 
+pip install Queue-Analyzer
 ```
 
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
```

### Comparing `Queue_Analyzer-0.9/README.md` & `Queue_Analyzer-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,21 +58,21 @@
   ```
 
 **Install using pip**
 
 From **GitHub**
 
 ```
-pip install 
+pip install git+https://github.com/dipson94/Queue-Analyzer.git@main#subdirectory=singlepyfile 
 ```
 
 From **pypi**
 
 ```
-pip install 
+pip install Queue-Analyzer
 ```
 
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
```

### Comparing `Queue_Analyzer-0.9/setup.py` & `Queue_Analyzer-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
-    
+from setuptools import setup 
 with open("README.md", "r") as f:
 	long_description = f.read()
-
 setup(
 name="Queue_Analyzer",
-version="0.9",
+version="0.9.1",
 description="python package to retreive youtube comments and translate them",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/Queue-Analyzer",
 author="Dipson",
 author_email="dipson94.coding@gmail.com",
 license="GNU GPL V3",
-classifiers=["License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Programming Language :: Python :: 3.10","Operating System :: OS Independent"],
-install_requires=["matplotlib==3.7.2","numpy==1.25.1","pycairo==1.24.0","PyGObject==3.44.1","pandas==2.0.1",],
+classifiers=["License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Programming Language :: Python :: 3.10",'Operating System :: POSIX :: Linux','Operating System :: MacOS :: MacOS X',
+'Operating System :: Unix'],
+install_requires=["matplotlib>=3.5.1","numpy>=1.21.5","pycairo>=1.20.1","pandas>=2.0.1","PyGObject>3.42.0"],
 extras_require={
         "dev": ["pytest >= 7.0"]
         },
 entry_points={
 'console_scripts': ['queueanalyzer=Queue_Analyzer:main',],},
-python_requires=">=3.10",    
+python_requires=">=3.7",    
 )
+#"PyGObject==3.44.1",
```

### Comparing `Queue_Analyzer-0.9/src/Queue_Analyzer/__init__.py` & `Queue_Analyzer-0.9.1/src/Queue_Analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `Queue_Analyzer-0.9/src/Queue_Analyzer.egg-info/PKG-INFO` & `Queue_Analyzer-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: Queue-Analyzer
-Version: 0.9
+Name: Queue_Analyzer
+Version: 0.9.1
 Summary: python package to retreive youtube comments and translate them
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Queue Analyzer
 
 This standalone app is the Graphical user interface version of the python program written to generate a distribution for arrival and analyse the results from the Dosimis software. The app is written in python version 3.11 and GUI is enabled with GTK 3.0 with Glide software.
@@ -74,21 +76,21 @@
   ```
 
 **Install using pip**
 
 From **GitHub**
 
 ```
-pip install 
+pip install git+https://github.com/dipson94/Queue-Analyzer.git@main#subdirectory=singlepyfile 
 ```
 
 From **pypi**
 
 ```
-pip install 
+pip install Queue-Analyzer
 ```
 
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
```

