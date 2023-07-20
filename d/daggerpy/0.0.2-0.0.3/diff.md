# Comparing `tmp/daggerpy-0.0.2.tar.gz` & `tmp/daggerpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daggerpy-0.0.2.tar", last modified: Thu Jul 20 11:08:17 2023, max compression
+gzip compressed data, was "daggerpy-0.0.3.tar", last modified: Thu Jul 20 14:21:22 2023, max compression
```

## Comparing `daggerpy-0.0.2.tar` & `daggerpy-0.0.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.2/AUTHORS.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       85 2023-07-20 08:04:31.000000 daggerpy-0.0.2/HISTORY.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.2/LICENSE
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.2/MANIFEST.in
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 11:08:17.153822 daggerpy-0.0.2/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.2/README.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.149822 daggerpy-0.0.2/daggerpy.egg-info/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2408 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1470 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/SOURCES.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/dependency_links.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/entry_points.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.2/daggerpy.egg-info/not-zip-safe
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/requires.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-20 11:08:17.000000 daggerpy-0.0.2/daggerpy.egg-info/top_level.txt
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.149822 daggerpy-0.0.2/docs/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/Makefile
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/authors.rst
--rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.2/docs/conf.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/contributing.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/history.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/index.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/installation.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/make.bat
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/readme.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.2/docs/usage.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/includes/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/D4connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121804 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/PerlinNoise.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26014 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_old_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/_priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/boost_spread_sort.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/boundary_conditions.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3178 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/connector_checker.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26421 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14090 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/depression_hierarchy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126074 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/fastflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/fastflood_recorder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64105 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    87785 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/graphflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/hillshading.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/npy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    17857 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/popscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/popscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15617 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27925 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/simple_depression_solver.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94622 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape_enum.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/trackscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1110 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/veclike_holder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/veque.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_MATLAB.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_cpp.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_julia.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-20 11:06:36.000000 daggerpy-0.0.2/includes/wrap_helper_python.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82286 2023-07-20 11:06:36.000000 daggerpy-0.0.2/main.cpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-20 11:08:17.153822 daggerpy-0.0.2/setup.cfg
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-20 11:08:13.000000 daggerpy-0.0.2/setup.py
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 11:08:17.153822 daggerpy-0.0.2/tests/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.2/tests/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.2/tests/test_dagger.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:21:22.191346 daggerpy-0.0.3/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.3/AUTHORS.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      229 2023-07-20 14:20:53.000000 daggerpy-0.0.3/HISTORY.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.3/LICENSE
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.3/MANIFEST.in
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2552 2023-07-20 14:21:22.191346 daggerpy-0.0.3/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.3/README.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:21:22.187346 daggerpy-0.0.3/daggerpy.egg-info/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2552 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1470 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/entry_points.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.3/daggerpy.egg-info/not-zip-safe
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/requires.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-20 14:21:22.000000 daggerpy-0.0.3/daggerpy.egg-info/top_level.txt
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:21:22.191346 daggerpy-0.0.3/docs/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/Makefile
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/authors.rst
+-rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.3/docs/conf.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/contributing.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/history.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/index.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/installation.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/make.bat
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/readme.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.3/docs/usage.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:21:22.191346 daggerpy-0.0.3/includes/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/D4connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121804 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/PerlinNoise.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26014 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/_cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/_graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/_old_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/_priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/boost_spread_sort.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/boundary_conditions.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3178 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/connector_checker.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26421 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14090 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/depression_hierarchy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126074 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/fastflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/fastflood_recorder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64105 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    87785 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/graphflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/hillshading.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/npy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18089 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/popscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/popscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15617 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27925 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/simple_depression_solver.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94622 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/trackscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/trackscape_enum.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/trackscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1110 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/veclike_holder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/veque.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/wrap_helper.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/wrap_helper_MATLAB.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/wrap_helper_cpp.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/wrap_helper_julia.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-20 14:21:04.000000 daggerpy-0.0.3/includes/wrap_helper_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82286 2023-07-20 14:21:04.000000 daggerpy-0.0.3/main.cpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-20 14:21:22.191346 daggerpy-0.0.3/setup.cfg
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-20 14:19:23.000000 daggerpy-0.0.3/setup.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:21:22.191346 daggerpy-0.0.3/tests/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.3/tests/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.3/tests/test_dagger.py
```

### Comparing `daggerpy-0.0.2/CONTRIBUTING.rst` & `daggerpy-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/LICENSE` & `daggerpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/PKG-INFO` & `daggerpy-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -72,11 +72,18 @@
 Some I/O operations are using `libnpy <https://github.com/llohse/libnpy>`_ (MIT), a header-only c++ library to write/load simple `numpy` arrays.
 
 
 =======
 History
 =======
 
+0.0.3 (20/07/2023)
+------------------
+
+* Fixing compilation for conda-forge on MacOS and Windows
+* Adding a quick topo function as quick test
+
 0 (2023-07-20)
 ------------------
 
 * First release on PyPI.
