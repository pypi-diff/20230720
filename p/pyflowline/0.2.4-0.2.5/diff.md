# Comparing `tmp/pyflowline-0.2.4.tar.gz` & `tmp/pyflowline-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowline-0.2.4.tar", last modified: Wed Jun 14 19:40:31 2023, max compression
+gzip compressed data, was "pyflowline-0.2.5.tar", last modified: Thu Jul 20 20:25:15 2023, max compression
```

## Comparing `pyflowline-0.2.4.tar` & `pyflowline-0.2.5.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-14 19:40:18.000000 pyflowline-0.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-14 19:40:18.000000 pyflowline-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 19:40:18.000000 pyflowline-0.2.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-14 19:40:18.000000 pyflowline-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 19:40:18.000000 pyflowline-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-14 19:40:31.866621 pyflowline-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-14 19:40:18.000000 pyflowline-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.838619 pyflowline-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.846619 pyflowline-0.2.4/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    67244 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/after_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)    64320 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/after_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)    66495 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/basic_element.png
--rw-r--r--   0 runner    (1001) docker     (123)    76858 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/before_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)    68959 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/before_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)    69874 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/data_mode.png
--rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/disconnect_flowline.png
--rw-r--r--   0 runner    (1001) docker     (123)   146717 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/find_vertex.png
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/flow_direction.png
--rw-r--r--   0 runner    (1001) docker     (123)   252712 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/flow_direction_matrix.png
--rw-r--r--   0 runner    (1001) docker     (123)   525380 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/hexagon.png
--rw-r--r--   0 runner    (1001) docker     (123)   628942 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/hexagon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)   524174 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/lat_lon.png
--rw-r--r--   0 runner    (1001) docker     (123)   734342 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/lat_lon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)    45168 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/merge_flowline.png
--rw-r--r--   0 runner    (1001) docker     (123)  1191889 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/meshes.png
--rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/remove_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)   596253 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/remove_loop_matrix.png
--rw-r--r--   0 runner    (1001) docker     (123)    93563 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/simplification01.png
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/small_river.png
--rw-r--r--   0 runner    (1001) docker     (123)   148387 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/sqaure_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)    61180 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/square.png
--rw-r--r--   0 runner    (1001) docker     (123)    46783 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/structure_pyflowline.png
--rw-r--r--   0 runner    (1001) docker     (123)   160993 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/algorithm/algorithm.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/api/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/application/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/application/application.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/data/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/installation/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/support.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 19:40:18.000000 pyflowline-0.2.4/examples/create_model_condfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/pyflowline/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/check_head_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_index_in_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/longlat_to_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/cython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/direction/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/direction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/direction/correct_flowline_direction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/index/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_segment_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/intersect/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/loop/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/loop/remove_flowline_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/merge/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/merge/merge_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/simplification/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_duplicate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_returning_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_small_river.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/split/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_vertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_by_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline_to_edge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.862620 pyflowline-0.2.4/pyflowline/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    47953 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/basin.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/hexagon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/latlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/square.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/tin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_flowline_to_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_vertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/dggrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/dggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/dggrid/create_dggrid_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/hexagon/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/hexagon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17396 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/latlon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/latlon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/latlon/create_latlon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/mpas/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/mpas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/mpas/create_mpas_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/square/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/square/create_square_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/tin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/tin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/tin/create_tin_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/pyflowline_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/pyflowline_read_model_configuration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/pyflowline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 19:40:31.866621 pyflowline-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-14 19:40:18.000000 pyflowline-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 19:40:18.000000 pyflowline-0.2.4/tests/test_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 20:25:03.000000 pyflowline-0.2.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 20:25:03.000000 pyflowline-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 20:25:03.000000 pyflowline-0.2.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 20:25:03.000000 pyflowline-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 20:25:03.000000 pyflowline-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-07-20 20:25:15.233045 pyflowline-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-20 20:25:03.000000 pyflowline-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.205045 pyflowline-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    67244 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/after_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64320 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/after_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66495 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/basic_element.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76858 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/before_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68959 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/before_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69874 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/data_mode.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/disconnect_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146717 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/find_vertex.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/flow_direction.png
+-rw-r--r--   0 runner    (1001) docker     (123)   252712 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/flow_direction_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)   525380 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/hexagon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   628942 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/hexagon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)   524174 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/lat_lon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   734342 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/lat_lon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45168 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/merge_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1191889 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/meshes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/remove_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   596253 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/remove_loop_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93563 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/simplification01.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/small_river.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148387 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/sqaure_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61180 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46783 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/structure_pyflowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160993 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/figures/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/algorithm/algorithm.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/api/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/application/application.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/data/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.217045 pyflowline-0.2.5/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/installation/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 20:25:03.000000 pyflowline-0.2.5/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:03.000000 pyflowline-0.2.5/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-20 20:25:03.000000 pyflowline-0.2.5/examples/create_model_condfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/check_head_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/find_index_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/auxiliary/longlat_to_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/direction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/direction/correct_flowline_direction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/index/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/index/define_stream_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/index/define_stream_segment_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline/algorithms/intersect/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.225045 pyflowline-0.2.5/pyflowline/algorithms/loop/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/loop/remove_flowline_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.225045 pyflowline-0.2.5/pyflowline/algorithms/merge/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/merge/merge_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.225045 pyflowline-0.2.5/pyflowline/algorithms/simplification/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_duplicate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_returning_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_small_river.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.225045 pyflowline-0.2.5/pyflowline/algorithms/split/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/find_flowline_confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/find_flowline_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/split_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/split_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/algorithms/split/split_flowline_to_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48652 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/dggrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/hexagon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43990 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/square.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/tin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/classes/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/convert_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/convert_flowline_to_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/export_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/export_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/read_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/read_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/dggrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/dggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/dggrid/create_dggrid_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/hexagon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/hexagon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/latlon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/latlon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/latlon/create_latlon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/mpas/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/mpas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/mpas/create_mpas_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/square/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/square/create_square_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/pyflowline/mesh/tin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/tin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/mesh/tin/create_tin_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/pyflowline_create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyflowline/pyflowline_read_model_configuration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.221045 pyflowline-0.2.5/pyflowline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-07-20 20:25:15.000000 pyflowline-0.2.5/pyflowline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-20 20:25:15.000000 pyflowline-0.2.5/pyflowline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:25:15.000000 pyflowline-0.2.5/pyflowline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 20:25:15.000000 pyflowline-0.2.5/pyflowline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 20:25:15.000000 pyflowline-0.2.5/pyflowline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 20:25:04.000000 pyflowline-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 20:25:15.233045 pyflowline-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-20 20:25:04.000000 pyflowline-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:25:15.229045 pyflowline-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 20:25:04.000000 pyflowline-0.2.5/tests/test_installation.py
```

### Comparing `pyflowline-0.2.4/CONTRIBUTING.rst` & `pyflowline-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/LICENSE` & `pyflowline-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/PKG-INFO` & `pyflowline-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.2.4
+Version: 0.2.5
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,25 @@
 ### PyFlowline
 
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models. 
 
