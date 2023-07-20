# Comparing `tmp/smartplot-0.0.0.tar.gz` & `tmp/smartplot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartplot-0.0.0.tar", last modified: Thu Jul 20 11:29:48 2023, max compression
+gzip compressed data, was "smartplot-0.1.0.tar", last modified: Thu Jul 20 12:04:41 2023, max compression
```

## Comparing `smartplot-0.0.0.tar` & `smartplot-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 11:29:48.222400 smartplot-0.0.0/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 11:29:48.222241 smartplot-0.0.0/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      170 2023-07-20 11:27:28.000000 smartplot-0.0.0/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      822 2023-07-20 11:05:52.000000 smartplot-0.0.0/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 11:29:48.222449 smartplot-0.0.0/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 11:29:48.220633 smartplot-0.0.0/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 11:29:48.221182 smartplot-0.0.0/src/smartplot/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 10:57:34.000000 smartplot-0.0.0/src/smartplot/__init__.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     6169 2023-07-20 10:56:02.000000 smartplot-0.0.0/src/smartplot/smartplot.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 11:29:48.221981 smartplot-0.0.0/src/smartplot.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 11:29:48.000000 smartplot-0.0.0/src/smartplot.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      225 2023-07-20 11:29:48.000000 smartplot-0.0.0/src/smartplot.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 11:29:48.000000 smartplot-0.0.0/src/smartplot.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 11:29:48.000000 smartplot-0.0.0/src/smartplot.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.561482 smartplot-0.1.0/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 11:38:57.000000 smartplot-0.1.0/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 12:04:41.561312 smartplot-0.1.0/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      170 2023-07-20 11:27:28.000000 smartplot-0.1.0/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      789 2023-07-20 12:03:20.000000 smartplot-0.1.0/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 smartplot-0.1.0/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 12:04:41.561527 smartplot-0.1.0/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.559509 smartplot-0.1.0/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.560366 smartplot-0.1.0/src/smartplot/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 12:04:28.000000 smartplot-0.1.0/src/smartplot/__init__.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     6169 2023-07-20 10:56:02.000000 smartplot-0.1.0/src/smartplot/smartplot.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.561081 smartplot-0.1.0/src/smartplot.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      289 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/top_level.txt
```

### Comparing `smartplot-0.0.0/PKG-INFO` & `smartplot-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartplot
-Version: 0.0.0
+Version: 0.1.0
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

### Comparing `smartplot-0.0.0/pyproject.toml` & `smartplot-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.0"
 keywords = ["save data", "matplotlib", "plt"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Framework :: Matplotlib",
     "Programming Language :: Python :: 3",
 ]
-#dependencies = [
-#    "requests",
-#    'importlib-metadata; python_version<"3.8"',
-#]
+dependencies = [
+    "matplotlib",
+    "numpy",
+]
 dynamic = ["version"]
 
-#[project.scripts]
-#my-script = "my_package.module:function"
+[tool.setuptools.dynamic]
+version = {attr = "smartplot.VERSION"}
```

### Comparing `smartplot-0.0.0/src/smartplot/smartplot.py` & `smartplot-0.1.0/src/smartplot/smartplot.py`

 * *Files identical despite different names*

### Comparing `smartplot-0.0.0/src/smartplot.egg-info/PKG-INFO` & `smartplot-0.1.0/src/smartplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartplot
-Version: 0.0.0
+Version: 0.1.0
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

