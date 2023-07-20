# Comparing `tmp/daggerpy-0.0.1.tar.gz` & `tmp/daggerpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daggerpy-0.0.1.tar", last modified: Thu Jul 20 09:12:14 2023, max compression
+gzip compressed data, was "daggerpy-0.0.2.tar", last modified: Thu Jul 20 11:08:17 2023, max compression
```

## Comparing `daggerpy-0.0.1.tar` & `daggerpy-0.0.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 09:12:14.299260 daggerpy-0.0.1/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.1/AUTHORS.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       85 2023-07-20 08:04:31.000000 daggerpy-0.0.1/HISTORY.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.1/LICENSE
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.1/MANIFEST.in
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 09:12:14.299260 daggerpy-0.0.1/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.1/README.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 09:12:14.299260 daggerpy-0.0.1/daggerpy.egg-info/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1470 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/SOURCES.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/dependency_links.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/entry_points.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/not-zip-safe
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/requires.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-20 09:12:14.000000 daggerpy-0.0.1/daggerpy.egg-info/top_level.txt
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 09:12:14.299260 daggerpy-0.0.1/docs/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/Makefile
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/authors.rst
--rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.1/docs/conf.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/contributing.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/history.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/index.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/installation.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/make.bat
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/readme.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.1/docs/usage.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 09:12:14.299260 daggerpy-0.0.1/includes/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/D4connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121804 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/PerlinNoise.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26014 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/_cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/_graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/_old_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/_priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/boost_spread_sort.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/boundary_conditions.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3227 2023-07-20 08:53:44.000000 daggerpy-0.0.1/includes/connector_checker.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26421 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14090 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/depression_hierarchy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126074 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/fastflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/fastflood_recorder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64105 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    87785 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/graphflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/hillshading.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/npy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    17874 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/popscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/popscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15617 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27925 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/simple_depression_solver.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94639 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/trackscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/trackscape_enum.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/trackscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1061 2023-07-20 08:53:44.000000 daggerpy-0.0.1/includes/veclike_holder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/veque.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/wrap_helper.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/wrap_helper_MATLAB.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/wrap_helper_cpp.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/wrap_helper_julia.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-20 08:46:36.000000 daggerpy-0.0.1/includes/wrap_helper_python.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82286 2023-07-20 08:46:36.000000 daggerpy-0.0.1/main.cpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-20 09:12:14.299260 daggerpy-0.0.1/setup.cfg
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3704 2023-07-20 09:10:49.000000 daggerpy-0.0.1/setup.py
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 09:12:14.299260 daggerpy-0.0.1/tests/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.1/tests/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 08:04:31.000000 daggerpy-0.0.1/tests/test_dagger.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.2/AUTHORS.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       85 2023-07-20 08:04:31.000000 daggerpy-0.0.2/HISTORY.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.2/LICENSE
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.2/MANIFEST.in
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 11:08:17.153822 daggerpy-0.0.2/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.2/README.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.149822 daggerpy-0.0.2/daggerpy.egg-info/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1470 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/entry_points.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.2/daggerpy.egg-info/not-zip-safe
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/requires.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/top_level.txt
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.149822 daggerpy-0.0.2/docs/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/Makefile
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/authors.rst
+-rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.2/docs/conf.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/contributing.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/history.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/index.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/installation.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/make.bat
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/readme.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/usage.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/includes/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/D4connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121804 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/PerlinNoise.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26014 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_old_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/boost_spread_sort.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/boundary_conditions.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3178 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/connector_checker.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26421 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14090 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/depression_hierarchy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126074 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/fastflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/fastflood_recorder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64105 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    87785 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/graphflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/hillshading.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/npy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    17857 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/popscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/popscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15617 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27925 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/simple_depression_solver.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94622 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape_enum.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1110 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/veclike_holder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/veque.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_MATLAB.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_cpp.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_julia.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82286 2023-07-20 11:06:36.000000 daggerpy-0.0.2/main.cpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-20 11:08:17.153822 daggerpy-0.0.2/setup.cfg
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-20 11:08:13.000000 daggerpy-0.0.2/setup.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/tests/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.2/tests/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.2/tests/test_dagger.py
```

### Comparing `daggerpy-0.0.1/CONTRIBUTING.rst` & `daggerpy-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/LICENSE` & `daggerpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/PKG-INFO` & `daggerpy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `daggerpy-0.0.1/README.rst` & `daggerpy-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/daggerpy.egg-info/PKG-INFO` & `daggerpy-0.0.2/daggerpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `daggerpy-0.0.1/daggerpy.egg-info/SOURCES.txt` & `daggerpy-0.0.2/daggerpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/docs/Makefile` & `daggerpy-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/docs/conf.py` & `daggerpy-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/docs/installation.rst` & `daggerpy-0.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/docs/make.bat` & `daggerpy-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/D4connector.hpp` & `daggerpy-0.0.2/includes/D4connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/D8connector.hpp` & `daggerpy-0.0.2/includes/D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/PerlinNoise.hpp` & `daggerpy-0.0.2/includes/PerlinNoise.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/_D8connector.hpp` & `daggerpy-0.0.2/includes/_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/_cordonnier_versatile_2019.hpp` & `daggerpy-0.0.2/includes/_cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/_graph.hpp` & `daggerpy-0.0.2/includes/_graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/_old_D8connector.hpp` & `daggerpy-0.0.2/includes/_old_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/_priority_flood.hpp` & `daggerpy-0.0.2/includes/_priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/boost_spread_sort.hpp` & `daggerpy-0.0.2/includes/boost_spread_sort.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/boundary_conditions.hpp` & `daggerpy-0.0.2/includes/boundary_conditions.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/connector_checker.hpp` & `daggerpy-0.0.2/includes/connector_checker.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,134 @@
 /*
-Defines the standardised loose connection of the connectors.
+Defines the standardised loose connection of the connectors. 
 
 There are 2 different level of standards:
 
-        - the generic standard, defining the functions that will be called in
-the different modules. They are the only one allowed in module accepting
-different types of connectors.
-
-        - the specifyers standards, defining function specific to build, set and
-customise given subsets of connectors. For example a regular grid will need nx
-and ny, not needed by a voronoi one. THESE CAN ONLY BE CALLED OUTSIDE OF THE
-MODULES. The modules should not need to know how the connector is structured
-(loosely connected).
-
-It uses phantom functions, called during the building of a new connector,
-checking the said connector has all the required functions to fit the template.
-
-
-A typical script would construct the connector first, calling generic and
-specific functions, then throw the connector inside the module (e.g. graph,
-graphflood, trackscape) where it would only use the generic functions.
-
-That way, I can for example build a connector from a regular grid, setting the
-nx, ny, dx, dy and boundary condition efficiently and then build graphflood with
-that connector.
+	- the generic standard, defining the functions that will be called in the different modules. 
+They are the only one allowed in module accepting different types of connectors.
+	
+	- the specifyers standards, defining function specific to build, set and customise given subsets of connectors. 
+For example a regular grid will need nx and ny, not needed by a voronoi one. 
+THESE CAN ONLY BE CALLED OUTSIDE OF THE MODULES. The modules should not need to know how the connector is structured (loosely connected). 
+
+It uses phantom functions, called during the building of a new connector, 
+checking the said connector has all the required functions to fit the template. 
+
+
+A typical script would construct the connector first, calling generic and specific functions, 
+then throw the connector inside the module (e.g. graph, graphflood, trackscape)
+where it would only use the generic functions.
+
+That way, I can for example build a connector from a regular grid, setting the nx, ny, dx, dy and boundary condition efficiently
+and then build graphflood with that connector.
 
 */
 
