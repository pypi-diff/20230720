# Comparing `tmp/crossroads-schematization-0.3.0.tar.gz` & `tmp/crossroads-schematization-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.3.0.tar", last modified: Thu Jul 20 07:39:43 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.3.1.tar", last modified: Thu Jul 20 07:51:53 2023, max compression
```

## Comparing `crossroads-schematization-0.3.0.tar` & `crossroads-schematization-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,64 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.439849 crossroads-schematization-0.3.0/
--rw-r--r--   0 jm        (1000) jm        (1000)      141 2023-07-10 12:56:10.000000 crossroads-schematization-0.3.0/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-20 07:39:43.439849 crossroads-schematization-0.3.0/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.3.0/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.431846 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-20 07:39:43.000000 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1760 2023-07-20 07:39:43.000000 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-20 07:39:43.000000 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-20 07:39:43.000000 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-20 07:39:43.000000 crossroads-schematization-0.3.0/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.431846 crossroads-schematization-0.3.0/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-20 07:39:27.000000 crossroads-schematization-0.3.0/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     8563 2023-07-10 13:13:14.000000 crossroads-schematization-0.3.0/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    28821 2023-07-19 17:30:59.000000 crossroads-schematization-0.3.0/crschem/crossroad_schematization.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.435848 crossroads-schematization-0.3.0/crschem/model/
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.435848 crossroads-schematization-0.3.0/crschem/model/__pycache__/
--rw-r--r--   0 jm        (1000) jm        (1000)    12786 2023-07-19 15:35:46.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/branch.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)    28695 2023-07-13 18:19:24.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/crossing.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)     3035 2023-07-10 13:12:42.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/simple_way.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)     4069 2023-07-11 09:15:45.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)     8607 2023-07-13 08:54:20.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/straight_way.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)    27958 2023-07-19 09:21:05.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/traffic_island.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)    23402 2023-07-13 08:54:44.000000 crossroads-schematization-0.3.0/crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc
--rw-r--r--   0 jm        (1000) jm        (1000)     7000 2023-07-19 15:35:42.000000 crossroads-schematization-0.3.0/crschem/model/branch.py
--rw-r--r--   0 jm        (1000) jm        (1000)    17540 2023-07-13 18:14:59.000000 crossroads-schematization-0.3.0/crschem/model/crossing.py
--rw-r--r--   0 jm        (1000) jm        (1000)     1573 2023-07-10 13:12:39.000000 crossroads-schematization-0.3.0/crschem/model/simple_way.py
--rw-r--r--   0 jm        (1000) jm        (1000)     1790 2023-07-11 09:15:36.000000 crossroads-schematization-0.3.0/crschem/model/straight_sidewalk.py
--rw-r--r--   0 jm        (1000) jm        (1000)     4123 2023-07-13 08:54:07.000000 crossroads-schematization-0.3.0/crschem/model/straight_way.py
--rw-r--r--   0 jm        (1000) jm        (1000)    14267 2023-07-19 09:20:55.000000 crossroads-schematization-0.3.0/crschem/model/traffic_island.py
--rw-r--r--   0 jm        (1000) jm        (1000)    13081 2023-07-13 08:54:41.000000 crossroads-schematization-0.3.0/crschem/model/turning_sidewalk.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7199 2023-07-11 08:33:31.000000 crossroads-schematization-0.3.0/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.431846 crossroads-schematization-0.3.0/crschem/resources/
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.439849 crossroads-schematization-0.3.0/crschem/resources/400/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.3.0/crschem/resources/400/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.3.0/crschem/resources/400/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.3.0/crschem/resources/400/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.3.0/crschem/resources/400/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.3.0/crschem/resources/400/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.3.0/crschem/resources/400/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.3.0/crschem/resources/400/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.3.0/crschem/resources/400/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:48:21.000000 crossroads-schematization-0.3.0/crschem/resources/400/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     4100 2023-07-10 14:48:52.000000 crossroads-schematization-0.3.0/crschem/resources/400/style-96.xml
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:39:43.439849 crossroads-schematization-0.3.0/crschem/resources/500/
--rw-r--r--   0 jm        (1000) jm        (1000)     1941 2023-07-07 10:01:36.000000 crossroads-schematization-0.3.0/crschem/resources/500/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1932 2023-07-07 10:02:54.000000 crossroads-schematization-0.3.0/crschem/resources/500/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.0/crschem/resources/500/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1519 2023-07-07 10:06:34.000000 crossroads-schematization-0.3.0/crschem/resources/500/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.0/crschem/resources/500/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1516 2023-07-07 10:06:11.000000 crossroads-schematization-0.3.0/crschem/resources/500/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.0/crschem/resources/500/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.0/crschem/resources/500/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     4102 2023-07-10 14:49:05.000000 crossroads-schematization-0.3.0/crschem/resources/500/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:49:12.000000 crossroads-schematization-0.3.0/crschem/resources/500/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     9456 2023-07-19 16:55:26.000000 crossroads-schematization-0.3.0/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.3.0/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-20 07:39:43.439849 crossroads-schematization-0.3.0/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.3.0/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.861540 crossroads-schematization-0.3.1/
+-rw-r--r--   0 jm        (1000) jm        (1000)      183 2023-07-20 07:49:29.000000 crossroads-schematization-0.3.1/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-20 07:51:53.861540 crossroads-schematization-0.3.1/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.3.1/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.853540 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-20 07:51:53.000000 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1968 2023-07-20 07:51:53.000000 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-20 07:51:53.000000 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-20 07:51:53.000000 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-20 07:51:53.000000 crossroads-schematization-0.3.1/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.853540 crossroads-schematization-0.3.1/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-20 07:51:40.000000 crossroads-schematization-0.3.1/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     8563 2023-07-10 13:13:14.000000 crossroads-schematization-0.3.1/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    28821 2023-07-19 17:30:59.000000 crossroads-schematization-0.3.1/crschem/crossroad_schematization.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.857540 crossroads-schematization-0.3.1/crschem/model/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.857540 crossroads-schematization-0.3.1/crschem/model/__pycache__/
+-rw-r--r--   0 jm        (1000) jm        (1000)    12786 2023-07-19 15:35:46.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/branch.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    28695 2023-07-13 18:19:24.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/crossing.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     3035 2023-07-10 13:12:42.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/simple_way.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     4069 2023-07-11 09:15:45.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     8607 2023-07-13 08:54:20.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/straight_way.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    27958 2023-07-19 09:21:05.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/traffic_island.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    23402 2023-07-13 08:54:44.000000 crossroads-schematization-0.3.1/crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     7000 2023-07-19 15:35:42.000000 crossroads-schematization-0.3.1/crschem/model/branch.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    17540 2023-07-13 18:14:59.000000 crossroads-schematization-0.3.1/crschem/model/crossing.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     1573 2023-07-10 13:12:39.000000 crossroads-schematization-0.3.1/crschem/model/simple_way.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     1790 2023-07-11 09:15:36.000000 crossroads-schematization-0.3.1/crschem/model/straight_sidewalk.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     4123 2023-07-13 08:54:07.000000 crossroads-schematization-0.3.1/crschem/model/straight_way.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    14267 2023-07-19 09:20:55.000000 crossroads-schematization-0.3.1/crschem/model/traffic_island.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    13081 2023-07-13 08:54:41.000000 crossroads-schematization-0.3.1/crschem/model/turning_sidewalk.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.857540 crossroads-schematization-0.3.1/crschem/normalization/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.857540 crossroads-schematization-0.3.1/crschem/normalization/__pycache__/
+-rw-r--r--   0 jm        (1000) jm        (1000)    15425 2023-07-19 16:15:25.000000 crossroads-schematization-0.3.1/crschem/normalization/__pycache__/normalized_branch.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     8223 2023-07-19 17:29:04.000000 crossroads-schematization-0.3.1/crschem/normalization/__pycache__/normalizer.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     8522 2023-07-19 16:15:17.000000 crossroads-schematization-0.3.1/crschem/normalization/normalized_branch.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     4414 2023-07-19 17:29:00.000000 crossroads-schematization-0.3.1/crschem/normalization/normalizer.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7199 2023-07-11 08:33:31.000000 crossroads-schematization-0.3.1/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.853540 crossroads-schematization-0.3.1/crschem/resources/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.861540 crossroads-schematization-0.3.1/crschem/resources/400/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.3.1/crschem/resources/400/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.3.1/crschem/resources/400/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.3.1/crschem/resources/400/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.3.1/crschem/resources/400/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.3.1/crschem/resources/400/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.3.1/crschem/resources/400/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.3.1/crschem/resources/400/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.3.1/crschem/resources/400/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:48:21.000000 crossroads-schematization-0.3.1/crschem/resources/400/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     4100 2023-07-10 14:48:52.000000 crossroads-schematization-0.3.1/crschem/resources/400/style-96.xml
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-20 07:51:53.861540 crossroads-schematization-0.3.1/crschem/resources/500/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1941 2023-07-07 10:01:36.000000 crossroads-schematization-0.3.1/crschem/resources/500/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1932 2023-07-07 10:02:54.000000 crossroads-schematization-0.3.1/crschem/resources/500/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.1/crschem/resources/500/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1519 2023-07-07 10:06:34.000000 crossroads-schematization-0.3.1/crschem/resources/500/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.1/crschem/resources/500/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1516 2023-07-07 10:06:11.000000 crossroads-schematization-0.3.1/crschem/resources/500/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.1/crschem/resources/500/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.3.1/crschem/resources/500/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     4102 2023-07-10 14:49:05.000000 crossroads-schematization-0.3.1/crschem/resources/500/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:49:12.000000 crossroads-schematization-0.3.1/crschem/resources/500/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     9456 2023-07-19 16:55:26.000000 crossroads-schematization-0.3.1/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.3.1/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-20 07:51:53.861540 crossroads-schematization-0.3.1/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.3.1/setup.py
```

### Comparing `crossroads-schematization-0.3.0/PKG-INFO` & `crossroads-schematization-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.3.0
+Version: 0.3.1
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.3.0/README.md` & `crossroads-schematization-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.3.1/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.3.0
+Version: 0.3.1
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.3.0/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.3.1/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 crschem/model/__pycache__/branch.cpython-311.pyc
 crschem/model/__pycache__/crossing.cpython-311.pyc
 crschem/model/__pycache__/simple_way.cpython-311.pyc
 crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc
 crschem/model/__pycache__/straight_way.cpython-311.pyc
 crschem/model/__pycache__/traffic_island.cpython-311.pyc
 crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc
