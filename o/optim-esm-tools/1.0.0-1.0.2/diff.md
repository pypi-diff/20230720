# Comparing `tmp/optim_esm_tools-1.0.0.tar.gz` & `tmp/optim_esm_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-1.0.0.tar", last modified: Tue Jul 18 09:37:36 2023, max compression
+gzip compressed data, was "optim_esm_tools-1.0.2.tar", last modified: Thu Jul 20 14:32:53 2023, max compression
```

## Comparing `optim_esm_tools-1.0.0.tar` & `optim_esm_tools-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/bin/oet_plot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    25670 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/xarray_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.081616 optim_esm_tools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-20 14:32:53.085616 optim_esm_tools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.069616 optim_esm_tools-1.0.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/bin/oet_plot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.069616 optim_esm_tools-1.0.2/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27831 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/xarray_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.073616 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-20 14:32:53.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-20 14:32:53.085616 optim_esm_tools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.081616 optim_esm_tools-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-1.0.0/PKG-INFO` & `optim_esm_tools-1.0.2/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: optim_esm_tools
-Version: 1.0.0
+Name: optim-esm-tools
+Version: 1.0.2
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,24 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.0.1 / 2023-07-20
+        ------------------
+        * fix /0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/89
+        * Cache region maps by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/90
+        * Clusting bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.0...v1.0.1
+        
+        
         1.0.0 / 2023-07-18
         ------------------
         **major change**
         * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
         
         **minor changes**
         * Plotting routine for masked regions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/82
```

### Comparing `optim_esm_tools-1.0.0/README.md` & `optim_esm_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/bin/oet_plot` & `optim_esm_tools-1.0.2/bin/oet_plot`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     from optim_esm_tools.analyze.pre_process import NoDataInTimeRangeError
     setup_plt()
     constructors = [getattr(optim_esm_tools.analyze.region_finding, meth, 'not found') for meth in methods]
     if any(c=='not found' for c in constructors): raise ValueError(f'One or more non-existing methods {methods}')
 
     from optim_esm_tools.analyze.cmip_handler import read_ds
 
-    log.warning('Read path')
+    log.info('Read path')
     read_ds_kw=read_ds_kw if read_ds_kw is not None else dict()
     ds = read_ds(path, **read_ds_kw)
     kw = dict(data_set=ds, variable=variable, path=None, read_ds_kw=read_ds_kw)
 
     # For cons in constructors
     for cons in constructors:
         result = cons(**kw, save_kw=save_kw, extra_opt=extra_opt, )
@@ -55,15 +55,15 @@
              continue
         except ValueError as e:
             if 'moving average window' in str(e):
                 log.error(f'ValueError for {result.__class__.__name__} as the dataset is too short. Probably in LocalHistory and unharmfull.')
                 continue
             raise e
         result.show=show
-        log.warning(f'====== {result.__class__.__name__} ======')
+        log.warning(f'{result.__class__.__name__}')
         result.workflow()
 
     log.warning('All done')
 
 
 def get_log(args):
     from optim_esm_tools.analyze.find_matches import folder_to_dict
@@ -87,23 +87,19 @@
 
 if __name__ == '__main__':
     args = parse_args()
     if args.profile_memory:
         from memory_profiler import memory_usage
         import time
         import numpy as np
-
         log = get_log(args)
         start = time.time()
         mem = memory_usage(proc=(main, (log, args,)), max_iterations=1)
-        message = f"Memory profiler says peak RAM usage was: {max(mem):.1f} MB, average: {np.mean(mem): .1f} MB"
-        log.warning(message)
-        print(message)
-        message = f'Took {time.time() - start:.1f} s = {(time.time() - start) / 3600:.2f} h '
+        message = f"RAM usage was: {max(mem):.0f} MB (max), {np.mean(mem): .0f} MB (avg). "
+        message += f'Took {time.time() - start:.1f} s = {(time.time() - start) / 3600:.2f} h '
         log.warning(message)
         print(message)
-        # print(f'Took {time.time() - start:.1f} s = {(time.time() - start) / 3600:.2f} h ')
         log.info('Bye, bye')
     else:
         log = get_log(args)
         main(log, args)
         log.info('Done, bye')
```

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/_test_utils.py` & `optim_esm_tools-1.0.2/optim_esm_tools/_test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/clustering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from optim_esm_tools.utils import tqdm, timed
 from optim_esm_tools.config import get_logger
 import typing as ty
 from warnings import warn
 import numba
 from math import sin, cos, sqrt, atan2, radians