+
 #ifndef CONNECTOR_CHECKER_HPP
 #define CONNECTOR_CHECKER_HPP
 
-/// Generic checker: checks if the connector has the minimal set of functions to
-/// be accepted by the other modules
-template <class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT,
-          class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
-void check_connector_template_generic(Connector_t &con) {
-
-  // Generic init function
-  // Return nothing, initialise the data structure.
-  // Argument: the number of nodes in the connector (includes no data)
-  void (Connector_t::*initialisation)(int) = &Connector_t::init;
-
-  // Generic function precomputing elements in the graph.
-  // Its interpretation is free and really depends on the type of
-  // grid/connection is needed. This is where, for example, a connector
-  // optimised for cpu can compute all the receivers/donors information from
-  // topography; an irregular grid could regrid there, or simply, if the
-  // neighbouring never caches anything for a memory-saving connector, do
-  // nothing.
-  void (Connector_t::*preco)() = &Connector_t::compute;
-
-  // Connect a (new) topography, to be used for computing receivers/donors.
-  void (Connector_t::*connect_topo)(VECLIKE &) =
-      &Connector_t::connect_topography;
-
-  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with
-  // nn neighbours
-  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &) =
-      &Connector_t::neighbouring_nodes;
-
-  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and
-  // with nn neighbours
-  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &,
-                                 CONTAINER_NEIGHBOURS_fT &) =
-      &Connector_t::neighbouring_nodes_and_distance;
-
-  // // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT
-  // with nn links int (Connector_t::*Neighbours) (int,
-  // CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
 
