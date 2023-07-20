# Comparing `tmp/smartplot-0.1.0.tar.gz` & `tmp/smartplot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartplot-0.1.0.tar", last modified: Thu Jul 20 12:04:41 2023, max compression
+gzip compressed data, was "smartplot-0.1.1.tar", last modified: Thu Jul 20 12:52:23 2023, max compression
```

## Comparing `smartplot-0.1.0.tar` & `smartplot-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.561482 smartplot-0.1.0/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 11:38:57.000000 smartplot-0.1.0/.gitignore
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 12:04:41.561312 smartplot-0.1.0/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      170 2023-07-20 11:27:28.000000 smartplot-0.1.0/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      789 2023-07-20 12:03:20.000000 smartplot-0.1.0/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 smartplot-0.1.0/requirements.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 12:04:41.561527 smartplot-0.1.0/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.559509 smartplot-0.1.0/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.560366 smartplot-0.1.0/src/smartplot/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 12:04:28.000000 smartplot-0.1.0/src/smartplot/__init__.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     6169 2023-07-20 10:56:02.000000 smartplot-0.1.0/src/smartplot/smartplot.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:04:41.561081 smartplot-0.1.0/src/smartplot.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      701 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      289 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/requires.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 12:04:41.000000 smartplot-0.1.0/src/smartplot.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:52:23.782356 smartplot-0.1.1/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 smartplot-0.1.1/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3496 2023-07-20 12:52:23.782180 smartplot-0.1.1/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2965 2023-07-20 12:44:37.000000 smartplot-0.1.1/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      789 2023-07-20 12:03:20.000000 smartplot-0.1.1/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 smartplot-0.1.1/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 12:52:23.782406 smartplot-0.1.1/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:52:23.780386 smartplot-0.1.1/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:52:23.781272 smartplot-0.1.1/src/smartplot/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       71 2023-07-20 12:49:43.000000 smartplot-0.1.1/src/smartplot/__init__.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     6250 2023-07-20 12:49:43.000000 smartplot-0.1.1/src/smartplot/smartplot.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 12:52:23.781951 smartplot-0.1.1/src/smartplot.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3496 2023-07-20 12:52:23.000000 smartplot-0.1.1/src/smartplot.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      289 2023-07-20 12:52:23.000000 smartplot-0.1.1/src/smartplot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 12:52:23.000000 smartplot-0.1.1/src/smartplot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 12:52:23.000000 smartplot-0.1.1/src/smartplot.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 12:52:23.000000 smartplot-0.1.1/src/smartplot.egg-info/top_level.txt
```

### Comparing `smartplot-0.1.0/pyproject.toml` & `smartplot-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartplot-0.1.0/src/smartplot/smartplot.py` & `smartplot-0.1.1/src/smartplot/smartplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 def is_primitive(thing):
     return any(isinstance(thing, primitive) for primitive in primitives)
 
 
 script_template = """import numpy as np
 import matplotlib.pyplot as plt
-import pickle
+from smartplot import load_pickle
 
 
 {load_variables_code}
 
 {do_plot_code}
 """
-pickle_load_template = "{var_name} = pickle.load(open('{var_name}.pkl', 'rb'))"
+pickle_load_template = "{var_name} = load_pickle('{var_name}.pkl')"
 
 
 def insert_next_available(dict_, key, val):
     postfix = ''
     ind = 1
     while key + postfix in dict_:
         ind += 1
@@ -186,22 +186,23 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.save()
         return False
 
 
+def load_pickle(filename):
+    with open(filename, 'rb') as f:
+        return pickle.load(f)
+
+
 if __name__ == '__main__':
     x_data = np.linspace(0, 2 * np.pi, 1000)
     y_data = np.sin(x_data)
-    with SmartPlotContext(
-        "./test",
-        locals(),
-        overwrite=True,
-    ) as spl:
+    with SmartPlotContext("./data-save-dir", locals(), overwrite=True) as spl:
         spl.plot(x_data, y_data, c='k', label='sin')
         spl.plot(x_data, np.cos(x_data), c='b', label='cos')
         spl.xlabel('xaxis')
         spl.ylabel('yaxis')
         spl.title('Title')
         spl.legend()
```