-PyFlowline is mesh independent, meaning you can apply it to both structured (e.g., traditional rectangle mesh, latitude-longitude, hexagon) and unstructured mesh systems (e.g., Triangulated Irregular Network (TIN) mesh and Model for Prediction Across Scales (MPAS) mesh).
+PyFlowline is mesh independent, meaning you can apply it to both structured 
+
+1. traditional rectangle mesh 
+2. latitude-longitude 
+3. hexagon
+4. dggs ([dggrid](https://github.com/sahrk/DGGRID))
+
+and unstructured mesh systems 
+
+1. Model for Prediction Across Scales mesh ([MPAS](https://github.com/MPAS-Dev))
+2. Triangulated Irregular Network (TIN) mesh
 
 This package generates the mesh cell-based conceptual river networks using the following steps:
 
 1. `Flowline simplification`: PyFlowline checks the vector dataset and corrects undesired flowlines, such as braided rivers.
 2. `Mesh generation`: PyFlowline generates structured meshes (e.g., rectangle, hexagon) or imports user-provided unstructured meshes into the PyFlowline-compatible GEOJSON format.
 3. `Topological relationship reconstruction`: PyFlowline reconstructs the topological relationship using the mesh and flowline intersections.
 
@@ -49,14 +59,15 @@
 4. `shapely`
 
 PyFlowline also has three optional dependency packages
 
 1. `cython` for performance 
 2. `matplotlin` for visualization
 3. `cartopy` for visulization
+4. `simplekml` for Google Earth KML support
 
 ### Quickstart
 
 Please refer to the [quickstart documentation](https://pyflowline.readthedocs.io/en/latest/quickstart.html) for details on how to get started using the PyFlowline package.
 
 ### Installation
 
@@ -66,14 +77,16 @@
 
 We provide several examples in the `examples` folder to demonstrate the model capability. We also recommend starting with the `notebooks/mpas_example.ipynb` notebook, after following the Quickstart and Installation instructions.
 
 ### Acknowledgment
 
 This work was supported by the Earth System Model Development program areas of the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research as part of the multi-program, collaborative Integrated Coastal Modeling (ICoM) project and the Interdisciplinary Research for Arctic Coastal Environments (InteRFACE) project.
 
+This research was supported as part of the Next Generation Ecosystem Experiments-Tropics, funded by the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research at Pacific Northwest National Laboratory. The study was also partly supported by U.S. Department of Energy Office of Science Biological and Environmental Research through the Earth and Environmental System Modeling program as part of the Energy Exascale Earth System Model (E3SM) project.
+
 ### License
 
 BSD 3-Clause License
 
 Copyright © 2022, Battelle Memorial Institute
 
 1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software and may permit others to do so, subject to the following conditions:
```

### Comparing `pyflowline-0.2.4/README.md` & `pyflowline-0.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 ### PyFlowline
 
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models. 
 
-PyFlowline is mesh independent, meaning you can apply it to both structured (e.g., traditional rectangle mesh, latitude-longitude, hexagon) and unstructured mesh systems (e.g., Triangulated Irregular Network (TIN) mesh and Model for Prediction Across Scales (MPAS) mesh).
+PyFlowline is mesh independent, meaning you can apply it to both structured 
+
+1. traditional rectangle mesh 
+2. latitude-longitude 
+3. hexagon
+4. dggs ([dggrid](https://github.com/sahrk/DGGRID))
+
+and unstructured mesh systems 
+
+1. Model for Prediction Across Scales mesh ([MPAS](https://github.com/MPAS-Dev))
+2. Triangulated Irregular Network (TIN) mesh
 
 This package generates the mesh cell-based conceptual river networks using the following steps:
 
 1. `Flowline simplification`: PyFlowline checks the vector dataset and corrects undesired flowlines, such as braided rivers.
 2. `Mesh generation`: PyFlowline generates structured meshes (e.g., rectangle, hexagon) or imports user-provided unstructured meshes into the PyFlowline-compatible GEOJSON format.
 3. `Topological relationship reconstruction`: PyFlowline reconstructs the topological relationship using the mesh and flowline intersections.
 
@@ -24,14 +34,15 @@
 4. `shapely`
 
 PyFlowline also has three optional dependency packages
 
 1. `cython` for performance 
 2. `matplotlin` for visualization
 3. `cartopy` for visulization
+4. `simplekml` for Google Earth KML support
 
 ### Quickstart
 
 Please refer to the [quickstart documentation](https://pyflowline.readthedocs.io/en/latest/quickstart.html) for details on how to get started using the PyFlowline package.
 
 ### Installation
 
@@ -41,14 +52,16 @@
 
 We provide several examples in the `examples` folder to demonstrate the model capability. We also recommend starting with the `notebooks/mpas_example.ipynb` notebook, after following the Quickstart and Installation instructions.
 
 ### Acknowledgment
 
 This work was supported by the Earth System Model Development program areas of the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research as part of the multi-program, collaborative Integrated Coastal Modeling (ICoM) project and the Interdisciplinary Research for Arctic Coastal Environments (InteRFACE) project.
 
+This research was supported as part of the Next Generation Ecosystem Experiments-Tropics, funded by the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research at Pacific Northwest National Laboratory. The study was also partly supported by U.S. Department of Energy Office of Science Biological and Environmental Research through the Earth and Environmental System Modeling program as part of the Energy Exascale Earth System Model (E3SM) project.
+
 ### License
 
 BSD 3-Clause License
 
 Copyright © 2022, Battelle Memorial Institute
 
 1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software and may permit others to do so, subject to the following conditions:
```

### Comparing `pyflowline-0.2.4/docs/Makefile` & `pyflowline-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/after_loop.png` & `pyflowline-0.2.5/docs/figures/after_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/after_merge.png` & `pyflowline-0.2.5/docs/figures/after_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/basic_element.png` & `pyflowline-0.2.5/docs/figures/basic_element.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/before_loop.png` & `pyflowline-0.2.5/docs/figures/before_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/before_merge.png` & `pyflowline-0.2.5/docs/figures/before_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/data_mode.png` & `pyflowline-0.2.5/docs/figures/data_mode.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/disconnect_flowline.png` & `pyflowline-0.2.5/docs/figures/disconnect_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/find_vertex.png` & `pyflowline-0.2.5/docs/figures/find_vertex.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/flow_direction.png` & `pyflowline-0.2.5/docs/figures/flow_direction.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/flow_direction_matrix.png` & `pyflowline-0.2.5/docs/figures/flow_direction_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/hexagon.png` & `pyflowline-0.2.5/docs/figures/hexagon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/hexagon_intersect.png` & `pyflowline-0.2.5/docs/figures/hexagon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/lat_lon.png` & `pyflowline-0.2.5/docs/figures/lat_lon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/lat_lon_intersect.png` & `pyflowline-0.2.5/docs/figures/lat_lon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/merge_flowline.png` & `pyflowline-0.2.5/docs/figures/merge_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/meshes.png` & `pyflowline-0.2.5/docs/figures/meshes.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/remove_loop.png` & `pyflowline-0.2.5/docs/figures/remove_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/remove_loop_matrix.png` & `pyflowline-0.2.5/docs/figures/remove_loop_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/simplification01.png` & `pyflowline-0.2.5/docs/figures/simplification01.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/small_river.png` & `pyflowline-0.2.5/docs/figures/small_river.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/sqaure_intersect.png` & `pyflowline-0.2.5/docs/figures/sqaure_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/square.png` & `pyflowline-0.2.5/docs/figures/square.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/structure_pyflowline.png` & `pyflowline-0.2.5/docs/figures/structure_pyflowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/figures/workflow.png` & `pyflowline-0.2.5/docs/figures/workflow.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/make.bat` & `pyflowline-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/algorithm/algorithm.rst` & `pyflowline-0.2.5/docs/source/algorithm/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/api/api.rst` & `pyflowline-0.2.5/docs/source/api/api.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/application/application.rst` & `pyflowline-0.2.5/docs/source/application/application.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/conf.py` & `pyflowline-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/data/data.rst` & `pyflowline-0.2.5/docs/source/data/data.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/faq.rst` & `pyflowline-0.2.5/docs/source/faq.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
    Because the `GDAL` library is used by this project and the `proj` library is often not configured correctly automatically. 
    On Linux or Mac, you can set it up using the `.bash_profile` such as:
 
    Anaconda:
 
    `export PROJ_LIB=/people/user/.conda/envs/hexwatershed/share/proj`
+   
    `export PROJ_LIB=$HOME/opt/anaconda3/envs/pyflowline/share/proj`
 
    Miniconda:
 
    `export PROJ_LIB=/opt/miniconda3/envs/hexwatershed/share/proj`
 
 4. I am getting errors using the plot functions
```

### Comparing `pyflowline-0.2.4/docs/source/glossary.rst` & `pyflowline-0.2.5/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/index.rst` & `pyflowline-0.2.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/docs/source/installation/installation.rst` & `pyflowline-0.2.5/docs/source/installation/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,12 @@
 
 PyFlowline only provides experimental support for visualization through the optional `matplotlib` and `cartopy` packages.
 
 You need to manually speicify these packages during the installation process
 
     conda install -c conda-forge pyflowline matplotlib cartopy
 
-"""
-
 or install manually after the installation of PyFlowline:
 
     conda install -c conda-forge matplotlib cartopy
```

### Comparing `pyflowline-0.2.4/docs/source/quickstart.rst` & `pyflowline-0.2.5/docs/source/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 
 Users can run a PyFlowline simulation in the following steps:
 
 1. Create a new Python environment using Conda, and activate the new environment.
 2. Install the package using `conda install -c conda-forge pyflowline`. Conda will automatically install all the required dependencies.
 3. Clone the latest PyFlowline repository from https://github.com/changliao1025/pyflowline. 
 4. Download the additional large MPAS mesh file `lnd_cull_mesh.nc` from https://github.com/changliao1025/pyflowline/releases/tag/0.2.0 and move it under the `data/susquehanna/input` folder.
-5. Open the `examples/susquehanna/pyflowline_susquehanna_mpas.json` file and change `sWorkspace_output` to the full path to the directory where you want to save the output (e.g. `/full/path/to/pyflowline/data/susquehanna/output`), change `"sFilename_mesh_netcdf"` to the full path to `lnd_cull_mesh.nc`, `"sFilename_mesh_boundary"` to the full path to `data/susquehanna/input/mesh_boundary_buffer.geojson`, and `"sFilename_basins"` to the full path to `examples/susquehanna/pyflowline_susquehanna_basins.json`.
+5. Open the `examples/susquehanna/pyflowline_susquehanna_mpas.json` file and change `sWorkspace_output` to the full path to the directory where you want to save the output (e.g. `/full/path/to/pyflowline/data/susquehanna/output`), change `"sFilename_mesh_netcdf"` to the full path to `lnd_cull_mesh.nc`, `"sFilename_mesh_boundary"` to the full path to `data/susquehanna/input/boundary_wgs.geojson`, and `"sFilename_basins"` to the full path to `examples/susquehanna/pyflowline_susquehanna_basins.json`.
 6. Open the `examples/susquehanna/pyflowline_susquehanna_basins.json` file and change `"sFilename_flowline_filter"` to the full path to `data/susquehanna/input/flowline.geojson`. Ignore the other settings in these json files for now.
 7. Open the preferred Python IDE (Visual Studio Code recommended) and run the  `examples/susquehanna/run_simulation_mpas.py` Python script. Optionally, you can also run the `notebooks/mpas_example.ipynb` notebook.
+The visualization of the model outputs is only experimental, and you can use other tools to visualize the model outputs.
 8. You should produce a list of model outputs in the `data/susquehanna/output` folder or the user-specified output folder.
 
 If you encounter any issues, refer to the FAQ or submit a GitHub issue (https://github.com/changliao1025/pyflowline/issues).
```

### Comparing `pyflowline-0.2.4/examples/create_model_condfiguration.py` & `pyflowline-0.2.5/examples/create_model_condfiguration.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py` & `pyflowline-0.2.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/check_head_water.py` & `pyflowline-0.2.5/pyflowline/algorithms/auxiliary/check_head_water.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_index_in_list.py` & `pyflowline-0.2.5/pyflowline/algorithms/auxiliary/find_index_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py` & `pyflowline-0.2.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py` & `pyflowline-0.2.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/direction/correct_flowline_direction.py` & `pyflowline-0.2.5/pyflowline/algorithms/direction/correct_flowline_direction.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_order.py` & `pyflowline-0.2.5/pyflowline/algorithms/index/define_stream_order.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py` & `pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py` & `pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py` & `pyflowline-0.2.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/loop/remove_flowline_loop.py` & `pyflowline-0.2.5/pyflowline/algorithms/loop/remove_flowline_loop.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/merge/merge_flowline.py` & `pyflowline-0.2.5/pyflowline/algorithms/merge/merge_flowline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 import importlib
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
+
 lID = 0
+
 def merge_flowline(aFlowline_in, aVertex_in, \
     pVertex_outlet_in, \
         aIndex_headwater_in,\
             aIndex_middle_in, \
                 aIndex_confluence_in ):
 
     nVertex=len(aVertex_in)
```

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_returning_flowline.py` & `pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_returning_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_small_river.py` & `pyflowline-0.2.5/pyflowline/algorithms/simplification/remove_small_river.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_confluence.py` & `pyflowline-0.2.5/pyflowline/algorithms/split/find_flowline_confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_vertex.py` & `pyflowline-0.2.5/pyflowline/algorithms/split/find_flowline_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/split/split_by_length.py` & `pyflowline-0.2.5/pyflowline/algorithms/split/split_by_length.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline.py` & `pyflowline-0.2.5/pyflowline/algorithms/split/split_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline_to_edge.py` & `pyflowline-0.2.5/pyflowline/algorithms/split/split_flowline_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/_hpc.py` & `pyflowline-0.2.5/pyflowline/classes/_hpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,19 +79,24 @@
     ofs.write(sLine)
     sLine = '#SBATCH -e stderr.err\n'
     ofs.write(sLine)    
     sLine = 'module purge\n'
     ofs.write(sLine)
     sLine = 'module load gcc/8.1.0' + '\n'
     ofs.write(sLine)
+    
+    if self.iFlag_dggrid ==1:
+        sLine = 'module load gdal/2.3.1' + '\n'
+        ofs.write(sLine)
+
     sLine = 'module load anaconda3/2019.03' + '\n'
     ofs.write(sLine)
     sLine = 'source /share/apps/anaconda3/2019.03/etc/profile.d/conda.sh' + '\n'
     ofs.write(sLine)    
-    sLine = 'conda activate pyflowline' + '\n'
+    sLine = 'conda activate hexwatershed' + '\n'
     ofs.write(sLine)
     sLine = 'cd $SLURM_SUBMIT_DIR\n'
     ofs.write(sLine)
     sLine = 'JOB_DIRECTORY='+ self.sWorkspace_output +  '\n'
     ofs.write(sLine)
     sLine = 'cd $JOB_DIRECTORY' +  '\n'
     ofs.write(sLine)
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/_visual.py` & `pyflowline-0.2.5/pyflowline/classes/_visual.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,227 @@
 import os
-import json
 #dependency packages
-import numpy as np
-
-from pyflowline.external.pyearth.toolbox.reader.text_reader_string import text_reader_string
-
 from pyflowline.external.pyearth.visual.map.map_vector_polygon_data import map_vector_polygon_data
 from pyflowline.external.pyearth.visual.map.map_vector_polyline_data import map_vector_polyline_data
 from pyflowline.external.pyearth.visual.map.map_multiple_vector_data import map_multiple_vector_data
 
 #plot function
-def plot(self, sFilename_output_in=None,iFlag_title = None, sVariable_in=None, aExtent_in = None):
-    if sVariable_in == 'mesh':
-        self._plot_mesh(sFilename_output_in=sFilename_output_in, aExtent_in = aExtent_in)
+def plot(self,
+         iFlag_type_in = None,
+         iFlag_title_in = None,
+         sFilename_output_in = None,
+         sVariable_in = None,
+         aExtent_in = None,
+         pProjection_map_in = None):
+    """_summary_
+
+    Args:
+        iFlag_type_in (_type_, optional): _description_. Defaults to None.
+        iFlag_title_in (_type_, optional): _description_. Defaults to None.
+        sFilename_output_in (_type_, optional): _description_. Defaults to None.
+        sVariable_in (_type_, optional): _description_. Defaults to None.
+        aExtent_in (_type_, optional): _description_. Defaults to None.
+        pProjection_map_in (_type_, optional): _description_. Defaults to None.
+    """
+
+    if iFlag_type_in is None:
+        iFlag_type_in = 2 #polyline based, only flowline
+
+    if iFlag_title_in is None:
+        iFlag_title_in = 1
+
+    if sVariable_in is None:
+        sVariable_in = 'flowline_conceptual'
     else:
-        if sVariable_in == 'overlap':
-            self._plot_mesh_with_flowline( sFilename_output_in=sFilename_output_in, iFlag_title= iFlag_title, aExtent_in=aExtent_in)
+        if sVariable_in == 'mesh': 
+            iFlag_type_in = 3
         else:
+            if sVariable_in == 'overlap':
+                iFlag_type_in = 4
+    
+
+    if iFlag_type_in == 1: #point based, such as dam
+        #currently, this feature is not supported
+        pass
+    else:
+        if iFlag_type_in == 2:
+            #polyline based, only flowline
             for pBasin in self.aBasin:
                 pBasin.basin_plot(self.iCase_index,
                                   self.iMesh_type,
                                   self.sMesh_type,
-                                  sFilename_output_in=sFilename_output_in,                                 
+                                  iFlag_title_in= iFlag_title_in,
+                                  sFilename_output_in=sFilename_output_in,
                                   sVariable_in= sVariable_in,
-                                  aExtent_in=aExtent_in)
-            pass
+                                  aExtent_in=aExtent_in,
+                                  pProjection_map_in = pProjection_map_in)
+        else:
+            if iFlag_type_in == 3: #polygon based
+                if sVariable_in == 'mesh':
+                    self._plot_mesh(sFilename_output_in=sFilename_output_in,
+                                    aExtent_in = aExtent_in,
+                                    pProjection_map_in = pProjection_map_in)
+
+            else:
+                if iFlag_type_in == 4: #mixed based mesh + flowline
+                    if sVariable_in == 'overlap':
+                        self._plot_mesh_with_flowline(sFilename_output_in=sFilename_output_in,
+                                                      iFlag_title_in= iFlag_title_in,
+                                                      aExtent_in=aExtent_in,
+                                                      pProjection_map_in = pProjection_map_in)
 
-    return
 
-#this function is used to plot the study area
-def _plot_study_area(self, sFilename_boundary_in = None, sFilename_slope_in = None, sFilename_nhd_in = None):
-    return
+
+                    pass
+                else:
+                    pass
+
+        return
 
 def _plot_mesh(self, sFilename_output_in=None, aExtent_in=None, pProjection_map_in = None):
 
-    sFilename_in = self.sFilename_mesh
+    sFilename_in = self.sFilename_mesh 
     sMesh_type = self.sMesh_type
 
-    map_vector_polygon_data(sFilename_in, sFilename_output_in=sFilename_output_in, sTitle_in= sMesh_type)
-
+    map_vector_polygon_data(sFilename_in,
+                            sFilename_output_in = sFilename_output_in,
+                            sTitle_in = sMesh_type,
+                            aExtent_in = aExtent_in,
+                            pProjection_map_in = pProjection_map_in)
 
     return
 
-
 #plot both polygon and polyline
-def _plot_mesh_with_flowline(self, 
-                             sFilename_output_in=None, 
-                             iFlag_title=None, 
-                             aExtent_in=None, 
+def _plot_mesh_with_flowline(self,
+                             sFilename_output_in=None,
+                             iFlag_title_in=None,
+                             aExtent_in=None,
                              pProjection_map_in = None):
 
     aFiletype_in = list()
     aFilename_in = list()
+    aFlag_color = list()
     aFilename_in.append(self.sFilename_mesh)
-    aFiletype_in.append(1)
+    aFiletype_in.append(3)
+    aFlag_color.append(0)
 
     for pBasin in self.aBasin:
         aFiletype_in.append(2)
         dummy = pBasin.sFilename_flowline_conceptual
         sFilename_json = os.path.join(pBasin.sWorkspace_output_basin, dummy)
         aFilename_in.append(sFilename_json)
+        aFlag_color.append(1)
 
-    map_multiple_vector_data(aFiletype_in, aFilename_in, 
-                             sFilename_output_in=sFilename_output_in, 
+    map_multiple_vector_data(aFiletype_in,
+                             aFilename_in,
+                             sFilename_output_in=sFilename_output_in,
                              sTitle_in= 'Mesh with flowline',
-                             aFlag_color_in=[0, 1])
-    return
-
-#this is a reserved function
-def _compare_with_raster_dem_method(self, sFilename_dem_flowline, sFilename_in, aExtent_in=None, pProjection_map_in = None):
-
+                             aFlag_color_in=aFlag_color,
+                             aExtent_in = aExtent_in,
+                             pProjection_map_in = pProjection_map_in)
     return
 
 def basin_plot(self,
                iCase_index,
                iMesh_type,
                sMesh_type,
                sFilename_output_in=None,
                iFlag_title_in=None,
                sVariable_in=None,
                aExtent_in = None,
                pProjection_map_in = None):
-    #docstring for basin_plot
-           
+    """_summary_
+
+    Args:
+        iCase_index (_type_): _description_
+        iMesh_type (_type_): _description_
+        sMesh_type (_type_): _description_
+        sFilename_output_in (_type_, optional): _description_. Defaults to None.
+        iFlag_title_in (_type_, optional): _description_. Defaults to None.
+        sVariable_in (_type_, optional): _description_. Defaults to None.
+        aExtent_in (_type_, optional): _description_. Defaults to None.
+        pProjection_map_in (_type_, optional): _description_. Defaults to None.
+    """
+
+
     iFlag_label = 0
     sWorkspace_output_basin = self.sWorkspace_output_basin
     if sVariable_in is not None:
         if sVariable_in == 'flowline_raw':
             sFilename_json = self.sFilename_flowline_raw
             sTitle = 'Original flowline'
             iFlag_color = 0
         else:
             if sVariable_in == 'flowline_filter':
                 sFilename_json = self.sFilename_flowline_filter
                 sTitle = 'Filtered flowline'
                 iFlag_color = 0
             else:
                 if sVariable_in == 'flowline_simplified':
-                    sFilename_out = self.sFilename_flowline_simplified
-                    sFilename_json = os.path.join(sWorkspace_output_basin, sFilename_out)
+                    sFilename_json = self.sFilename_flowline_simplified                    
                     sTitle = 'Simplified flowline'
                     iFlag_color = 1
                     if aExtent_in is None:
                         iFlag_label = 1
                     else:
                         iFlag_label=0
                 else:
                     if sVariable_in == 'flowline_conceptual':
-                        sFilename_out = self.sFilename_flowline_conceptual
-                        sFilename_json = os.path.join(sWorkspace_output_basin, sFilename_out)
+                        sFilename_json = self.sFilename_flowline_conceptual                        
                         sTitle = 'Conceptual flowline'
                         iFlag_color = 1
                         if aExtent_in is None:
                             iFlag_label = 1
                         else:
                             iFlag_label=0
                     else:
                         if sVariable_in == 'aof':
-                            sFilename_out = 'area_of_difference.geojson'
-                            sFilename_json = os.path.join(sWorkspace_output_basin, sFilename_out)
+                            sFilename_json = self.sFilename_area_of_difference                            
                             sTitle = 'Conceptual flowline'
                             iFlag_label = 1
-                            self.plot_area_of_difference(iCase_index, 
-                                                         iMesh_type, 
-                                                         sMesh_type, 
-                                                         sFilename_output_in, 
+                            self.plot_area_of_difference(iCase_index,
+                                                         iMesh_type,
+                                                         sMesh_type,
+                                                         sFilename_output_in,
                                                          aExtent_in = aExtent_in)
                             return
                         else:
+                            print('Unsupported variable: ', sVariable_in, ' in basin_plot.')
                             pass
                 pass
     else:
         #default
         sFilename_json = self.sFilename_flowline_conceptual
 
 
-    map_vector_polyline_data(sFilename_json, 
-                             sFilename_output_in,                       
-                             iFlag_thickness_in=0  , 
-                             sTitle_in=sTitle, 
+    map_vector_polyline_data(sFilename_json,
+                             sFilename_output_in= sFilename_output_in,
+                             iFlag_title_in=iFlag_title_in,
+                             iFlag_thickness_in=0  ,
+                             sTitle_in=sTitle,
                              iFlag_color_in= iFlag_color,
-                             iFlag_label_in=iFlag_label, 
-                             aExtent_in = aExtent_in, 
-                             pProjection_map_in = pProjection_map_in)    
+                             iFlag_label_in=iFlag_label,
+                             aExtent_in = aExtent_in,
+                             pProjection_map_in = pProjection_map_in)
+
+    return
 
+#this function is used to plot the study area
+def _plot_study_area(self, sFilename_boundary_in = None, sFilename_slope_in = None, sFilename_nhd_in = None):
     return
 
+#this is a reserved function
+def _compare_with_raster_dem_method(self, sFilename_dem_flowline, sFilename_in, aExtent_in=None, pProjection_map_in = None):
 
+    return
 
 #this is a reserved function
 def _plot_area_of_difference(self, iCase_index, iMesh_type, sMesh_type, sFilename_figure_in, aExtent_in = None, pProjection_map_in = None):
 
-    sFilename_json = self.sFilename_area_of_difference
-    sFilename_json = os.path.join(self.sWorkspace_output_basin, sFilename_json)
+    sFilename_json = self.sFilename_area_of_difference    
 
     sFilename_in = self.sFilename_mesh
     sFilename_out = sFilename_figure_in
 
     map_vector_polygon_data(1, sFilename_in, sFilename_out, 'cell')
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/basin.py` & `pyflowline-0.2.5/pyflowline/classes/basin.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from pyflowline.formats.read_nhdplus_flowline_shapefile import extract_nhdplus_flowline_shapefile_by_attribute
 from pyflowline.formats.read_nhdplus_flowline_shapefile import track_nhdplus_flowline
 from pyflowline.formats.convert_flowline_to_geojson import convert_flowline_to_geojson
 from pyflowline.formats.export_flowline import export_flowline_to_geojson
 from pyflowline.formats.export_vertex import export_vertex_to_geojson
 from pyflowline.external.pyearth.toolbox.reader.text_reader_string import text_reader_string
 
-
-
 from pyflowline.algorithms.split.find_flowline_vertex import find_flowline_vertex
 from pyflowline.algorithms.split.find_flowline_confluence import find_flowline_confluence
 from pyflowline.algorithms.split.split_flowline import split_flowline
 from pyflowline.algorithms.split.split_flowline_to_edge import split_flowline_to_edge
 from pyflowline.algorithms.split.split_by_length import split_flowline_by_length
 from pyflowline.algorithms.merge.merge_flowline import merge_flowline
 from pyflowline.algorithms.direction.correct_flowline_direction import correct_flowline_direction
@@ -113,21 +111,35 @@
     sFilename_flowline_conceptual=''
     sFilename_flowline_edge=''
     sFilename_basin_info=''
     sFilename_flowline_simplified_info=''
     sFilename_flowline_conceptual_info=''
     sFilename_confluence_simplified_info=''
     sFilename_confluence_conceptual_info=''    
+
     aFlowline_basin_filtered=None
     aFlowline_basin_simplified=None
     aFlowline_basin_conceptual=None    
     pVertex_outlet=None
     aConfluence_basin_simplified= None
     aConfluence_basin_conceptual= None
 
+    #json
+    sFilename_hexwatershed_json=''
+    sFilename_stream_edge_json =''
+
+    #geojson for hexwatershed compatibility
+    sFilename_elevation=''
+    sFilename_slope=''
+    sFilename_drainage_area=''
+    sFilename_flow_direction ='' 
+    sFilename_distance_to_outlet = ''
+    sFilename_stream_segment=''
+    sFilename_stream_edge=''
+
     
     iFlag_visual = importlib.util.find_spec("cartopy") 
     if iFlag_visual is not None:
         from ._visual import basin_plot
         from ._visual import _plot_area_of_difference 
     else:
         pass
@@ -190,64 +202,77 @@
             self.sFilename_flowline_raw = aParameter['sFilename_flowline_raw']
         else:
             self.sFilename_flowline_raw   = ''
        
         if 'sFilename_flowline_filter' in aParameter:
             self.sFilename_flowline_filter = aParameter['sFilename_flowline_filter']
         else:
-            self.sFilename_flowline_filter   = ''
+            self.sFilename_flowline_filter = ''
 
         if 'sWorkspace_output_basin' in aParameter:
             self.sWorkspace_output_basin = aParameter['sWorkspace_output_basin']
         else:
-            self.sWorkspace_output_basin   = '.'
+            self.sWorkspace_output_basin = '.'
             
         Path(self.sWorkspace_output_basin).mkdir(parents=True, exist_ok=True)
 
         self.sFilename_flowline_filter_geojson = os.path.join(str(self.sWorkspace_output_basin ), "flowline_filter.geojson"  )
 
         if 'sFilename_dam' in aParameter:
             self.sFilename_dam = aParameter['sFilename_dam']
         else:
-            self.sFilename_dam   = ''
+            self.sFilename_dam  = ''
 
         if 'sFilename_flowline_topo' in aParameter:
             self.sFilename_flowline_topo = aParameter['sFilename_flowline_topo']
         else:
-            self.sFilename_flowline_topo   =''
+            self.sFilename_flowline_topo = ''
 
         self.sBasinID  = "{:08d}".format(self.lBasinID)
 
-
         if not os.path.isfile(self.sFilename_flowline_filter):
             print("The filtered flowline file does not exist!")
             exit
         if self.iFlag_dam==1:
             if not os.path.isfile(self.sFilename_flowline_raw):
                 print("The raw flowline file does not exist!")
                 exit
             if not os.path.isfile(self.sFilename_flowline_topo):
                 print("The flowline topology file does not exist!")
                 exit
             pass
 
-        #geojson
-        self.sFilename_flowline_segment_index_before_intersect = 'flowline_segment_index_before_intersect.geojson'
-        self.sFilename_flowline_simplified = 'flowline_simplified.geojson'
-        self.sFilename_flowline_split = 'flowline_split.geojson'
-        self.sFilename_flowline_intersect  = 'flowline_intersect_mesh.geojson'
-        self.sFilename_flowline_conceptual = 'flowline_conceptual.geojson'
-        self.sFilename_flowline_edge = 'flowline_edge.geojson'
-        self.sFilename_area_of_difference = 'area_of_difference.geojson'
-
-        self.sFilename_basin_info = 'basin_info.json'
-        self.sFilename_flowline_conceptual_info = 'flowline_conceptual_info.json'
-        self.sFilename_flowline_simplified_info = 'flowline_simplified_info.json'
-        self.sFilename_confluence_conceptual_info = 'confluence_conceptual_info.json'
-        self.sFilename_confluence_simplified_info = 'confluence_simplified_info.json'
+        #json
+        self.sFilename_hexwatershed_json = os.path.join(str(self.sWorkspace_output_basin ), "watershed.json" )
+        self.sFilename_stream_edge_json = os.path.join(str(self.sWorkspace_output_basin ), 'stream_edge.json')
+        self.sFilename_basin_info = os.path.join(str(self.sWorkspace_output_basin ), 'basin_info.json')
+        self.sFilename_flowline_conceptual_info = os.path.join(str(self.sWorkspace_output_basin ), 'flowline_conceptual_info.json')
+        self.sFilename_flowline_simplified_info = os.path.join(str(self.sWorkspace_output_basin ), 'flowline_simplified_info.json')
+        self.sFilename_confluence_conceptual_info = os.path.join(str(self.sWorkspace_output_basin ),'confluence_conceptual_info.json')
+        self.sFilename_confluence_simplified_info = os.path.join(str(self.sWorkspace_output_basin ),'confluence_simplified_info.json')
+        
+        #geojson, full path of the file
+        #full paths are required for the following files
+        #for hexwatershed compatibility, the geojson files will be generated by the pyhexwatershed front end
+        self.sFilename_flowline_segment_index_before_intersect = os.path.join(str(self.sWorkspace_output_basin ),'flowline_segment_index_before_intersect.geojson')
+        self.sFilename_flowline_simplified = os.path.join(str(self.sWorkspace_output_basin ),'flowline_simplified.geojson')
+        self.sFilename_flowline_split = os.path.join(str(self.sWorkspace_output_basin ),'flowline_split.geojson')
+        self.sFilename_flowline_intersect  = os.path.join(str(self.sWorkspace_output_basin ),'flowline_intersect_mesh.geojson')
+        self.sFilename_flowline_conceptual = os.path.join(str(self.sWorkspace_output_basin ),'flowline_conceptual.geojson')
+        self.sFilename_flowline_edge = os.path.join(str(self.sWorkspace_output_basin ),'flowline_edge.geojson')
+        self.sFilename_area_of_difference = os.path.join(str(self.sWorkspace_output_basin ),'area_of_difference.geojson')
+         
+        self.sFilename_elevation = os.path.join(str(self.sWorkspace_output_basin ), "elevation.geojson" )
+        self.sFilename_slope = os.path.join(str(self.sWorkspace_output_basin ), "slope.geojson" )
+        self.sFilename_drainage_area =  os.path.join(str(self.sWorkspace_output_basin ), "drainage_area.geojson" )
+        self.sFilename_flow_direction = os.path.join(str(self.sWorkspace_output_basin ), "flow_direction.geojson" )
+        self.sFilename_distance_to_outlet = os.path.join(str(self.sWorkspace_output_basin ), "distance_to_outlet.geojson" )
+        self.sFilename_stream_edge = os.path.join(str(self.sWorkspace_output_basin ), "stream_edge.geojson" )
+        self.sFilename_stream_segment = os.path.join(str(self.sWorkspace_output_basin ), "stream_segment.geojson" )
+        
         return
         
     def flowline_simplification(self):
         """
         Run the basin flowline simplification
 
         Returns:
@@ -481,33 +506,31 @@
         
 
         #build segment index
         ptimer.start()
         aFlowline_basin_simplified, aStream_segment = define_stream_segment_index(aFlowline_basin_simplified)
         ptimer.stop()
         if self.iFlag_debug ==1:
-            sFilename_out = self.sFilename_flowline_segment_index_before_intersect
-            sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
+            sFilename_out = self.sFilename_flowline_segment_index_before_intersect            
             export_flowline_to_geojson(  aFlowline_basin_simplified, sFilename_out, \
                 aAttribute_data=[aStream_segment], aAttribute_field=['iseg'], aAttribute_dtype=['int'])
         #build stream order 
         ptimer.start()
         aFlowline_basin_simplified, aStream_order = define_stream_order(aFlowline_basin_simplified)
         ptimer.stop()
-        sFilename_out = self.sFilename_flowline_simplified
-        sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
+        sFilename_out = self.sFilename_flowline_simplified        
         export_flowline_to_geojson(  aFlowline_basin_simplified, sFilename_out, \
                 aAttribute_data=[aStream_segment, aStream_order], aAttribute_field=['iseg','iord'], aAttribute_dtype=['int','int'])
         
         if self.iFlag_break_by_distance==1:
             ptimer.start()
             aFlowline_basin_simplified_split = split_flowline_by_length(aFlowline_basin_simplified, self.dThreshold_break_by_distance)
             ptimer.stop()
+          
             sFilename_out = self.sFilename_flowline_split
-            sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             export_flowline_to_geojson(  aFlowline_basin_simplified_split, sFilename_out  )
 
         self.aFlowline_basin_simplified= aFlowline_basin_simplified
         print('Finish flowline simplification:',  self.sBasinID)
         sys.stdout.flush()
         return aFlowline_basin_simplified
 
@@ -523,23 +546,21 @@
             list [pyflowline]: A list of intersected cells
         """
         print('Start topology reconstruction:',  self.sBasinID)
         
         ptimer = pytimer()
         
         sWorkspace_output_basin = self.sWorkspace_output_basin
-        sFilename_flowline = self.sFilename_flowline_simplified
-        sFilename_flowline_in = os.path.join(sWorkspace_output_basin, sFilename_flowline)
+        sFilename_flowline_in = self.sFilename_flowline_simplified
+        sFilename_flowline_intersect_out = self.sFilename_flowline_intersect
 
-                
-        sFilename_flowline_intersect = self.sFilename_flowline_intersect
-        sFilename_flowline_intersect_out = os.path.join(sWorkspace_output_basin, sFilename_flowline_intersect)
         ptimer.start()
         aCell, aCell_intersect_basin, aFlowline_intersect_all = intersect_flowline_with_mesh(iMesh_type, sFilename_mesh, \
             sFilename_flowline_in, sFilename_flowline_intersect_out)
+        
         ptimer.stop()
         sys.stdout.flush()
         
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_intersect_flowline_with_mesh.geojson'
             sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)  
             export_flowline_to_geojson(aFlowline_intersect_all,  sFilename_out)
@@ -608,22 +629,23 @@
         else:
             #there is no confluence
             pass
           
 
         #edge based
         aFlowline_basin_edge, aEdge = split_flowline_to_edge(aFlowline_basin_conceptual)
-        sFilename_out = self.sFilename_flowline_edge
-        sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
+        sFilename_out = self.sFilename_flowline_edge    
         export_flowline_to_geojson(  aFlowline_basin_edge, sFilename_out)
-
+      
         sFilename_out = self.sFilename_flowline_conceptual
-        sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
-        export_flowline_to_geojson(  aFlowline_basin_conceptual, sFilename_out, \
-            aAttribute_data=[aStream_segment, aStream_order], aAttribute_field=['iseg','iord'], aAttribute_dtype=['int','int'])
+        export_flowline_to_geojson(  aFlowline_basin_conceptual, 
+                                   sFilename_out, 
+            aAttribute_data=[aStream_segment, aStream_order], 
+            aAttribute_field=['iseg','iord'], 
+            aAttribute_dtype=['int','int'])
 
         self.aFlowline_basin_conceptual = aFlowline_basin_conceptual     
         
         self.lCellID_outlet = lCellID_outlet
         self.dLongitude_outlet_degree = pVertex_outlet.dLongitude_degree
         self.dLatitude_outlet_degree = pVertex_outlet.dLatitude_degree
         
@@ -670,33 +692,31 @@
             self.aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter_geojson )   
             self.dLength_flowline_filtered = self.calculate_flowline_length(self.aFlowline_basin_filtered)
         
         point= dict()
         point['dLongitude_degree'] = self.dLongitude_outlet_degree
         point['dLatitude_degree'] = self.dLatitude_outlet_degree
         pVertex_outlet_initial=pyvertex(point)
-        if self.aFlowline_basin_simplified is None:
-            sFilename_flowline = self.sFilename_flowline_simplified
-            sFilename_flowline_in = os.path.join(self.sWorkspace_output_basin, sFilename_flowline)
+        if self.aFlowline_basin_simplified is None:            
+            sFilename_flowline_in = self.sFilename_flowline_simplified
             aFlowline_simplified,pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )   
         
             self.aFlowline_basin_simplified = aFlowline_simplified
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
             = find_flowline_confluence(self.aFlowline_basin_simplified,  pVertex_outlet_initial)  
             aVertex = np.array(aVertex)
             aIndex_confluence = np.array(aIndex_confluence)
             if aIndex_confluence.size > 0:        
                 aVertex_confluence = aVertex[aIndex_confluence] 
                 self.aConfluence_basin_simplified = self.build_confluence(self.aFlowline_basin_simplified, aVertex_confluence)
 
         self.dLength_flowline_simplified = self.calculate_flowline_length(self.aFlowline_basin_simplified)
 
         if self.aFlowline_basin_conceptual is None:
-            sFilename_flowline = self.sFilename_flowline_conceptual
-            sFilename_flowline_in = os.path.join(self.sWorkspace_output_basin, sFilename_flowline)
+            sFilename_flowline_in = self.sFilename_flowline_conceptual
             aFlowline_conceptual, pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )   
             self.aFlowline_basin_conceptual = aFlowline_conceptual
             
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
             = find_flowline_confluence(self.aFlowline_basin_conceptual,  pVertex_outlet_initial)  
             aVertex = np.array(aVertex)
             aIndex_confluence = np.array(aIndex_confluence)
@@ -735,15 +755,14 @@
         return
 
     def export_basin_info_to_json(self):
         """
         Export the basin basin object to json
         """
         sFilename_json = self.sFilename_basin_info
-        sFilename_json = os.path.join(str(Path(self.sWorkspace_output_basin)  ) , sFilename_json  )
 
         aSkip = ['aFlowline_basin_filtered', \
                 'aFlowline_basin_simplified','aFlowline_basin_conceptual','aConfluence_basin_simplified',
                 'aConfluence_basin_conceptual']
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
@@ -759,47 +778,44 @@
 
     def export_flowline_info_to_json(self):
         """
         Export the flowline object to json
         """
         iFlag_export_simplified=0
         if iFlag_export_simplified==1:
-            sFilename_json = self.sFilename_flowline_simplified_info
-            sFilename_json = os.path.join(str(Path(self.sWorkspace_output_basin)  ) , sFilename_json  )
+            sFilename_json = self.sFilename_flowline_simplified_info            
             with open(sFilename_json, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_simplified], indent = 4)        
                 f.write(sJson)    
                 f.close()
 
         sFilename_json = self.sFilename_flowline_conceptual_info
-        sFilename_json = os.path.join(str(Path(self.sWorkspace_output_basin)  ) , sFilename_json  )
-
-        
+     
         with open(sFilename_json, 'w', encoding='utf-8') as f:
             sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_conceptual], indent = 4)        
             f.write(sJson)    
             f.close()
         return
 
     def export_confluence_info_to_json(self):
         """
         Export the confluence object to json
         """
         #iFlag_export_confluence =0
         if self.aConfluence_basin_simplified is not None:
             sFilename_json = self.sFilename_confluence_simplified_info
-            sFilename_json = os.path.join(str(Path(self.sWorkspace_output_basin)  ) , sFilename_json  )
+  
             with open(sFilename_json, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_simplified], indent = 4)        
                 f.write(sJson)    
                 f.close()
 
         if self.aConfluence_basin_conceptual is not None:
             sFilename_json = self.sFilename_confluence_conceptual_info
-            sFilename_json = os.path.join(str(Path(self.sWorkspace_output_basin)  ) , sFilename_json  )
+   
 
             with open(sFilename_json, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_conceptual], indent = 4)        
                 f.write(sJson)    
                 f.close()
                 
         return   
@@ -920,19 +936,19 @@
         Evaluate the model performance using area of difference
 
         Args:
             iMesh_type (int): The mesh type
             sMesh_type (str): The mesh type
         """
 
-        sFilename_simplified =  self.sFilename_flowline_simplified
-        sFilename_simplified= os.path.join(self.sWorkspace_output_basin, sFilename_simplified)
+        
+        sFilename_simplified = self.sFilename_flowline_simplified
 
+        
         sFilename_flowline_edge = self.sFilename_flowline_edge
-        sFilename_flowline_edge= os.path.join(self.sWorkspace_output_basin, sFilename_flowline_edge)
 
         #intersect first
         sFilename_output= os.path.join(self.sWorkspace_output_basin, 'flowline_intersect_flowline.json')
         aVertex_intersect = intersect_flowline_with_flowline(sFilename_simplified, sFilename_flowline_edge, sFilename_output)
 
         #get confluence simple
         point= dict()   
@@ -1010,16 +1026,15 @@
             sFilename_out = 'flowline_split_conceptual.json'
             sFilename_out = os.path.join(self.sWorkspace_output_basin, sFilename_out)  
             export_flowline_to_geojson(aFlowline_conceptual_split, sFilename_out)
             #aFlowline_conceptual_split, dummy = read_flowline_geojson(sFilename_out)
 
         aFlowline_all = aFlowline_simplified_split + aFlowline_conceptual_split
 
-        sFilename_area_of_difference = self.sFilename_area_of_difference
-        sFilename_output = os.path.join(self.sWorkspace_output_basin, sFilename_area_of_difference)
+        sFilename_output = self.sFilename_area_of_difference
         #remove headwater not needed here
 
         aPolygon_out, dArea = calculate_area_of_difference_simplified(aFlowline_all, aVertex_all, sFilename_output)
         print('Area of difference: ', dArea)
         self.dArea_of_difference = dArea
         self.dDistance_displace = dArea / self.dLength_flowline_simplified
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/confluence.py` & `pyflowline-0.2.5/pyflowline/classes/confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/edge.py` & `pyflowline-0.2.5/pyflowline/classes/edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/flowline.py` & `pyflowline-0.2.5/pyflowline/classes/flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/hexagon.py` & `pyflowline-0.2.5/pyflowline/classes/hexagon.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     aVertex=None
     aVertexID=None
     pVertex_center = None
     aFlowline=None   
     nNeighbor=-1
     nNeighbor_land=-1
     nNeighbor_ocean=-1
+    nNeighbor_land_virtual = -1
+    aNeighbor_land_virtual = None
     aNeighbor=None #the global ID of all neighbors
     aNeighbor_land=None #the global ID of all neighbors
     aNeighbor_ocean=None #the global ID of all neighbors
     aNeighbor_distance = None
 
     def __init__(self, dLon, dLat, aEdge, aVertex):
         """
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/latlon.py` & `pyflowline-0.2.5/pyflowline/classes/latlon.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     aVertex=None
     aVertexID=None
     pVertex_center = None
     aFlowline=None    
     nNeighbor=-1
     nNeighbor_land=-1
     nNeighbor_ocean=-1
+    nNeighbor_land_virtual = -1
+    aNeighbor_land_virtual = None
     aNeighbor=None #the global ID of all neighbors
     aNeighbor_land=None #the global ID of all neighbors
     aNeighbor_ocean=None #the global ID of all neighbors
     aNeighbor_distance = None
 
     def __init__(self, dLon, dLat, aEdge, aVertex):
         """
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/link.py` & `pyflowline-0.2.5/pyflowline/classes/link.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/mpas.py` & `pyflowline-0.2.5/pyflowline/classes/mpas.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,19 +64,22 @@
     iStream_segment_burned=-1
     aEdge=None
     aEdgeID=None
     aVertex=None
     aVertexID=None
     pVertex_center = None
     aFlowline=None    
-    nNeighbor=-1
+    nNeighbor=-1 
     nNeighbor_land=-1
+    nNeighbor_land_virtual = -1
+    aNeighbor_land_virtual = None
     nNeighbor_ocean=-1
-    aNeighbor=None #the global ID of all neighbors
+    aNeighbor=None #the global ID of all neighbors, execluding null
     aNeighbor_land=None #the global ID of all neighbors
+    
     aNeighbor_ocean=None #the global ID of all neighbors
     aNeighbor_distance = None
 
     def __init__(self, dLon, dLat, aEdge, aVertex):
         """
         Initilize a mpas cell object
 
@@ -92,16 +95,18 @@
             print('At lease 3 edges are required!', nEdge)
             pass
         else:                          
             self.aEdge = aEdge
             self.aVertex = aVertex #the first one and last one are the same
             self.nEdge = len(aEdge)
             self.nVertex = len(aVertex) 
+            #initialize the neighbor but without the actual neighbor information
             self.nNeighbor = -1
             self.nNeighbor_land = -1
+            self.nNeighbor_land_virtual = -1
             self.nNeighbor_ocean = -1
             self.iFlag_coast = 0      
             self.dLongitude_center_degree = dLon
             self.dLatitude_center_degree = dLat
             pVertex = dict()        
             pVertex['dLongitude_degree'] =self.dLongitude_center_degree
             pVertex['dLatitude_degree'] =self.dLatitude_center_degree
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/pycase.py` & `pyflowline-0.2.5/pyflowline/classes/pycase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,147 +1,166 @@
 import os
+import stat
 from pathlib import Path
 import json
 from json import JSONEncoder
 import datetime
 import importlib
+from shutil import copy2
 import numpy as np
-from osgeo import ogr, osr
-from shapely.wkt import loads
+from osgeo import ogr, osr, gdal
+
+from pyflowline.external.pyearth.system.define_global_variables import *
+
 from pyflowline.classes.mpas import pympas
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.square import pysquare
+from pyflowline.classes.dggrid import pydggrid
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.basin import pybasin
 from pyflowline.classes.flowline import pyflowline
 from pyflowline.classes.edge import pyedge
 from pyflowline.formats.read_mesh import read_mesh_json, read_mesh_json_w_topology
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates
 from pyflowline.external.pyearth.gis.gdal.gdal_functions  import degree_to_meter
 from pyflowline.external.pyearth.gis.gdal.gdal_functions  import meter_to_degree
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import retrieve_geotiff_metadata
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import read_mesh_boundary
+
+iFlag_kml = importlib.util.find_spec("simplekml") 
+if iFlag_kml is not None:
+    from pyflowline.external.pyearth.gis.kml.convert_geojson_to_kml import convert_geojson_to_kml
+else:
+    pass
+
 from pyflowline.mesh.hexagon.create_hexagon_mesh import create_hexagon_mesh
 from pyflowline.mesh.latlon.create_latlon_mesh import create_latlon_mesh
 from pyflowline.mesh.square.create_square_mesh import create_square_mesh
 from pyflowline.mesh.mpas.create_mpas_mesh import create_mpas_mesh
+from pyflowline.mesh.dggrid.create_dggrid_mesh import create_dggrid_mesh
 from pyflowline.mesh.tin.create_tin_mesh import create_tin_mesh
-
+gdal.UseExceptions()   
 pDate = datetime.datetime.today()
 sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
 class CaseClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, list):
-            pass  
+            pass
         if isinstance(obj, pyvertex):
             return json.loads(obj.tojson()) #lVertexID
         if isinstance(obj, pyedge):
-            return obj.lEdgeID        
+            return obj.lEdgeID
         if isinstance(obj, pyflowline):
             return obj.lFlowlineID
         if isinstance(obj, pyhexagon):
             return obj.lCellID
         if isinstance(obj, pysquare):
             return obj.lCellID
         if isinstance(obj, pylatlon):
             return obj.lCellID
         if isinstance(obj, pympas):
-            return obj.lCellID        
+            return obj.lCellID
+        if isinstance(obj, pydggrid):
+            return obj.lCellID
         if isinstance(obj, pybasin):
-            return obj.lBasinID    
-            
+            return obj.lBasinID
+
         return JSONEncoder.default(self, obj)
 
 class flowlinecase(object):
     """
     The flowline case class
 
     Args:
         object (obj): None
 
     Returns:
         flowlinecase: A flowlinecase object
     """
     iCase_index= 0
-    
+
     sMesh_type = 1
     iFlag_standalone=1
     iFlag_flowline = 1
     iFlag_global = 0
     iFlag_antarctic = 0
     iFlag_multiple_outlet = 0
     iFlag_mesh_boundary = 0
     #iFlag_use_shapefile_extent=1
     iFlag_use_mesh_dem=0
     iFlag_save_mesh = 0
     iFlag_simplification = 1 #user can turn on/off
     iFlag_create_mesh=1
     iFlag_intersect = 1
     iFlag_rotation=0
-    iFlag_break_by_distance = 0  #if the distance between two vertice are far, 
+    iFlag_break_by_distance = 0  #if the distance between two vertice are far,
+    iFlag_dggrid = 0
     nOutlet = 1 #by default , there shoule ne only one ouelet
     dResolution_degree=0.0
     dResolution_meter=0.0
     dThreshold_small_river=0.0
-    dThreshold_break_by_distance = 5000.0 
+    dThreshold_break_by_distance = 5000.0
     dLongitude_left = -180
     dLongitude_right = 180
     dLatitude_bot = -90
     dLatitude_top = 90
     dElevation_mean=-9999.0
     sFilename_model_configuration=''
     sFilename_mesh_boundary = ''
-    sWorkspace_input=''      
-    sWorkspace_output=''    
-    #sWorkspace_output_case=''    
+    sWorkspace_input=''
+    sWorkspace_output=''
+    #sWorkspace_output_case=''
     sRegion=''
     sModel=''
     sMesh_type ='hexagon'
 
     sCase=''
-    sDate=''    
+    sDate=''
+
+    sFilename_dggrid=''
 
     sFilename_spatial_reference=''
-    sFilename_dem=''   
+    sFilename_dem=''
 
     sFilename_mesh=''
     sFilename_mesh_info=''
     sFilename_mesh_netcdf=''
-    
+    sFilename_mesh_kml=''
+
     aBasin = list()
     aFlowline_simplified=list()
     aFlowline_conceptual=list()
     aCellID_outlet = list()
     aCell=list()
 
-    iFlag_visual = importlib.util.find_spec("cartopy") 
+    iFlag_visual = importlib.util.find_spec("cartopy")
     if iFlag_visual is not None:
         from ._visual import plot
         from ._visual import _plot_study_area
         from ._visual import _plot_mesh
         from ._visual import _plot_mesh_with_flowline
         from ._visual import _compare_with_raster_dem_method
     else:
         pass
 
     from ._hpc import _create_hpc_job
-    
+
     def __init__(self, aConfig_in,
-            iFlag_standalone_in= None,
-            sModel_in = None,
-            sDate_in = None,
-            sWorkspace_output_in = None):
+                 iFlag_standalone_in= None,
+                 sModel_in = None,
+                 sDate_in = None,
+                 sWorkspace_output_in = None):
         """
         Initialize a flowlinecase object
 
         Args:
             aConfig_in (dict): A dictionary of parameters
             iFlag_standalone_in (int, optional): Flag for whether run the case standalone. Defaults to None.
             sModel_in (str, optional): The model name. Defaults to None.
@@ -153,104 +172,110 @@
             self.iFlag_standalone = iFlag_standalone_in
         else:
             if 'iFlag_standalone' in aConfig_in:
                 self.iFlag_standalone = int(aConfig_in['iFlag_standalone'])
             else:
                 self.iFlag_standalone=1
 
-  
+
         if 'iFlag_flowline' in aConfig_in:
             self.iFlag_flowline             = int(aConfig_in[ 'iFlag_flowline'])
         else:
             #without iFlag_flowline the model is a mesh generator
             self.iFlag_flowline=1
-        
+
         if 'iFlag_global' in aConfig_in:
             self.iFlag_global             = int(aConfig_in[ 'iFlag_global'])
 
         if 'iFlag_antarctic' in aConfig_in:
-            self.iFlag_antarctic             = int(aConfig_in[ 'iFlag_antarctic'])    
+            self.iFlag_antarctic             = int(aConfig_in[ 'iFlag_antarctic'])
 
         if 'iFlag_mesh_boundary' in aConfig_in:
             self.iFlag_mesh_boundary             = int(aConfig_in[ 'iFlag_mesh_boundary'])
         else:
             self.iFlag_mesh_boundary=0
-        
+
         if 'iFlag_multiple_outlet' in aConfig_in:
-            self.iFlag_multiple_outlet             = int(aConfig_in[ 'iFlag_multiple_outlet'])  
-        
+            self.iFlag_multiple_outlet             = int(aConfig_in[ 'iFlag_multiple_outlet'])
+
         if 'iFlag_simplification' in aConfig_in:
             self.iFlag_simplification = int(aConfig_in['iFlag_simplification'])
             #if simplification is desired, then we must activate flowline flag
             #it can be turn off only when a previous simplification was done and you dont want to redo it
         else:
             self.iFlag_simplification  = 1
         if self.iFlag_simplification ==1:
             self.iFlag_flowline = 1
 
         if 'iFlag_create_mesh' in aConfig_in:
-            self.iFlag_create_mesh = int(aConfig_in['iFlag_create_mesh'])  
-        else:  
+            self.iFlag_create_mesh = int(aConfig_in['iFlag_create_mesh'])
+        else:
             self.iFlag_create_mesh=1
-        
+
         if 'iFlag_save_mesh' in aConfig_in:
             self.iFlag_save_mesh             = int(aConfig_in[ 'iFlag_save_mesh'])
-        
+
         if 'iFlag_use_mesh_dem' in aConfig_in:
             self.iFlag_use_mesh_dem = int(aConfig_in['iFlag_use_mesh_dem'])
 
         #if 'iFlag_use_shapefile_extent' in aConfig_in:
-        #    self.iFlag_use_shapefile_extent = int(aConfig_in['iFlag_use_shapefile_extent'])    
+        #    self.iFlag_use_shapefile_extent = int(aConfig_in['iFlag_use_shapefile_extent'])
 
         if 'iFlag_rotation' in aConfig_in:
             self.iFlag_rotation = int(aConfig_in['iFlag_rotation'])
-        
+
 
         if 'iFlag_intersect' in aConfig_in:
             self.iFlag_intersect = int(aConfig_in['iFlag_intersect'])
         else:
             self.iFlag_intersect=1
-        
+
         if 'iFlag_break_by_distance' in aConfig_in:
             self.iFlag_break_by_distance = int(aConfig_in['iFlag_break_by_distance'])
         else:
             self.iFlag_break_by_distance=0
 
+        if 'iFlag_dggrid' in aConfig_in:
+            self.iFlag_dggrid = int(aConfig_in['iFlag_dggrid'])
+        else:
+            self.iFlag_dggrid=0
+
         if 'nOutlet' in aConfig_in:
             self.nOutlet = int(aConfig_in['nOutlet'])
-             
+
         if 'iCase_index' in aConfig_in:
             iCase_index = int(aConfig_in['iCase_index'])
         else:
             iCase_index = 1
+        
         sCase_index = "{:03d}".format( iCase_index )
         self.iCase_index =   iCase_index
 
         if 'dResolution_degree' in aConfig_in:
-            self.dResolution_degree = float(aConfig_in['dResolution_degree']) 
+            self.dResolution_degree = float(aConfig_in['dResolution_degree'])
 
         if 'dResolution_meter' in aConfig_in:
-            self.dResolution_meter = float(aConfig_in['dResolution_meter']) 
+            self.dResolution_meter = float(aConfig_in['dResolution_meter'])
         else:
             print('Please specify resolution.')
 
         if 'dThreshold_break_by_distance' in aConfig_in:
-            self.dThreshold_break_by_distance = float(aConfig_in['dThreshold_break_by_distance']) 
+            self.dThreshold_break_by_distance = float(aConfig_in['dThreshold_break_by_distance'])
 
         if 'dLongitude_left' in aConfig_in:
-            self.dLongitude_left = float(aConfig_in['dLongitude_left']) 
+            self.dLongitude_left = float(aConfig_in['dLongitude_left'])
 
         if 'dLongitude_right' in aConfig_in:
-            self.dLongitude_right = float(aConfig_in['dLongitude_right']) 
+            self.dLongitude_right = float(aConfig_in['dLongitude_right'])
 
         if 'dLatitude_bot' in aConfig_in:
-            self.dLatitude_bot = float(aConfig_in['dLatitude_bot']) 
+            self.dLatitude_bot = float(aConfig_in['dLatitude_bot'])
 
         if 'dLatitude_top' in aConfig_in:
-            self.dLatitude_top = float(aConfig_in['dLatitude_top']) 
+            self.dLatitude_top = float(aConfig_in['dLatitude_top'])
 
         if 'sFilename_model_configuration' in aConfig_in:
             self.sFilename_model_configuration    = aConfig_in[ 'sFilename_model_configuration']
 
         if 'sFilename_mesh_boundary' in aConfig_in:
             self.sFilename_mesh_boundary    = aConfig_in[ 'sFilename_mesh_boundary']
 
@@ -262,214 +287,233 @@
 
         if 'sFilename_spatial_reference' in aConfig_in:
             self.sFilename_spatial_reference = aConfig_in['sFilename_spatial_reference']
 
 
         if 'sFilename_dem' in aConfig_in:
             self.sFilename_dem = aConfig_in['sFilename_dem']
+        
+        if self.iFlag_dggrid == 1:
+            if 'sFilename_dggrid' in aConfig_in:
+                self.sFilename_dggrid = aConfig_in['sFilename_dggrid']
+                if not os.path.isfile(self.sFilename_dggrid ):
+                    print("The dggrid binary file does not exist!")
+                    exit()
+                pass
+
+            else:
+                print('Please specify the dggrid binary file.')
+                exit()
 
         if 'sFilename_mesh_netcdf' in aConfig_in:
             self.sFilename_mesh_netcdf = aConfig_in['sFilename_mesh_netcdf']
-        
+
         if 'sWorkspace_bin' in aConfig_in:
             self.sWorkspace_bin= aConfig_in[ 'sWorkspace_bin']
-            
+
         if 'sWorkspace_input' in aConfig_in:
-            self.sWorkspace_input = aConfig_in[ 'sWorkspace_input']       
-       
-        
+            self.sWorkspace_input = aConfig_in[ 'sWorkspace_input']
+
+
         if sWorkspace_output_in is not None:
             self.sWorkspace_output = sWorkspace_output_in
         else:
             if 'sWorkspace_output' in aConfig_in:
                 self.sWorkspace_output = aConfig_in[ 'sWorkspace_output']
-        
+
         if 'sJob' in aConfig_in:
-            self.sJob =  aConfig_in['sJob'] 
+            self.sJob =  aConfig_in['sJob']
         if 'sRegion' in aConfig_in:
             self.sRegion               = aConfig_in[ 'sRegion']
-        
+
         if sModel_in is not None:
             self.sModel = sModel_in
         else:
             if 'sModel' in aConfig_in:
                 self.sModel                = aConfig_in[ 'sModel']
 
-                      
+
         sDate   = aConfig_in[ 'sDate']
         if sDate is not None:
             self.sDate= sDate
         else:
             self.sDate = sDate_default
-        
-        
+
+
         sCase = self.sModel  + self.sDate + sCase_index
         self.sCase = sCase
 
         if 'sMesh_type' in aConfig_in:
             self.sMesh_type =  aConfig_in['sMesh_type']
         else:
             self.sMesh_type = 'hexagon'
 
-                
-        
+
+
         sMesh_type = self.sMesh_type
         if sMesh_type =='hexagon': #hexagon
             self.iMesh_type = 1
         else:
             if sMesh_type =='square': #square
                 self.iMesh_type = 2
             else:
                 if sMesh_type =='latlon': #latlon
                     self.iMesh_type = 3
                 else:
                     if sMesh_type =='mpas': #mpas
                         self.iMesh_type = 4
                     else:
-                        if sMesh_type =='tin': #tin
+                        if sMesh_type =='dggrid':
                             self.iMesh_type = 5
                         else:
-                            print('Unsupported mesh type?')
-        
+                            if sMesh_type =='tin': #
+                                self.iMesh_type = 6
+                            else:
+                                print('Unsupported mesh type?')
+
         #the model can be run as part of hexwatershed or standalone
         if self.iFlag_standalone == 1:
             #in standalone case, will add case information and update output path
             sPath = str(Path(self.sWorkspace_output)  /  sCase)
             self.sWorkspace_output = sPath
         else:
             #use specified output path, also do not add output or input tag
             sPath = self.sWorkspace_output
-        
+
         Path(sPath).mkdir(parents=True, exist_ok=True)
 
         if self.iMesh_type == 4:
             if not os.path.isfile(self.sFilename_mesh_netcdf ):
                 print("The MPAS mesh file does not exist!")
                 exit()
         else:
             if not os.path.isfile(self.sFilename_dem ):
                 print("The DEM file does not exist!")
                 exit()
 
         self.aBasin = list()
-    
+
         if self.iFlag_flowline==1:
             if 'sFilename_basins' in aConfig_in:
                 self.sFilename_basins = aConfig_in['sFilename_basins']
                 if os.path.isfile(self.sFilename_basins):
                     pass
                 else:
                     print('This basin configuration file does not exist: ', self.sFilename_basins )
                     exit()
                 with open(self.sFilename_basins) as json_file:
-                    dummy_data = json.load(json_file)     
+                    dummy_data = json.load(json_file)
                     for i in range(self.nOutlet):
-                        sBasin =  "{:08d}".format(i+1)   
+                        sBasin =  "{:08d}".format(i+1)
                         dummy_basin = dummy_data[i]
                         dummy_basin['sWorkspace_output_basin'] = str(Path(self.sWorkspace_output) / sBasin )
                         pBasin = pybasin(dummy_basin)
                         self.aBasin.append(pBasin)
             else:
                 pass
         else:
             pass
-     
 
-        #model generated files         
-        self.sFilename_mesh = os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + ".geojson" )               
-        self.sFilename_mesh_info= os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + "_mesh_info.json"  )    
-                
-        return
+
+        #model generated files
+        
+        self.sFilename_mesh = os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + ".geojson" )
+        self.sFilename_mesh_info= os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + "_mesh_info.json"  )
+        self.sFilename_mesh_kml = os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + ".kml" ) #for google service
+
         
 
+        return
+
+
     def convert_flowline_to_geojson(self):
         if self.iFlag_flowline == 1:
-            for pBasin in self.aBasin:            
+            for pBasin in self.aBasin:
                 pBasin.convert_flowline_to_geojson()
                 pass
 
         return
- 
+
     def flowline_simplification(self):
         aFlowline_out = list()   #store all the flowline
         #export the outlet into a single file
         aOutlet = list()
-        if self.iFlag_simplification == 1: 
+        if self.iFlag_simplification == 1:
             for i in range(self.nOutlet):
                 pBasin = self.aBasin[i]
-                aFlowline_basin = pBasin.flowline_simplification()                
+                aFlowline_basin = pBasin.flowline_simplification()
                 aFlowline_out = aFlowline_out + aFlowline_basin
                 aOutlet.append(pBasin.pVertex_outlet)
-            
+
             self.aFlowline_simplified = aFlowline_out
-              
+
 
         return aFlowline_out
-    
+
     def mesh_generation(self, iFlag_antarctic_in=None):
         """
         The mesh generation operation
 
         Returns:
             list [pycell]: A list of cell object
         """
         print('Start mesh generation.')
         if iFlag_antarctic_in is None:
             iFlag_antarctic = 0
         else:
             iFlag_antarctic = iFlag_antarctic_in
 
-        aCell_out = list()  
+        aCell_out = list()
         if self.iFlag_create_mesh ==1:
             iFlag_global =  self.iFlag_global
             iMesh_type = self.iMesh_type
             iFlag_save_mesh = self.iFlag_save_mesh
             iFlag_rotation = self.iFlag_rotation
             iFlag_mesh_boundary = self.iFlag_mesh_boundary
             dResolution_degree = self.dResolution_degree
             dResolution_meter = self.dResolution_meter
             sFilename_dem = self.sFilename_dem
             sFilename_spatial_reference = self.sFilename_spatial_reference
-            sFilename_mesh = self.sFilename_mesh
+            sFilename_mesh = self.sFilename_mesh 
             if iMesh_type !=4: #mpas
-                spatial_reference_target = osr.SpatialReference()  
+                spatial_reference_target = osr.SpatialReference()
                 spatial_reference_target.ImportFromEPSG(4326)
-               
+
                 dPixelWidth, dOriginX, dOriginY, nrow, ncolumn, pSpatialRef_dem, pProjection, pGeotransform\
-                     = retrieve_geotiff_metadata(sFilename_dem)
+                    = retrieve_geotiff_metadata(sFilename_dem)
 
                 #lower left
                 dX_lowerleft  = dOriginX
                 dY_lowerleft = dOriginY - (nrow+1) * dPixelWidth
                 dLongitude_left0,  dLatitude_bot0= reproject_coordinates(dX_lowerleft, dY_lowerleft,pSpatialRef_dem,    spatial_reference_target)
-                
+
                 #upper right
                 dX_upperright = dOriginX + (ncolumn +1) * dPixelWidth
                 dY_upperright = dOriginY
                 dLongitude_right0, dLatitude_top0= reproject_coordinates(dX_upperright, dY_upperright,pSpatialRef_dem,  spatial_reference_target)
-                
+
                 #lower right
                 dX_lowerright = dOriginX + (ncolumn +1) * dPixelWidth
                 dY_lowerright = dOriginY - (nrow+1) * dPixelWidth
-                
+
                 dLongitude_right1,  dLatitude_bot1= reproject_coordinates(dX_lowerright, dY_lowerright,pSpatialRef_dem,    spatial_reference_target)
-                
-                #uppler left     
+
+                #uppler left
                 dX_upperleft   = dOriginX
                 dY_upperleft   =  dOriginY
                 dLongitude_left1, dLatitude_top1= reproject_coordinates(dX_upperleft, dY_upperleft,pSpatialRef_dem,  spatial_reference_target)
-                
+
                 dLatitude_top = np.max([dLatitude_top0, dLatitude_top1])
                 dLatitude_bot = np.min([dLatitude_bot0, dLatitude_bot1])
 
                 dLongitude_left = np.min([dLongitude_left0, dLongitude_left1])
                 dLongitude_right = np.max([dLongitude_right0, dLongitude_right1])
 
                 dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
-                    #pass
+                #pass
 
                 if dResolution_meter < 0:
                     #not used
                     pass
                 else:
                     dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
 
@@ -479,184 +523,222 @@
                 pass
 
             if iMesh_type ==1: #hexagon
                 #hexagon edge
                 dResolution_meter = degree_to_meter(dLatitude_mean, dResolution_degree )
                 dArea = np.power(dResolution_meter,2.0)
                 dLength_edge = np.sqrt(  2.0 * dArea / (3.0* np.sqrt(3.0))  )
-                if iFlag_rotation ==0:            
+                if iFlag_rotation ==0:
                     dX_spacing = dLength_edge * np.sqrt(3.0)
                     dY_spacing = dLength_edge * 1.5
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_spacing )
-                    nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing ) 
-                else:            
+                    nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
+                else:
                     dX_spacing = dLength_edge * 1.5
-                    dY_spacing = dLength_edge * np.sqrt(3.0)    
+                    dY_spacing = dLength_edge * np.sqrt(3.0)
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_spacing )+1
                     nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
-                
+
                 if iFlag_mesh_boundary ==1:
-                    #create a polygon based on real boundary 
-                    pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
-                    
-                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, pBoundary,\
-                        sFilename_mesh, sFilename_spatial_reference)
+                    #create a polygon based on real boundary
+                    pBoundary_wkt, pBoundary_shp = read_mesh_boundary(self.sFilename_mesh_boundary)
+
+                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                                                   sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                     pass
                 else:
                     pRing = ogr.Geometry(ogr.wkbLinearRing)
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                     pRing.AddPoint(dLongitude_right, dLatitude_top)
                     pRing.AddPoint(dLongitude_right, dLatitude_bot)
                     pRing.AddPoint(dLongitude_left, dLatitude_bot)
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                     pBoundary = ogr.Geometry(ogr.wkbPolygon)
                     pBoundary.AddGeometry(pRing)
-                    pBoundary_rec = loads( pBoundary.ExportToWkt() )
+                    pBoundary_wkt = pBoundary.ExportToWkt() #wkt format
 
-                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, pBoundary_rec,\
-                        sFilename_mesh, sFilename_spatial_reference)
+                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
+                                                   sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
 
                 return aHexagon
             else:
                 if iMesh_type ==2: #sqaure
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dResolution_meter )
                     nrow= int( (dY_upperleft - dY_lowerleft) / dResolution_meter )
                     if iFlag_mesh_boundary ==1:
-                        #create a polygon based on real boundary 
-                        pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
+                        #create a polygon based on real boundary
+                        pBoundary_wkt, pBoundary_shp = read_mesh_boundary(self.sFilename_mesh_boundary)
 
-                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, pBoundary ,\
-                            sFilename_mesh, sFilename_spatial_reference)
+                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                                                     sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                         pass
                     else:
                         pRing = ogr.Geometry(ogr.wkbLinearRing)
                         pRing.AddPoint(dLongitude_left, dLatitude_top)
                         pRing.AddPoint(dLongitude_right, dLatitude_top)
                         pRing.AddPoint(dLongitude_right, dLatitude_bot)
                         pRing.AddPoint(dLongitude_left, dLatitude_bot)
                         pRing.AddPoint(dLongitude_left, dLatitude_top)
                         pBoundary = ogr.Geometry(ogr.wkbPolygon)
                         pBoundary.AddGeometry(pRing)
-                        pBoundary_rec = loads( pBoundary.ExportToWkt() )
-                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, pBoundary_rec, \
-                            sFilename_mesh, sFilename_spatial_reference)
+                        pBoundary_wkt = pBoundary.ExportToWkt() 
+                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                                                     sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                         return aSquare
                 else:
                     if iMesh_type ==3: #latlon
                         dResolution_meter = degree_to_meter(dLatitude_mean, dResolution_degree)
                         dArea = np.power(dResolution_meter,2.0)
                         ncolumn= int( (dLongitude_right - dLongitude_left) / dResolution_degree )
                         nrow= int( (dLatitude_top - dLatitude_bot) / dResolution_degree )