+crschem/normalization/normalized_branch.py
+crschem/normalization/normalizer.py
+crschem/normalization/__pycache__/normalized_branch.cpython-311.pyc
+crschem/normalization/__pycache__/normalizer.cpython-311.pyc
 crschem/resources/400/crossing-3-300.svg
 crschem/resources/400/crossing-3-96.svg
 crschem/resources/400/island-300-white.svg
 crschem/resources/400/island-300.svg
 crschem/resources/400/island-96-white.svg
 crschem/resources/400/island-96.svg
 crschem/resources/400/point-300.svg
```

### Comparing `crossroads-schematization-0.3.0/crschem/cmd.py` & `crossroads-schematization-0.3.1/crschem/cmd.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/crossroad_schematization.py` & `crossroads-schematization-0.3.1/crschem/crossroad_schematization.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/branch.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/branch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/crossing.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/crossing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/simple_way.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/simple_way.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/straight_way.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/straight_way.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/traffic_island.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/traffic_island.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc` & `crossroads-schematization-0.3.1/crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/branch.py` & `crossroads-schematization-0.3.1/crschem/model/branch.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/crossing.py` & `crossroads-schematization-0.3.1/crschem/model/crossing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/simple_way.py` & `crossroads-schematization-0.3.1/crschem/model/simple_way.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/straight_sidewalk.py` & `crossroads-schematization-0.3.1/crschem/model/straight_sidewalk.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/straight_way.py` & `crossroads-schematization-0.3.1/crschem/model/straight_way.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/traffic_island.py` & `crossroads-schematization-0.3.1/crschem/model/traffic_island.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/model/turning_sidewalk.py` & `crossroads-schematization-0.3.1/crschem/model/turning_sidewalk.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/processing.py` & `crossroads-schematization-0.3.1/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/crossing-3-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/crossing-3-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/island-300-white.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/island-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/island-96-white.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/island-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/point-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/point-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/400/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.3.1/crschem/resources/400/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.3.1/crschem/resources/400/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/crossing-3-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/crossing-3-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/island-300-white.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/island-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/island-96-white.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/island-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/point-300.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/point-96.svg` & `crossroads-schematization-0.3.1/crschem/resources/500/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.3.1/crschem/resources/500/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.3.1/crschem/resources/500/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/crschem/utils.py` & `crossroads-schematization-0.3.1/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.3.0/setup.py` & `crossroads-schematization-0.3.1/setup.py`

 * *Files identical despite different names*