+
```

### Comparing `daggerpy-0.0.2/README.rst` & `daggerpy-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/daggerpy.egg-info/PKG-INFO` & `daggerpy-0.0.3/daggerpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -72,11 +72,18 @@
 Some I/O operations are using `libnpy <https://github.com/llohse/libnpy>`_ (MIT), a header-only c++ library to write/load simple `numpy` arrays.
 
 
 =======
 History
 =======
 
+0.0.3 (20/07/2023)
+------------------
+
+* Fixing compilation for conda-forge on MacOS and Windows
+* Adding a quick topo function as quick test
+
 0 (2023-07-20)
 ------------------
 
 * First release on PyPI.
+
```

### Comparing `daggerpy-0.0.2/daggerpy.egg-info/SOURCES.txt` & `daggerpy-0.0.3/daggerpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/docs/Makefile` & `daggerpy-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/docs/conf.py` & `daggerpy-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/docs/installation.rst` & `daggerpy-0.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/docs/make.bat` & `daggerpy-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/D4connector.hpp` & `daggerpy-0.0.3/includes/D4connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/D8connector.hpp` & `daggerpy-0.0.3/includes/D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/PerlinNoise.hpp` & `daggerpy-0.0.3/includes/PerlinNoise.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/_D8connector.hpp` & `daggerpy-0.0.3/includes/_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/_cordonnier_versatile_2019.hpp` & `daggerpy-0.0.3/includes/_cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/_graph.hpp` & `daggerpy-0.0.3/includes/_graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/_old_D8connector.hpp` & `daggerpy-0.0.3/includes/_old_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/_priority_flood.hpp` & `daggerpy-0.0.3/includes/_priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/boost_spread_sort.hpp` & `daggerpy-0.0.3/includes/boost_spread_sort.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/boundary_conditions.hpp` & `daggerpy-0.0.3/includes/boundary_conditions.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/connector_checker.hpp` & `daggerpy-0.0.3/includes/connector_checker.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/cordonnier_versatile_2019.hpp` & `daggerpy-0.0.3/includes/cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/depression_hierarchy.hpp` & `daggerpy-0.0.3/includes/depression_hierarchy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/fastflood.hpp` & `daggerpy-0.0.3/includes/fastflood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/fastflood_recorder.hpp` & `daggerpy-0.0.3/includes/fastflood_recorder.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/graph.hpp` & `daggerpy-0.0.3/includes/graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/graphflood.hpp` & `daggerpy-0.0.3/includes/graphflood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/hillshading.hpp` & `daggerpy-0.0.3/includes/hillshading.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/npy.hpp` & `daggerpy-0.0.3/includes/npy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/popscape.hpp` & `daggerpy-0.0.3/includes/popscape.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -596,11 +596,20 @@
     if (i < ncycles)
       psc.restriction(5);
   }
 
   return psc.topography;
 }
 
+
+
+template<class fT, class out_t>
+out_t quick_fluvial_topo(int ncycles, std::string boundaries)
+{
+  std::vector<fT> out = _quick_fluvial_topo<fT>(ncycles, boundaries);
+  return DAGGER::format_output<std::vector<fT>, out_t>(out);
+}
+
 // End of namespace fastflood
 }; // namespace DAGGER
 
 #endif
```

### Comparing `daggerpy-0.0.2/includes/popscape_utils.hpp` & `daggerpy-0.0.3/includes/popscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/priority_flood.hpp` & `daggerpy-0.0.3/includes/priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/simple_depression_solver.hpp` & `daggerpy-0.0.3/includes/simple_depression_solver.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/trackscape.hpp` & `daggerpy-0.0.3/includes/trackscape.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/trackscape_utils.hpp` & `daggerpy-0.0.3/includes/trackscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/utils.hpp` & `daggerpy-0.0.3/includes/utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/veclike_holder.hpp` & `daggerpy-0.0.3/includes/veclike_holder.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/veque.hpp` & `daggerpy-0.0.3/includes/veque.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/wrap_helper.hpp` & `daggerpy-0.0.3/includes/wrap_helper.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/wrap_helper_MATLAB.hpp` & `daggerpy-0.0.3/includes/wrap_helper_MATLAB.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/wrap_helper_julia.hpp` & `daggerpy-0.0.3/includes/wrap_helper_julia.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/includes/wrap_helper_python.hpp` & `daggerpy-0.0.3/includes/wrap_helper_python.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/main.cpp` & `daggerpy-0.0.3/main.cpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.2/setup.py` & `daggerpy-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # pybind11 is used for c++ integration
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup, find_packages
 import os
 import platform
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 
 #############################################
 # Admin inputs
 #############################################
```

### Comparing `daggerpy-0.0.2/tests/test_dagger.py` & `daggerpy-0.0.3/tests/test_dagger.py`

 * *Files identical despite different names*