-                         
+
                         if iFlag_mesh_boundary ==1:
-                            #create a polygon based on real boundary 
-                            pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
-                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow,pBoundary, \
-                                    sFilename_mesh)
+                            #create a polygon based on real boundary
+                            pBoundary_wkt, pBoundary_shp = read_mesh_boundary(self.sFilename_mesh_boundary)
+                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow, 
+                                                         sFilename_mesh, pBoundary_wkt)
                             pass
                         else:
                             pRing = ogr.Geometry(ogr.wkbLinearRing)
                             pRing.AddPoint(dLongitude_left, dLatitude_top)
                             pRing.AddPoint(dLongitude_right, dLatitude_top)
                             pRing.AddPoint(dLongitude_right, dLatitude_bot)
                             pRing.AddPoint(dLongitude_left, dLatitude_bot)
                             pRing.AddPoint(dLongitude_left, dLatitude_top)
                             pBoundary = ogr.Geometry(ogr.wkbPolygon)
                             pBoundary.AddGeometry(pRing)
-                            pBoundary_rec = loads( pBoundary.ExportToWkt() )
-                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow,pBoundary_rec, \
-                                    sFilename_mesh)
-                            
+                            pBoundary_wkt =  pBoundary.ExportToWkt() 
+                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow, \
+                                                         sFilename_mesh, pBoundary_wkt)
+
                             pass
 
                         return aLatlon
