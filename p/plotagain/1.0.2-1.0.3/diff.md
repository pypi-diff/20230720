# Comparing `tmp/plotagain-1.0.2.tar.gz` & `tmp/plotagain-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotagain-1.0.2.tar", last modified: Thu Jul 20 18:30:30 2023, max compression
+gzip compressed data, was "plotagain-1.0.3.tar", last modified: Thu Jul 20 18:33:23 2023, max compression
```

## Comparing `plotagain-1.0.2.tar` & `plotagain-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:30:30.535808 plotagain-1.0.2/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.2/.gitignore
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:30:30.535655 plotagain-1.0.2/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.2/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.2/bitbucket-pipelines.yml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.2/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.2/requirements.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:30:30.535855 plotagain-1.0.2/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:30:30.532709 plotagain-1.0.2/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:30:30.534552 plotagain-1.0.2/src/plotagain/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:30:23.000000 plotagain-1.0.2/src/plotagain/__init__.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.2/src/plotagain/iddict.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.2/src/plotagain/pyplotcall.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7846 2023-07-20 18:30:13.000000 plotagain-1.0.2/src/plotagain/saveplotcontext.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.2/src/plotagain/script_template.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.2/src/plotagain/utils.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:30:30.535304 plotagain-1.0.2/src/plotagain.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:30:30.000000 plotagain-1.0.2/src/plotagain.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:30:30.000000 plotagain-1.0.2/src/plotagain.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:30:30.000000 plotagain-1.0.2/src/plotagain.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:30:30.000000 plotagain-1.0.2/src/plotagain.egg-info/requires.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:30:30.000000 plotagain-1.0.2/src/plotagain.egg-info/top_level.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:30:30.535442 plotagain-1.0.2/tests/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.2/tests/test_nothing.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.446437 plotagain-1.0.3/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       26 2023-07-20 12:51:44.000000 plotagain-1.0.3/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:33:23.446278 plotagain-1.0.3/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3299 2023-07-20 17:59:37.000000 plotagain-1.0.3/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.3/bitbucket-pipelines.yml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.3/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-20 10:56:02.000000 plotagain-1.0.3/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-20 18:33:23.446489 plotagain-1.0.3/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.443475 plotagain-1.0.3/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.445167 plotagain-1.0.3/src/plotagain/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      109 2023-07-20 18:33:14.000000 plotagain-1.0.3/src/plotagain/__init__.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.3/src/plotagain/iddict.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-20 17:53:49.000000 plotagain-1.0.3/src/plotagain/pyplotcall.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7877 2023-07-20 18:33:08.000000 plotagain-1.0.3/src/plotagain/saveplotcontext.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.3/src/plotagain/script_template.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-20 17:37:51.000000 plotagain-1.0.3/src/plotagain/utils.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.445888 plotagain-1.0.3/src/plotagain.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3892 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      450 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-20 18:33:23.000000 plotagain-1.0.3/src/plotagain.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-20 18:33:23.446035 plotagain-1.0.3/tests/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.3/tests/test_nothing.py
```

### Comparing `plotagain-1.0.2/PKG-INFO` & `plotagain-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.2
+Version: 1.0.3
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plotagain-1.0.2/README.md` & `plotagain-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/bitbucket-pipelines.yml` & `plotagain-1.0.3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/pyproject.toml` & `plotagain-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/src/plotagain/iddict.py` & `plotagain-1.0.3/src/plotagain/iddict.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/src/plotagain/pyplotcall.py` & `plotagain-1.0.3/src/plotagain/pyplotcall.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/src/plotagain/saveplotcontext.py` & `plotagain-1.0.3/src/plotagain/saveplotcontext.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def __init__(
         self,
         save_dir: Union[Path, str],
         locals_dict: Dict[str, Any],
         overwrite: bool = False,
         globals_dict: Optional[Dict[str, Any]] = None,
         script_name: str = 'make_plot.py',
-        script_template: Union[Path, str] = here / 'script_template.txt',
+        script_template: Optional[Union[Path, str]] = None,
     ):
         """
 
         Parameters
         ----------
         save_dir
             The path to a directory into which the argument pickles and autogenerated script are saved. If the directory
@@ -90,15 +90,15 @@
             SavePlotContext. See script_template.txt for an example
         """
         self.save_dir = Path(save_dir)
         self.outer_locals_dict = locals_dict
         self.outer_globals_dict = globals_dict or {}
         self.overwrite = overwrite
         self.regenerate_script_name = script_name
-        self.script_template_path = Path(script_template)
+        self.script_template_path = Path(script_template or (here / 'script_template.txt')).absolute()
 
         self.used_variables = {}
         self.calls = []
 
         if not self.save_dir.exists():
             self.save_dir.mkdir()
         if not self.overwrite and len(list(self.save_dir.glob('*'))) > 0:
```

### Comparing `plotagain-1.0.2/src/plotagain/utils.py` & `plotagain-1.0.3/src/plotagain/utils.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.2/src/plotagain.egg-info/PKG-INFO` & `plotagain-1.0.3/src/plotagain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.2
+Version: 1.0.3
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

