# Comparing `tmp/mcu-geo-utils-0.1.tar.gz` & `tmp/mcu-geo-utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcu-geo-utils-0.1.tar", last modified: Thu Jul 20 19:12:35 2023, max compression
+gzip compressed data, was "mcu-geo-utils-0.2.tar", last modified: Thu Jul 20 19:26:33 2023, max compression
```

## Comparing `mcu-geo-utils-0.1.tar` & `mcu-geo-utils-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:12:35.459407 mcu-geo-utils-0.1/
--rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.1/LICENSE
--rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.1/MANIFEST.in
--rw-r--r--   0 martincontreras   (501) staff       (20)      372 2023-07-20 19:12:35.459277 mcu-geo-utils-0.1/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      140 2023-07-20 16:07:16.000000 mcu-geo-utils-0.1/README.md
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:12:35.458495 mcu-geo-utils-0.1/mcu_geo_utils/
--rw-r--r--   0 martincontreras   (501) staff       (20)     1987 2023-07-20 15:54:16.000000 mcu-geo-utils-0.1/mcu_geo_utils/OSM.py
--rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.1/mcu_geo_utils/__init__.py
--rw-r--r--   0 martincontreras   (501) staff       (20)     3621 2023-07-20 15:51:36.000000 mcu-geo-utils-0.1/mcu_geo_utils/census.py
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:12:35.459109 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/
--rw-r--r--   0 martincontreras   (501) staff       (20)      372 2023-07-20 19:12:35.000000 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-20 19:12:35.000000 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/SOURCES.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-20 19:12:35.000000 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/dependency_links.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       60 2023-07-20 19:12:35.000000 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/requires.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-20 19:12:35.000000 mcu-geo-utils-0.1/mcu_geo_utils.egg-info/top_level.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-20 19:12:35.459448 mcu-geo-utils-0.1/setup.cfg
--rw-r--r--   0 martincontreras   (501) staff       (20)      564 2023-07-20 19:12:31.000000 mcu-geo-utils-0.1/setup.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:26:33.219116 mcu-geo-utils-0.2/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.2/LICENSE
+-rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.2/MANIFEST.in
+-rw-r--r--   0 martincontreras   (501) staff       (20)      423 2023-07-20 19:26:33.218981 mcu-geo-utils-0.2/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      140 2023-07-20 16:07:16.000000 mcu-geo-utils-0.2/README.md
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:26:33.218021 mcu-geo-utils-0.2/mcu_geo_utils/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     2045 2023-07-20 19:24:45.000000 mcu-geo-utils-0.2/mcu_geo_utils/OSM.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.2/mcu_geo_utils/__init__.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)     3621 2023-07-20 15:51:36.000000 mcu-geo-utils-0.2/mcu_geo_utils/census.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 19:26:33.218809 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/
+-rw-r--r--   0 martincontreras   (501) staff       (20)      423 2023-07-20 19:26:33.000000 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-20 19:26:33.000000 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-20 19:26:33.000000 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       60 2023-07-20 19:26:33.000000 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/requires.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-20 19:26:33.000000 mcu-geo-utils-0.2/mcu_geo_utils.egg-info/top_level.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-20 19:26:33.219163 mcu-geo-utils-0.2/setup.cfg
+-rw-r--r--   0 martincontreras   (501) staff       (20)      564 2023-07-20 19:26:19.000000 mcu-geo-utils-0.2/setup.py
```

### Comparing `mcu-geo-utils-0.1/LICENSE` & `mcu-geo-utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.1/mcu_geo_utils/OSM.py` & `mcu-geo-utils-0.2/mcu_geo_utils/OSM.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 @dataclass
 class OSM_geometry:
     """
         Point of interest in lat, long format that retrieves Open 
         Street Maps's features
 
         Args:
-            lat: center point latitude.
-            lon: center point longitude.
+            center_point: lat, long tuple.
+            tags: OSM tags (e.g. {"amenity":["cafe", "bar"]})
             radio: distance in meters to cover from the center point.
     """
-    center_point: int
+    center_point: tuple
     tags: dict
     radio: int = field(default=1000)
 
     def get_features_from_point(self):
         features = ox.features.features_from_point(
             self.center_point,
             dist=self.radio,
@@ -29,16 +29,18 @@
         graph = ox.graph.graph_from_point(
             self.center_point,
             dist=self.radio
         )
         return graph
 
     def get_basic_stats(self):
-        return pd.DataFrame(
-            ox.stats.basic_stats(self.graph)
+        return (
+            pd.DataFrame(
+                ox.stats.basic_stats(self.graph)
+            )
             .drop(
                 columns=[
                     "streets_per_node_proportions",
                     "streets_per_node_counts"
                     ]
             )  # we dont wanna use this columns at the moment
             .drop_duplicates()
```

### Comparing `mcu-geo-utils-0.1/mcu_geo_utils/census.py` & `mcu-geo-utils-0.2/mcu_geo_utils/census.py`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.1/setup.py` & `mcu-geo-utils-0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='mcu-geo-utils',
-    version='0.1',
+    version='0.2',
     author='Martin Conur',
     author_email='martincontrerasur@gmail.com',
     packages=['mcu_geo_utils'],
     scripts=[],
-   # url='http://pypi.python.org/pypi/apiweather/',
+    url='https://pypi.org/project/mcu-geo-utils/',
     license='MIT',
     description='variaty of geo-related tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "pandas >= 1.5.1",
         "geopandas == 0.12.1",
         "shapely == 2.0.1",
         "osmnx == 1.5.1"
     ],
-)
+)
```