-                            
 
-                        
+
+
                     else:
                         if iMesh_type == 4: #mpas
                             iFlag_use_mesh_dem = self.iFlag_use_mesh_dem
-                            sFilename_mesh_netcdf = self.sFilename_mesh_netcdf                            
-                            dLatitude_top    = self.dLatitude_top   
-                            dLatitude_bot    = self.dLatitude_bot   
-                            dLongitude_left  = self.dLongitude_left 
+                            sFilename_mesh_netcdf = self.sFilename_mesh_netcdf
+                            dLatitude_top    = self.dLatitude_top
+                            dLatitude_bot    = self.dLatitude_bot
+                            dLongitude_left  = self.dLongitude_left
                             dLongitude_right = self.dLongitude_right
 
-                            if iFlag_antarctic ==1:                                                             
-                                aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
-                                            sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in )
+                            if iFlag_antarctic ==1:
+                                aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh,
+                                                         sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in )
                                 pass
                             else:
 
                                 if iFlag_mesh_boundary ==1:
-                                    #create a polygon based on 
-                                    #read boundary 
-                                    pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
+                                    #create a polygon based on
+                                    #read boundary
+                                    pBoundary_wkt, pBoundary_shp = read_mesh_boundary(self.sFilename_mesh_boundary)
 
-                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
-                                       sFilename_mesh_netcdf,  sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in, pBoundary_in = pBoundary)
+                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh,
+                                                             sFilename_mesh_netcdf,  sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in, pBoundary_in = pBoundary_wkt)
                                     pass
                                 else:
                                     pRing = ogr.Geometry(ogr.wkbLinearRing)
                                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                                     pRing.AddPoint(dLongitude_right, dLatitude_top)
                                     pRing.AddPoint(dLongitude_right, dLatitude_bot)
                                     pRing.AddPoint(dLongitude_left, dLatitude_bot)
                                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                                     pBoundary = ogr.Geometry(ogr.wkbPolygon)
                                     pBoundary.AddGeometry(pRing)
