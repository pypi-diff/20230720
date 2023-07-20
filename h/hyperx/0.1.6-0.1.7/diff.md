# Comparing `tmp/hyperx-0.1.6.tar.gz` & `tmp/hyperx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.6.tar", last modified: Thu Jul 20 18:49:09 2023, max compression
+gzip compressed data, was "hyperx-0.1.7.tar", last modified: Thu Jul 20 21:07:26 2023, max compression
```

## Comparing `hyperx-0.1.6.tar` & `hyperx-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.622119 hyperx-0.1.6/
--rw-rw-rw-   0        0        0      535 2023-07-20 18:49:09.621151 hyperx-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.580562 hyperx-0.1.6/hyperx/
--rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.6/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.607388 hyperx-0.1.6/hyperx/api/
--rw-rw-rw-   0        0        0   156811 2023-07-20 18:48:41.000000 hyperx-0.1.6/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.609605 hyperx-0.1.6/hyperx/api/types/
--rw-rw-rw-   0        0        0    23328 2023-07-20 18:48:20.000000 hyperx-0.1.6/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.616165 hyperx-0.1.6/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.620148 hyperx-0.1.6/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.6/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.605386 hyperx-0.1.6/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-07-20 18:39:47.000000 hyperx-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 18:49:09.622897 hyperx-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.667584 hyperx-0.1.7/
+-rw-rw-rw-   0        0        0      535 2023-07-20 21:07:26.667584 hyperx-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.634002 hyperx-0.1.7/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.7/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.653987 hyperx-0.1.7/hyperx/api/
+-rw-rw-rw-   0        0        0   156994 2023-07-20 20:55:24.000000 hyperx-0.1.7/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.655987 hyperx-0.1.7/hyperx/api/types/
+-rw-rw-rw-   0        0        0    23328 2023-07-20 20:27:34.000000 hyperx-0.1.7/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.660988 hyperx-0.1.7/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.7/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.7/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.7/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.665584 hyperx-0.1.7/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.7/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.7/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:26.650985 hyperx-0.1.7/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-20 21:07:26.000000 hyperx-0.1.7/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-20 21:07:26.000000 hyperx-0.1.7/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 21:07:26.000000 hyperx-0.1.7/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 21:07:26.000000 hyperx-0.1.7/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 21:07:26.000000 hyperx-0.1.7/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-07-20 19:43:55.000000 hyperx-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 21:07:26.668585 hyperx-0.1.7/setup.cfg
```

### Comparing `hyperx-0.1.6/PKG-INFO` & `hyperx-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.6
+Version: 0.1.7
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.6/hyperx/__init__.py` & `hyperx-0.1.7/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.6/hyperx/api/__init__.py` & `hyperx-0.1.7/hyperx/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -857,14 +857,17 @@
 class Vector3d:
 	'''
 	Represents a readonly 3D vector.
 	'''
 	def __init__(self, vector3d: _api.Vector3d):
 		self._Entity = vector3d
 
+	def Create_Vector3d(x: float, y: float, z: float):
+		return Vector3d(_api.Vector3d(x, y, z))
+
 	@property
 	def X(self) -> float:
 		return self._Entity.X
 
 	@property
 	def Y(self) -> float:
 		return self._Entity.Y
@@ -3373,14 +3376,17 @@
 class Vector2d:
 	'''
 	Represents a readonly 2D vector.
 	'''
 	def __init__(self, vector2d: _api.Vector2d):
 		self._Entity = vector2d
 
+	def Create_Vector2d(x: float, y: float):
+		return Vector2d(_api.Vector2d(x, y))
+
 	@property
 	def X(self) -> float:
 		return self._Entity.X
 
 	@property
 	def Y(self) -> float:
 		return self._Entity.Y
```

### Comparing `hyperx-0.1.6/hyperx/api/types/__init__.py` & `hyperx-0.1.7/hyperx/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.6/hyperx/library/find.py` & `hyperx-0.1.7/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.6/hyperx/library/library.py` & `hyperx-0.1.7/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.6/hyperx/utils/utils.py` & `hyperx-0.1.7/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.6/hyperx.egg-info/PKG-INFO` & `hyperx-0.1.7/hyperx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.6
+Version: 0.1.7
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.6/pyproject.toml` & `hyperx-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

