# Comparing `tmp/tilupy-0.1.3.tar.gz` & `tmp/tilupy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tilupy-0.1.3.tar", last modified: Thu Jul 20 12:56:58 2023, max compression
+gzip compressed data, was "tilupy-0.1.4.tar", last modified: Thu Jul 20 14:20:19 2023, max compression
```

## Comparing `tilupy-0.1.3.tar` & `tilupy-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-20 12:56:47.000000 tilupy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 12:56:47.000000 tilupy-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41646 2023-07-20 12:56:58.942057 tilupy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-20 12:56:47.000000 tilupy-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.934057 tilupy-0.1.3/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.934057 tilupy-0.1.3/data/frankslide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.938057 tilupy-0.1.3/data/frankslide/rasters/
--rw-r--r--   0 runner    (1001) docker     (123)   244005 2023-07-20 12:56:47.000000 tilupy-0.1.3/data/frankslide/rasters/Frankslide_pile.asc
--rw-r--r--   0 runner    (1001) docker     (123)   363702 2023-07-20 12:56:47.000000 tilupy-0.1.3/data/frankslide/rasters/Frankslide_topography.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-20 12:56:47.000000 tilupy-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:56:58.942057 tilupy-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.934057 tilupy-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.938057 tilupy-0.1.3/src/tilupy/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/initdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/src/tilupy/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/src/tilupy/models/ravaflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/ravaflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/ravaflow/initsimus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/ravaflow/read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/src/tilupy/models/shaltop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/shaltop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/shaltop/initsimus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/models/shaltop/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/notations.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-20 12:56:47.000000 tilupy-0.1.3/src/tilupy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/src/tilupy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41646 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 12:56:58.000000 tilupy-0.1.3/src/tilupy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:56:58.942057 tilupy-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-20 12:56:47.000000 tilupy-0.1.3/tests/test_shaltop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-20 14:20:06.000000 tilupy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 14:20:06.000000 tilupy-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41645 2023-07-20 14:20:19.971764 tilupy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-20 14:20:06.000000 tilupy-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.963764 tilupy-0.1.4/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.963764 tilupy-0.1.4/data/frankslide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.967764 tilupy-0.1.4/data/frankslide/rasters/
+-rw-r--r--   0 runner    (1001) docker     (123)   244005 2023-07-20 14:20:06.000000 tilupy-0.1.4/data/frankslide/rasters/Frankslide_pile.asc
+-rw-r--r--   0 runner    (1001) docker     (123)   363702 2023-07-20 14:20:06.000000 tilupy-0.1.4/data/frankslide/rasters/Frankslide_topography.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-20 14:20:06.000000 tilupy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:20:19.971764 tilupy-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.963764 tilupy-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.967764 tilupy-0.1.4/src/tilupy/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/initdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/src/tilupy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/src/tilupy/models/ravaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/ravaflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/ravaflow/initsimus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/ravaflow/read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/src/tilupy/models/shaltop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/shaltop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/shaltop/initsimus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/models/shaltop/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/notations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-20 14:20:06.000000 tilupy-0.1.4/src/tilupy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/src/tilupy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41645 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 14:20:19.000000 tilupy-0.1.4/src/tilupy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:20:19.971764 tilupy-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-20 14:20:06.000000 tilupy-0.1.4/tests/test_shaltop.py
```

### Comparing `tilupy-0.1.3/LICENSE` & `tilupy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/PKG-INFO` & `tilupy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilupy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Thin-layer models unified processing tool
 Author-email: Marc Peruzzetto <m.peruzzetto@brgm.fr>
 License: CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
         
@@ -520,15 +520,15 @@
         
         Version 1.0 dated 2006-09-05.
 Project-URL: Homepage, https://github.com/marcperuz/tilupy
 Keywords: thin-layer,shallow-water,display,simulation,model,processing,benchmark
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: gis
 License-File: LICENSE
 
 # tilupy