+import xarray as xr
 
 
 @timed()
 def build_clusters(
     coordinates_deg: np.ndarray,
     weights: ty.Optional[np.ndarray] = None,
     max_distance_km: ty.Union[float, int] = 750,
@@ -46,15 +47,15 @@
     # Thanks https://stackoverflow.com/a/38731787/18280620!
     try:
         db_fit = DBSCAN(eps=max_distance_km / 6371.0, **cluster_opts).fit(
             X=coordinates_rad, sample_weight=weights
         )
     except ValueError as e:
         raise ValueError(
-            f'With {coordinates_rad.shape} and {weights.shape} {coordinates_rad}, {weights}'
+            f'With {coordinates_rad.shape} and {getattr(weights, "shape", None)} {coordinates_rad}, {weights}'
         ) from e
 
     labels = db_fit.labels_
 
     unique_labels = sorted(set(labels))
     is_core_sample = np.zeros_like(labels, dtype=bool)
     is_core_sample[db_fit.core_sample_indices_] = True
@@ -76,16 +77,16 @@
 
     return return_masks
 
 
 @timed()
 def build_cluster_mask(
     global_mask: np.ndarray,
-    lon_coord: np.array,
     lat_coord: np.array,
+    lon_coord: np.array,
     show_tqdm: bool = False,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the global mask, basically a utility wrapper arround build_clusters'
 
     Args:
@@ -97,41 +98,44 @@
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
-    lon, lat = _check_input(global_mask, lon_coord, lat_coord)
-    xy_data = np.array([lon[global_mask], lat[global_mask]])
+    if max_distance_km == 'infer':
+        max_distance_km = _infer_max_step_size(lat_coord, lon_coord)
+    lat, lon = _check_input(
+        global_mask,
+        lat_coord,
+        lon_coord,
+    )
+    xy_data = np.array([lat[global_mask], lon[global_mask]])
 
     if len(xy_data.T) <= 2:
-        warn(f'No data from this mask {xy_data}!')
+        get_logger().info(f'No data from this mask {xy_data}!')
         return [], []
 
-    if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(lon_coord.flatten(), lat_coord.flatten())
-
     masks, clusters = _build_cluster_with_kw(
-        lon,
-        lat,
+        lat=lat,
+        lon=lon,
         coordinates_deg=xy_data,
         show_tqdm=show_tqdm,
         max_distance_km=max_distance_km,
         **kw,
     )
 
     return masks, clusters
 
 
 @timed()
 def build_weighted_cluster(
     weights: np.ndarray,
-    lon_coord: np.array,
     lat_coord: np.array,
+    lon_coord: np.array,
     show_tqdm: bool = False,
     threshold: ty.Optional[float] = 0.99,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the weights (which should be a grid)'
 
@@ -145,77 +149,115 @@
             Defaults to 'infer'.
         show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
         threshold: float, min value of the passed weights. Defaults to 0.99.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
-
-    lon, lat = _check_input(weights, lon_coord, lat_coord)
-    xy_data = np.array([lon.flatten(), lat.flatten()])
-
     if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(lon.flatten(), lat.flatten())
+        max_distance_km = _infer_max_step_size(lat_coord, lon_coord)
 
-    flat_weights = weights.T.flatten()
+    lat, lon = _check_input(weights, lat_coord, lon_coord)
+    xy_data = np.array([lat.flatten(), lon.flatten()])
+
+    flat_weights = weights.flatten()
     mask = flat_weights > threshold
     masks, clusters = _build_cluster_with_kw(
-        lon,
-        lat,
+        lat=lat,
+        lon=lon,
         coordinates_deg=xy_data[:, mask],
         weights=flat_weights[mask],
         show_tqdm=show_tqdm,
         max_distance_km=max_distance_km,
         **kw,
     )
 
     return masks, clusters
 
 
-def _check_input(data, lon_coord, lat_coord):
+def _check_input(data, lat_coord, lon_coord):
     """Check for consistancy and if we need to convert the lon/lat coordinates to a meshgrid"""
     if len(lon_coord.shape) <= 1:
-        get_logger().warning('Expected lon and lat values, but got x, y values')
-        # seperate x, y values, bad practice?
         lon, lat = np.meshgrid(lon_coord, lat_coord)
     else:
-        lon, lat = lon_coord, lat_coord
+        # In an older version, this would have been the default.
+        lat, lon = lat_coord, lon_coord
 
     if data.shape != lon.shape or data.shape != lat.shape:
         message = f'Wrong input {data.shape} != {lon.shape, lat.shape}'
         raise ValueError(message)
-    return lon, lat
+    return lat, lon
 
 
-def _build_cluster_with_kw(lon, lat, show_tqdm=False, **cluster_kw):
+def _build_cluster_with_kw(lat, lon, show_tqdm=False, **cluster_kw):
     """Overlapping logic between functions to get the masks and clusters"""
     masks = []
     clusters = [np.rad2deg(cluster) for cluster in build_clusters(**cluster_kw)]
     if lat.shape != lon.shape:
         raise ValueError(f'Got inconsistent input {lat.shape} != {lon.shape}')
     for cluster in clusters:
         mask = np.zeros(lat.shape, np.bool_)
-        for s_x, s_y in tqdm(cluster, desc='fill_mask', disable=not show_tqdm):
+        for coord_lat, coord_lon in tqdm(
+            cluster, desc='fill_mask', disable=not show_tqdm
+        ):
             # This is a bit blunt, but it's fast enough to regain the indexes such that we can build a 2d masked array.
-            mask_x = np.isclose(lon, s_x)
-            mask_y = np.isclose(lat, s_y)
+            mask_x = np.isclose(lon, coord_lon)
+            mask_y = np.isclose(lat, coord_lat)
             mask |= mask_x & mask_y
         masks.append(mask)
     return masks, clusters
 
 
-def _infer_max_step_size(xs, ys):
-    ys = ys[ys > 0]
-    # coords = [[[xs[0], ys[0]], [xs[0], ys[1]]], [[xs[0], ys[0]], [xs[1], ys[0]]]]
-    # Return long:lat
-    coords = [[[ys[0], xs[0]], [ys[0], xs[1]]], [[ys[0], xs[0]], [ys[1], xs[0]]]]
+def _infer_max_step_size(lat, lon, off_by_factor=1.1):
+    if len(lat.shape) == 1:
+        return np.max(calculate_distance_map(lat, lon)) * off_by_factor
+    lat = lat[lat > 0]
+    coords = [
+        [[lat[0], lon[0]], [lat[0], lon[1]]],
+        [[lat[0], lon[0]], [lat[1], lon[0]]],
+    ]
     # Return 2x the distance between grid cells
     return 2 * max(_distance(c) for c in coords)
 
 
+def calculate_distance_map(lat, lon):
+    """For each point in a spanned lat lon grid, calculate the distance to the neighbouring points"""
+    if isinstance(lat, xr.DataArray):
+        lat = lat.values
+        lon = lon.values
+    return _calculate_distance_map(lat, lon)
+
+
+@numba.njit
+def _calculate_distance_map(lat, lon):
+    n_lat = len(lat)
+    n_lon = len(lon)
+    distances = np.zeros((n_lat, n_lon))
+
+    shift_by_index = np.array(
+        [(-1, 0), (1, 0), (0, -1), (0, 1), (-1, -1), (1, 1), (1, -1), (-1, 1)]
+    )
+    neighbourgs = np.zeros(len(shift_by_index), dtype=np.float64)
+    for lon_i in range(n_lon):
+        for lat_i in range(n_lat):
+            neighbourgs[:] = 0
+            current = (lat[lat_i], lon[lon_i])
+            for i, (x, y) in enumerate(shift_by_index):
+                alt_lon = np.mod(lon_i + x, n_lon)
+                alt_lat = lat_i + y
+                if alt_lat == n_lat or alt_lat < 0:
+                    continue
+                alt_coord = (lat[alt_lat], lon[alt_lon])
+                if alt_coord == current:
+                    continue
+                neighbourgs[i] = _distance_bf_coord(*current, *alt_coord)
+            distances[lat_i][lon_i] = np.max(neighbourgs)
+    return distances
+
+
 def _distance(coords, force_math=False):
     """Wrapper for if geopy is not installed"""
     if not force_math:
         try:
             from geopy.distance import geodesic
 
             return geodesic(*coords).km
```

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/cmip_handler.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/io.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/io.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/pre_process.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/pre_process.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/region_finding.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,51 +5,85 @@
 from optim_esm_tools.analyze.clustering import (
     build_cluster_mask,
     build_weighted_cluster,
 )
 from optim_esm_tools.plotting.plot import setup_map, _show
 from optim_esm_tools.analyze.tipping_criteria import rank2d
 from optim_esm_tools.analyze.find_matches import base_from_path
+from .globals import _CMIP_HANDLER_VERSION
 
 import numpy as np
 import matplotlib.pyplot as plt
 import logging
 import xarray as xr
 
 import typing as ty
 from functools import wraps
 import inspect
 import matplotlib.pyplot as plt
 import immutabledict
+import os
 
 
 # >>> import scipy
 # >>> scipy.stats.norm.cdf(3)
 # 0.9986501019683699
 # >> scipy.stats.norm.cdf(2)
 # 0.9772498680518208
 _two_sigma_percent = 97.72498680518208
 
 
-def mask_xr_ds(data_set, da_mask, masked_dims=None):
+def mask_xr_ds(data_set, da_mask, masked_dims=None, drop=False):
+    # Modify the ds in place - make a copy!
+    data_set = data_set.copy()
     if masked_dims is None:
         masked_dims = oet.config.config['analyze']['lon_lat_dim'].split(',')
 
     ds_start = data_set.copy()
+    func_by_drop = {True: _drop_by_mask, False: _mask_xr_ds}[drop]
+    data_set = func_by_drop(data_set, masked_dims, ds_start, da_mask)
+    data_set = data_set.assign_attrs(ds_start.attrs)
+    return data_set
+
+
+def _drop_by_mask(data_set, masked_dims, ds_start, da_mask):
+    """Drop values with masked_dims dimentions.
+    Unfortunately, data_set.where(da_mask, drop=True) sometimes leads to bad results,
+    for example for time_bnds (time, bnds) being dropped by (lon, lat). So we have to do
+    some funny bookkeeping of which datavars we can drop with data_set.where.
+    """
+
+    dropped = []
+    for k, data_array in data_set.data_vars.items():
+        if not all(dim in list(data_array.dims) for dim in masked_dims):
+            dropped += [k]
+
+    data_set = data_set.drop_vars(dropped)
+
+    data_set = data_set.where(da_mask, drop=True)
+
+    # Restore ignored variables and attributes
+    for k in dropped:
+        data_set[k] = ds_start[k]
+    return data_set
+
+
+def _mask_xr_ds(data_set, masked_dims, ds_start, da_mask):
+    """Rebuild data_set for each variabled that has all masked_dims"""
     for k, data_array in data_set.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
             # First dim is time?
             if (
                 'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape
             ) or data_array.shape == da_mask.T.shape:
                 raise ValueError(f'Please make "{k}" lat, lon, now "{data_array.dims}"')
             da = data_set[k].where(da_mask, drop=False)
             da = da.assign_attrs(ds_start[k].attrs)
             data_set[k] = da
-    data_set = data_set.assign_attrs(ds_start.attrs)
+
     return data_set
 
 
 def plt_show(*a):
     """Wrapper to disable class methods to follow up with show"""
 
     def somedec_outer(fn):
@@ -200,23 +234,43 @@
         ret_m = []
         ret_c = []
         for m, c in zip(*masks_and_clusters):
             if self.mask_is_large_enough(m):
                 ret_m.append(m)
                 ret_c.append(c)
 
-        self.log.warn(f'Keeping {len(ret_m)}/{len(masks_and_clusters[0])} of masks')
+        self.log.info(f'Keeping {len(ret_m)}/{len(masks_and_clusters[0])} of masks')
         return ret_m, ret_c
 
     @plt_show
     def summarize_mask(self, mask, m_i):
         self._summarize_mask(mask)
         plt.suptitle(self.title + f' cluster {m_i}')
         self.save(f'{self.title_label}_cluster_{m_i}')
 
+        self.store_mask(mask, m_i)
+
+    @apply_options
+    def store_mask(self, mask, m_i, store_masks=True):
+        if not store_masks:
+            return
+        save_in = self.save_kw['save_in']
+        store_in_dir = os.path.join(save_in, 'masks')
+        os.makedirs(store_in_dir, exist_ok=True)
+        # Mask twice, "mask" is a np.ndarray, whereas ds.where needs a xr.DataArray.
+        # While we could make this more efficient (and only use the second step), the first step does only take ~10 ms
+        ds_masked = mask_xr_ds(self.data_set.copy(), mask)
+        ds_masked = mask_xr_ds(ds_masked, ~ds_masked['cell_area'].isnull(), drop=True)
+        ds_masked.to_netcdf(
+            os.path.join(
+                store_in_dir,
+                f'{self.title_label}_cluster-{m_i}_v{_CMIP_HANDLER_VERSION}.nc',
+            )
+        )
+
     def _summarize_mask(self, mask, plot=None):
         axes = oet.plotting.map_maker.summarize_mask(self.data_set, mask, plot=plot)
         return axes
 
     def make_mask_figures(self, masks):
         for m_i, mask in enumerate(masks):
             if np.sum(mask) == 0:
@@ -617,15 +671,15 @@
                 dict(version='*'),
                 # can lead to funny behavior as grid differences may cause breaking compares
                 dict(grid_label='*'),
             ]
 
         for try_n, update_query in enumerate(query_updates):
             if try_n:
-                self.log.warning(
+                self.log.info(
                     f'No results after {try_n} try, retying with {update_query}'
                 )
             search.update(update_query)
             this_try = oet.analyze.find_matches.find_matches(base, **search)
             if this_try:
                 return this_try
         raise RuntimeError(f'Looked for {search}, in {base} found nothing')
@@ -713,20 +767,24 @@
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
             arr = self.data_set[lab].values
             arr_historical = historical_ds[lab].values
-            mask_divide = arr / arr_historical > n_times_historical
+
             # If arr_historical is 0, the devision is going to get a nan assigned,
             # despite this being the most interesting region (no historical
             # changes, only in the scenario's)!
-            mask_no_std = (arr_historical == 0) & (arr > 0)
-            masks.append(mask_divide | mask_no_std)
+            mask_no_std = arr_historical == 0
+            mask_divide = np.zeros_like(mask_no_std)
+            mask_divide[~mask_no_std] = (
+                arr[~mask_no_std] / arr_historical[~mask_no_std] > n_times_historical
+            )
+            masks.append(mask_divide | (mask_no_std & (arr != 0)))
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         self.check_shape(all_mask)
```

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-1.0.2/optim_esm_tools/analyze/xarray_tools.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/config.py` & `optim_esm_tools-1.0.2/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/optim_esm_conf.ini` & `optim_esm_tools-1.0.2/optim_esm_tools/optim_esm_conf.ini`

 * *Files 7% similar despite different names*

```diff
@@ -26,24 +26,25 @@
 folder_fmt = activity_id institution_id source_id experiment_id variant_label domain variable_id grid_label version
 base_name = merged.nc
 temp_file_name = temp_pre.nc
 
 excluded =
         ; # This one only has a dataset which is 5 years long, rendering it quite useless for 10yr running means
         E3SM-Project       E3SM-1-1-ECA     piControl   r1i1p1f1  *        *  gr  v20201204
+        E3SM-Project       E3SM-1-1-ECA     piControl   r1i1p1f1  *        *  *   v20201203
 
         ; # Bad data https://errata.es-doc.org/static/index.html?experiment=ssp585&institute=thu&project=cmip6&source=ciesm
         ; THU                CIESM            ssp585      r1i1p1f1  *        *  *   v20200417
 
         ; ### Too short datasets ###
         ; BCC_BCC            ESM1             ssp370      r3i1p1f1  tas      *  *   v20190702
         ; HAMMOZ-Consortium  MPI-ESM-1-2-HAM  ssp370      r3i1p1f1  tas      *  *   v20191218
-        ; NCC                NorESM2-LM       ssp245      r1i1p1f2  tas      *  *   v20210908
+        NCC                NorESM2-LM       ssp245      r1i1p1f2  tas      *  *   v20210908
         E3SM-Project       E3SM-1-1         ssp245      r1i1p1f1  *        *  gr  v20201109
-        CNRM-CERFACS       CNRM-CM6-1       ssp245      *         *        *  gr  v20200212
+        CNRM-CERFACS       CNRM-CM6-1       ssp245      *         *        *  *   v20200212
 
         ; # These sets have data in the 1e20 range:
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  siconc   *  gn  v20201124
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  tos      *  gn  v20210416
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  sithick  *  gn  v20210416
 
         ; #  --- TODO ---
@@ -55,14 +56,15 @@
         ; DKRZ               MPI-ESM1-2-LR    ssp119      r1i1p1f1  siconc   *  *   v20210901
 
 
         ; unstructured source grid non conformal indexing for lat/lon (one iterator i for x and y)
         MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20210215
         MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20220111
         AWI                AWI-ESM-1-1-LR   *           r1i1p1f1  *       *   gn  v20200212
+        AWI                AWI-CM-1-1-MR    *           *         Oyear   *   gn  v20181218
 
 [log]
 logging_level = WARNING
 
 
 # For the wrapper that monitors real time of functions (@timed)
 [time_tool]
```

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-1.0.2/optim_esm_tools/plotting/map_maker.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/plotting/plot.py` & `optim_esm_tools-1.0.2/optim_esm_tools/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-1.0.2/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools/utils.py` & `optim_esm_tools-1.0.2/optim_esm_tools/utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: optim-esm-tools
-Version: 1.0.0
+Name: optim_esm_tools
+Version: 1.0.2
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,24 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.0.1 / 2023-07-20
+        ------------------
+        * fix /0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/89
+        * Cache region maps by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/90
+        * Clusting bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.0...v1.0.1
+        
+        
         1.0.0 / 2023-07-18
         ------------------
         **major change**
         * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
         
         **minor changes**
         * Plotting routine for masked regions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/82
```

### Comparing `optim_esm_tools-1.0.0/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-1.0.2/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/setup.py` & `optim_esm_tools-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='1.0.0',
+    version='1.0.2',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
```

### Comparing `optim_esm_tools-1.0.0/test/test_find_matches.py` & `optim_esm_tools-1.0.2/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/test/test_region_finding.py` & `optim_esm_tools-1.0.2/test/test_region_finding.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/test/test_utils.py` & `optim_esm_tools-1.0.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/test/test_viewer.py` & `optim_esm_tools-1.0.2/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/test/test_workflow.py` & `optim_esm_tools-1.0.2/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.0/test/test_xarray_tools.py` & `optim_esm_tools-1.0.2/test/test_xarray_tools.py`

 * *Files identical despite different names*