-  // Returns the area at a diven node index
-  fT (Connector_t::*Area)(int) = &Connector_t::Area;
+/// Generic checker: checks if the connector has the minimal set of functions to be accepted by the other modules
+template<class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT, class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
+void check_connector_template_generic(Connector_t& con)
+{
+
+	// Generic init function
+	// Return nothing, initialise the data structure.
+	// Argument: the number of nodes in the connector (includes no data)
+	void (Connector_t::*initialisation)(int) = &Connector_t::init;
+
+	// Generic function precomputing elements in the graph.
+	// Its interpretation is free and really depends on the type of grid/connection is needed.
+	// This is where, for example, a connector optimised for cpu can compute all the receivers/donors information from topography;
+	// an irregular grid could regrid there, or simply, if the neighbouring never caches anything for a memory-saving connector, do nothing.
+	void (Connector_t::*preco)() = &Connector_t::compute;
+
+	// Connect a (new) topography, to be used for computing receivers/donors.
+	void (Connector_t::*connect_topo)(VECLIKE&) = &Connector_t::connect_topography;
+
+	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn neighbours
+	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_nodes;
+
+	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and  with nn neighbours
+	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&, CONTAINER_NEIGHBOURS_fT&) = &Connector_t::neighbouring_nodes_and_distance;
+
+	// // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn links
+	// int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
+
+	// Returns the area at a diven node index
+	fT (Connector_t::*Area)(int) = &Connector_t::Area;
+
 }
 
-#endif
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+#endif
```

### Comparing `daggerpy-0.0.1/includes/cordonnier_versatile_2019.hpp` & `daggerpy-0.0.2/includes/cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/depression_hierarchy.hpp` & `daggerpy-0.0.2/includes/depression_hierarchy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/fastflood.hpp` & `daggerpy-0.0.2/includes/fastflood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/fastflood_recorder.hpp` & `daggerpy-0.0.2/includes/fastflood_recorder.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/graph.hpp` & `daggerpy-0.0.2/includes/graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/graphflood.hpp` & `daggerpy-0.0.2/includes/graphflood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/hillshading.hpp` & `daggerpy-0.0.2/includes/hillshading.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/npy.hpp` & `daggerpy-0.0.2/includes/npy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/popscape.hpp` & `daggerpy-0.0.2/includes/popscape.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #include <cmath>
 #include <ctime>
 #include <fstream>
 #include <initializer_list>
 #include <iostream>
 #include <map>
 #include <numeric>
-#include <omp.h>
 #include <queue>
 #include <stack>
 #include <stdlib.h>
 #include <string>
 #include <thread>
 #include <vector>
```

### Comparing `daggerpy-0.0.1/includes/popscape_utils.hpp` & `daggerpy-0.0.2/includes/popscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/priority_flood.hpp` & `daggerpy-0.0.2/includes/priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/simple_depression_solver.hpp` & `daggerpy-0.0.2/includes/simple_depression_solver.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/trackscape.hpp` & `daggerpy-0.0.2/includes/trackscape.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 #include <cmath>
 #include <ctime>
 #include <fstream>
 #include <initializer_list>
 #include <iostream>
 #include <map>
 #include <numeric>
-#include <omp.h>
 #include <queue>
 #include <stack>
 #include <stdlib.h>
 #include <string>
 #include <thread>
 #include <vector>
```

### Comparing `daggerpy-0.0.1/includes/trackscape_utils.hpp` & `daggerpy-0.0.2/includes/trackscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/utils.hpp` & `daggerpy-0.0.2/includes/utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/veque.hpp` & `daggerpy-0.0.2/includes/veque.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/wrap_helper.hpp` & `daggerpy-0.0.2/includes/wrap_helper.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/wrap_helper_MATLAB.hpp` & `daggerpy-0.0.2/includes/wrap_helper_MATLAB.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/wrap_helper_julia.hpp` & `daggerpy-0.0.2/includes/wrap_helper_julia.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/includes/wrap_helper_python.hpp` & `daggerpy-0.0.2/includes/wrap_helper_python.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/main.cpp` & `daggerpy-0.0.2/main.cpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.1/setup.py` & `daggerpy-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # pybind11 is used for c++ integration
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup, find_packages
 import os
 import platform
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 
 #############################################
 # Admin inputs
 #############################################
 
@@ -104,11 +104,11 @@
     include_package_data=True,
     keywords='dagger',
     name='daggerpy',
     test_suite='tests',
     tests_require=test_requirements,
     ext_modules=ext_modules,
     url='https://github.com/bgailleton/DAGGER',
-    version='0.0.1',
+    version=__version__,
     zip_safe=False,
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `daggerpy-0.0.1/tests/test_dagger.py` & `daggerpy-0.0.2/tests/test_dagger.py`

 * *Files identical despite different names*