```

### Comparing `tilupy-0.1.3/README.md` & `tilupy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/data/frankslide/rasters/Frankslide_pile.asc` & `tilupy-0.1.4/data/frankslide/rasters/Frankslide_pile.asc`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/data/frankslide/rasters/Frankslide_topography.asc` & `tilupy-0.1.4/data/frankslide/rasters/Frankslide_topography.asc`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/pyproject.toml` & `tilupy-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tilupy"
-version = "0.1.3"
+version = "0.1.4"
 description = "Thin-layer models unified processing tool"
 readme = "README.md"
 authors = [{ name = "Marc Peruzzetto", email = "m.peruzzetto@brgm.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: CeCILL-C Free Software License Agreement (CECILL-C)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["thin-layer", "shallow-water", "display", "simulation", "model", "processing", "benchmark"]
 dependencies = [
     "seaborn", "requests",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 test = ["pytest"]
 dev = ["pipreqs"]
 gis = ["rasterio", "shapely"]
 
 [tools.setuptools]
```

### Comparing `tilupy-0.1.3/src/tilupy/__init__.py` & `tilupy-0.1.4/src/tilupy/__init__.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/calibration.py` & `tilupy-0.1.4/src/tilupy/calibration.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/cmd.py` & `tilupy-0.1.4/src/tilupy/cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,68 +7,71 @@
 
 import tilupy.raster
 import tilupy.read
 
 import os
 import argparse
 import glob
-    
+
 
 def process_results(fn_name, model, res_name, folder=None, param_files=None,
                     kwargs_read=None, **kwargs_fn):
-    
+
     assert(model is not None)
-    
+
     if folder is None:
         folder = os.getcwd()
-        
+
     if param_files is None:
         param_files = '*.txt'
-        
+
     print(folder, param_files)
-        
-    param_files = glob.glob(param_files, root_dir=folder)
-    
+
+    param_files = glob.glob(os.path.join(folder, param_files))
+
     if len(param_files) == 0:
         print('No parameter file matching param_files pattern was found')
         return
-        
+
     if kwargs_read is None:
         kwargs_read = dict()
-     
-    kw_read = dict(folder_base=folder)   
+
+    kw_read = dict(folder_base=folder)
     kw_read.update(kwargs_read)
-     
+
     for param_file in param_files:
         print_str = 'Processing simulation {:s}, {:s} {:s} .....'
         print(print_str.format(param_file, fn_name, res_name))
         kw_read['file_params'] = param_file
         res = tilupy.read.get_results(model, **kw_read)
         getattr(res, fn_name)(res_name, **kwargs_fn)
-        
-def to_raster(model=None, res_name='h', param_files=None, folder=None, 
+
+
+def to_raster(model=None, res_name='h', param_files=None, folder=None,
               kwargs_read=None, **kwargs):
-    
+
     kw = dict(fmt='asc')
     kw.update(kwargs)
-    
+
     process_results('save', model, res_name,
                     folder=folder, param_files=param_files,
                     kwargs_read=kwargs_read, **kw)
-    
-def plot_results(model=None, res_name='h', param_files=None, folder=None, 
+
+
+def plot_results(model=None, res_name='h', param_files=None, folder=None,
                  kwargs_read=None, **kwargs):
-    
+
     kw = dict(save=True)
     kw.update(kwargs)
-    
+
     process_results('plot', model, res_name,
                     folder=folder, param_files=param_files,
                     kwargs_read=kwargs_read, **kwargs)
-    
+
+
 def _get_parser(prog, description):
     parser = argparse.ArgumentParser(prog=prog,
                                      description=description,
                                      formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('model', help="Model name",
                         type=str)
     parser.add_argument('-n', '--res_name', help="Name of output, only for maps",
@@ -76,14 +79,15 @@
                         )
     parser.add_argument('-p', '--param_files', help="Parameter file (globbing)",
                         default='*.txt', type=str)
     parser.add_argument('-f', '--folder', help="Root folder, default is current folder",
                         default=None, type=str)
     return parser
 
+
 def _tilupy_plot():
     parser = _get_parser('tilupy_plot', 'Plot thin-layer simulation results')
     parser.add_argument('--fmt', help=("Plot output format "
                                        "(any accepted by matplotlib.savefig)"),
                         default='png', type=str,
                         )
     parser.add_argument('--vmin', help=("Minimum plotted value, "
@@ -96,26 +100,26 @@
                         )
     parser.add_argument('--minval_abs', help=("Minimum plotted absolute value,"
                                               " adapted to data by default"),
                         default=None, type=float,
                         )
     args = parser.parse_args()
     plot_results(**vars(args))
-    
+
+
 def _tilupy_to_raster():
     parser = _get_parser('tilupy_to_raster',
                          'Convert simulation results to rasters')
     parser.add_argument('--fmt', help=("File output format, "
                                        "tif/tiff requires rasterio"),
                         default='asc', type=str,
                         choices=['tif', 'tiff', 'txt', 'asc', 'ascii'])
     args = parser.parse_args()
     # plot_results(parser.model, parser.res_name)
     to_raster(**vars(args))
-    
-    
+
+
 if __name__ == '__main__':
-    
+
     # folder = 'd:/Documents/peruzzetto/tmp/test_shaltop/7p30e04_m3/coulomb'
     # plot_results('shaltop', 'h_max', '*18p00.txt', folder=folder)
     _tilupy_plot()
-
```

### Comparing `tilupy-0.1.3/src/tilupy/compare.py` & `tilupy-0.1.4/src/tilupy/compare.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/download_data.py` & `tilupy-0.1.4/src/tilupy/download_data.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/initdata.py` & `tilupy-0.1.4/src/tilupy/initdata.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/models/ravaflow/initsimus.py` & `tilupy-0.1.4/src/tilupy/models/ravaflow/initsimus.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/models/ravaflow/read.py` & `tilupy-0.1.4/src/tilupy/models/ravaflow/read.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/models/shaltop/initsimus.py` & `tilupy-0.1.4/src/tilupy/models/shaltop/initsimus.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/models/shaltop/read.py` & `tilupy-0.1.4/src/tilupy/models/shaltop/read.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/notations.py` & `tilupy-0.1.4/src/tilupy/notations.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/plot.py` & `tilupy-0.1.4/src/tilupy/plot.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/raster.py` & `tilupy-0.1.4/src/tilupy/raster.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/read.py` & `tilupy-0.1.4/src/tilupy/read.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy/utils.py` & `tilupy-0.1.4/src/tilupy/utils.py`

 * *Files identical despite different names*

### Comparing `tilupy-0.1.3/src/tilupy.egg-info/PKG-INFO` & `tilupy-0.1.4/src/tilupy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilupy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Thin-layer models unified processing tool
 Author-email: Marc Peruzzetto <m.peruzzetto@brgm.fr>
 License: CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
         
@@ -520,15 +520,15 @@
         
         Version 1.0 dated 2006-09-05.
 Project-URL: Homepage, https://github.com/marcperuz/tilupy
 Keywords: thin-layer,shallow-water,display,simulation,model,processing,benchmark
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: gis
 License-File: LICENSE
 
 # tilupy
```

### Comparing `tilupy-0.1.3/src/tilupy.egg-info/SOURCES.txt` & `tilupy-0.1.4/src/tilupy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

