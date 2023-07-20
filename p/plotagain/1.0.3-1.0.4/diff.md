# Comparing `tmp/plotagain-1.0.3.tar.gz` & `tmp/plotagain-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotagain-1.0.3.tar", last modified: Thu Jul 20 18:33:23 2023, max compression
+gzip compressed data, was "plotagain-1.0.4.tar", last modified: Thu Jul 20 18:34:55 2023, max compression
```

## Comparing `plotagain-1.0.3.tar` & `plotagain-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.446437 plotagain-1.0.3/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.3/.gitignore
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:33:23.446278 plotagain-1.0.3/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.3/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.3/bitbucket-pipelines.yml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.3/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.3/requirements.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:33:23.446489 plotagain-1.0.3/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.443475 plotagain-1.0.3/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.445167 plotagain-1.0.3/src/plotagain/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:33:14.000000 plotagain-1.0.3/src/plotagain/__init__.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.3/src/plotagain/iddict.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.3/src/plotagain/pyplotcall.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7877 2023-07-20 18:33:08.000000 plotagain-1.0.3/src/plotagain/saveplotcontext.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.3/src/plotagain/script_template.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.3/src/plotagain/utils.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.445888 plotagain-1.0.3/src/plotagain.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/requires.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/top_level.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.446035 plotagain-1.0.3/tests/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.3/tests/test_nothing.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:34:55.212576 plotagain-1.0.4/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.4/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:34:55.212409 plotagain-1.0.4/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.4/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.4/bitbucket-pipelines.yml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.4/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.4/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:34:55.212631 plotagain-1.0.4/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:34:55.209322 plotagain-1.0.4/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:34:55.210992 plotagain-1.0.4/src/plotagain/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:34:50.000000 plotagain-1.0.4/src/plotagain/__init__.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.4/src/plotagain/iddict.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.4/src/plotagain/pyplotcall.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7882 2023-07-20 18:34:38.000000 plotagain-1.0.4/src/plotagain/saveplotcontext.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.4/src/plotagain/script_template.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.4/src/plotagain/utils.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:34:55.212018 plotagain-1.0.4/src/plotagain.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:34:55.000000 plotagain-1.0.4/src/plotagain.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:34:55.000000 plotagain-1.0.4/src/plotagain.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:34:55.000000 plotagain-1.0.4/src/plotagain.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:34:55.000000 plotagain-1.0.4/src/plotagain.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:34:55.000000 plotagain-1.0.4/src/plotagain.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:34:55.212167 plotagain-1.0.4/tests/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.4/tests/test_nothing.py
```

### Comparing `plotagain-1.0.3/PKG-INFO` & `plotagain-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plotagain-1.0.3/README.md` & `plotagain-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/bitbucket-pipelines.yml` & `plotagain-1.0.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/pyproject.toml` & `plotagain-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/src/plotagain/iddict.py` & `plotagain-1.0.4/src/plotagain/iddict.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/src/plotagain/pyplotcall.py` & `plotagain-1.0.4/src/plotagain/pyplotcall.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/src/plotagain/saveplotcontext.py` & `plotagain-1.0.4/src/plotagain/saveplotcontext.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from plotagain.iddict import IDDict
 from plotagain.pyplotcall import PyplotCall
 from plotagain.utils import write_pickle
 
-here = Path('.').parent
+here = Path(__file__).parent
 pickle_load_template = "{var_name} = load_pickle('{var_name}.pkl')"
 
 
 class SavePlotContext:
     """
     Context manager which wraps matplotlib.pyplot. Usage:
```

### Comparing `plotagain-1.0.3/src/plotagain/utils.py` & `plotagain-1.0.4/src/plotagain/utils.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.3/src/plotagain.egg-info/PKG-INFO` & `plotagain-1.0.4/src/plotagain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