-                                    pBoundary_rec = loads( pBoundary.ExportToWkt() )
-                                  
+                                    pBoundary_wkt =  pBoundary.ExportToWkt() 
+
                                     #new method using polygon object
-                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, \
-                                           sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in= iFlag_antarctic_in, pBoundary_in = pBoundary_rec  )
+                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
+                                                             sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in= iFlag_antarctic_in, pBoundary_in = pBoundary_wkt  )
                             return aMpas
                         else:
-                            if iMesh_type ==5: #tin this one need to be updated because central location issue
-                                #tin edge
-                                dArea = np.power(dResolution_meter,2.0)
-                                dLength_edge = np.sqrt(  4.0 * dArea /  np.sqrt(3.0) )  
-                                dX_shift = 0.5 * dLength_edge
-                                dY_shift = 0.5 * dLength_edge * np.sqrt(3.0) 
-                                dX_spacing = dX_shift * 2
-                                dY_spacing = dY_shift
-                                ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_shift )
-                                nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing ) 
-                                aTin = create_tin_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,sFilename_mesh, sFilename_spatial_reference)
-                                return aTin
+                            if iMesh_type == 5: #dggrid
+                                dLatitude_top    = self.dLatitude_top
+                                dLatitude_bot    = self.dLatitude_bot
+                                dLongitude_left  = self.dLongitude_left
+                                dLongitude_right = self.dLongitude_right                                
+                                sWorkspace_output = self.sWorkspace_output + slash + 'dggrid'
+                                
+                                if iFlag_mesh_boundary ==1:
+                                        #create a polygon based on
+
+                                    aDggrid = create_dggrid_mesh(iFlag_global,
+                                                                     iFlag_save_mesh,
+                                                                     dResolution_meter,
+                                                                     sFilename_mesh,
+                                                                     sWorkspace_output,
+                                                                     iFlag_antarctic_in=iFlag_antarctic_in,
+                                                                     sFilename_boundary_in = self.sFilename_mesh_boundary)
+                                    pass
+                                else:                                       
+                                    aDggrid = create_dggrid_mesh(iFlag_global,
+                                                                     iFlag_save_mesh,
+                                                                     dResolution_meter,
+                                                                     sFilename_mesh,
+                                                                     sWorkspace_output)
+
+
+                                return aDggrid
+
                             else:
-                                print('Unsupported mesh type?')
+                                if iMesh_type == 6: #tin this one need to be updated because central location issue
+
+                                    #tin edge
+                                    dArea = np.power(dResolution_meter,2.0)
+                                    dLength_edge = np.sqrt( 4.0 * dArea / np.sqrt(3.0) )
+                                    dX_shift = 0.5 * dLength_edge
+                                    dY_shift = 0.5 * dLength_edge * np.sqrt(3.0)
+                                    dX_spacing = dX_shift * 2
+                                    dY_spacing = dY_shift
+                                    ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_shift )
+                                    nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
+                                    aTin = create_tin_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, sFilename_mesh, sFilename_spatial_reference)
+                                    return aTin
+                                else:
+
+                                    print('Unsupported mesh type?')
                                 return
         else:
             #read mesh?
             iMesh_type = self.iMesh_type
             aCell_out = read_mesh_json_w_topology(iMesh_type, self.sFilename_mesh)
             pass
+
+        #convert the mesh into the kml format so it can be visualized in google earth and google map
+
+        
+        if iFlag_kml is not None:
+            convert_geojson_to_kml(self.sFilename_mesh, self.sFilename_mesh_kml)
+
         print('Finish mesh generation.')
         return aCell_out
-    
+
     def reconstruct_topological_relationship(self, aCell_raw):
         """
         The topological relationship reconstruction operation
 
         Args:
             aCell_raw (list [pycell]): A list of intersected cell objects
 
         Returns:
             tuple [list [pycell], list [pyflowline], list [long]]: A list of cells, flowlines, and outlet cell IDs.
         """
         print('Start topology reconstruction.')
         iFlag_intersect = self.iFlag_intersect
         if iFlag_intersect == 1:
-            iMesh_type = self.iMesh_type        
+            iMesh_type = self.iMesh_type
             sWorkspace_output = self.sWorkspace_output
             nOutlet = self.nOutlet
             sFilename_mesh=self.sFilename_mesh
             self.aCell, pSpatial_reference_mesh = read_mesh_json(iMesh_type, sFilename_mesh)
-            self.aCell = self.merge_cell_info(aCell_raw)        
+            self.aCell = self.merge_cell_info(aCell_raw)
             aFlowline_conceptual = list()   #store all the flowline
             aCellID_outlet = list()
             aBasin = list()
             aCell_intersect=list()
             ncell=len(self.aCell)
             for pBasin in self.aBasin:
                 aCell_intersect_basin = pBasin.reconstruct_topological_relationship(iMesh_type,sFilename_mesh)
@@ -705,23 +787,23 @@
 
 
                 #update length?
             for pCell in self.aCell:
                 for pCell2 in aCell_intersect:
                     if pCell2.lCellID == pCell.lCellID:
                         pCell.dLength_flowline = pCell2.dLength_flowline
-            
+
             self.aFlowline_conceptual = aFlowline_conceptual
             self.aCellID_outlet = aCellID_outlet
             print('Finish topology reconstruction.')
             return self.aCell, aFlowline_conceptual, aCellID_outlet
         else:
-            
+
             return None
-            
+
     def merge_cell_info(self, aCell_raw):
         """
         Merge cell information after reconstruction
 
         Args:
             aCell_raw (list [pycell]): The original cell information that contains neighbor definition
 
@@ -737,15 +819,15 @@
                     pCell.aNeighbor_land= pCell2.aNeighbor_land
                     pCell.nNeighbor_land= pCell2.nNeighbor_land
                     pCell.aNeighbor_distance= pCell2.aNeighbor_distance
 
                     break
 
         return self.aCell
-        
+
     def analyze(self):
         """
         Analyze the domain results for every watershed
         """
         if self.iFlag_flowline == 1:
             for pBasin in self.aBasin:
                 pBasin.analyze()
@@ -754,51 +836,69 @@
     def setup(self):
         """
         Set up the flowlinecase
         """
         if self.iFlag_flowline == 1:
             self.convert_flowline_to_geojson()
             pass
+        
+        if self.iFlag_dggrid == 1:
+            #create dggrid output folder
+            sWorkspace_output = self.sWorkspace_output + slash + 'dggrid'
+
+            #if (os.path.exists(sWorkspace_output)):
+            #    sCommand = 'rm -rf '  + sWorkspace_output
+            #    print(sCommand)
+            #    p = subprocess.Popen(sCommand, shell= True)
+            #    p.wait()
+
+            Path(sWorkspace_output).mkdir(parents=True, exist_ok=True)
+            #then copy the binary file to the folder
+            #copy execulate
+            sFilename_new = sWorkspace_output + slash + 'dggrid'
+            copy2(self.sFilename_dggrid, sFilename_new)
+            os.chmod(sFilename_new, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)
+            pass
         return
 
     def run(self):
         """
         Run the flowlinecase simulation
 
         Returns:
             list: A list of cell objects
         """
         aCell_out = None
         if self.iFlag_flowline == 1:
-            self.flowline_simplification()        
+            self.flowline_simplification()
             aCell = self.mesh_generation()
             if self.iFlag_intersect ==1:
                 aCell_out, a, b = self.reconstruct_topological_relationship(aCell)
             else:
                 pass
         else:
             #only mesh generator
             aCell = self.mesh_generation(iFlag_antarctic_in= self.iFlag_antarctic)
-            self.aCell = aCell      
+            self.aCell = aCell
             aCell_out = aCell
-        
+
         return aCell_out
 
     def evaluate(self):
         """
         Evaluate the model performance
         """
         for pBasin in self.aBasin:
             pBasin.evaluate(self.iMesh_type, self.sMesh_type)
         return
-   
+
     def export(self):
         """
         Export the model outputs
-        """        
+        """
         self.export_mesh_info_to_json()
         if self.iFlag_flowline ==1:
             for pBasin in self.aBasin:
                 pBasin.export()
 
         self.tojson()
         return
@@ -807,48 +907,48 @@
         """
         Export the mesh information to a json file
         """
 
         aCell_all = self.aCell
         sFilename_json = self.sFilename_mesh_info
         ncell=len(aCell_all)
-        iFlag_flowline = self.iFlag_flowline 
-        #if iFlag_flowline == 1: #if there is conceptual flowline 
+        iFlag_flowline = self.iFlag_flowline
+        #if iFlag_flowline == 1: #if there is conceptual flowline
         #    pass
         #else:
         #    #only mesh, no flowline
         #    pass
-        
+
 
         with open(sFilename_json, 'w', encoding='utf-8') as f:
-            sJson = json.dumps([json.loads(ob.tojson()) for ob in aCell_all], indent = 4)        
-            f.write(sJson)    
+            sJson = json.dumps([json.loads(ob.tojson()) for ob in aCell_all], indent = 4)
+            f.write(sJson)
             f.close()
 
         return
 
-    def tojson(self): 
+    def tojson(self):
         """
         Convert the flowline case object to a json string
 
         Returns:
             json str: A json string
         """
         aSkip = ['aBasin', \
-                'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
-                'aCell']      
+                 'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
+                 'aCell']
 
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
-        sJson = json.dumps(obj,\
-            sort_keys=True, \
-                indent = 4, \
-                    ensure_ascii=True, \
-                        cls=CaseClassEncoder)
+            sJson = json.dumps(obj,\
+                               sort_keys=True, \
+                               indent = 4, \
+                               ensure_ascii=True, \
+                               cls=CaseClassEncoder)
         return sJson
 
     def export_config_to_json(self, sFilename_output_in = None):
         """
         Export the configuration to a json file
 
         Args:
@@ -857,62 +957,62 @@
 
         if self.iFlag_standalone == 1:
             if sFilename_output_in is not None:
                 sFilename_output = sFilename_output_in
             else:
                 #use current output path
                 sFilename_output = os.path.join(self.sWorkspace_output, 'configuration.json' )
-            
-            #all basins            
+
+            #all basins
             sName = 'configuration_basin.json'
             sFilename_configuration  =  os.path.join( self.sWorkspace_output  , sName)
             with open(sFilename_configuration, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aBasin],\
-                    sort_keys=True, \
-                    indent = 4)   
-                f.write(sJson)    
+                                   sort_keys=True, \
+                                   indent = 4)
+                f.write(sJson)
                 f.close()
-            #update
+                #update
             self.sFilename_basins = sFilename_configuration
-            
+
         else:
             if sFilename_output_in is not None:
                 sFilename_output = sFilename_output_in
             else:
                 #use parent path
-                sPath = Path(self.sWorkspace_output)                
+                sPath = Path(self.sWorkspace_output)
                 sFilename_output = os.path.join(sPath.parent.absolute(), 'configuration.json' )
-            #all basins
+                #all basins
             sPath = Path(self.sWorkspace_output)
             sName = 'configuration_basin.json'
             sFilename_configuration  =  os.path.join( sPath.parent.absolute() , sName)
             with open(sFilename_configuration, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aBasin],\
-                    sort_keys=True, \
-                    indent = 4)   
-                f.write(sJson)    
+                                   sort_keys=True, \
+                                   indent = 4)
+                f.write(sJson)
                 f.close()
-            #update for pyhexwatershed
+                #update for pyhexwatershed
             self.sFilename_basins = sFilename_configuration
             self.sWorkspace_output =   sPath.parent.absolute()
 
 
         aSkip = ['aBasin', \
-                'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
-                'aCell']
+                 'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
+                 'aCell']
 
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
 
         with open(sFilename_output, 'w', encoding='utf-8') as f:
             json.dump(obj, f,sort_keys=True, \
-                ensure_ascii=False, \
-                indent=4, \
-                cls=CaseClassEncoder)
+                      ensure_ascii=False, \
+                      indent=4, \
+                      cls=CaseClassEncoder)
         return
 
     def export_basin_config_to_json(self, sFilename_output_in= None):
         """
         Export the member basin configuration to a json file
 
         Args:
