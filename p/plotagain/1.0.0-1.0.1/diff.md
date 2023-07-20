# Comparing `tmp/plotagain-1.0.0.tar.gz` & `tmp/plotagain-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotagain-1.0.0.tar", last modified: Thu Jul 20 18:24:54 2023, max compression
+gzip compressed data, was "plotagain-1.0.1.tar", last modified: Thu Jul 20 18:27:53 2023, max compression
```

## Comparing `plotagain-1.0.0.tar` & `plotagain-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:24:54.339720 plotagain-1.0.0/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.0/.gitignore
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:24:54.339544 plotagain-1.0.0/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.0/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.0/bitbucket-pipelines.yml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.0/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.0/requirements.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:24:54.339769 plotagain-1.0.0/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:24:54.336379 plotagain-1.0.0/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:24:54.338123 plotagain-1.0.0/src/plotagain/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:01:06.000000 plotagain-1.0.0/src/plotagain/__init__.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.0/src/plotagain/iddict.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.0/src/plotagain/pyplotcall.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7839 2023-07-20 18:01:06.000000 plotagain-1.0.0/src/plotagain/saveplotcontext.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.0/src/plotagain/script_template.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.0/src/plotagain/utils.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:24:54.339053 plotagain-1.0.0/src/plotagain.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:24:54.000000 plotagain-1.0.0/src/plotagain.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:24:54.000000 plotagain-1.0.0/src/plotagain.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:24:54.000000 plotagain-1.0.0/src/plotagain.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:24:54.000000 plotagain-1.0.0/src/plotagain.egg-info/requires.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:24:54.000000 plotagain-1.0.0/src/plotagain.egg-info/top_level.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:24:54.339302 plotagain-1.0.0/tests/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.0/tests/test_nothing.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:27:53.729870 plotagain-1.0.1/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.1/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:27:53.729702 plotagain-1.0.1/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.1/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.1/bitbucket-pipelines.yml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.1/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.1/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:27:53.729917 plotagain-1.0.1/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:27:53.727022 plotagain-1.0.1/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:27:53.728658 plotagain-1.0.1/src/plotagain/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:27:48.000000 plotagain-1.0.1/src/plotagain/__init__.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.1/src/plotagain/iddict.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.1/src/plotagain/pyplotcall.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7839 2023-07-20 18:01:06.000000 plotagain-1.0.1/src/plotagain/saveplotcontext.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.1/src/plotagain/script_template.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.1/src/plotagain/utils.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:27:53.729370 plotagain-1.0.1/src/plotagain.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:27:53.000000 plotagain-1.0.1/src/plotagain.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:27:53.000000 plotagain-1.0.1/src/plotagain.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:27:53.000000 plotagain-1.0.1/src/plotagain.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:27:53.000000 plotagain-1.0.1/src/plotagain.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:27:53.000000 plotagain-1.0.1/src/plotagain.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:27:53.729500 plotagain-1.0.1/tests/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.1/tests/test_nothing.py
```

### Comparing `plotagain-1.0.0/PKG-INFO` & `plotagain-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.0
+Version: 1.0.1
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plotagain-1.0.0/README.md` & `plotagain-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/bitbucket-pipelines.yml` & `plotagain-1.0.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/pyproject.toml` & `plotagain-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/src/plotagain/iddict.py` & `plotagain-1.0.1/src/plotagain/iddict.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/src/plotagain/pyplotcall.py` & `plotagain-1.0.1/src/plotagain/pyplotcall.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/src/plotagain/saveplotcontext.py` & `plotagain-1.0.1/src/plotagain/saveplotcontext.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/src/plotagain/utils.py` & `plotagain-1.0.1/src/plotagain/utils.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.0/src/plotagain.egg-info/PKG-INFO` & `plotagain-1.0.1/src/plotagain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.0
+Version: 1.0.1
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

