# Comparing `tmp/ptlibs-1.0.0.tar.gz` & `tmp/ptlibs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptlibs-1.0.0.tar", last modified: Mon Jul 17 18:13:06 2023, max compression
+gzip compressed data, was "ptlibs-1.0.1.tar", last modified: Thu Jul 20 12:48:34 2023, max compression
```

## Comparing `ptlibs-1.0.0.tar` & `ptlibs-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.803499 ptlibs-1.0.0/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    35149 2023-07-17 17:40:35.000000 ptlibs-1.0.0/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2442 2023-07-17 18:13:06.803499 ptlibs-1.0.0/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1880 2023-07-17 18:04:26.000000 ptlibs-1.0.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.799499 ptlibs-1.0.0/ptlibs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1115 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptcharsethelper.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      753 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptdefs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4328 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptjsonlib.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6542 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptmisclib.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2096 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptnethelper.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5118 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptpathtypedetector.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5949 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptprinthelper.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.803499 ptlibs-1.0.0/ptlibs/threads/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1042 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/arraylock.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1316 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/printlock.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1783 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/ptthreads.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.799499 ptlibs-1.0.0/ptlibs.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2442 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        7 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-17 18:13:06.803499 ptlibs-1.0.0/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      816 2023-07-17 17:42:13.000000 ptlibs-1.0.0/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-20 12:48:34.000052 ptlibs-1.0.1/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    35149 2023-07-17 17:40:35.000000 ptlibs-1.0.1/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2499 2023-07-20 12:48:34.000052 ptlibs-1.0.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1937 2023-07-20 12:48:15.000000 ptlibs-1.0.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-20 12:48:33.996052 ptlibs-1.0.1/ptlibs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1115 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptcharsethelper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      753 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptdefs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4328 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptjsonlib.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6542 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptmisclib.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2096 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptnethelper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5118 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptpathtypedetector.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5949 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/ptprinthelper.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-20 12:48:34.000052 ptlibs-1.0.1/ptlibs/threads/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/threads/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1042 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/threads/arraylock.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1316 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/threads/printlock.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1783 2023-07-17 17:40:35.000000 ptlibs-1.0.1/ptlibs/threads/ptthreads.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-20 12:48:34.000052 ptlibs-1.0.1/ptlibs.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2499 2023-07-20 12:48:33.000000 ptlibs-1.0.1/ptlibs.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-07-20 12:48:33.000000 ptlibs-1.0.1/ptlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-20 12:48:33.000000 ptlibs-1.0.1/ptlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       27 2023-07-20 12:48:33.000000 ptlibs-1.0.1/ptlibs.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        7 2023-07-20 12:48:33.000000 ptlibs-1.0.1/ptlibs.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-20 12:48:34.000052 ptlibs-1.0.1/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      838 2023-07-20 12:42:48.000000 ptlibs-1.0.1/setup.py
```

### Comparing `ptlibs-1.0.0/LICENSE` & `ptlibs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/PKG-INFO` & `ptlibs-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptlibs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Support library for penterepTools
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -23,14 +23,16 @@
 ## Installation
 ```
 pip install ptlibs
 ```
 
 ## Version History
 ```
+- 1.0.1
+    - added missing requests-toolbelt dependency
 - 1.0.0
     - Cookie redirect fix
 - 0.1.3
     - ptpathtypedetector - get_type() method tweaks
     - arraylock - new ThreadSafeArray class
     - added windows support (for tools that do not use functions that depend on fcntl, termios libraries)
 - 0.1.2
```

### Comparing `ptlibs-1.0.0/README.md` & `ptlibs-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 ## Installation
 ```
 pip install ptlibs
 ```
 
 ## Version History
 ```
+- 1.0.1
+    - added missing requests-toolbelt dependency
 - 1.0.0
     - Cookie redirect fix
 - 0.1.3
     - ptpathtypedetector - get_type() method tweaks
     - arraylock - new ThreadSafeArray class
     - added windows support (for tools that do not use functions that depend on fcntl, termios libraries)
 - 0.1.2
```

### Comparing `ptlibs-1.0.0/ptlibs/ptcharsethelper.py` & `ptlibs-1.0.1/ptlibs/ptcharsethelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptdefs.py` & `ptlibs-1.0.1/ptlibs/ptdefs.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptjsonlib.py` & `ptlibs-1.0.1/ptlibs/ptjsonlib.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptmisclib.py` & `ptlibs-1.0.1/ptlibs/ptmisclib.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptnethelper.py` & `ptlibs-1.0.1/ptlibs/ptnethelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptpathtypedetector.py` & `ptlibs-1.0.1/ptlibs/ptpathtypedetector.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/ptprinthelper.py` & `ptlibs-1.0.1/ptlibs/ptprinthelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/threads/arraylock.py` & `ptlibs-1.0.1/ptlibs/threads/arraylock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/threads/printlock.py` & `ptlibs-1.0.1/ptlibs/threads/printlock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs/threads/ptthreads.py` & `ptlibs-1.0.1/ptlibs/threads/ptthreads.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.0/ptlibs.egg-info/PKG-INFO` & `ptlibs-1.0.1/ptlibs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptlibs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Support library for penterepTools
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -23,14 +23,16 @@
 ## Installation
 ```
 pip install ptlibs
 ```
 
 ## Version History
 ```
+- 1.0.1
+    - added missing requests-toolbelt dependency
 - 1.0.0
     - Cookie redirect fix
 - 0.1.3
     - ptpathtypedetector - get_type() method tweaks
     - arraylock - new ThreadSafeArray class
     - added windows support (for tools that do not use functions that depend on fcntl, termios libraries)
 - 0.1.2
```

### Comparing `ptlibs-1.0.0/setup.py` & `ptlibs-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 setuptools.setup(
     name="ptlibs",
     description="Support library for penterepTools",
     author="Penterep",
     author_email="info@penterep.com",
     url="https://www.penterep.com/",
-    version="1.0.0",
+    version="1.0.1",
     license="GPLv3+",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
     ],
     python_requires = '>=3.6',
-    install_requires=["requests"],
+    install_requires=["requests", "requests-toolbelt"],
     long_description=long_description,
     long_description_content_type="text/markdown"
-)
+)
```