@@ -920,41 +1020,39 @@
         """
         if self.iFlag_standalone == 1:
             if sFilename_output_in is not None:
                 sFilename_output = sFilename_output_in
             else:
                 #use current output path
                 sName = 'configuration_basin.json'
-                sFilename_output  =  os.path.join( self.sWorkspace_output  , sName)                
-            
-            #all basins 
+                sFilename_output  =  os.path.join( self.sWorkspace_output  , sName)
+
+            #all basins
             with open(sFilename_output, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aBasin],\
-                    sort_keys=True, \
-                    indent = 4)   
-                f.write(sJson)    
+                                   sort_keys=True, \
+                                   indent = 4)
+                f.write(sJson)
                 f.close()
-            #update
+                #update
             self.sFilename_basins = sFilename_output
-            
+
         else:
             if sFilename_output_in is not None:
                 sFilename_output = sFilename_output_in
             else:
                 #use current output path
                 sPath = Path(self.sWorkspace_output)
                 sName = 'configuration_basin.json'
                 sFilename_output  =  os.path.join( sPath.parent.absolute() , sName)
-            
-            #all basins                       
+
+            #all basins
             with open(sFilename_output, 'w', encoding='utf-8') as f:
                 sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aBasin],\
-                    sort_keys=True, \
-                    indent = 4)   
-                f.write(sJson)    
+                                   sort_keys=True, \
+                                   indent = 4)
+                f.write(sJson)
                 f.close()
-            #update for pyhexwatershed
+                #update for pyhexwatershed
             self.sFilename_basins = sFilename_output
-            
-        return
 
-    
+        return
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/square.py` & `pyflowline-0.2.5/pyflowline/classes/square.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     aVertex=None
     aVertexID=None
     pVertex_center = None
     aFlowline=None    
     nNeighbor=-1
     nNeighbor_land=-1
     nNeighbor_ocean=-1
+    nNeighbor_land_virtual = -1
+    aNeighbor_land_virtual = None
     aNeighbor=None #the global ID of all neighbors
     aNeighbor_land=None #the global ID of all neighbors
     aNeighbor_ocean=None #the global ID of all neighbors
     aNeighbor_distance = None
 
     def __init__(self, dLon, dLat, aEdge, aVertex):    
         """
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/timer.py` & `pyflowline-0.2.5/pyflowline/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/classes/tin.py` & `pyflowline-0.2.5/pyflowline/classes/tin.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     dX_center_meter=0.0
     dY_center_meter=0.0
     aEdge=None
     aVertex=None
     aFlowline=None
     lCellID  = -1
     aNeighbor=None #the global ID of all neighbors
+    nNeighbor_land_virtual = -1
+    aNeighbor_land_virtual = None
     nNeighbor=-1
     def __init__(self, aEdge,aVertex, dLon, dLat):       
         nEdge = len(aEdge)
         if nEdge !=3:
             pass
         else:           
             self.aEdge = aEdge
```

### Comparing `pyflowline-0.2.4/pyflowline/classes/vertex.py` & `pyflowline-0.2.5/pyflowline/classes/vertex.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import numpy as np
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_distance_based_on_lon_lat
 else:
-    from pyflowline.algorithms.auxiliary.gdal_functions import calculate_distance_based_on_lon_lat
+    from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_distance_based_on_lon_lat
 
 class VertexClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
```

### Comparing `pyflowline-0.2.4/pyflowline/formats/convert_attributes.py` & `pyflowline-0.2.5/pyflowline/formats/convert_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.classes.square import pysquare
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.mpas import pympas
 from pyflowline.classes.tin import pytin
     
-def convert_gcs_attributes_to_cell(iMesh_type_in, dLongitude_center_in, dLatitude_center_in, \
-        aCoordinates_gcs_in, \
-        aVertexID_in, \
-        aEdgeID_in, \
+def convert_gcs_attributes_to_cell(iMesh_type_in, dLongitude_center_in, dLatitude_center_in, 
+        aCoordinates_gcs_in, 
+        aVertexID_in, 
+        aEdgeID_in, 
         aVertexIndexOnEdge_in):  
         
     npoint = len(aVertexID_in)     
     aVertex=list()        
     aEdge=list()
     
     if iMesh_type_in == 1: #hexagon
@@ -66,18 +66,18 @@
                         return pTin
                     
                     else:
                         print('What mesh type are you using?')
                         return None
                     
   
-def convert_pcs_attributes_to_cell(iMesh_type_in, \
-    aCoordinates_pcs_in, \
-    aVertexID_in, \
-    aEdgeID_in,\
+def convert_pcs_attributes_to_cell(iMesh_type_in, 
+    aCoordinates_pcs_in, 
+    aVertexID_in, 
+    aEdgeID_in,
     aVertexIndexOnEdge_in):  
 
     npoint = len(aVertexID_in)     
     aVertex=list()        
     aEdge=list()
     
     if iMesh_type_in ==1: #hexagon
```

### Comparing `pyflowline-0.2.4/pyflowline/formats/convert_flowline_to_geojson.py` & `pyflowline-0.2.5/pyflowline/formats/convert_flowline_to_geojson.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/formats/export_flowline.py` & `pyflowline-0.2.5/pyflowline/formats/export_flowline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import json
 from osgeo import ogr, osr
 from shapely.geometry import Point, LineString
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.link import pycelllink
 
-def export_flowline_to_geojson( aFlowline_in, \
-    sFilename_json_in, \
-    iFlag_projected_in= None, \
-    pSpatial_reference_in=None, \
-    aAttribute_field=None,\
-    aAttribute_data=None,\
+def export_flowline_to_geojson( aFlowline_in, 
+    sFilename_json_in, 
+    iFlag_projected_in= None, 
+    pSpatial_reference_in=None, 
+    aAttribute_field=None,
+    aAttribute_data=None,
     aAttribute_dtype=None):
+    
+    
     """
     convert a shpefile to json format.
     This function should be used for stream flowline only.
     """
 
     if os.path.exists(sFilename_json_in): 
         os.remove(sFilename_json_in)
```

### Comparing `pyflowline-0.2.4/pyflowline/formats/export_vertex.py` & `pyflowline-0.2.5/pyflowline/formats/export_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/formats/read_flowline.py` & `pyflowline-0.2.5/pyflowline/formats/read_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/formats/read_mesh.py` & `pyflowline-0.2.5/pyflowline/formats/read_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
             aCell_out.append(pCell)
 
     return aCell_out, pSpatial_reference_out
 
 def read_mesh_json_w_topology(iMesh_type_in, sFilename_mesh_in):
     """
-    convert a shpefile to json format.
+    
     This function should be used for stream flowline only.
     """
     iReturn_code = 1
     if os.path.isfile(sFilename_mesh_in):
         pass
     else:
         print('This mesh file does not exist: ', sFilename_mesh_in )
```

### Comparing `pyflowline-0.2.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py` & `pyflowline-0.2.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py` & `pyflowline-0.2.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 #we will use some GIS way to define it
 #longitude left and latitude bottom and nrow and ncolumn and resolution is used to define the rectangle
 #because it is mesh, it represent the edge instead of center
 #we will use gdal api for most operations
 import os
 import numpy as np
 from osgeo import ogr, osr
-from shapely.wkt import loads
-from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
-
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
 
 def create_hexagon_mesh(iFlag_rotation_in, 
-        dX_left_in, dY_bot_in, 
+        dX_left_in, 
+        dY_bot_in, 
         dResolution_meter_in, 
         ncolumn_in, 
-        nrow_in,
-        pPolygon_in, 
+        nrow_in, 
         sFilename_output_in, 
-        sFilename_spatial_reference_in):
+        sFilename_spatial_reference_in,
+        pBoundary_in):
     """
     _summary_
 
     Args:
         iFlag_rotation_in (_type_): _description_
         dX_left_in (_type_): _description_
         dY_bot_in (_type_): _description_
@@ -33,14 +31,19 @@
         nrow_in (_type_): _description_
         sFilename_output_in (_type_): _description_
         sFilename_spatial_reference_in (_type_): _description_
 
     Returns:
         _type_: _description_
     """
+
+    
+    #for the reason that a geometry object will be crash if the associated dataset is closed, we must pass wkt string
+    #https://gdal.org/api/python_gotchas.html
+    pBoundary = ogr.CreateGeometryFromWkt(pBoundary_in)
     
     if os.path.exists(sFilename_output_in): 
         os.remove(sFilename_output_in)
     
     if os.path.exists(sFilename_spatial_reference_in): 
         pass
     else:
@@ -171,26 +174,28 @@
                 aCoords[5,0] = x6
                 aCoords[5,1] = y6
                 aCoords[6,0] = x1
                 aCoords[6,1] = y1
            
                 dummy1= np.array(aCoords)
                 dLongitude_center = np.mean(aCoords[0:6,0])
-                dLatitude_center = np.mean(aCoords[0:6,1])
-                pCenter = ogr.Geometry(ogr.wkbPoint)
-                pCenter.AddPoint(dLongitude_center, dLatitude_center)
-                pCenter1 = loads( pCenter.ExportToWkt() )
-                iFlag = pCenter1.within(pPolygon_in)
+                dLatitude_center = np.mean(aCoords[0:6,1])                
+
+                iFlag = False
+                if pPolygon.Within(pBoundary):
+                    iFlag = True
+                else:
+                    #then check intersection
+                    if pPolygon.Intersects(pBoundary):
+                        iFlag = True
+                    else:
+                        pass
+
                 if ( iFlag == True ):
-                    pFeature.SetGeometry(pPolygon)
-                    pFeature.SetField("id", lCellID) 
-                    pFeature.SetField("lon", dLongitude_center )
-                    pFeature.SetField("lat", dLatitude_center )
-                    pFeature.SetField("area", dArea )
-                    pLayer.CreateFeature(pFeature)
+                    
 
                     pHexagon = convert_gcs_coordinates_to_cell(1, dLongitude_center, dLatitude_center, dummy1)
                     pHexagon.lCellID = lCellID
                     dArea = pHexagon.calculate_cell_area()
                     pHexagon.calculate_edge_length()
                    
                     lCellID_center = lCellID
@@ -246,14 +251,23 @@
                         print('error')        
 
                     pHexagon.aNeighbor = aNeighbor
                     pHexagon.nNeighbor = len(aNeighbor)
                     pHexagon.aNeighbor_land= aNeighbor
                     pHexagon.nNeighbor_land= pHexagon.nNeighbor
                     aHexagon.append(pHexagon)
+
+                    #save feature
+                    pFeature.SetGeometry(pPolygon)
+                    pFeature.SetField("id", lCellID) 
+                    pFeature.SetField("lon", dLongitude_center )
+                    pFeature.SetField("lat", dLatitude_center )
+                    pFeature.SetField("area", dArea )
+                    pLayer.CreateFeature(pFeature)
+
                     lCellID= lCellID + 1    
                     pass
                 else:
                     #this cell center is out of boundary
                     continue
               
         pass
@@ -344,34 +358,31 @@
                 aCoords[5,1] = y6
                 aCoords[6,0] = x1
                 aCoords[6,1] = y1
                     
                 dummy1= np.array(aCoords)
                 dLongitude_center = np.mean(aCoords[0:6,0])
                 dLatitude_center = np.mean(aCoords[0:6,1])     
-                pCenter = ogr.Geometry(ogr.wkbPoint)
-                pCenter.AddPoint(dLongitude_center, dLatitude_center)
-                pCenter1 = loads( pCenter.ExportToWkt() )
-                iFlag = pCenter1.within(pPolygon_in)
+                iFlag == False
+                if pPolygon.Within(pBoundary):
+                    iFlag = True
+                else:
+                    #then check intersection
+                    if pPolygon.Intersects(pBoundary):
+                        iFlag = True
+                    else:
+                        pass
                 if ( iFlag == True ):  
                     
                     pHexagon = convert_gcs_coordinates_to_cell(1, dLongitude_center, dLatitude_center, dummy1)
                     pHexagon.lCellID = lCellID
                     dArea = pHexagon.calculate_cell_area()
                     pHexagon.dArea = dArea
                     pHexagon.calculate_edge_length() 
                     
-
-                    pFeature.SetGeometry(pPolygon)
-                    pFeature.SetField("id", lCellID)
-                    pFeature.SetField("lon", dLongitude_center )
-                    pFeature.SetField("lat", dLatitude_center )
-                    pFeature.SetField("area", dArea )
-                    pLayer.CreateFeature(pFeature)
-
                     lCellID_center = lCellID                
                     aNeighbor=list()
                     if iRow > 1:#0
                         lCellID0 = lCellID_center - 1
                         aNeighbor.append(lCellID0)
 
                     if iColumn> 1:#1 ans 2
@@ -384,15 +395,14 @@
                         else:
                             lCellID2 = nrow_in * (iColumn-2) + iRow
                             aNeighbor.append(lCellID2)
                             if iRow != 1:
                                 lCellID1 = nrow_in * (iColumn-2) + iRow -1
                                 aNeighbor.append(lCellID1)
 
-
                     if iRow < nrow_in:#3
                         lCellID3 = lCellID_center + 1
                         aNeighbor.append(lCellID3)
 
                     if iColumn  < ncolumn_in  : #4 and 5
                         if iColumn %2 ==1:
                             lCellID4 = nrow_in * iColumn + iRow 
@@ -412,14 +422,21 @@
 
                     pHexagon.aNeighbor = aNeighbor
                     pHexagon.nNeighbor = len(aNeighbor)
                     pHexagon.aNeighbor_land= aNeighbor
                     pHexagon.nNeighbor_land= pHexagon.nNeighbor
                     aHexagon.append(pHexagon)
 
+                    pFeature.SetGeometry(pPolygon)
+                    pFeature.SetField("id", lCellID)
+                    pFeature.SetField("lon", dLongitude_center )
+                    pFeature.SetField("lat", dLatitude_center )
+                    pFeature.SetField("area", dArea )
+                    pLayer.CreateFeature(pFeature)
+
                     lCellID= lCellID +1
 
                     pass
                 else:
                     #out of bound
                     pass
```

### Comparing `pyflowline-0.2.4/pyflowline/mesh/latlon/create_latlon_mesh.py` & `pyflowline-0.2.5/pyflowline/mesh/latlon/create_latlon_mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 #we will use some GIS way to define it
 #longitude left and latitude bottom and nrow and ncolumn and resolution is used to define the rectangle
 #because it is mesh, it represent the edge instead of center
 #we will use gdal api for most operations
 import os
 import numpy as np
 from osgeo import ogr, osr
-from shapely.wkt import loads
-from pyflowline.classes.latlon import pylatlon
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-
-def create_latlon_mesh(dLongitude_left_in, dLatitude_bot_in, dResolution_degree_in, ncolumn_in, nrow_in, pPolygon_in, sFilename_output_in):
+def create_latlon_mesh(dLongitude_left_in, 
+                       dLatitude_bot_in, 
+                       dResolution_degree_in, 
+                       ncolumn_in, nrow_in, 
+                       sFilename_output_in,
+                       pBoundary_in):
     """
     _summary_
 
     Args:
         dLongitude_left_in (_type_): _description_
         dLatitude_bot_in (_type_): _description_
         dResolution_degree_in (_type_): _description_
         ncolumn_in (_type_): _description_
         nrow_in (_type_): _description_
         sFilename_output_in (_type_): _description_
 
     Returns:
         _type_: _description_
     """
+    #for the reason that a geometry object will be crash if the associated dataset is closed, we must pass wkt string
+    #https://gdal.org/api/python_gotchas.html
+    pBoundary = ogr.CreateGeometryFromWkt(pBoundary_in)
        
     
     if os.path.exists(sFilename_output_in): 
         os.remove(sFilename_output_in)
 
     #pDriver_shapefile = ogr.GetDriverByName('Esri Shapefile')
     pDriver_geojson = ogr.GetDriverByName('GeoJSON')    
@@ -93,33 +98,31 @@
             aCoords[2,1] = y3
             aCoords[3,0] = x4
             aCoords[3,1] = y4
             aCoords[4,0] = x1
             aCoords[4,1] = y1
             
 
-            pCenter = ogr.Geometry(ogr.wkbPoint)
-            pCenter.AddPoint(dLongitude_center, dLatitude_center)
-            pCenter1 = loads( pCenter.ExportToWkt() )
-            iFlag = pCenter1.within(pPolygon_in)
+            iFlag = False
+            if pPolygon.Within(pBoundary):
+                iFlag = True
+            else:
+                #then check intersection
+                if pPolygon.Intersects(pBoundary):
+                    iFlag = True
+                else:
+                    pass
 
             if ( iFlag == True ):
 
                 dummy1= np.array(aCoords)           
                 pLatlon = convert_gcs_coordinates_to_cell(3, dLongitude_center, dLatitude_center, dummy1)
                 pLatlon.lCellID = lCellID
                 dArea = pLatlon.calculate_cell_area()
-                pLatlon.calculate_edge_length()
-                
-                pFeature.SetGeometry(pPolygon)
-                pFeature.SetField("id", lCellID)
-                pFeature.SetField("lon", dLongitude_center )
-                pFeature.SetField("lat", dLatitude_center )
-                pFeature.SetField("area", dArea )
-                pLayer.CreateFeature(pFeature)
+                pLatlon.calculate_edge_length()      
 
                 lCellID_center = lCellID
 
                 aNeighbor = list()
                 if iRow > 1:#under
                     lCellID0 = lCellID_center - 1
                     aNeighbor.append(lCellID0)
@@ -149,14 +152,23 @@
                         aNeighbor.append(lCellID7) 
 
                 pLatlon.aNeighbor = aNeighbor
                 pLatlon.nNeighbor = len(aNeighbor)
                 pLatlon.aNeighbor_land= aNeighbor
                 pLatlon.nNeighbor_land= pLatlon.nNeighbor            
                 aLatlon.append(pLatlon)
+
+                #save feature
+                pFeature.SetGeometry(pPolygon)
+                pFeature.SetField("id", lCellID)
+                pFeature.SetField("lon", dLongitude_center )
+                pFeature.SetField("lat", dLatitude_center )
+                pFeature.SetField("area", dArea )
+                pLayer.CreateFeature(pFeature)
+
                 lCellID = lCellID + 1
 
                 pass
         
     pDataset = pLayer = pFeature  = None      
 
     aLatlon_out = list()
```

### Comparing `pyflowline-0.2.4/pyflowline/mesh/square/create_square_mesh.py` & `pyflowline-0.2.5/pyflowline/mesh/square/create_square_mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 #we will use some GIS way to define it
 #longitude left and latitude bottom and nrow and ncolumn and resolution is used to define the rectangle
 #because it is mesh, it represent the edge instead of center
 #we will use gdal api for most operations
 import os
 from osgeo import ogr, osr
 import numpy as np
-from shapely.wkt import loads
-from pyflowline.classes.square import pysquare
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import  reproject_coordinates_batch
 
-def create_square_mesh(dX_left_in, dY_bot_in, dResolution_meter_in, ncolumn_in, nrow_in, pPolygon_in,
-    sFilename_output_in, sFilename_spatial_reference_in):   
+def create_square_mesh(dX_left_in, dY_bot_in,
+                        dResolution_meter_in,
+                        ncolumn_in, nrow_in,
+    sFilename_output_in, 
+    sFilename_spatial_reference_in, 
+    pBoundary_in):   
     """
     _summary_
 
     Args:
         dX_left_in (_type_): _description_
         dY_bot_in (_type_): _description_
         dResolution_meter_in (_type_): _description_
@@ -25,15 +26,17 @@
         nrow_in (_type_): _description_
         sFilename_output_in (_type_): _description_
         sFilename_spatial_reference_in (_type_): _description_
 
     Returns:
         _type_: _description_
     """
-
+    #for the reason that a geometry object will be crash if the associated dataset is closed, we must pass wkt string
+    #https://gdal.org/api/python_gotchas.html
+    pBoundary = ogr.CreateGeometryFromWkt(pBoundary_in)
 
     if os.path.exists(sFilename_output_in): 
         os.remove(sFilename_output_in)
 
     pDriver_shapefile = ogr.GetDriverByName('Esri Shapefile')
     pDriver_geojson = ogr.GetDriverByName('GeoJSON')
     pDataset_shapefile = pDriver_shapefile.Open(sFilename_spatial_reference_in, 0)
@@ -127,30 +130,31 @@
             aCoords[4,0] = x1
             aCoords[4,1] = y1
 
             dummy1= np.array(aCoords)
             dLongitude_center = np.mean(aCoords[0:4,0])
             dLatitude_center = np.mean(aCoords[0:4,1])     
 
-            pCenter = ogr.Geometry(ogr.wkbPoint)
-            pCenter.AddPoint(dLongitude_center, dLatitude_center)
-            pCenter1 = loads( pCenter.ExportToWkt() )
-            iFlag = pCenter1.within(pPolygon_in)
+            iFlag = False
+            if pPolygon.Within(pBoundary):
+                iFlag = True
+            else:
+                #then check intersection
+                if pPolygon.Intersects(pBoundary):
+                    iFlag = True
+                else:
+                    pass
+
             if ( iFlag == True ):
                 pSquare = convert_gcs_coordinates_to_cell(2, dLongitude_center, dLatitude_center, dummy1)
                 pSquare.lCellID = lCellID
                 dArea = pSquare.calculate_cell_area()
                 pSquare.calculate_edge_length()
 
-                pFeature.SetGeometry(pPolygon)
-                pFeature.SetField("id", lCellID)
-                pFeature.SetField("lon", dLongitude_center )
-                pFeature.SetField("lat", dLatitude_center )
-                pFeature.SetField("area", dArea )
-                pLayer.CreateFeature(pFeature)
+                
 
                 #build topoloy
                 aNeighbor=list()
 
                 lCellID_center = lCellID
 
                 if iRow > 1:#under
@@ -182,27 +186,37 @@
                         aNeighbor.append(lCellID7) 
 
                 pSquare.aNeighbor = aNeighbor
                 pSquare.nNeighbor = len(aNeighbor)
                 pSquare.aNeighbor_land= aNeighbor
                 pSquare.nNeighbor_land= pSquare.nNeighbor
                 aSquare.append(pSquare)
+
+                #save feature
+                pFeature.SetGeometry(pPolygon)
+                pFeature.SetField("id", lCellID)
+                pFeature.SetField("lon", dLongitude_center )
+                pFeature.SetField("lat", dLatitude_center )
+                pFeature.SetField("area", dArea )
+                pLayer.CreateFeature(pFeature)
+
                 lCellID = lCellID + 1
 
                 pass
 
     pDataset = pLayer = pFeature  = None  
 
     aSquare_out = list()
     ncell = len(aSquare)
     aCellID  = list()
     for i in range(ncell):
         pCell = aSquare[i]
         lCellID = pCell.lCellID
         aCellID.append(lCellID)
+        
     for i in range(ncell):
         pCell = aSquare[i]
         aNeighbor = pCell.aNeighbor
         nNeighbor = pCell.nNeighbor
         aNeighbor_new = list()
         nNeighbor_new = 0 
         for j in range(nNeighbor):
```

### Comparing `pyflowline-0.2.4/pyflowline/mesh/tin/create_tin_mesh.py` & `pyflowline-0.2.5/pyflowline/mesh/tin/create_tin_mesh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import os, sys
-
+import os
 import numpy as np
-
 from osgeo import ogr, osr
-from shapely.wkt import loads
-from pyflowline.classes.tin import pytin
-
-from pyflowline.formats.convert_coordinates import convert_pcs_coordinates_to_cell
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
-
 from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
 
-def create_tin_mesh(dX_left_in, dY_bot_in, dResolution_meter_in, ncolumn_in, nrow_in, pPolygon_in,
-sFilename_output_in, sFilename_spatial_reference_in):
+def create_tin_mesh(dX_left_in, dY_bot_in, 
+                    dResolution_meter_in, 
+                    ncolumn_in, nrow_in, 
+sFilename_output_in, 
+sFilename_spatial_reference_in, 
+pBoundary_in):
      
-    
+    #for the reason that a geometry object will be crash if the associated dataset is closed, we must pass wkt string
+    #https://gdal.org/api/python_gotchas.html
+    pBoundary = ogr.CreateGeometryFromWkt(pBoundary_in)
     if os.path.exists(sFilename_output_in): 
         #delete it if it exists
         os.remove(sFilename_output_in)
 
     pDriver_shapefile = ogr.GetDriverByName('Esri Shapefile')
 
     pDataset_shapefile = pDriver_shapefile.Open(sFilename_spatial_reference_in, 0)
@@ -130,34 +128,42 @@
             aCoords[2,1] = y3         
             aCoords[3,0] = x1
             aCoords[3,1] = y1
                 
             dummy1= np.array(aCoords)
             dLongitude_center = np.mean(aCoords[0:3,0])
             dLatitude_center = np.mean(aCoords[0:3,1])     
-            pCenter = ogr.Geometry(ogr.wkbPoint)
-            pCenter.AddPoint(dLongitude_center, dLatitude_center)
-            pCenter1 = loads( pCenter.ExportToWkt() )
-            iFlag = pCenter1.within(pPolygon_in)
+
+            iFlag = False
+            if pPolygon.Within(pBoundary):
+                iFlag = True
+            else:
+                #then check intersection
+                if pPolygon.Intersects(pBoundary):
+                    iFlag = True
+                else:
+                    pass
+
             if ( iFlag == True ):         
            
                 pTIN = convert_gcs_coordinates_to_cell(5, dLongitude_center, dLatitude_center, dummy1)
                 pTIN.lCellID = lCellID
                 dArea = pTIN.calculate_cell_area()
                 pTIN.dArea = dArea
                 pTIN.calculate_edge_length() 
-                
+                aTin.append(pTIN)
+
                 pFeature.SetGeometry(pPolygon)
                 pFeature.SetField("id", lCellID)
                 pFeature.SetField("lon", dLongitude_center )
                 pFeature.SetField("lat", dLatitude_center )
                 pFeature.SetField("area", dArea )
                 pLayer.CreateFeature(pFeature)
                           
-                aTin.append(pTIN)
+                
                 lCellID = lCellID + 1   
 
             pass
         
     pDataset = pLayer = pFeature  = None
```

### Comparing `pyflowline-0.2.4/pyflowline/pyflowline_create_template_configuration_file.py` & `pyflowline-0.2.5/pyflowline/pyflowline_create_template_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.4/pyflowline/pyflowline_read_model_configuration_file.py` & `pyflowline-0.2.5/pyflowline/pyflowline_read_model_configuration_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         iFlag_use_mesh_dem = iFlag_use_mesh_dem_in
     else:       
         iFlag_use_mesh_dem = int(aConfig['iFlag_use_mesh_dem'])
 
     if sMesh_type_in is not None:
         sMesh_type = sMesh_type_in
     else:
-        sMesh_type = aConfig['sModel']
+        sMesh_type = aConfig['sMesh_type']
         pass
         
     if sModel_in is not None:
         sModel = sModel_in
     else:
         sModel = aConfig['sModel']
         pass
@@ -106,14 +106,15 @@
     aConfig['iFlag_standalone'] = iFlag_standalone
     aConfig['iFlag_use_mesh_dem'] = iFlag_use_mesh_dem
     aConfig['dResolution_degree'] = dResolution_degree
     aConfig['dResolution_meter'] = dResolution_meter
 
     aConfig['sDate'] = sDate
     aConfig['sModel'] = sModel
+    aConfig['sMesh_type'] = sMesh_type
     aConfig['sWorkspace_output'] = sWorkspace_output
 
     aConfig["sFilename_model_configuration"] = sFilename_configuration_in
    
     
 
     #based on global variable, a few variables are calculate once
```

### Comparing `pyflowline-0.2.4/pyflowline.egg-info/PKG-INFO` & `pyflowline-0.2.5/pyflowline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.2.4
+Version: 0.2.5
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,25 @@
 ### PyFlowline
 
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models. 
 
-PyFlowline is mesh independent, meaning you can apply it to both structured (e.g., traditional rectangle mesh, latitude-longitude, hexagon) and unstructured mesh systems (e.g., Triangulated Irregular Network (TIN) mesh and Model for Prediction Across Scales (MPAS) mesh).
+PyFlowline is mesh independent, meaning you can apply it to both structured 
+
+1. traditional rectangle mesh 
+2. latitude-longitude 
+3. hexagon
+4. dggs ([dggrid](https://github.com/sahrk/DGGRID))
+
+and unstructured mesh systems 
+
+1. Model for Prediction Across Scales mesh ([MPAS](https://github.com/MPAS-Dev))
+2. Triangulated Irregular Network (TIN) mesh
 
 This package generates the mesh cell-based conceptual river networks using the following steps:
 
 1. `Flowline simplification`: PyFlowline checks the vector dataset and corrects undesired flowlines, such as braided rivers.
 2. `Mesh generation`: PyFlowline generates structured meshes (e.g., rectangle, hexagon) or imports user-provided unstructured meshes into the PyFlowline-compatible GEOJSON format.
 3. `Topological relationship reconstruction`: PyFlowline reconstructs the topological relationship using the mesh and flowline intersections.
 
@@ -49,14 +59,15 @@
 4. `shapely`
 
 PyFlowline also has three optional dependency packages
 
 1. `cython` for performance 
 2. `matplotlin` for visualization
 3. `cartopy` for visulization
+4. `simplekml` for Google Earth KML support
 
 ### Quickstart
 
 Please refer to the [quickstart documentation](https://pyflowline.readthedocs.io/en/latest/quickstart.html) for details on how to get started using the PyFlowline package.
 
 ### Installation
 
@@ -66,14 +77,16 @@
 
 We provide several examples in the `examples` folder to demonstrate the model capability. We also recommend starting with the `notebooks/mpas_example.ipynb` notebook, after following the Quickstart and Installation instructions.
 
 ### Acknowledgment
 
 This work was supported by the Earth System Model Development program areas of the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research as part of the multi-program, collaborative Integrated Coastal Modeling (ICoM) project and the Interdisciplinary Research for Arctic Coastal Environments (InteRFACE) project.
 
+This research was supported as part of the Next Generation Ecosystem Experiments-Tropics, funded by the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research at Pacific Northwest National Laboratory. The study was also partly supported by U.S. Department of Energy Office of Science Biological and Environmental Research through the Earth and Environmental System Modeling program as part of the Energy Exascale Earth System Model (E3SM) project.
+
 ### License
 
 BSD 3-Clause License
 
 Copyright © 2022, Battelle Memorial Institute
 
 1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software and may permit others to do so, subject to the following conditions:
```

### Comparing `pyflowline-0.2.4/pyflowline.egg-info/SOURCES.txt` & `pyflowline-0.2.5/pyflowline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 pyflowline/algorithms/split/split_flowline_to_edge.py
 pyflowline/classes/__init__.py
 pyflowline/classes/_hpc.py
 pyflowline/classes/_visual.py
 pyflowline/classes/basin.py
 pyflowline/classes/cell.py
 pyflowline/classes/confluence.py
+pyflowline/classes/dggrid.py
 pyflowline/classes/edge.py
 pyflowline/classes/flowline.py
 pyflowline/classes/hexagon.py
 pyflowline/classes/latlon.py
 pyflowline/classes/link.py
 pyflowline/classes/mesh.py
 pyflowline/classes/mpas.py
```

### Comparing `pyflowline-0.2.4/setup.py` & `pyflowline-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = "pyflowline"
 DESCRIPTION = \
     "A mesh-independent river network generator for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyflowline"
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [
     "numpy", 
     "gdal",
     "netCDF4",
@@ -57,10 +57,10 @@
     python_requires=REQUIRES_PYTHON,
     keywords=KEYWORDS,
     url=URL,
     packages=find_packages(),
     install_requires=REQUIRED,
     classifiers=CLASSIFY,
     extras_require={
-        'visualization': ['cython', 'matplotlib', 'cartopy>=0.21.0']
+        'visualization': ['cython', 'matplotlib', 'cartopy>=0.21.0','simplekml']
     }
 )
```

