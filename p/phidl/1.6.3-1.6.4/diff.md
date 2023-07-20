# Comparing `tmp/phidl-1.6.3.tar.gz` & `tmp/phidl-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phidl-1.6.3.tar", last modified: Fri Feb 10 03:35:19 2023, max compression
+gzip compressed data, was "phidl-1.6.4.tar", last modified: Thu Jul 20 18:11:35 2023, max compression
```

## Comparing `phidl-1.6.3.tar` & `phidl-1.6.4.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 amcc       (501) staff       (20)        0 2023-02-10 03:35:19.884324 phidl-1.6.3/
--rw-r--r--   0 amcc       (501) staff       (20)     1074 2022-04-27 04:45:52.000000 phidl-1.6.3/LICENSE
--rw-r--r--   0 amcc       (501) staff       (20)       16 2021-09-20 00:12:06.000000 phidl-1.6.3/MANIFEST.in
--rw-r--r--   0 amcc       (501) staff       (20)     7108 2023-02-10 03:35:19.884498 phidl-1.6.3/PKG-INFO
--rw-r--r--   0 amcc       (501) staff       (20)     6888 2023-02-10 03:12:57.000000 phidl-1.6.3/README.md
-drwxr-xr-x   0 amcc       (501) staff       (20)        0 2023-02-10 03:35:19.881178 phidl-1.6.3/phidl/
--rw-r--r--   0 amcc       (501) staff       (20)      541 2022-03-23 16:24:17.000000 phidl-1.6.3/phidl/__init__.py
--rw-r--r--   0 amcc       (501) staff       (20)    38409 2022-03-23 16:24:17.000000 phidl-1.6.3/phidl/constants.py
--rw-r--r--   0 amcc       (501) staff       (20)   107252 2023-02-10 03:15:57.000000 phidl-1.6.3/phidl/device_layout.py
--rw-r--r--   0 amcc       (501) staff       (20)     8052 2022-07-25 02:45:28.000000 phidl-1.6.3/phidl/font.py
--rw-r--r--   0 amcc       (501) staff       (20)   188483 2023-02-10 02:58:01.000000 phidl-1.6.3/phidl/geometry.py
--rw-r--r--   0 amcc       (501) staff       (20)    15306 2023-02-10 02:55:49.000000 phidl-1.6.3/phidl/path.py
--rw-r--r--   0 amcc       (501) staff       (20)    47548 2022-03-23 16:24:17.000000 phidl-1.6.3/phidl/phidl_tutorial_example.py
--rw-r--r--   0 amcc       (501) staff       (20)    35769 2022-07-25 02:45:28.000000 phidl-1.6.3/phidl/quickplotter.py
--rw-r--r--   0 amcc       (501) staff       (20)    69245 2022-07-25 02:45:28.000000 phidl-1.6.3/phidl/routing.py
--rw-r--r--   0 amcc       (501) staff       (20)     8945 2022-07-25 02:45:28.000000 phidl-1.6.3/phidl/utilities.py
-drwxr-xr-x   0 amcc       (501) staff       (20)        0 2023-02-10 03:35:19.883849 phidl-1.6.3/phidl.egg-info/
--rw-r--r--   0 amcc       (501) staff       (20)     7108 2023-02-10 03:35:19.000000 phidl-1.6.3/phidl.egg-info/PKG-INFO
--rw-r--r--   0 amcc       (501) staff       (20)      388 2023-02-10 03:35:19.000000 phidl-1.6.3/phidl.egg-info/SOURCES.txt
--rw-r--r--   0 amcc       (501) staff       (20)        1 2023-02-10 03:35:19.000000 phidl-1.6.3/phidl.egg-info/dependency_links.txt
--rw-r--r--   0 amcc       (501) staff       (20)       28 2023-02-10 03:35:19.000000 phidl-1.6.3/phidl.egg-info/requires.txt
--rw-r--r--   0 amcc       (501) staff       (20)        6 2023-02-10 03:35:19.000000 phidl-1.6.3/phidl.egg-info/top_level.txt
--rw-r--r--   0 amcc       (501) staff       (20)      250 2023-02-10 03:35:19.885121 phidl-1.6.3/setup.cfg
--rw-r--r--   0 amcc       (501) staff       (20)      765 2023-02-10 03:34:39.000000 phidl-1.6.3/setup.py
+drwxr-xr-x   0 amccaugh   (501) staff       (20)        0 2023-07-20 18:11:35.914297 phidl-1.6.4/
+-rw-r--r--   0 amccaugh   (501) staff       (20)     1074 2023-06-27 02:39:05.000000 phidl-1.6.4/LICENSE
+-rw-r--r--   0 amccaugh   (501) staff       (20)       16 2023-06-27 02:39:05.000000 phidl-1.6.4/MANIFEST.in
+-rw-r--r--   0 amccaugh   (501) staff       (20)     6494 2023-07-20 18:11:35.914376 phidl-1.6.4/PKG-INFO
+-rw-r--r--   0 amccaugh   (501) staff       (20)     6311 2023-07-20 18:06:17.000000 phidl-1.6.4/README.md
+drwxr-xr-x   0 amccaugh   (501) staff       (20)        0 2023-07-20 18:11:35.912653 phidl-1.6.4/phidl/
+-rw-r--r--   0 amccaugh   (501) staff       (20)      541 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/__init__.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    38409 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/constants.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)   107357 2023-07-20 18:06:17.000000 phidl-1.6.4/phidl/device_layout.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)     8052 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/font.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)   188610 2023-07-20 18:07:00.000000 phidl-1.6.4/phidl/geometry.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    15306 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/path.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    47548 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/phidl_tutorial_example.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    35769 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/quickplotter.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    69245 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/routing.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)     8945 2023-06-27 02:39:05.000000 phidl-1.6.4/phidl/utilities.py
+drwxr-xr-x   0 amccaugh   (501) staff       (20)        0 2023-07-20 18:11:35.913273 phidl-1.6.4/phidl.egg-info/
+-rw-r--r--   0 amccaugh   (501) staff       (20)     6494 2023-07-20 18:11:35.000000 phidl-1.6.4/phidl.egg-info/PKG-INFO
+-rw-r--r--   0 amccaugh   (501) staff       (20)      473 2023-07-20 18:11:35.000000 phidl-1.6.4/phidl.egg-info/SOURCES.txt
+-rw-r--r--   0 amccaugh   (501) staff       (20)        1 2023-07-20 18:11:35.000000 phidl-1.6.4/phidl.egg-info/dependency_links.txt
+-rw-r--r--   0 amccaugh   (501) staff       (20)       28 2023-07-20 18:11:35.000000 phidl-1.6.4/phidl.egg-info/requires.txt
+-rw-r--r--   0 amccaugh   (501) staff       (20)        6 2023-07-20 18:11:35.000000 phidl-1.6.4/phidl.egg-info/top_level.txt
+-rw-r--r--   0 amccaugh   (501) staff       (20)      250 2023-07-20 18:11:35.914859 phidl-1.6.4/setup.cfg
+-rw-r--r--   0 amccaugh   (501) staff       (20)      765 2023-07-20 18:06:17.000000 phidl-1.6.4/setup.py
+drwxr-xr-x   0 amccaugh   (501) staff       (20)        0 2023-07-20 18:11:35.914085 phidl-1.6.4/tests/
+-rw-r--r--   0 amccaugh   (501) staff       (20)    11095 2023-06-27 02:39:05.000000 phidl-1.6.4/tests/test_device.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)    10029 2023-06-27 03:23:46.000000 phidl-1.6.4/tests/test_geometry.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)     5717 2023-06-27 02:39:05.000000 phidl-1.6.4/tests/test_path.py
+-rw-r--r--   0 amccaugh   (501) staff       (20)     5812 2023-06-27 02:39:05.000000 phidl-1.6.4/tests/test_routing.py
```

### Comparing `phidl-1.6.3/LICENSE` & `phidl-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/PKG-INFO` & `phidl-1.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 Metadata-Version: 2.1
 Name: phidl
-Version: 1.6.3
+Version: 1.6.4
 Summary: PHIDL
 Author: Adam McCaughan
 Author-email: amccaugh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pytest](https://github.com/amccaugh/phidl/actions/workflows/pytest.yml/badge.svg)](https://github.com/amccaugh/phidl/actions/workflows/pytest.yml)
 [![pre-commit](https://github.com/amccaugh/phidl/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/amccaugh/phidl/actions/workflows/pre-commit.yml)
 
 # PHIDL
 GDS scripting for Python that's intuitive, fast, and powerful.
 
 - [**Installation / requirements**](#installation--requirements)
 - [**Tutorial + examples**](https://phidl.readthedocs.io/en/latest/tutorials.html) (or [try an interactive notebook](https://mybinder.org/v2/gh/amccaugh/phidl/master?filepath=phidl_tutorial_example.ipynb))
 - [**Geometry library + function documentation**](https://phidl.readthedocs.io/en/latest/geometry_reference.html)
-- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on Feb 9, 2023)
-    - Huge new routing rewrite for `phidl.routing`, including automatic manhattan routing with custom cross-sections!  See [the routing documentation](https://phidl.readthedocs.io/en/latest/tutorials/routing.html) for details. Big thanks to Jeffrey Holzgrafe @jolzgrafe for this contribution
-    - `Path`s can now be used to produce sharp angles, in addition to smooth bends. See [the Path documentation](https://phidl.readthedocs.io/en/latest/tutorials/waveguides.html#Sharp/angular-paths)
-
-```python
-import phidl.routing as pr
-D_left = pr.route_smooth(port1, port2, radius=8, layer = 2)
-D_right = pr.route_sharp(port1, port2, layer = 2)
-```
-
-![phidl example image](https://amccaugh.github.io/phidl/readme_9.png)
+- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on July 20, 2023)
+    - New `pg.fill_rectangle()` [examples and documentation](https://phidl.readthedocs.io/en/latest/geometry_reference.html#Fill-tool)
 
 # Citation
 
 If you found PHIDL useful, please consider citing it in (just one!) of your publications -- we appreciate it greatly. ([BibTeX](https://raw.githubusercontent.com/amccaugh/phidl/master/CITATION.bib))
  - McCaughan, A. N., et. al. PHIDL: Python-based layout and geometry creation for nanolithography. *J. Vac. Sci. Technol. B* 39, 062601 (2021). http://dx.doi.org/10.1116/6.0001203
 
 # Gallery
@@ -100,9 +89,7 @@
 There are also handy functions to help pack shapes into as small an area as possible:
 
 ```
 pg.packer(D_list, spacing = 1.25, aspect_ratio = (2,1))
 ```
 
 ![phidl example image](https://amccaugh.github.io/phidl/packer.png)
-
-
```

### Comparing `phidl-1.6.3/README.md` & `phidl-1.6.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,16 @@
 
 # PHIDL
 GDS scripting for Python that's intuitive, fast, and powerful.
 
 - [**Installation / requirements**](#installation--requirements)
 - [**Tutorial + examples**](https://phidl.readthedocs.io/en/latest/tutorials.html) (or [try an interactive notebook](https://mybinder.org/v2/gh/amccaugh/phidl/master?filepath=phidl_tutorial_example.ipynb))
 - [**Geometry library + function documentation**](https://phidl.readthedocs.io/en/latest/geometry_reference.html)
-- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on Feb 9, 2023)
-    - Huge new routing rewrite for `phidl.routing`, including automatic manhattan routing with custom cross-sections!  See [the routing documentation](https://phidl.readthedocs.io/en/latest/tutorials/routing.html) for details. Big thanks to Jeffrey Holzgrafe @jolzgrafe for this contribution
-    - `Path`s can now be used to produce sharp angles, in addition to smooth bends. See [the Path documentation](https://phidl.readthedocs.io/en/latest/tutorials/waveguides.html#Sharp/angular-paths)
-
-```python
-import phidl.routing as pr
-D_left = pr.route_smooth(port1, port2, radius=8, layer = 2)
-D_right = pr.route_sharp(port1, port2, layer = 2)
-```
-
-![phidl example image](https://amccaugh.github.io/phidl/readme_9.png)
+- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on July 20, 2023)
+    - New `pg.fill_rectangle()` [examples and documentation](https://phidl.readthedocs.io/en/latest/geometry_reference.html#Fill-tool)
 
 # Citation
 
 If you found PHIDL useful, please consider citing it in (just one!) of your publications -- we appreciate it greatly. ([BibTeX](https://raw.githubusercontent.com/amccaugh/phidl/master/CITATION.bib))
  - McCaughan, A. N., et. al. PHIDL: Python-based layout and geometry creation for nanolithography. *J. Vac. Sci. Technol. B* 39, 062601 (2021). http://dx.doi.org/10.1116/6.0001203
 
 # Gallery
```

### Comparing `phidl-1.6.3/phidl/__init__.py` & `phidl-1.6.4/phidl/__init__.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/constants.py` & `phidl-1.6.4/phidl/constants.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/device_layout.py` & `phidl-1.6.4/phidl/device_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,20 @@
 
 import gdspy
 
 # Remove this once gdspy fully deprecates current_library
 import gdspy.library
 import numpy as np
 from numpy import cos, mod, pi, sin, sqrt
-from numpy.linalg import norm
 
 from phidl.constants import _CSS3_NAMES_TO_HEX
 
 gdspy.library.use_current_library = False
 
-__version__ = "1.6.3"
+__version__ = "1.6.4"
 
 
 # ==============================================================================
 # Useful transformation functions
 # ==============================================================================
 
 
@@ -107,31 +106,34 @@
     p2 : array-like[2]
         Coordinates of the end of the reflecting line.
 
     Returns
     -------
     A new set of points that are reflected across ``p1`` and ``p2``.
     """
-    # From http://math.stackexchange.com/questions/11515/point-reflection-across-a-line
-    points = np.array(points)
     p1 = np.array(p1)
     p2 = np.array(p2)
-    if np.asarray(points).ndim == 1:
-        return (
-            2 * (p1 + (p2 - p1) * np.dot((p2 - p1), (points - p1)) / norm(p2 - p1) ** 2)
-            - points
-        )
-    if np.asarray(points).ndim == 2:
-        return np.array(
-            [
-                2 * (p1 + (p2 - p1) * np.dot((p2 - p1), (p - p1)) / norm(p2 - p1) ** 2)
-                - p
-                for p in points
-            ]
-        )
+    line_vec = p2 - p1
+    line_vec_norm = np.linalg.norm(line_vec, axis=-1, keepdims=True) ** 2
+
+    # Checking if the input is 1D and adding an extra dimension if it is
+    input_was_1d = np.asarray(points).ndim == 1
+    if input_was_1d:
+        points = np.array([points])
+
+    reflected_points_projection = (
+        np.sum(line_vec * (points - p1), axis=-1, keepdims=True) / line_vec_norm
+    )
+    reflected_points = 2 * (p1 + line_vec * reflected_points_projection) - points
+
+    # If the input was 1D, remove the extra dimension from the output
+    if input_was_1d:
+        reflected_points = np.squeeze(reflected_points, axis=0)
+
+    return reflected_points
 
 
 def _is_iterable(items):
     """Checks if the passed variable is iterable.
 
     Parameters
     ----------
```

### Comparing `phidl-1.6.3/phidl/font.py` & `phidl-1.6.4/phidl/font.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/geometry.py` & `phidl-1.6.4/phidl/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -6536,5246 +6536,5254 @@
 00019870: 6565 6e3b 2069 6620 2046 616c 7365 2c20  een; if  False, 
 00019880: 656c 656d 656e 7473 2061 7265 2073 7061  elements are spa
 00019890: 6365 6420 6576 656e 6c79 2061 6c6f 6e67  ced evenly along
 000198a0: 2061 2067 7269 642e 0a20 2020 2073 6861   a grid..    sha
 000198b0: 7065 203a 2061 7272 6179 2d6c 696b 655b  pe : array-like[
 000198c0: 325d 0a20 2020 2020 2020 2078 2c20 7920  2].        x, y 
 000198d0: 7368 6170 6520 6f66 2074 6865 2067 7269  shape of the gri
-000198e0: 6420 2873 6565 206e 702e 7265 7368 6170  d (see np.reshap
-000198f0: 6529 2e20 4966 206e 6f20 7368 6170 6520  e). If no shape 
-00019900: 6973 2067 6976 656e 2061 6e64 2074 6865  is given and the
-00019910: 0a20 2020 2020 2020 206c 6973 7420 6973  .        list is
-00019920: 2031 442c 2074 6865 206f 7574 7075 7420   1D, the output 
-00019930: 6973 2061 7320 6966 206e 702e 7265 7368  is as if np.resh
-00019940: 6170 6520 7765 7265 2072 756e 2077 6974  ape were run wit
-00019950: 6820 2831 2c20 2d31 292e 0a20 2020 2061  h (1, -1)..    a
-00019960: 6c69 676e 5f78 203a 207b 2778 272c 2027  lign_x : {'x', '
-00019970: 786d 696e 272c 2027 786d 6178 277d 0a20  xmin', 'xmax'}. 
-00019980: 2020 2020 2020 2057 6869 6368 2065 6467         Which edg
-00019990: 6520 746f 2070 6572 666f 726d 2074 6865  e to perform the
-000199a0: 2078 2028 636f 6c75 6d6e 2920 616c 6967   x (column) alig
-000199b0: 6e6d 656e 7420 616c 6f6e 670a 2020 2020  nment along.    
-000199c0: 616c 6967 6e5f 7920 3a20 7b27 7927 2c20  align_y : {'y', 
-000199d0: 2779 6d69 6e27 2c20 2779 6d61 7827 7d0a  'ymin', 'ymax'}.
-000199e0: 2020 2020 2020 2020 5768 6963 6820 6564          Which ed
-000199f0: 6765 2074 6f20 7065 7266 6f72 6d20 7468  ge to perform th
-00019a00: 6520 7920 2872 6f77 2920 616c 6967 6e6d  e y (row) alignm
-00019a10: 656e 7420 616c 6f6e 670a 2020 2020 6564  ent along.    ed
-00019a20: 6765 5f78 203a 207b 2778 272c 2027 786d  ge_x : {'x', 'xm
-00019a30: 696e 272c 2027 786d 6178 277d 0a20 2020  in', 'xmax'}.   
-00019a40: 2020 2020 2057 6869 6368 2065 6467 6520       Which edge 
-00019a50: 746f 2070 6572 666f 726d 2074 6865 2078  to perform the x
-00019a60: 2028 636f 6c75 6d6e 2920 6469 7374 7269   (column) distri
-00019a70: 6275 7469 6f6e 2061 6c6f 6e67 2028 756e  bution along (un
-00019a80: 7573 6564 2069 660a 2020 2020 2020 2020  used if.        
-00019a90: 7365 7061 7261 7469 6f6e 203d 3d20 5472  separation == Tr
-00019aa0: 7565 290a 2020 2020 6564 6765 5f79 203a  ue).    edge_y :
-00019ab0: 207b 2779 272c 2027 796d 696e 272c 2027   {'y', 'ymin', '
-00019ac0: 796d 6178 277d 0a20 2020 2020 2020 2057  ymax'}.        W
-00019ad0: 6869 6368 2065 6467 6520 746f 2070 6572  hich edge to per
-00019ae0: 666f 726d 2074 6865 2079 2028 726f 7729  form the y (row)
-00019af0: 2064 6973 7472 6962 7574 696f 6e20 616c   distribution al
-00019b00: 6f6e 6720 2875 6e75 7365 6420 6966 0a20  ong (unused if. 
-00019b10: 2020 2020 2020 2073 6570 6172 6174 696f         separatio
-00019b20: 6e20 3d3d 2054 7275 6529 0a0a 2020 2020  n == True)..    
-00019b30: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00019b40: 2d2d 2d0a 2020 2020 6465 7669 6365 5f6d  ---.    device_m
-00019b50: 6174 7269 7820 3a20 4465 7669 6365 0a20  atrix : Device. 
-00019b60: 2020 2020 2020 2041 2044 6576 6963 6520         A Device 
-00019b70: 636f 6e74 6169 6e69 6e67 2061 6c6c 2074  containing all t
-00019b80: 6865 2044 6576 6963 6573 2069 6e20 6064  he Devices in `d
-00019b90: 6576 6963 655f 6c69 7374 6020 696e 2061  evice_list` in a
-00019ba0: 2067 7269 642e 0a20 2020 2022 2222 0a0a   grid..    """..
-00019bb0: 2020 2020 2320 4368 616e 6765 2028 792c      # Change (y,
-00019bc0: 7829 2073 6861 7065 2074 6f20 2878 2c79  x) shape to (x,y
-00019bd0: 2920 7368 6170 650a 2020 2020 7368 6170  ) shape.    shap
-00019be0: 6520 3d20 7368 6170 655b 3a3a 2d31 5d0a  e = shape[::-1].
-00019bf0: 2020 2020 6465 7669 6365 5f61 7272 6179      device_array
-00019c00: 203d 206e 702e 6173 6172 7261 7928 6465   = np.asarray(de
-00019c10: 7669 6365 5f6c 6973 7429 0a20 2020 2023  vice_list).    #
-00019c20: 2043 6865 636b 2061 7267 756d 656e 7473   Check arguments
-00019c30: 0a20 2020 2069 6620 6465 7669 6365 5f61  .    if device_a
-00019c40: 7272 6179 2e6e 6469 6d20 6e6f 7420 696e  rray.ndim not in
-00019c50: 2028 312c 2032 293a 0a20 2020 2020 2020   (1, 2):.       
-00019c60: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00019c70: 7228 225b 5048 4944 4c5d 2067 7269 6428  r("[PHIDL] grid(
-00019c80: 2920 5468 6520 6465 7669 6365 5f6c 6973  ) The device_lis
-00019c90: 7420 6e65 6564 7320 746f 2062 6520 3144  t needs to be 1D
-00019ca0: 206f 7220 3244 2e22 290a 2020 2020 6966   or 2D.").    if
-00019cb0: 2073 6861 7065 2069 7320 6e6f 7420 4e6f   shape is not No
-00019cc0: 6e65 2061 6e64 206c 656e 2873 6861 7065  ne and len(shape
-00019cd0: 2920 213d 2032 3a0a 2020 2020 2020 2020  ) != 2:.        
-00019ce0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00019cf0: 280a 2020 2020 2020 2020 2020 2020 225b  (.            "[
-00019d00: 5048 4944 4c5d 2067 7269 6428 2920 7368  PHIDL] grid() sh
-00019d10: 6170 6520 6172 6775 6d65 6e74 206d 7573  ape argument mus
-00019d20: 7420 6265 204e 6f6e 6520 6f72 220a 2020  t be None or".  
-00019d30: 2020 2020 2020 2020 2020 2b20 2220 6861            + " ha
-00019d40: 7665 2061 206c 656e 6774 6820 6f66 2032  ve a length of 2
-00019d50: 2c20 666f 7220 6578 616d 706c 6520 7368  , for example sh
-00019d60: 6170 653d 2834 2c36 2922 0a20 2020 2020  ape=(4,6)".     
-00019d70: 2020 2029 0a0a 2020 2020 2320 4368 6563     )..    # Chec
-00019d80: 6b20 7468 6174 2073 6861 7065 2069 7320  k that shape is 
-00019d90: 7661 6c69 6420 616e 6420 7265 7368 6170  valid and reshap
-00019da0: 6520 6172 7261 7920 6966 206e 6565 6465  e array if neede
-00019db0: 640a 2020 2020 6966 2028 7368 6170 6520  d.    if (shape 
-00019dc0: 6973 204e 6f6e 6529 2061 6e64 2028 6465  is None) and (de
-00019dd0: 7669 6365 5f61 7272 6179 2e6e 6469 6d20  vice_array.ndim 
-00019de0: 3d3d 2032 293a 2020 2320 416c 7265 6164  == 2):  # Alread
-00019df0: 7920 696e 2064 6573 6972 6564 2073 6861  y in desired sha
-00019e00: 7065 0a20 2020 2020 2020 2073 6861 7065  pe.        shape
-00019e10: 203d 2064 6576 6963 655f 6172 7261 792e   = device_array.
-00019e20: 7368 6170 650a 2020 2020 656c 6966 2028  shape.    elif (
-00019e30: 7368 6170 6520 6973 204e 6f6e 6529 2061  shape is None) a
-00019e40: 6e64 2028 6465 7669 6365 5f61 7272 6179  nd (device_array
-00019e50: 2e6e 6469 6d20 3d3d 2031 293a 0a20 2020  .ndim == 1):.   
-00019e60: 2020 2020 2073 6861 7065 203d 2028 6465       shape = (de
-00019e70: 7669 6365 5f61 7272 6179 2e73 697a 652c  vice_array.size,
-00019e80: 202d 3129 0a20 2020 2065 6c69 6620 3020   -1).    elif 0 
-00019e90: 3c20 7368 6170 655b 305d 202a 2073 6861  < shape[0] * sha
-00019ea0: 7065 5b31 5d20 3c20 6465 7669 6365 5f61  pe[1] < device_a
-00019eb0: 7272 6179 2e73 697a 653a 0a20 2020 2020  rray.size:.     
-00019ec0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00019ed0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00019ee0: 2022 5b50 4849 444c 5d20 6772 6964 2829   "[PHIDL] grid()
-00019ef0: 2054 6865 2073 6861 7065 2069 7320 746f   The shape is to
-00019f00: 6f20 736d 616c 6c20 666f 7220 616c 6c20  o small for all 
-00019f10: 7468 6520 6974 656d 7320 696e 2064 6576  the items in dev
-00019f20: 6963 655f 6c69 7374 220a 2020 2020 2020  ice_list".      
-00019f30: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-00019f40: 2020 2020 2020 6966 206e 702e 6d69 6e28        if np.min(
-00019f50: 7368 6170 6529 203d 3d20 2d31 3a0a 2020  shape) == -1:.  
-00019f60: 2020 2020 2020 2020 2020 6d61 785f 7368            max_sh
-00019f70: 6170 6520 3d20 6e70 2e6d 6178 2873 6861  ape = np.max(sha
-00019f80: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
-00019f90: 6d69 6e5f 6465 7669 6365 7320 3d20 696e  min_devices = in
-00019fa0: 7428 6e70 2e63 6569 6c28 6465 7669 6365  t(np.ceil(device
-00019fb0: 5f61 7272 6179 2e73 697a 6520 2f20 6d61  _array.size / ma
-00019fc0: 785f 7368 6170 6529 202a 206d 6178 5f73  x_shape) * max_s
-00019fd0: 6861 7065 290a 2020 2020 2020 2020 2020  hape).          
-00019fe0: 2020 6578 7472 615f 6465 7669 6365 7320    extra_devices 
-00019ff0: 3d20 6d69 6e5f 6465 7669 6365 7320 2d20  = min_devices - 
-0001a000: 6465 7669 6365 5f61 7272 6179 2e73 697a  device_array.siz
-0001a010: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-0001a020: 2020 2020 2020 2020 2020 2020 6578 7472              extr
-0001a030: 615f 6465 7669 6365 7320 3d20 7368 6170  a_devices = shap
-0001a040: 655b 305d 202a 2073 6861 7065 5b31 5d20  e[0] * shape[1] 
-0001a050: 2d20 6465 7669 6365 5f61 7272 6179 2e73  - device_array.s
-0001a060: 697a 650a 2020 2020 2020 2020 6966 2065  ize.        if e
-0001a070: 7874 7261 5f64 6576 6963 6573 2021 3d20  xtra_devices != 
-0001a080: 303a 0a20 2020 2020 2020 2020 2020 2064  0:.            d
-0001a090: 6576 6963 655f 6172 7261 7920 3d20 6e70  evice_array = np
-0001a0a0: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-0001a0b0: 2020 2020 2020 2020 2064 6576 6963 655f           device_
-0001a0c0: 6172 7261 792c 0a20 2020 2020 2020 2020  array,.         
-0001a0d0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0001a0e0: 2020 2020 2020 2020 2020 2020 204e 6f6e               Non
-0001a0f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001a100: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-0001a110: 2020 2020 202a 2065 7874 7261 5f64 6576       * extra_dev
-0001a120: 6963 6573 2c0a 2020 2020 2020 2020 2020  ices,.          
-0001a130: 2020 290a 2020 2020 6465 7669 6365 5f61    ).    device_a
-0001a140: 7272 6179 203d 206e 702e 7265 7368 6170  rray = np.reshap
-0001a150: 6528 6465 7669 6365 5f61 7272 6179 2c20  e(device_array, 
-0001a160: 7368 6170 6529 0a0a 2020 2020 2320 4372  shape)..    # Cr
-0001a170: 6561 7465 2061 2062 6c61 6e6b 2044 6576  eate a blank Dev
-0001a180: 6963 6520 616e 6420 7265 6665 7265 6e63  ice and referenc
-0001a190: 6520 616c 6c20 7468 6520 4465 7669 6365  e all the Device
-0001a1a0: 7320 696e 2069 740a 2020 2020 4420 3d20  s in it.    D = 
-0001a1b0: 4465 7669 6365 2822 6772 6964 2229 0a20  Device("grid"). 
-0001a1c0: 2020 2072 6566 5f61 7272 6179 203d 206e     ref_array = n
-0001a1d0: 702e 656d 7074 7928 6465 7669 6365 5f61  p.empty(device_a
-0001a1e0: 7272 6179 2e73 6861 7065 2c20 6474 7970  rray.shape, dtyp
-0001a1f0: 653d 6f62 6a65 6374 290a 2020 2020 6475  e=object).    du
-0001a200: 6d6d 7920 3d20 4465 7669 6365 2829 0a20  mmy = Device(). 
-0001a210: 2020 2066 6f72 2069 6478 2c20 6420 696e     for idx, d in
-0001a220: 206e 702e 6e64 656e 756d 6572 6174 6528   np.ndenumerate(
-0001a230: 6465 7669 6365 5f61 7272 6179 293a 0a20  device_array):. 
-0001a240: 2020 2020 2020 2069 6620 6420 6973 206e         if d is n
-0001a250: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001a260: 2020 2020 2072 6566 5f61 7272 6179 5b69       ref_array[i
-0001a270: 6478 5d20 3d20 4420 3c3c 2064 0a20 2020  dx] = D << d.   
-0001a280: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001a290: 2020 2020 2020 2072 6566 5f61 7272 6179         ref_array
-0001a2a0: 5b69 6478 5d20 3d20 4420 3c3c 2064 756d  [idx] = D << dum
-0001a2b0: 6d79 2020 2320 4372 6561 7465 2064 756d  my  # Create dum
-0001a2c0: 6d79 2064 6576 6963 6573 0a0a 2020 2020  my devices..    
-0001a2d0: 726f 7773 203d 205b 4772 6f75 7028 7265  rows = [Group(re
-0001a2e0: 665f 6172 7261 795b 6e2c 203a 5d29 2066  f_array[n, :]) f
-0001a2f0: 6f72 206e 2069 6e20 7261 6e67 6528 7265  or n in range(re
-0001a300: 665f 6172 7261 792e 7368 6170 655b 305d  f_array.shape[0]
-0001a310: 295d 0a20 2020 2063 6f6c 7320 3d20 5b47  )].    cols = [G
-0001a320: 726f 7570 2872 6566 5f61 7272 6179 5b3a  roup(ref_array[:
-0001a330: 2c20 6e5d 2920 666f 7220 6e20 696e 2072  , n]) for n in r
-0001a340: 616e 6765 2872 6566 5f61 7272 6179 2e73  ange(ref_array.s
-0001a350: 6861 7065 5b31 5d29 5d0a 0a20 2020 2023  hape[1])]..    #
-0001a360: 2041 6c69 676e 2072 6f77 7320 616e 6420   Align rows and 
-0001a370: 636f 6c75 6d6e 7320 696e 6465 7065 6e64  columns independ
-0001a380: 656e 746c 790a 2020 2020 666f 7220 6e2c  ently.    for n,
-0001a390: 2072 2069 6e20 656e 756d 6572 6174 6528   r in enumerate(
-0001a3a0: 726f 7773 293a 0a20 2020 2020 2020 2072  rows):.        r
-0001a3b0: 2e61 6c69 676e 2861 6c69 676e 6d65 6e74  .align(alignment
-0001a3c0: 3d61 6c69 676e 5f79 290a 2020 2020 666f  =align_y).    fo
-0001a3d0: 7220 6e2c 2063 2069 6e20 656e 756d 6572  r n, c in enumer
-0001a3e0: 6174 6528 636f 6c73 293a 0a20 2020 2020  ate(cols):.     
-0001a3f0: 2020 2063 2e61 6c69 676e 2861 6c69 676e     c.align(align
-0001a400: 6d65 6e74 3d61 6c69 676e 5f78 290a 0a20  ment=align_x).. 
-0001a410: 2020 2023 2044 6973 7472 6962 7574 6520     # Distribute 
-0001a420: 726f 7773 2061 6e64 2063 6f6c 756d 6e73  rows and columns
-0001a430: 0a20 2020 2047 726f 7570 2863 6f6c 7329  .    Group(cols)
-0001a440: 2e64 6973 7472 6962 7574 6528 0a20 2020  .distribute(.   
-0001a450: 2020 2020 2064 6972 6563 7469 6f6e 3d22       direction="
-0001a460: 7822 2c20 7370 6163 696e 673d 7370 6163  x", spacing=spac
-0001a470: 696e 675b 305d 2c20 7365 7061 7261 7469  ing[0], separati
-0001a480: 6f6e 3d73 6570 6172 6174 696f 6e2c 2065  on=separation, e
-0001a490: 6467 653d 6564 6765 5f78 0a20 2020 2029  dge=edge_x.    )
-0001a4a0: 0a20 2020 2047 726f 7570 2872 6f77 735b  .    Group(rows[
-0001a4b0: 3a3a 2d31 5d29 2e64 6973 7472 6962 7574  ::-1]).distribut
-0001a4c0: 6528 0a20 2020 2020 2020 2064 6972 6563  e(.        direc
-0001a4d0: 7469 6f6e 3d22 7922 2c20 7370 6163 696e  tion="y", spacin
-0001a4e0: 673d 7370 6163 696e 675b 315d 2c20 7365  g=spacing[1], se
-0001a4f0: 7061 7261 7469 6f6e 3d73 6570 6172 6174  paration=separat
-0001a500: 696f 6e2c 2065 6467 653d 6564 6765 5f79  ion, edge=edge_y
-0001a510: 0a20 2020 2029 0a0a 2020 2020 2320 7265  .    )..    # re
-0001a520: 7475 726e 2064 6576 6963 655f 6d61 7472  turn device_matr
-0001a530: 6978 0a20 2020 2072 6574 7572 6e20 440a  ix.    return D.
-0001a540: 0a0a 6465 6620 5f70 6172 616d 6574 6572  ..def _parameter
-0001a550: 5f63 6f6d 6269 6e61 7469 6f6e 7328 7061  _combinations(pa
-0001a560: 7261 6d65 7465 7273 5f64 6963 7429 3a0a  rameters_dict):.
-0001a570: 2020 2020 2222 2243 7265 6174 6573 2070      """Creates p
-0001a580: 6172 616d 6574 6572 2063 6f6d 6269 6e61  arameter combina
-0001a590: 7469 6f6e 7320 6672 6f6d 2061 2064 6963  tions from a dic
-0001a5a0: 7420 6669 6c6c 6564 2077 6974 6820 6c69  t filled with li
-0001a5b0: 7374 2076 616c 7565 732c 2065 2e67 2e0a  st values, e.g..
-0001a5c0: 2020 2020 7061 7261 6d65 7465 7273 5f64      parameters_d
-0001a5d0: 6963 7420 3d20 7b0a 2020 2020 2020 2020  ict = {.        
-0001a5e0: 2777 6964 7468 2720 3a20 5b30 2e31 2c30  'width' : [0.1,0
-0001a5f0: 2e32 5d2c 0a20 2020 2020 2020 2027 6c65  .2],.        'le
-0001a600: 6e67 7468 2720 3a20 5b34 2c35 2c36 5d2c  ngth' : [4,5,6],
-0001a610: 0a20 2020 2020 2020 2027 6865 6967 6874  .        'height
-0001a620: 2720 3a20 5b32 325d 0a20 2020 2020 2020  ' : [22].       
-0001a630: 207d 0a20 2020 2057 696c 6c20 7072 6f64   }.    Will prod
-0001a640: 7563 6520 6120 6c69 7374 206f 6620 6469  uce a list of di
-0001a650: 6374 696f 6e61 7269 6573 2c20 6561 6368  ctionaries, each
-0001a660: 206f 6620 7768 6963 6820 6361 6e20 6265   of which can be
-0001a670: 2075 7365 6420 6173 206b 7761 7267 7320   used as kwargs 
-0001a680: 696e 7075 743a 0a20 2020 2020 2020 205b  input:.        [
-0001a690: 7b27 6865 6967 6874 273a 2032 322c 2027  {'height': 22, '
-0001a6a0: 6c65 6e67 7468 273a 2034 2c20 2777 6964  length': 4, 'wid
-0001a6b0: 7468 273a 2030 2e31 7d2c 0a20 2020 2020  th': 0.1},.     
-0001a6c0: 2020 2020 7b27 6865 6967 6874 273a 2032      {'height': 2
-0001a6d0: 322c 2027 6c65 6e67 7468 273a 2035 2c20  2, 'length': 5, 
-0001a6e0: 2777 6964 7468 273a 2030 2e31 7d2c 0a20  'width': 0.1},. 
-0001a6f0: 2020 2020 2020 2020 7b27 6865 6967 6874          {'height
-0001a700: 273a 2032 322c 2027 6c65 6e67 7468 273a  ': 22, 'length':
-0001a710: 2036 2c20 2777 6964 7468 273a 2030 2e31   6, 'width': 0.1
-0001a720: 7d2c 0a20 2020 2020 2020 2020 7b27 6865  },.         {'he
-0001a730: 6967 6874 273a 2032 322c 2027 6c65 6e67  ight': 22, 'leng
-0001a740: 7468 273a 2034 2c20 2777 6964 7468 273a  th': 4, 'width':
-0001a750: 2030 2e32 7d2c 0a20 2020 2020 2020 2020   0.2},.         
-0001a760: 7b27 6865 6967 6874 273a 2032 322c 2027  {'height': 22, '
-0001a770: 6c65 6e67 7468 273a 2035 2c20 2777 6964  length': 5, 'wid
-0001a780: 7468 273a 2030 2e32 7d2c 0a20 2020 2020  th': 0.2},.     
-0001a790: 2020 2020 7b27 6865 6967 6874 273a 2032      {'height': 2
-0001a7a0: 322c 2027 6c65 6e67 7468 273a 2036 2c20  2, 'length': 6, 
-0001a7b0: 2777 6964 7468 273a 2030 2e32 7d5d 2222  'width': 0.2}]""
-0001a7c0: 220a 2020 2020 7661 6c75 655f 636f 6d62  ".    value_comb
-0001a7d0: 696e 6174 696f 6e73 203d 206c 6973 7428  inations = list(
-0001a7e0: 6974 6572 746f 6f6c 732e 7072 6f64 7563  itertools.produc
-0001a7f0: 7428 2a70 6172 616d 6574 6572 735f 6469  t(*parameters_di
-0001a800: 6374 2e76 616c 7565 7328 2929 290a 2020  ct.values())).  
-0001a810: 2020 6b65 7973 203d 206c 6973 7428 7061    keys = list(pa
-0001a820: 7261 6d65 7465 7273 5f64 6963 742e 6b65  rameters_dict.ke
-0001a830: 7973 2829 290a 2020 2020 7265 7475 726e  ys()).    return
-0001a840: 205b 0a20 2020 2020 2020 207b 6b65 7973   [.        {keys
-0001a850: 5b6e 5d3a 2076 616c 7565 735b 6e5d 2066  [n]: values[n] f
-0001a860: 6f72 206e 2069 6e20 7261 6e67 6528 6c65  or n in range(le
-0001a870: 6e28 6b65 7973 2929 7d20 666f 7220 7661  n(keys))} for va
-0001a880: 6c75 6573 2069 6e20 7661 6c75 655f 636f  lues in value_co
-0001a890: 6d62 696e 6174 696f 6e73 0a20 2020 205d  mbinations.    ]
-0001a8a0: 0a0a 0a64 6566 205f 6765 6e5f 7061 7261  ...def _gen_para
-0001a8b0: 6d5f 7661 7269 6174 696f 6e73 280a 2020  m_variations(.  
-0001a8c0: 2020 6675 6e63 7469 6f6e 2c20 7061 7261    function, para
-0001a8d0: 6d5f 7661 7269 6174 696f 6e73 2c20 7061  m_variations, pa
-0001a8e0: 7261 6d5f 6465 6661 756c 7473 3d7b 7d2c  ram_defaults={},
-0001a8f0: 2070 6172 616d 5f6f 7665 7272 6964 653d   param_override=
-0001a900: 7b7d 2c20 6c61 6265 6c5f 6c61 7965 723d  {}, label_layer=
-0001a910: 3235 350a 293a 0a20 2020 2022 2222 5461  255.):.    """Ta
-0001a920: 6b65 7320 652e 672e 0a0a 2020 2020 7061  kes e.g...    pa
-0001a930: 7261 6d5f 7661 7269 6174 696f 6e73 203d  ram_variations =
-0001a940: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0001a950: 6368 616e 6e65 6c5f 7769 6474 6827 203a  channel_width' :
-0001a960: 205b 312c 322c 335d 0a20 2020 2020 2020   [1,2,3].       
-0001a970: 2020 2020 2027 6761 7465 5f77 6964 7468       'gate_width
-0001a980: 2720 3a20 5b30 2e31 2c30 2e32 2c30 2e34  ' : [0.1,0.2,0.4
-0001a990: 5d2c 0a20 2020 2020 2020 2020 2020 207d  ],.            }
-0001a9a0: 0a20 2020 2020 2020 6f72 2065 7175 6976  .       or equiv
-0001a9b0: 616c 656e 746c 790a 2020 2020 7061 7261  alently.    para
-0001a9c0: 6d5f 7661 7269 6174 696f 6e73 203d 2064  m_variations = d
-0001a9d0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
-0001a9e0: 2063 6861 6e6e 656c 5f77 6964 7468 203d   channel_width =
-0001a9f0: 205b 312c 322c 335d 2c0a 2020 2020 2020   [1,2,3],.      
-0001aa00: 2020 2020 2020 6761 7465 5f77 6964 7468        gate_width
-0001aa10: 203d 205b 302e 312c 302e 322c 302e 345d   = [0.1,0.2,0.4]
-0001aa20: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0001aa30: 2020 2020 2222 220a 2020 2020 7061 7261      """.    para
-0001aa40: 6d65 7465 725f 6c69 7374 203d 205f 7061  meter_list = _pa
-0001aa50: 7261 6d65 7465 725f 636f 6d62 696e 6174  rameter_combinat
-0001aa60: 696f 6e73 2870 6172 616d 5f76 6172 6961  ions(param_varia
-0001aa70: 7469 6f6e 7329 0a0a 2020 2020 445f 6c69  tions)..    D_li
-0001aa80: 7374 203d 205b 5d0a 2020 2020 666f 7220  st = [].    for 
-0001aa90: 7061 7261 6d73 2069 6e20 7061 7261 6d65  params in parame
-0001aaa0: 7465 725f 6c69 7374 3a0a 2020 2020 2020  ter_list:.      
-0001aab0: 2020 6e65 775f 7061 7261 6d73 203d 2064    new_params = d
-0001aac0: 6963 7428 290a 2020 2020 2020 2020 6e65  ict().        ne
-0001aad0: 775f 7061 7261 6d73 2e75 7064 6174 6528  w_params.update(
-0001aae0: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
-0001aaf0: 6e65 775f 7061 7261 6d73 2e75 7064 6174  new_params.updat
-0001ab00: 6528 7061 7261 6d5f 6f76 6572 7269 6465  e(param_override
-0001ab10: 290a 2020 2020 2020 2020 445f 6e65 7720  ).        D_new 
-0001ab20: 3d20 6d61 6b65 5f64 6576 6963 6528 6675  = make_device(fu
-0001ab30: 6e63 7469 6f6e 2c20 636f 6e66 6967 3d70  nction, config=p
-0001ab40: 6172 616d 5f64 6566 6175 6c74 732c 202a  aram_defaults, *
-0001ab50: 2a6e 6577 5f70 6172 616d 7329 0a20 2020  *new_params).   
-0001ab60: 2020 2020 206c 6162 656c 5f74 6578 7420       label_text 
-0001ab70: 3d20 2222 0a20 2020 2020 2020 2066 6f72  = "".        for
-0001ab80: 206e 616d 652c 2076 616c 7565 2069 6e20   name, value in 
-0001ab90: 7061 7261 6d73 2e69 7465 6d73 2829 3a0a  params.items():.
-0001aba0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-0001abb0: 6c5f 7465 7874 202b 3d20 2866 227b 6e61  l_text += (f"{na
-0001abc0: 6d65 7d3d 7b76 616c 7565 7d22 2920 2b20  me}={value}") + 
-0001abd0: 225c 6e22 0a20 2020 2020 2020 2069 6620  "\n".        if 
-0001abe0: 6c61 6265 6c5f 6c61 7965 7220 6973 206e  label_layer is n
-0001abf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001ac00: 2020 2020 2044 5f6e 6577 2e61 6464 5f6c       D_new.add_l
-0001ac10: 6162 656c 2874 6578 743d 6c61 6265 6c5f  abel(text=label_
-0001ac20: 7465 7874 2c20 706f 7369 7469 6f6e 3d44  text, position=D
-0001ac30: 5f6e 6577 2e63 656e 7465 722c 206c 6179  _new.center, lay
-0001ac40: 6572 3d6c 6162 656c 5f6c 6179 6572 290a  er=label_layer).
-0001ac50: 0a20 2020 2020 2020 2044 5f6c 6973 742e  .        D_list.
-0001ac60: 6170 7065 6e64 2844 5f6e 6577 290a 2020  append(D_new).  
-0001ac70: 2020 7265 7475 726e 2044 5f6c 6973 740a    return D_list.
-0001ac80: 0a0a 6465 6620 6772 6964 7377 6565 7028  ..def gridsweep(
-0001ac90: 0a20 2020 2066 756e 6374 696f 6e2c 0a20  .    function,. 
-0001aca0: 2020 2070 6172 616d 5f78 3d7b 2277 6964     param_x={"wid
-0001acb0: 7468 223a 205b 312c 2035 2c20 362c 2037  th": [1, 5, 6, 7
-0001acc0: 5d7d 2c0a 2020 2020 7061 7261 6d5f 793d  ]},.    param_y=
-0001acd0: 7b22 6c65 6e67 7468 223a 205b 312e 312c  {"length": [1.1,
-0001ace0: 2032 2c20 3730 5d7d 2c0a 2020 2020 7061   2, 70]},.    pa
-0001acf0: 7261 6d5f 6465 6661 756c 7473 3d7b 7d2c  ram_defaults={},
-0001ad00: 0a20 2020 2070 6172 616d 5f6f 7665 7272  .    param_overr
-0001ad10: 6964 653d 7b7d 2c0a 2020 2020 7370 6163  ide={},.    spac
-0001ad20: 696e 673d 2835 302c 2031 3030 292c 0a20  ing=(50, 100),. 
-0001ad30: 2020 2073 6570 6172 6174 696f 6e3d 5472     separation=Tr
-0001ad40: 7565 2c0a 2020 2020 616c 6967 6e5f 783d  ue,.    align_x=
-0001ad50: 2278 222c 0a20 2020 2061 6c69 676e 5f79  "x",.    align_y
-0001ad60: 3d22 7922 2c0a 2020 2020 6564 6765 5f78  ="y",.    edge_x
-0001ad70: 3d22 7822 2c0a 2020 2020 6564 6765 5f79  ="x",.    edge_y
-0001ad80: 3d22 796d 696e 222c 0a20 2020 206c 6162  ="ymin",.    lab
-0001ad90: 656c 5f6c 6179 6572 3d32 3535 2c0a 293a  el_layer=255,.):
-0001ada0: 0a20 2020 2022 2222 4372 6561 7465 7320  .    """Creates 
-0001adb0: 6120 7061 7261 6d65 7465 7220 7377 6565  a parameter swee
-0001adc0: 7020 6f66 2064 6576 6963 6573 2061 6e64  p of devices and
-0001add0: 2070 6c61 6365 7320 7468 656d 206f 6e20   places them on 
-0001ade0: 6120 6772 6964 2077 6974 680a 2020 2020  a grid with.    
-0001adf0: 6c61 6265 6c73 2066 6f72 2065 6163 6820  labels for each 
-0001ae00: 6465 7669 6365 2e20 466f 7220 696e 7374  device. For inst
-0001ae10: 616e 6365 2c20 6769 7665 6e20 6120 6675  ance, given a fu
-0001ae20: 6e63 7469 6f6e 2064 6566 696e 6564 206c  nction defined l
-0001ae30: 696b 650a 2020 2020 606d 7973 6861 7065  ike.    `myshape
-0001ae40: 2877 6964 7468 2c20 6865 6967 6874 2c20  (width, height, 
-0001ae50: 6f66 6673 6574 2c20 6c61 7965 7229 6020  offset, layer)` 
-0001ae60: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
-0001ae70: 6720 7061 7261 6d65 7465 7273 3a0a 2020  g parameters:.  
-0001ae80: 2020 2020 2020 7061 7261 6d5f 7820 3d20        param_x = 
-0001ae90: 7b27 7769 6474 6827 203a 2020 5b34 2c20  {'width' :  [4, 
-0001aea0: 352c 2036 5d20 207d 2c0a 2020 2020 2020  5, 6]  },.      
-0001aeb0: 2020 7061 7261 6d5f 7920 3d20 7b27 6865    param_y = {'he
-0001aec0: 6967 6874 2720 3a20 5b37 2c20 395d 2c0a  ight' : [7, 9],.
-0001aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aee0: 2020 2027 6c61 7965 7227 203a 2020 5b31     'layer' :  [1
-0001aef0: 2c20 322c 2033 5d20 207d 2c0a 2020 2020  , 2, 3]  },.    
-0001af00: 2020 2020 7061 7261 6d5f 6465 6661 756c      param_defaul
-0001af10: 7473 203d 207b 2773 6361 6c65 2720 3a20  ts = {'scale' : 
-0001af20: 317d 0a0a 2020 2020 6772 6964 7377 6565  1}..    gridswee
-0001af30: 7028 2920 7072 6f64 7563 6520 6120 6772  p() produce a gr
-0001af40: 6964 206f 6620 6465 7669 6365 7320 7769  id of devices wi
-0001af50: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
-0001af60: 206c 6179 6f75 742f 7061 7261 6d65 7465   layout/paramete
-0001af70: 7273 3a0a 2020 2020 2020 2020 2877 3d34  rs:.        (w=4
-0001af80: 2c20 683d 372c 2073 3d31 2c20 6c3d 3129  , h=7, s=1, l=1)
-0001af90: 2020 2020 2877 3d35 2c20 683d 372c 2073      (w=5, h=7, s
-0001afa0: 3d31 2c20 6c3d 3129 2020 2020 2877 3d36  =1, l=1)    (w=6
-0001afb0: 2c20 683d 372c 2073 3d31 2c20 6c3d 3129  , h=7, s=1, l=1)
-0001afc0: 0a20 2020 2020 2020 2028 773d 342c 2068  .        (w=4, h
-0001afd0: 3d37 2c20 733d 312c 206c 3d32 2920 2020  =7, s=1, l=2)   
-0001afe0: 2028 773d 352c 2068 3d37 2c20 733d 312c   (w=5, h=7, s=1,
-0001aff0: 206c 3d32 2920 2020 2028 773d 362c 2068   l=2)    (w=6, h
-0001b000: 3d37 2c20 733d 312c 206c 3d32 290a 2020  =7, s=1, l=2).  
-0001b010: 2020 2020 2020 2877 3d34 2c20 683d 372c        (w=4, h=7,
-0001b020: 2073 3d31 2c20 6c3d 3329 2020 2020 2877   s=1, l=3)    (w
-0001b030: 3d35 2c20 683d 372c 2073 3d31 2c20 6c3d  =5, h=7, s=1, l=
-0001b040: 3329 2020 2020 2877 3d36 2c20 683d 372c  3)    (w=6, h=7,
-0001b050: 2073 3d31 2c20 6c3d 3329 0a20 2020 2020   s=1, l=3).     
-0001b060: 2020 2028 773d 342c 2068 3d39 2c20 733d     (w=4, h=9, s=
-0001b070: 312c 206c 3d31 2920 2020 2028 773d 352c  1, l=1)    (w=5,
-0001b080: 2068 3d39 2c20 733d 312c 206c 3d31 2920   h=9, s=1, l=1) 
-0001b090: 2020 2028 773d 362c 2068 3d39 2c20 733d     (w=6, h=9, s=
-0001b0a0: 312c 206c 3d31 290a 2020 2020 2020 2020  1, l=1).        
-0001b0b0: 2877 3d34 2c20 683d 392c 2073 3d31 2c20  (w=4, h=9, s=1, 
-0001b0c0: 6c3d 3229 2020 2020 2877 3d35 2c20 683d  l=2)    (w=5, h=
-0001b0d0: 392c 2073 3d31 2c20 6c3d 3229 2020 2020  9, s=1, l=2)    
-0001b0e0: 2877 3d36 2c20 683d 392c 2073 3d31 2c20  (w=6, h=9, s=1, 
-0001b0f0: 6c3d 3229 0a20 2020 2020 2020 2028 773d  l=2).        (w=
-0001b100: 342c 2068 3d39 2c20 733d 312c 206c 3d33  4, h=9, s=1, l=3
-0001b110: 2920 2020 2028 773d 352c 2068 3d39 2c20  )    (w=5, h=9, 
-0001b120: 733d 312c 206c 3d33 2920 2020 2028 773d  s=1, l=3)    (w=
-0001b130: 362c 2068 3d39 2c20 733d 312c 206c 3d33  6, h=9, s=1, l=3
-0001b140: 290a 0a0a 2020 2020 5061 7261 6d65 7465  )...    Paramete
-0001b150: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0001b160: 2d0a 2020 2020 6675 6e63 7469 6f6e 203a  -.    function :
-0001b170: 2066 756e 6374 696f 6e20 7468 6174 2070   function that p
-0001b180: 726f 6475 6365 7320 6120 4465 7669 6365  roduces a Device
-0001b190: 0a20 2020 2020 2020 2054 6865 2066 756e  .        The fun
-0001b1a0: 6374 696f 6e20 7768 6963 6820 7769 6c6c  ction which will
-0001b1b0: 2062 6520 7573 6564 2074 6f20 6372 6561   be used to crea
-0001b1c0: 7465 2074 6865 2069 6e64 6976 6964 7561  te the individua
-0001b1d0: 6c20 6465 7669 6365 7320 696e 2074 6865  l devices in the
-0001b1e0: 0a20 2020 2020 2020 2067 7269 642e 2020  .        grid.  
-0001b1f0: 4d75 7374 206f 6e6c 7920 7265 7475 726e  Must only return
-0001b200: 2061 2073 696e 676c 6520 4465 7669 6365   a single Device
-0001b210: 2028 652e 672e 2061 6e79 206f 6620 7468   (e.g. any of th
-0001b220: 6520 6675 6e63 7469 6f6e 7320 696e 0a20  e functions in. 
-0001b230: 2020 2020 2020 2070 672e 6765 6f6d 6574         pg.geomet
-0001b240: 7279 290a 2020 2020 7061 7261 6d5f 7820  ry).    param_x 
-0001b250: 3a20 6469 6374 0a20 2020 2020 2020 2041  : dict.        A
-0001b260: 2064 6963 7469 6f6e 6172 7920 6f66 206f   dictionary of o
-0001b270: 6e65 206f 7220 6d6f 7265 2070 6172 616d  ne or more param
-0001b280: 6574 6572 7320 746f 2073 7765 6570 2069  eters to sweep i
-0001b290: 6e20 7468 6520 782d 6469 7265 6374 696f  n the x-directio
-0001b2a0: 6e0a 2020 2020 7061 7261 6d5f 7920 3a20  n.    param_y : 
-0001b2b0: 6469 6374 0a20 2020 2020 2020 2041 2064  dict.        A d
-0001b2c0: 6963 7469 6f6e 6172 7920 6f66 206f 6e65  ictionary of one
-0001b2d0: 206f 7220 6d6f 7265 2070 6172 616d 6574   or more paramet
-0001b2e0: 6572 7320 746f 2073 7765 6570 2069 6e20  ers to sweep in 
-0001b2f0: 7468 6520 792d 6469 7265 6374 696f 6e0a  the y-direction.
-0001b300: 2020 2020 7061 7261 6d5f 6465 6661 756c      param_defaul
-0001b310: 7473 203a 2064 6963 740a 2020 2020 2020  ts : dict.      
-0001b320: 2020 4465 6661 756c 7420 7061 7261 6d65    Default parame
-0001b330: 7465 7273 2074 6f20 7061 7373 2074 6f20  ters to pass to 
-0001b340: 6576 6572 7920 6465 7669 6365 2069 6e20  every device in 
-0001b350: 7468 6520 6772 6964 0a20 2020 2070 6172  the grid.    par
-0001b360: 616d 5f6f 7665 7272 6964 6520 3a20 6469  am_override : di
-0001b370: 6374 0a20 2020 2020 2020 2050 6172 616d  ct.        Param
-0001b380: 6574 6572 7320 7468 6174 2077 696c 6c20  eters that will 
-0001b390: 6f76 6572 7269 6465 2060 7061 7261 6d5f  override `param_
-0001b3a0: 6465 6661 756c 7473 602c 2065 7175 6976  defaults`, equiv
-0001b3b0: 616c 656e 7420 746f 2063 6861 6e67 696e  alent to changin
-0001b3c0: 670a 2020 2020 2020 2020 7061 7261 6d5f  g.        param_
-0001b3d0: 6465 6661 756c 7473 2028 7573 6566 756c  defaults (useful
-0001b3e0: 2029 0a20 2020 2073 7061 6369 6e67 203a   ).    spacing :
-0001b3f0: 2069 6e74 2c20 666c 6f61 742c 206f 7220   int, float, or 
-0001b400: 6172 7261 792d 6c69 6b65 5b32 5d20 6f66  array-like[2] of
-0001b410: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
-0001b420: 2020 2020 2020 5370 6163 696e 6720 6265        Spacing be
-0001b430: 7477 6565 6e20 6164 6a61 6365 6e74 2065  tween adjacent e
-0001b440: 6c65 6d65 6e74 7320 6f6e 2074 6865 2067  lements on the g
-0001b450: 7269 642c 2063 616e 2062 6520 6120 7475  rid, can be a tu
-0001b460: 706c 6520 666f 720a 2020 2020 2020 2020  ple for.        
-0001b470: 6469 6666 6572 656e 7420 6469 7374 616e  different distan
-0001b480: 6365 7320 696e 2077 6964 7468 2061 6e64  ces in width and
-0001b490: 2068 6569 6768 7420 2878 2c79 292e 0a20   height (x,y).. 
-0001b4a0: 2020 2073 6570 6172 6174 696f 6e20 3a20     separation : 
-0001b4b0: 626f 6f6c 0a20 2020 2020 2020 2049 6620  bool.        If 
-0001b4c0: 5472 7565 2c20 6775 6172 616e 7465 6573  True, guarantees
-0001b4d0: 2065 6c65 6d65 6e74 7320 6172 6520 7365   elements are se
-0001b4e0: 7061 7261 7465 6420 7769 7468 2061 2066  parated with a f
-0001b4f0: 6978 6564 2073 7061 6369 6e67 0a20 2020  ixed spacing.   
-0001b500: 2020 2020 2062 6574 7765 656e 3b20 6966       between; if
-0001b510: 2046 616c 7365 2c20 656c 656d 656e 7473   False, elements
-0001b520: 2061 7265 2073 7061 6365 6420 6576 656e   are spaced even
-0001b530: 6c79 2061 6c6f 6e67 2061 2067 7269 642e  ly along a grid.
-0001b540: 0a20 2020 2073 6861 7065 203a 2061 7272  .    shape : arr
-0001b550: 6179 2d6c 696b 655b 325d 0a20 2020 2020  ay-like[2].     
-0001b560: 2020 2078 2c20 7920 7368 6170 6520 6f66     x, y shape of
-0001b570: 2074 6865 2067 7269 6420 2873 6565 206e   the grid (see n
-0001b580: 702e 7265 7368 6170 6529 2e20 4966 206e  p.reshape). If n
-0001b590: 6f20 7368 6170 6520 6973 2067 6976 656e  o shape is given
-0001b5a0: 2061 6e64 2074 6865 0a20 2020 2020 2020   and the.       
-0001b5b0: 206c 6973 7420 6973 2031 442c 2074 6865   list is 1D, the
-0001b5c0: 206f 7574 7075 7420 6973 2061 7320 6966   output is as if
-0001b5d0: 206e 702e 7265 7368 6170 6520 7765 7265   np.reshape were
-0001b5e0: 2072 756e 2077 6974 6820 2831 2c20 2d31   run with (1, -1
-0001b5f0: 292e 0a20 2020 2061 6c69 676e 5f78 203a  )..    align_x :
-0001b600: 207b 2778 272c 2027 786d 696e 272c 2027   {'x', 'xmin', '
-0001b610: 786d 6178 277d 0a20 2020 2020 2020 2057  xmax'}.        W
-0001b620: 6869 6368 2065 6467 6520 746f 2070 6572  hich edge to per
-0001b630: 666f 726d 2074 6865 2078 2028 636f 6c75  form the x (colu
-0001b640: 6d6e 2920 616c 6967 6e6d 656e 7420 616c  mn) alignment al
-0001b650: 6f6e 670a 2020 2020 616c 6967 6e5f 7920  ong.    align_y 
-0001b660: 3a20 7b27 7927 2c20 2779 6d69 6e27 2c20  : {'y', 'ymin', 
-0001b670: 2779 6d61 7827 7d0a 2020 2020 2020 2020  'ymax'}.        
-0001b680: 5768 6963 6820 6564 6765 2074 6f20 7065  Which edge to pe
-0001b690: 7266 6f72 6d20 7468 6520 7920 2872 6f77  rform the y (row
-0001b6a0: 2920 616c 6967 6e6d 656e 7420 616c 6f6e  ) alignment alon
-0001b6b0: 670a 2020 2020 6564 6765 5f78 203a 207b  g.    edge_x : {
-0001b6c0: 2778 272c 2027 786d 696e 272c 2027 786d  'x', 'xmin', 'xm
-0001b6d0: 6178 277d 0a20 2020 2020 2020 2057 6869  ax'}.        Whi
-0001b6e0: 6368 2065 6467 6520 746f 2070 6572 666f  ch edge to perfo
-0001b6f0: 726d 2074 6865 2078 2028 636f 6c75 6d6e  rm the x (column
-0001b700: 2920 6469 7374 7269 6275 7469 6f6e 2061  ) distribution a
-0001b710: 6c6f 6e67 2028 756e 7573 6564 2069 660a  long (unused if.
-0001b720: 2020 2020 2020 2020 7365 7061 7261 7469          separati
-0001b730: 6f6e 203d 3d20 5472 7565 290a 2020 2020  on == True).    
-0001b740: 6564 6765 5f79 203a 207b 2779 272c 2027  edge_y : {'y', '
-0001b750: 796d 696e 272c 2027 796d 6178 277d 0a20  ymin', 'ymax'}. 
-0001b760: 2020 2020 2020 2057 6869 6368 2065 6467         Which edg
-0001b770: 6520 746f 2070 6572 666f 726d 2074 6865  e to perform the
-0001b780: 2079 2028 726f 7729 2064 6973 7472 6962   y (row) distrib
-0001b790: 7574 696f 6e20 616c 6f6e 6720 2875 6e75  ution along (unu
-0001b7a0: 7365 6420 6966 0a20 2020 2020 2020 2073  sed if.        s
-0001b7b0: 6570 6172 6174 696f 6e20 3d3d 2054 7275  eparation == Tru
-0001b7c0: 6529 0a20 2020 206c 6162 656c 5f6c 6179  e).    label_lay
-0001b7d0: 6572 203a 204e 6f6e 6520 6f72 206c 6179  er : None or lay
-0001b7e0: 6572 0a20 2020 2020 2020 2049 6620 6e6f  er.        If no
-0001b7f0: 7420 4e6f 6e65 2c20 7769 6c6c 2070 6c61  t None, will pla
-0001b800: 6365 2061 206c 6162 656c 2074 6861 7420  ce a label that 
-0001b810: 6465 7363 7269 6265 7320 7468 6520 7061  describes the pa
-0001b820: 7261 6d65 7465 7273 206f 6e20 7468 6520  rameters on the 
-0001b830: 6465 7669 6365 0a0a 2020 2020 5265 7475  device..    Retu
-0001b840: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001b850: 2020 2020 6465 7669 6365 5f6d 6174 7269      device_matri
-0001b860: 7820 3a20 4465 7669 6365 0a20 2020 2020  x : Device.     
-0001b870: 2020 2041 2044 6576 6963 6520 636f 6e74     A Device cont
-0001b880: 6169 6e69 6e67 2061 6c6c 2074 6865 2044  aining all the D
-0001b890: 6576 6963 6573 2069 6e20 6064 6576 6963  evices in `devic
-0001b8a0: 655f 6c69 7374 6020 696e 2061 2067 7269  e_list` in a gri
-0001b8b0: 642e 0a20 2020 2022 2222 0a0a 2020 2020  d..    """..    
-0001b8c0: 7061 7261 6d5f 7661 7269 6174 696f 6e73  param_variations
-0001b8d0: 203d 204f 7264 6572 6564 4469 6374 2829   = OrderedDict()
-0001b8e0: 0a20 2020 2070 6172 616d 5f76 6172 6961  .    param_varia
-0001b8f0: 7469 6f6e 732e 7570 6461 7465 2870 6172  tions.update(par
-0001b900: 616d 5f79 290a 2020 2020 7061 7261 6d5f  am_y).    param_
-0001b910: 7661 7269 6174 696f 6e73 2e75 7064 6174  variations.updat
-0001b920: 6528 7061 7261 6d5f 7829 0a0a 2020 2020  e(param_x)..    
-0001b930: 445f 6c69 7374 203d 205f 6765 6e5f 7061  D_list = _gen_pa
-0001b940: 7261 6d5f 7661 7269 6174 696f 6e73 280a  ram_variations(.
-0001b950: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-0001b960: 3d66 756e 6374 696f 6e2c 0a20 2020 2020  =function,.     
-0001b970: 2020 2070 6172 616d 5f76 6172 6961 7469     param_variati
-0001b980: 6f6e 733d 7061 7261 6d5f 7661 7269 6174  ons=param_variat
-0001b990: 696f 6e73 2c0a 2020 2020 2020 2020 7061  ions,.        pa
-0001b9a0: 7261 6d5f 6465 6661 756c 7473 3d70 6172  ram_defaults=par
-0001b9b0: 616d 5f64 6566 6175 6c74 732c 0a20 2020  am_defaults,.   
-0001b9c0: 2020 2020 2070 6172 616d 5f6f 7665 7272       param_overr
-0001b9d0: 6964 653d 7061 7261 6d5f 6f76 6572 7269  ide=param_overri
-0001b9e0: 6465 2c0a 2020 2020 2020 2020 6c61 6265  de,.        labe
-0001b9f0: 6c5f 6c61 7965 723d 6c61 6265 6c5f 6c61  l_layer=label_la
-0001ba00: 7965 722c 0a20 2020 2029 0a0a 2020 2020  yer,.    )..    
-0001ba10: 6e75 6d5f 785f 7061 7261 6d65 7465 7273  num_x_parameters
-0001ba20: 203d 206c 656e 285f 7061 7261 6d65 7465   = len(_paramete
-0001ba30: 725f 636f 6d62 696e 6174 696f 6e73 2870  r_combinations(p
-0001ba40: 6172 616d 5f78 2929 0a20 2020 206e 756d  aram_x)).    num
-0001ba50: 5f79 5f70 6172 616d 6574 6572 7320 3d20  _y_parameters = 
-0001ba60: 6c65 6e28 5f70 6172 616d 6574 6572 5f63  len(_parameter_c
-0001ba70: 6f6d 6269 6e61 7469 6f6e 7328 7061 7261  ombinations(para
-0001ba80: 6d5f 7929 290a 2020 2020 4420 3d20 6772  m_y)).    D = gr
-0001ba90: 6964 280a 2020 2020 2020 2020 445f 6c69  id(.        D_li
-0001baa0: 7374 2c0a 2020 2020 2020 2020 7370 6163  st,.        spac
-0001bab0: 696e 673d 7370 6163 696e 672c 0a20 2020  ing=spacing,.   
-0001bac0: 2020 2020 2073 6570 6172 6174 696f 6e3d       separation=
-0001bad0: 7365 7061 7261 7469 6f6e 2c0a 2020 2020  separation,.    
-0001bae0: 2020 2020 7368 6170 653d 286e 756d 5f78      shape=(num_x
-0001baf0: 5f70 6172 616d 6574 6572 732c 206e 756d  _parameters, num
-0001bb00: 5f79 5f70 6172 616d 6574 6572 7329 2c0a  _y_parameters),.
-0001bb10: 2020 2020 2020 2020 616c 6967 6e5f 783d          align_x=
-0001bb20: 616c 6967 6e5f 782c 0a20 2020 2020 2020  align_x,.       
-0001bb30: 2061 6c69 676e 5f79 3d61 6c69 676e 5f79   align_y=align_y
-0001bb40: 2c0a 2020 2020 2020 2020 6564 6765 5f78  ,.        edge_x
-0001bb50: 3d65 6467 655f 782c 0a20 2020 2020 2020  =edge_x,.       
-0001bb60: 2065 6467 655f 793d 6564 6765 5f79 2c0a   edge_y=edge_y,.
-0001bb70: 2020 2020 290a 0a20 2020 206c 6162 656c      )..    label
-0001bb80: 5f74 6578 7420 3d20 7b7d 0a20 2020 206c  _text = {}.    l
-0001bb90: 6162 656c 5f74 6578 742e 7570 6461 7465  abel_text.update
-0001bba0: 2870 6172 616d 5f64 6566 6175 6c74 7329  (param_defaults)
-0001bbb0: 0a20 2020 206c 6162 656c 5f74 6578 742e  .    label_text.
-0001bbc0: 7570 6461 7465 2870 6172 616d 5f6f 7665  update(param_ove
-0001bbd0: 7272 6964 6529 0a20 2020 2069 6620 6c61  rride).    if la
-0001bbe0: 6265 6c5f 6c61 7965 7220 6973 206e 6f74  bel_layer is not
-0001bbf0: 204e 6f6e 653a 0a20 2020 2020 2020 2044   None:.        D
-0001bc00: 2e61 6464 5f6c 6162 656c 2874 6578 743d  .add_label(text=
-0001bc10: 7374 7228 6c61 6265 6c5f 7465 7874 292c  str(label_text),
-0001bc20: 2070 6f73 6974 696f 6e3d 2844 2e78 6d69   position=(D.xmi
-0001bc30: 6e2c 2044 2e79 6d69 6e29 2c20 6c61 7965  n, D.ymin), laye
-0001bc40: 723d 6c61 6265 6c5f 6c61 7965 7229 0a0a  r=label_layer)..
-0001bc50: 2020 2020 7265 7475 726e 2044 0a0a 0a64      return D...d
-0001bc60: 6566 205f 7061 636b 5f73 696e 676c 655f  ef _pack_single_
-0001bc70: 6269 6e28 0a20 2020 2072 6563 745f 6469  bin(.    rect_di
-0001bc80: 6374 2c20 6173 7065 6374 5f72 6174 696f  ct, aspect_ratio
-0001bc90: 2c20 6d61 785f 7369 7a65 2c20 736f 7274  , max_size, sort
-0001bca0: 5f62 795f 6172 6561 2c20 6465 6e73 6974  _by_area, densit
-0001bcb0: 792c 2070 7265 6369 7369 6f6e 2c20 7665  y, precision, ve
-0001bcc0: 7262 6f73 650a 293a 0a20 2020 2022 2222  rbose.):.    """
-0001bcd0: 5461 6b65 7320 6120 6072 6563 745f 6469  Takes a `rect_di
-0001bce0: 6374 6020 6172 6775 6d65 6e74 206f 6620  ct` argument of 
-0001bcf0: 7468 6520 666f 726d 207b 6964 3a28 772c  the form {id:(w,
-0001bd00: 2068 297d 2061 6e64 2074 7269 6573 2074   h)} and tries t
-0001bd10: 6f0a 2020 2020 7061 636b 2069 7420 696e  o.    pack it in
-0001bd20: 746f 2061 2062 696e 2061 7320 736d 616c  to a bin as smal
-0001bd30: 6c20 6173 2070 6f73 7369 626c 6520 7769  l as possible wi
-0001bd40: 7468 2061 7370 6563 7420 7261 7469 6f20  th aspect ratio 
-0001bd50: 6061 7370 6563 745f 7261 7469 6f60 2e0a  `aspect_ratio`..
-0001bd60: 2020 2020 5769 6c6c 2069 7465 7261 7469      Will iterati
-0001bd70: 7665 6c79 2067 726f 7720 7468 6520 6269  vely grow the bi
-0001bd80: 6e20 7369 7a65 2075 6e74 696c 2065 7665  n size until eve
-0001bd90: 7279 7468 696e 6720 6669 7473 206f 7220  rything fits or 
-0001bda0: 7468 6520 6269 6e20 7369 7a65 0a20 2020  the bin size.   
-0001bdb0: 2072 6561 6368 6573 2060 6d61 785f 7369   reaches `max_si
-0001bdc0: 7a65 602e 2052 6574 7572 6e73 2061 2064  ze`. Returns a d
-0001bdd0: 6963 7469 6f6e 6172 7920 6f66 2074 6865  ictionary of the
-0001bde0: 2070 6163 6b65 6420 7265 6374 616e 676c   packed rectangl
-0001bdf0: 6573 6e20 696e 2074 6865 0a20 2020 2066  esn in the.    f
-0001be00: 6f72 6d20 7b69 643a 2878 2c20 792c 2077  orm {id:(x, y, w
-0001be10: 2c20 6829 7d2c 2061 6e64 2061 2064 6963  , h)}, and a dic
-0001be20: 7469 6f6e 6172 7920 6f66 2072 656d 6169  tionary of remai
-0001be30: 6e69 6e67 2075 6e70 6163 6b65 6420 7265  ning unpacked re
-0001be40: 6374 732e 0a20 2020 2022 2222 0a20 2020  cts..    """.   
-0001be50: 2074 7279 3a0a 2020 2020 2020 2020 696d   try:.        im
-0001be60: 706f 7274 2072 6563 7470 6163 6b0a 2020  port rectpack.  
-0001be70: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0001be80: 6f6e 3a0a 2020 2020 2020 2020 7261 6973  on:.        rais
-0001be90: 6520 496d 706f 7274 4572 726f 7228 0a20  e ImportError(. 
-0001bea0: 2020 2020 2020 2020 2020 2022 5b50 4849             "[PHI
-0001beb0: 444c 5d20 5468 6520 7061 636b 6572 2829  DL] The packer()
-0001bec0: 2066 756e 6374 696f 6e20 7265 7175 6972   function requir
-0001bed0: 6573 2074 6865 2022 0a20 2020 2020 2020  es the ".       
-0001bee0: 2020 2020 2027 6d6f 6475 6c65 2022 7265       'module "re
-0001bef0: 6374 7061 636b 2220 746f 206f 7065 7261  ctpack" to opera
-0001bf00: 7465 2e20 2050 6c65 6173 6520 7265 7472  te.  Please retr
-0001bf10: 7920 270a 2020 2020 2020 2020 2020 2020  y '.            
-0001bf20: 2261 6674 6572 2069 6e73 7461 6c6c 696e  "after installin
-0001bf30: 6720 7265 6374 7061 636b 3a5c 6e5c 6e22  g rectpack:\n\n"
-0001bf40: 0a20 2020 2020 2020 2020 2020 2022 2420  .            "$ 
-0001bf50: 7069 7020 696e 7374 616c 6c20 7265 6374  pip install rect
-0001bf60: 7061 636b 220a 2020 2020 2020 2020 290a  pack".        ).
-0001bf70: 0a20 2020 2023 2043 6f6d 7075 7465 2074  .    # Compute t
-0001bf80: 6f74 616c 2061 7265 6120 616e 6420 7573  otal area and us
-0001bf90: 6520 6974 2066 6f72 2061 6e20 696e 6974  e it for an init
-0001bfa0: 6961 6c20 6573 7469 6d61 7465 206f 6620  ial estimate of 
-0001bfb0: 7468 6520 6269 6e20 7369 7a65 0a20 2020  the bin size.   
-0001bfc0: 2074 6f74 616c 5f61 7265 6120 3d20 300a   total_area = 0.
-0001bfd0: 2020 2020 666f 7220 7220 696e 2072 6563      for r in rec
-0001bfe0: 745f 6469 6374 2e76 616c 7565 7328 293a  t_dict.values():
-0001bff0: 0a20 2020 2020 2020 2074 6f74 616c 5f61  .        total_a
-0001c000: 7265 6120 2b3d 2072 5b30 5d20 2a20 725b  rea += r[0] * r[
-0001c010: 315d 0a20 2020 2023 204e 6f72 6d61 6c69  1].    # Normali
-0001c020: 7a65 0a20 2020 2061 7370 6563 745f 7261  ze.    aspect_ra
-0001c030: 7469 6f20 3d20 6e70 2e61 7361 7272 6179  tio = np.asarray
-0001c040: 2861 7370 6563 745f 7261 7469 6f29 202f  (aspect_ratio) /
-0001c050: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0001c060: 6173 7065 6374 5f72 6174 696f 290a 0a20  aspect_ratio).. 
-0001c070: 2020 2023 2053 6574 7570 2076 6172 6961     # Setup varia
-0001c080: 626c 6573 0a20 2020 2062 6f78 5f73 697a  bles.    box_siz
-0001c090: 6520 3d20 6e70 2e61 7361 7272 6179 2861  e = np.asarray(a
-0001c0a0: 7370 6563 745f 7261 7469 6f20 2a20 6e70  spect_ratio * np
-0001c0b0: 2e73 7172 7428 746f 7461 6c5f 6172 6561  .sqrt(total_area
-0001c0c0: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
-0001c0d0: 7436 3429 0a20 2020 2062 6f78 5f73 697a  t64).    box_siz
-0001c0e0: 6520 3d20 6e70 2e63 6c69 7028 626f 785f  e = np.clip(box_
-0001c0f0: 7369 7a65 2c20 4e6f 6e65 2c20 6d61 785f  size, None, max_
-0001c100: 7369 7a65 290a 2020 2020 6966 2073 6f72  size).    if sor
-0001c110: 745f 6279 5f61 7265 613a 0a20 2020 2020  t_by_area:.     
-0001c120: 2020 2072 705f 736f 7274 203d 2072 6563     rp_sort = rec
-0001c130: 7470 6163 6b2e 534f 5254 5f41 5245 410a  tpack.SORT_AREA.
-0001c140: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001c150: 2020 7270 5f73 6f72 7420 3d20 7265 6374    rp_sort = rect
-0001c160: 7061 636b 2e53 4f52 545f 4e4f 4e45 0a0a  pack.SORT_NONE..
-0001c170: 2020 2020 2320 5265 7065 6174 6564 6c79      # Repeatedly
-0001c180: 2072 756e 2074 6865 2072 6563 7461 6e67   run the rectang
-0001c190: 6c65 2d70 6163 6b69 6e67 2061 6c67 6f72  le-packing algor
-0001c1a0: 6974 686d 2077 6974 6820 696e 6372 6561  ithm with increa
-0001c1b0: 7369 6e67 6c79 206c 6172 6765 720a 2020  singly larger.  
-0001c1c0: 2020 2320 6172 6561 7320 756e 7469 6c20    # areas until 
-0001c1d0: 6576 6572 7974 6869 6e67 2066 6974 7320  everything fits 
-0001c1e0: 6f72 2077 6527 7665 2072 6561 6368 6564  or we've reached
-0001c1f0: 2074 6865 206d 6178 696d 756d 2073 697a   the maximum siz
-0001c200: 650a 2020 2020 7768 696c 6520 5472 7565  e.    while True
-0001c210: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
-0001c220: 7465 2074 6865 2070 6163 6b65 7220 6f62  te the packer ob
-0001c230: 6a65 6374 0a20 2020 2020 2020 2072 6563  ject.        rec
-0001c240: 745f 7061 636b 6572 203d 2072 6563 7470  t_packer = rectp
-0001c250: 6163 6b2e 6e65 7750 6163 6b65 7228 0a20  ack.newPacker(. 
-0001c260: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
-0001c270: 7265 6374 7061 636b 2e50 6163 6b69 6e67  rectpack.Packing
-0001c280: 4d6f 6465 2e4f 6666 6c69 6e65 2c0a 2020  Mode.Offline,.  
-0001c290: 2020 2020 2020 2020 2020 7061 636b 5f61            pack_a
-0001c2a0: 6c67 6f3d 7265 6374 7061 636b 2e4d 6178  lgo=rectpack.Max
-0001c2b0: 5265 6374 7342 6c73 662c 0a20 2020 2020  RectsBlsf,.     
-0001c2c0: 2020 2020 2020 2073 6f72 745f 616c 676f         sort_algo
-0001c2d0: 3d72 705f 736f 7274 2c0a 2020 2020 2020  =rp_sort,.      
-0001c2e0: 2020 2020 2020 6269 6e5f 616c 676f 3d72        bin_algo=r
-0001c2f0: 6563 7470 6163 6b2e 5061 636b 696e 6742  ectpack.PackingB
-0001c300: 696e 2e42 4246 2c0a 2020 2020 2020 2020  in.BBF,.        
-0001c310: 2020 2020 726f 7461 7469 6f6e 3d46 616c      rotation=Fal
-0001c320: 7365 2c0a 2020 2020 2020 2020 290a 0a20  se,.        ).. 
-0001c330: 2020 2020 2020 2023 2041 6464 2065 6163         # Add eac
-0001c340: 6820 7265 6374 616e 676c 6520 746f 2074  h rectangle to t
-0001c350: 6865 2070 6163 6b65 722c 2063 7265 6174  he packer, creat
-0001c360: 6520 6120 7369 6e67 6c65 2062 696e 2c20  e a single bin, 
-0001c370: 616e 6420 7061 636b 0a20 2020 2020 2020  and pack.       
-0001c380: 2066 6f72 2072 6964 2c20 7220 696e 2072   for rid, r in r
-0001c390: 6563 745f 6469 6374 2e69 7465 6d73 2829  ect_dict.items()
-0001c3a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001c3b0: 6374 5f70 6163 6b65 722e 6164 645f 7265  ct_packer.add_re
-0001c3c0: 6374 2877 6964 7468 3d72 5b30 5d2c 2068  ct(width=r[0], h
-0001c3d0: 6569 6768 743d 725b 315d 2c20 7269 643d  eight=r[1], rid=
-0001c3e0: 7269 6429 0a20 2020 2020 2020 2072 6563  rid).        rec
-0001c3f0: 745f 7061 636b 6572 2e61 6464 5f62 696e  t_packer.add_bin
-0001c400: 2877 6964 7468 3d62 6f78 5f73 697a 655b  (width=box_size[
-0001c410: 305d 2c20 6865 6967 6874 3d62 6f78 5f73  0], height=box_s
-0001c420: 697a 655b 315d 290a 2020 2020 2020 2020  ize[1]).        
-0001c430: 7265 6374 5f70 6163 6b65 722e 7061 636b  rect_packer.pack
-0001c440: 2829 0a0a 2020 2020 2020 2020 2320 4164  ()..        # Ad
-0001c450: 6a75 7374 2074 6865 2062 6f78 2073 697a  just the box siz
-0001c460: 6520 666f 7220 6e65 7874 2074 696d 650a  e for next time.
-0001c470: 2020 2020 2020 2020 626f 785f 7369 7a65          box_size
-0001c480: 202a 3d20 6465 6e73 6974 7920 2023 2049   *= density  # I
-0001c490: 6e63 7265 6173 6520 6172 6561 2074 6f20  ncrease area to 
-0001c4a0: 7472 7920 746f 2066 6974 0a20 2020 2020  try to fit.     
-0001c4b0: 2020 2062 6f78 5f73 697a 6520 3d20 6e70     box_size = np
-0001c4c0: 2e63 6c69 7028 626f 785f 7369 7a65 2c20  .clip(box_size, 
-0001c4d0: 4e6f 6e65 2c20 6d61 785f 7369 7a65 290a  None, max_size).
-0001c4e0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0001c4f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001c500: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0001c510: 2020 2020 2020 2022 5472 7969 6e67 2074         "Trying t
-0001c520: 6f20 7061 636b 2069 6e20 6269 6e20 7369  o pack in bin si
-0001c530: 7a65 2022 0a20 2020 2020 2020 2020 2020  ze ".           
-0001c540: 2020 2020 2022 2825 302e 3266 2c20 2530       "(%0.2f, %0
-0001c550: 2e32 6629 2220 2520 7475 706c 6528 626f  .2f)" % tuple(bo
-0001c560: 785f 7369 7a65 202a 2070 7265 6369 7369  x_size * precisi
-0001c570: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-0001c580: 290a 0a20 2020 2020 2020 2023 2051 7569  )..        # Qui
-0001c590: 7420 7468 6520 6c6f 6f70 2069 6620 7765  t the loop if we
-0001c5a0: 2776 6520 7061 636b 6564 2061 6c6c 2074  've packed all t
-0001c5b0: 6865 2072 6563 7461 6e67 6c65 730a 2020  he rectangles.  
-0001c5c0: 2020 2020 2020 2320 6f72 2072 6561 6368        # or reach
-0001c5d0: 6564 2074 6865 206d 6178 2073 697a 650a  ed the max size.
-0001c5e0: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-0001c5f0: 6563 745f 7061 636b 6572 2e72 6563 745f  ect_packer.rect_
-0001c600: 6c69 7374 2829 2920 3d3d 206c 656e 2872  list()) == len(r
-0001c610: 6563 745f 6469 6374 293a 0a20 2020 2020  ect_dict):.     
-0001c620: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-0001c630: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001c640: 2020 2070 7269 6e74 2822 5375 6363 6573     print("Succes
-0001c650: 7321 2229 0a20 2020 2020 2020 2020 2020  s!").           
-0001c660: 2062 7265 616b 0a20 2020 2020 2020 2065   break.        e
-0001c670: 6c69 6620 616c 6c28 626f 785f 7369 7a65  lif all(box_size
-0001c680: 203e 3d20 6d61 785f 7369 7a65 293a 0a20   >= max_size):. 
-0001c690: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
-0001c6a0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-0001c6b0: 2020 2020 2020 2070 7269 6e74 2822 5265         print("Re
-0001c6c0: 6163 6865 6420 6d61 785f 7369 7a65 2c20  ached max_size, 
-0001c6d0: 6372 6561 7469 6e67 2022 2022 616e 2061  creating " "an a
-0001c6e0: 6464 6974 696f 6e61 6c20 6269 6e22 290a  dditional bin").
-0001c6f0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0001c700: 6b0a 0a20 2020 2023 2053 6570 6172 6174  k..    # Separat
-0001c710: 6520 7061 636b 6564 2066 726f 6d20 756e  e packed from un
-0001c720: 7061 636b 6564 2072 6563 7461 6e67 6c65  packed rectangle
-0001c730: 732c 206d 616b 6520 6469 6374 7320 6f66  s, make dicts of
-0001c740: 2066 6f72 6d0a 2020 2020 2320 7b69 643a   form.    # {id:
-0001c750: 2878 2c79 2c77 2c68 297d 0a20 2020 2070  (x,y,w,h)}.    p
-0001c760: 6163 6b65 645f 7265 6374 5f64 6963 7420  acked_rect_dict 
-0001c770: 3d20 7b72 5b2d 315d 3a20 725b 3a2d 315d  = {r[-1]: r[:-1]
-0001c780: 2066 6f72 2072 2069 6e20 7265 6374 5f70   for r in rect_p
-0001c790: 6163 6b65 725b 305d 2e72 6563 745f 6c69  acker[0].rect_li
-0001c7a0: 7374 2829 7d0a 2020 2020 756e 7061 636b  st()}.    unpack
-0001c7b0: 6564 5f72 6563 745f 6469 6374 203d 207b  ed_rect_dict = {
-0001c7c0: 7d0a 2020 2020 666f 7220 6b2c 2076 2069  }.    for k, v i
-0001c7d0: 6e20 7265 6374 5f64 6963 742e 6974 656d  n rect_dict.item
-0001c7e0: 7328 293a 0a20 2020 2020 2020 2069 6620  s():.        if 
-0001c7f0: 6b20 6e6f 7420 696e 2070 6163 6b65 645f  k not in packed_
-0001c800: 7265 6374 5f64 6963 743a 0a20 2020 2020  rect_dict:.     
-0001c810: 2020 2020 2020 2075 6e70 6163 6b65 645f         unpacked_
-0001c820: 7265 6374 5f64 6963 745b 6b5d 203d 2076  rect_dict[k] = v
-0001c830: 0a0a 2020 2020 7265 7475 726e 2028 7061  ..    return (pa
-0001c840: 636b 6564 5f72 6563 745f 6469 6374 2c20  cked_rect_dict, 
-0001c850: 756e 7061 636b 6564 5f72 6563 745f 6469  unpacked_rect_di
-0001c860: 6374 290a 0a0a 6465 6620 7061 636b 6572  ct)...def packer
-0001c870: 280a 2020 2020 445f 6c69 7374 2c0a 2020  (.    D_list,.  
-0001c880: 2020 7370 6163 696e 673d 3130 2c0a 2020    spacing=10,.  
-0001c890: 2020 6173 7065 6374 5f72 6174 696f 3d28    aspect_ratio=(
-0001c8a0: 312c 2031 292c 0a20 2020 206d 6178 5f73  1, 1),.    max_s
-0001c8b0: 697a 653d 284e 6f6e 652c 204e 6f6e 6529  ize=(None, None)
-0001c8c0: 2c0a 2020 2020 736f 7274 5f62 795f 6172  ,.    sort_by_ar
-0001c8d0: 6561 3d54 7275 652c 0a20 2020 2064 656e  ea=True,.    den
-0001c8e0: 7369 7479 3d31 2e31 2c0a 2020 2020 7072  sity=1.1,.    pr
-0001c8f0: 6563 6973 696f 6e3d 3165 2d32 2c0a 2020  ecision=1e-2,.  
-0001c900: 2020 7665 7262 6f73 653d 4661 6c73 652c    verbose=False,
-0001c910: 0a29 3a0a 2020 2020 2222 2250 6163 6b73  .):.    """Packs
-0001c920: 2067 656f 6d65 7472 6965 7320 746f 6765   geometries toge
-0001c930: 7468 6572 2069 6e74 6f20 7265 6374 616e  ther into rectan
-0001c940: 6775 6c61 7220 6269 6e73 2e0a 0a20 2020  gular bins...   
-0001c950: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0001c960: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044  ----------.    D
-0001c970: 5f6c 6973 7420 3a20 6172 7261 792d 6c69  _list : array-li
-0001c980: 6b65 206f 6620 4465 7669 6365 730a 2020  ke of Devices.  
-0001c990: 2020 2020 2020 496e 7075 7420 4465 7669        Input Devi
-0001c9a0: 6365 7320 746f 2062 6520 7061 636b 6564  ces to be packed
-0001c9b0: 2e0a 2020 2020 7370 6163 696e 6720 3a20  ..    spacing : 
-0001c9c0: 696e 7420 6f72 2066 6c6f 6174 0a20 2020  int or float.   
-0001c9d0: 2020 2020 2054 6865 206d 696e 696d 756d       The minimum
-0001c9e0: 2064 6973 7461 6e63 6520 6265 7477 6565   distance betwee
-0001c9f0: 6e20 6164 6a61 6365 6e74 2073 6861 7065  n adjacent shape
-0001ca00: 732e 0a20 2020 2061 7370 6563 745f 7261  s..    aspect_ra
-0001ca10: 7469 6f20 3a20 6172 7261 792d 6c69 6b65  tio : array-like
-0001ca20: 0a20 2020 2020 2020 2054 6865 2028 7769  .        The (wi
-0001ca30: 6474 682c 2068 6569 6768 7429 2072 6174  dth, height) rat
-0001ca40: 696f 206f 6620 7468 6520 7265 6374 616e  io of the rectan
-0001ca50: 6775 6c61 7220 6269 6e2e 0a20 2020 206d  gular bin..    m
-0001ca60: 6178 5f73 697a 6520 3a20 6172 7261 792d  ax_size : array-
-0001ca70: 6c69 6b65 0a20 2020 2020 2020 204c 696d  like.        Lim
-0001ca80: 6974 7320 7468 6520 7369 7a65 2069 6e74  its the size int
-0001ca90: 6f20 7768 6963 6820 7468 6520 7368 6170  o which the shap
-0001caa0: 6573 2077 696c 6c20 6265 2070 6163 6b65  es will be packe
-0001cab0: 642e 0a20 2020 2073 6f72 745f 6279 5f61  d..    sort_by_a
-0001cac0: 7265 6120 3a20 626f 6f6c 0a20 2020 2020  rea : bool.     
-0001cad0: 2020 2049 6620 7472 7565 2c20 7072 652d     If true, pre-
-0001cae0: 736f 7274 7320 7468 6520 7368 6170 6573  sorts the shapes
-0001caf0: 2062 7920 6172 6561 2e0a 2020 2020 6465   by area..    de
-0001cb00: 6e73 6974 7920 3a20 696e 7420 6f72 2066  nsity : int or f
-0001cb10: 6c6f 6174 0a20 2020 2020 2020 2044 656e  loat.        Den
-0001cb20: 7369 7479 206f 6620 7061 636b 696e 672e  sity of packing.
-0001cb30: 2056 616c 7565 7320 636c 6f73 6572 2074   Values closer t
-0001cb40: 6f20 3120 7061 636b 2074 6967 6874 6572  o 1 pack tighter
-0001cb50: 2062 7574 2072 6571 7569 7265 206d 6f72   but require mor
-0001cb60: 650a 2020 2020 2020 2020 636f 6d70 7574  e.        comput
-0001cb70: 6174 696f 6e2e 0a20 2020 2070 7265 6369  ation..    preci
-0001cb80: 7369 6f6e 203a 2066 6c6f 6174 0a20 2020  sion : float.   
-0001cb90: 2020 2020 2044 6573 6972 6564 2070 7265       Desired pre
-0001cba0: 6369 7369 6f6e 2066 6f72 2072 6f75 6e64  cision for round
-0001cbb0: 696e 6720 7665 7274 6578 2063 6f6f 7264  ing vertex coord
-0001cbc0: 696e 6174 6573 2e0a 2020 2020 7665 7262  inates..    verb
-0001cbd0: 6f73 6520 3a20 626f 6f6c 0a20 2020 2020  ose : bool.     
-0001cbe0: 2020 2057 6865 7468 6572 2074 6f20 6469     Whether to di
-0001cbf0: 7370 6c61 7920 7265 7375 6c74 7320 6f66  splay results of
-0001cc00: 2070 6163 6b69 6e67 2061 7474 656d 7074   packing attempt
-0001cc10: 730a 0a0a 2020 2020 5265 7475 726e 730a  s...    Returns.
-0001cc20: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001cc30: 445f 7061 636b 6564 5f6c 6973 7420 3a20  D_packed_list : 
-0001cc40: 4465 7669 6365 206f 7220 6c69 7374 206f  Device or list o
-0001cc50: 6620 4465 7669 6365 730a 2020 2020 2020  f Devices.      
-0001cc60: 2020 4120 4465 7669 6365 206f 7220 6c69    A Device or li
-0001cc70: 7374 206f 6620 4465 7669 6365 7320 636f  st of Devices co
-0001cc80: 6e74 6169 6e69 6e67 2061 6c6c 2074 6865  ntaining all the
-0001cc90: 2070 6163 6b65 6420 7265 6374 616e 6775   packed rectangu
-0001cca0: 6c61 720a 2020 2020 2020 2020 6269 6e73  lar.        bins
-0001ccb0: 2067 656e 6572 6174 6564 2e0a 0a20 2020   generated...   
-0001ccc0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-0001ccd0: 0a20 2020 2049 6620 6120 6d61 782d 7369  .    If a max-si
-0001cce0: 7a65 2069 7320 7370 6563 6966 6965 642c  ze is specified,
-0001ccf0: 2074 6865 2066 756e 6374 696f 6e20 7769   the function wi
-0001cd00: 6c6c 2063 7265 6174 6520 6173 206d 616e  ll create as man
-0001cd10: 7920 6269 6e73 2061 730a 2020 2020 6e65  y bins as.    ne
-0001cd20: 6365 7373 6172 7920 746f 2070 6163 6b20  cessary to pack 
-0001cd30: 616c 6c20 7468 6520 6765 6f6d 6574 7269  all the geometri
-0001cd40: 6573 2061 6e64 2074 6865 6e20 7265 7475  es and then retu
-0001cd50: 726e 2061 206c 6973 7420 6f66 2074 6865  rn a list of the
-0001cd60: 0a20 2020 2066 696c 6c65 642d 6269 6e20  .    filled-bin 
-0001cd70: 4465 7669 6365 732e 0a20 2020 2022 2222  Devices..    """
-0001cd80: 0a20 2020 2069 6620 6465 6e73 6974 7920  .    if density 
-0001cd90: 3c20 312e 3031 3a0a 2020 2020 2020 2020  < 1.01:.        
-0001cda0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001cdb0: 280a 2020 2020 2020 2020 2020 2020 225b  (.            "[
-0001cdc0: 5048 4944 4c5d 2070 6163 6b65 7228 2920  PHIDL] packer() 
-0001cdd0: 7761 7320 6769 7665 6e20 6120 6064 656e  was given a `den
-0001cde0: 7369 7479 6020 6172 6775 6d65 6e74 2022  sity` argument "
-0001cdf0: 0a20 2020 2020 2020 2020 2020 2022 7468  .            "th
-0001ce00: 6174 2069 7320 746f 6f20 736d 616c 6c2e  at is too small.
-0001ce10: 2020 5468 6520 6465 6e73 6974 7920 6172    The density ar
-0001ce20: 6775 6d65 6e74 206d 7573 7420 6265 2022  gument must be "
-0001ce30: 0a20 2020 2020 2020 2020 2020 2022 3e3d  .            ">=
-0001ce40: 2031 2e30 3122 0a20 2020 2020 2020 2029   1.01".        )
-0001ce50: 0a0a 2020 2020 2320 5361 6e74 697a 6520  ..    # Santize 
-0001ce60: 6d61 785f 7369 7a65 2076 6172 6961 626c  max_size variabl
-0001ce70: 650a 2020 2020 6d61 785f 7369 7a65 203d  e.    max_size =
-0001ce80: 205b 6e70 2e69 6e66 2069 6620 7620 6973   [np.inf if v is
-0001ce90: 204e 6f6e 6520 656c 7365 2076 2066 6f72   None else v for
-0001cea0: 2076 2069 6e20 6d61 785f 7369 7a65 5d0a   v in max_size].
-0001ceb0: 2020 2020 6d61 785f 7369 7a65 203d 206e      max_size = n
-0001cec0: 702e 6173 6172 7261 7928 6d61 785f 7369  p.asarray(max_si
-0001ced0: 7a65 2c20 6474 7970 653d 6e70 2e66 6c6f  ze, dtype=np.flo
-0001cee0: 6174 3634 2920 2023 2049 6e20 6361 7365  at64)  # In case
-0001cef0: 2069 7427 7320 696e 7465 6765 7273 0a20   it's integers. 
-0001cf00: 2020 206d 6178 5f73 697a 6520 3d20 6d61     max_size = ma
-0001cf10: 785f 7369 7a65 202f 2070 7265 6369 7369  x_size / precisi
-0001cf20: 6f6e 0a0a 2020 2020 2320 436f 6e76 6572  on..    # Conver
-0001cf30: 7420 4465 7669 6365 7320 746f 2072 6563  t Devices to rec
-0001cf40: 7461 6e67 6c65 730a 2020 2020 7265 6374  tangles.    rect
-0001cf50: 5f64 6963 7420 3d20 7b7d 0a20 2020 2066  _dict = {}.    f
-0001cf60: 6f72 206e 2c20 4420 696e 2065 6e75 6d65  or n, D in enume
-0001cf70: 7261 7465 2844 5f6c 6973 7429 3a0a 2020  rate(D_list):.  
-0001cf80: 2020 2020 2020 772c 2068 203d 2028 442e        w, h = (D.
-0001cf90: 7369 7a65 202b 2073 7061 6369 6e67 2920  size + spacing) 
-0001cfa0: 2f20 7072 6563 6973 696f 6e0a 2020 2020  / precision.    
-0001cfb0: 2020 2020 772c 2068 203d 2069 6e74 2877      w, h = int(w
-0001cfc0: 292c 2069 6e74 2868 290a 2020 2020 2020  ), int(h).      
-0001cfd0: 2020 6966 2028 7720 3e20 6d61 785f 7369    if (w > max_si
-0001cfe0: 7a65 5b30 5d29 206f 7220 2868 203e 206d  ze[0]) or (h > m
-0001cff0: 6178 5f73 697a 655b 315d 293a 0a20 2020  ax_size[1]):.   
-0001d000: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0001d010: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0001d020: 2020 2020 2020 2020 2020 2022 5b50 4849             "[PHI
-0001d030: 444c 5d20 7061 636b 6572 2829 2066 6169  DL] packer() fai
-0001d040: 6c65 6420 6265 6361 7573 6520 6f6e 6520  led because one 
-0001d050: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
-0001d060: 2020 2020 2022 7468 6520 6f62 6a65 6374       "the object
-0001d070: 7320 696e 2060 445f 6c69 7374 6020 6973  s in `D_list` is
-0001d080: 2068 6173 2061 6e20 7820 6f72 2022 0a20   has an x or ". 
-0001d090: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001d0a0: 7920 6469 6d65 6e73 696f 6e20 6c61 7267  y dimension larg
-0001d0b0: 6572 2074 6861 6e20 606d 6178 5f73 697a  er than `max_siz
-0001d0c0: 6560 2061 6e64 2022 0a20 2020 2020 2020  e` and ".       
-0001d0d0: 2020 2020 2020 2020 2022 736f 2063 616e           "so can
-0001d0e0: 6e6f 7420 6265 2070 6163 6b65 6422 0a20  not be packed". 
-0001d0f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001d100: 2020 2020 2072 6563 745f 6469 6374 5b6e       rect_dict[n
-0001d110: 5d20 3d20 2877 2c20 6829 0a0a 2020 2020  ] = (w, h)..    
-0001d120: 7061 636b 6564 5f6c 6973 7420 3d20 5b5d  packed_list = []
-0001d130: 0a20 2020 2077 6869 6c65 206c 656e 2872  .    while len(r
-0001d140: 6563 745f 6469 6374 2920 3e20 303a 0a20  ect_dict) > 0:. 
-0001d150: 2020 2020 2020 2028 7061 636b 6564 5f72         (packed_r
-0001d160: 6563 745f 6469 6374 2c20 7265 6374 5f64  ect_dict, rect_d
-0001d170: 6963 7429 203d 205f 7061 636b 5f73 696e  ict) = _pack_sin
-0001d180: 676c 655f 6269 6e28 0a20 2020 2020 2020  gle_bin(.       
-0001d190: 2020 2020 2072 6563 745f 6469 6374 2c0a       rect_dict,.
-0001d1a0: 2020 2020 2020 2020 2020 2020 6173 7065              aspe
-0001d1b0: 6374 5f72 6174 696f 3d61 7370 6563 745f  ct_ratio=aspect_
-0001d1c0: 7261 7469 6f2c 0a20 2020 2020 2020 2020  ratio,.         
-0001d1d0: 2020 206d 6178 5f73 697a 653d 6d61 785f     max_size=max_
-0001d1e0: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
-0001d1f0: 2020 736f 7274 5f62 795f 6172 6561 3d73    sort_by_area=s
-0001d200: 6f72 745f 6279 5f61 7265 612c 0a20 2020  ort_by_area,.   
-0001d210: 2020 2020 2020 2020 2064 656e 7369 7479           density
-0001d220: 3d64 656e 7369 7479 2c0a 2020 2020 2020  =density,.      
-0001d230: 2020 2020 2020 7072 6563 6973 696f 6e3d        precision=
-0001d240: 7072 6563 6973 696f 6e2c 0a20 2020 2020  precision,.     
-0001d250: 2020 2020 2020 2076 6572 626f 7365 3d76         verbose=v
-0001d260: 6572 626f 7365 2c0a 2020 2020 2020 2020  erbose,.        
-0001d270: 290a 2020 2020 2020 2020 7061 636b 6564  ).        packed
-0001d280: 5f6c 6973 742e 6170 7065 6e64 2870 6163  _list.append(pac
-0001d290: 6b65 645f 7265 6374 5f64 6963 7429 0a0a  ked_rect_dict)..
-0001d2a0: 2020 2020 445f 7061 636b 6564 5f6c 6973      D_packed_lis
-0001d2b0: 7420 3d20 5b5d 0a20 2020 2066 6f72 2072  t = [].    for r
-0001d2c0: 6563 745f 6469 6374 2069 6e20 7061 636b  ect_dict in pack
-0001d2d0: 6564 5f6c 6973 743a 0a20 2020 2020 2020  ed_list:.       
-0001d2e0: 2044 5f70 6163 6b65 6420 3d20 4465 7669   D_packed = Devi
-0001d2f0: 6365 2829 0a20 2020 2020 2020 2066 6f72  ce().        for
-0001d300: 206e 2c20 7265 6374 2069 6e20 7265 6374   n, rect in rect
-0001d310: 5f64 6963 742e 6974 656d 7328 293a 0a20  _dict.items():. 
-0001d320: 2020 2020 2020 2020 2020 2078 2c20 792c             x, y,
-0001d330: 2077 2c20 6820 3d20 7265 6374 0a20 2020   w, h = rect.   
-0001d340: 2020 2020 2020 2020 2078 6365 6e74 6572           xcenter
-0001d350: 203d 2078 202b 2077 202f 2032 202b 2073   = x + w / 2 + s
-0001d360: 7061 6369 6e67 202f 2032 0a20 2020 2020  pacing / 2.     
-0001d370: 2020 2020 2020 2079 6365 6e74 6572 203d         ycenter =
-0001d380: 2079 202b 2068 202f 2032 202b 2073 7061   y + h / 2 + spa
-0001d390: 6369 6e67 202f 2032 0a20 2020 2020 2020  cing / 2.       
-0001d3a0: 2020 2020 2064 203d 2044 5f70 6163 6b65       d = D_packe
-0001d3b0: 642e 6164 645f 7265 6628 445f 6c69 7374  d.add_ref(D_list
-0001d3c0: 5b6e 5d29 0a20 2020 2020 2020 2020 2020  [n]).           
-0001d3d0: 2064 2e63 656e 7465 7220 3d20 2878 6365   d.center = (xce
-0001d3e0: 6e74 6572 202a 2070 7265 6369 7369 6f6e  nter * precision
-0001d3f0: 2c20 7963 656e 7465 7220 2a20 7072 6563  , ycenter * prec
-0001d400: 6973 696f 6e29 0a20 2020 2020 2020 2044  ision).        D
-0001d410: 5f70 6163 6b65 645f 6c69 7374 2e61 7070  _packed_list.app
-0001d420: 656e 6428 445f 7061 636b 6564 290a 0a20  end(D_packed).. 
-0001d430: 2020 2072 6574 7572 6e20 445f 7061 636b     return D_pack
-0001d440: 6564 5f6c 6973 740a 0a0a 6465 6620 5f72  ed_list...def _r
-0001d450: 6173 7465 7269 7a65 5f70 6f6c 7967 6f6e  asterize_polygon
-0001d460: 7328 706f 6c79 676f 6e73 2c20 626f 756e  s(polygons, boun
-0001d470: 6473 3d5b 5b2d 3130 302c 202d 3130 305d  ds=[[-100, -100]
-0001d480: 2c20 5b31 3030 2c20 3130 305d 5d2c 2064  , [100, 100]], d
-0001d490: 783d 312c 2064 793d 3129 3a0a 2020 2020  x=1, dy=1):.    
-0001d4a0: 2222 2243 6f6e 7665 7274 7320 706f 6c79  """Converts poly
-0001d4b0: 676f 6e73 2074 6f20 6120 626c 6163 6b2f  gons to a black/
-0001d4c0: 7768 6974 6520 2831 2f30 2920 6d61 7472  white (1/0) matr
-0001d4d0: 6978 2222 220a 2020 2020 7472 793a 0a20  ix""".    try:. 
-0001d4e0: 2020 2020 2020 2066 726f 6d20 736b 696d         from skim
-0001d4f0: 6167 6520 696d 706f 7274 2064 7261 770a  age import draw.
-0001d500: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0001d510: 7469 6f6e 3a0a 2020 2020 2020 2020 7261  tion:.        ra
-0001d520: 6973 6520 496d 706f 7274 4572 726f 7228  ise ImportError(
-0001d530: 0a20 2020 2020 2020 2020 2020 2022 5468  .            "Th
-0001d540: 6520 6669 6c6c 2066 756e 6374 696f 6e20  e fill function 
-0001d550: 7265 7175 6972 6573 2074 6865 206d 6f64  requires the mod
-0001d560: 756c 6520 220a 2020 2020 2020 2020 2020  ule ".          
-0001d570: 2020 2722 7363 696b 6974 2d69 6d61 6765    '"scikit-image
-0001d580: 2220 746f 206f 7065 7261 7465 2e20 2050  " to operate.  P
-0001d590: 6c65 6173 6520 7265 7472 7920 270a 2020  lease retry '.  
-0001d5a0: 2020 2020 2020 2020 2020 2261 6674 6572            "after
-0001d5b0: 2069 6e73 7461 6c6c 696e 6720 7363 696b   installing scik
-0001d5c0: 6974 2d69 6d61 6765 3a5c 6e5c 6e22 0a20  it-image:\n\n". 
-0001d5d0: 2020 2020 2020 2020 2020 2022 2420 7069             "$ pi
-0001d5e0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-0001d5f0: 6164 6520 7363 696b 6974 2d69 6d61 6765  ade scikit-image
-0001d600: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
-0001d610: 2023 2050 7265 7061 7265 2070 6f6c 7967   # Prepare polyg
-0001d620: 6f6e 2061 7272 6179 2062 7920 7368 6966  on array by shif
-0001d630: 7469 6e67 2061 6c6c 2070 6f69 6e74 7320  ting all points 
-0001d640: 696e 746f 2074 6865 2066 6972 7374 2071  into the first q
-0001d650: 7561 6472 616e 7420 616e 640a 2020 2020  uadrant and.    
-0001d660: 2320 7365 7061 7261 7469 6e67 2070 6f69  # separating poi
-0001d670: 6e74 7320 696e 746f 2078 2061 6e64 2079  nts into x and y
-0001d680: 206c 6973 7473 0a20 2020 2078 7074 7320   lists.    xpts 
-0001d690: 3d20 5b5d 0a20 2020 2079 7074 7320 3d20  = [].    ypts = 
-0001d6a0: 5b5d 0a20 2020 2066 6f72 2070 2069 6e20  [].    for p in 
-0001d6b0: 706f 6c79 676f 6e73 3a0a 2020 2020 2020  polygons:.      
-0001d6c0: 2020 705f 6172 7261 7920 3d20 6e70 2e61    p_array = np.a
-0001d6d0: 7361 7272 6179 2870 290a 2020 2020 2020  sarray(p).      
-0001d6e0: 2020 7820 3d20 705f 6172 7261 795b 3a2c    x = p_array[:,
-0001d6f0: 2030 5d0a 2020 2020 2020 2020 7920 3d20   0].        y = 
-0001d700: 705f 6172 7261 795b 3a2c 2031 5d0a 2020  p_array[:, 1].  
-0001d710: 2020 2020 2020 7870 7473 2e61 7070 656e        xpts.appen
-0001d720: 6428 2878 202d 2062 6f75 6e64 735b 305d  d((x - bounds[0]
-0001d730: 5b30 5d29 202f 2064 7820 2d20 302e 3529  [0]) / dx - 0.5)
-0001d740: 0a20 2020 2020 2020 2079 7074 732e 6170  .        ypts.ap
-0001d750: 7065 6e64 2828 7920 2d20 626f 756e 6473  pend((y - bounds
-0001d760: 5b30 5d5b 315d 2920 2f20 6479 202d 2030  [0][1]) / dy - 0
-0001d770: 2e35 290a 0a20 2020 2023 2049 6e69 7469  .5)..    # Initi
-0001d780: 616c 697a 6520 7468 6520 7261 7374 6572  alize the raster
-0001d790: 206d 6174 7269 7820 7765 276c 6c20 6265   matrix we'll be
-0001d7a0: 2077 7269 7469 6e67 2074 6f0a 2020 2020   writing to.    
-0001d7b0: 7873 697a 6520 3d20 696e 7428 6e70 2e63  xsize = int(np.c
-0001d7c0: 6569 6c28 626f 756e 6473 5b31 5d5b 305d  eil(bounds[1][0]
-0001d7d0: 202d 2062 6f75 6e64 735b 305d 5b30 5d29   - bounds[0][0])
-0001d7e0: 202f 2064 7829 0a20 2020 2079 7369 7a65   / dx).    ysize
-0001d7f0: 203d 2069 6e74 286e 702e 6365 696c 2862   = int(np.ceil(b
-0001d800: 6f75 6e64 735b 315d 5b31 5d20 2d20 626f  ounds[1][1] - bo
-0001d810: 756e 6473 5b30 5d5b 315d 2920 2f20 6479  unds[0][1]) / dy
-0001d820: 290a 2020 2020 7261 7374 6572 203d 206e  ).    raster = n
-0001d830: 702e 7a65 726f 7328 2879 7369 7a65 2c20  p.zeros((ysize, 
-0001d840: 7873 697a 6529 2c20 6474 7970 653d 6e70  xsize), dtype=np
-0001d850: 2e62 6f6f 6c29 0a0a 2020 2020 2320 544f  .bool)..    # TO
-0001d860: 444f 3a20 5265 706c 6163 6520 706f 6c79  DO: Replace poly
-0001d870: 676f 6e5f 7065 7269 6d65 7465 7220 7769  gon_perimeter wi
-0001d880: 7468 2074 6865 2073 7570 6572 636f 7665  th the supercove
-0001d890: 7220 7665 7273 696f 6e0a 2020 2020 666f  r version.    fo
-0001d8a0: 7220 6e20 696e 2072 616e 6765 286c 656e  r n in range(len
-0001d8b0: 2878 7074 7329 293a 0a20 2020 2020 2020  (xpts)):.       
-0001d8c0: 2072 722c 2063 6320 3d20 6472 6177 2e70   rr, cc = draw.p
-0001d8d0: 6f6c 7967 6f6e 2879 7074 735b 6e5d 2c20  olygon(ypts[n], 
-0001d8e0: 7870 7473 5b6e 5d2c 2073 6861 7065 3d72  xpts[n], shape=r
-0001d8f0: 6173 7465 722e 7368 6170 6529 0a20 2020  aster.shape).   
-0001d900: 2020 2020 2072 7270 2c20 6363 7020 3d20       rrp, ccp = 
-0001d910: 6472 6177 2e70 6f6c 7967 6f6e 5f70 6572  draw.polygon_per
-0001d920: 696d 6574 6572 280a 2020 2020 2020 2020  imeter(.        
-0001d930: 2020 2020 7970 7473 5b6e 5d2c 2078 7074      ypts[n], xpt
-0001d940: 735b 6e5d 2c20 7368 6170 653d 7261 7374  s[n], shape=rast
-0001d950: 6572 2e73 6861 7065 2c20 636c 6970 3d46  er.shape, clip=F
-0001d960: 616c 7365 0a20 2020 2020 2020 2029 0a20  alse.        ). 
-0001d970: 2020 2020 2020 2072 6173 7465 725b 7272         raster[rr
-0001d980: 2c20 6363 5d20 3d20 310a 2020 2020 2020  , cc] = 1.      
-0001d990: 2020 7261 7374 6572 5b72 7270 2c20 6363    raster[rrp, cc
-0001d9a0: 705d 203d 2031 0a0a 2020 2020 7265 7475  p] = 1..    retu
-0001d9b0: 726e 2072 6173 7465 720a 0a0a 6465 6620  rn raster...def 
-0001d9c0: 5f72 6173 7465 725f 696e 6465 785f 746f  _raster_index_to
-0001d9d0: 5f63 6f6f 7264 7328 692c 206a 2c20 626f  _coords(i, j, bo
-0001d9e0: 756e 6473 3d5b 5b2d 3130 302c 202d 3130  unds=[[-100, -10
-0001d9f0: 305d 2c20 5b31 3030 2c20 3130 305d 5d2c  0], [100, 100]],
-0001da00: 2064 783d 312c 2064 793d 3129 3a0a 2020   dx=1, dy=1):.  
-0001da10: 2020 2222 2243 6f6e 7665 7274 7320 2869    """Converts (i
-0001da20: 2c6a 2920 696e 6465 7820 6f66 2072 6173  ,j) index of ras
-0001da30: 7465 7220 6d61 7472 6978 2074 6f20 7265  ter matrix to re
-0001da40: 616c 2063 6f6f 7264 696e 6174 6573 2222  al coordinates""
-0001da50: 220a 2020 2020 7820 3d20 286a 202b 2030  ".    x = (j + 0
-0001da60: 2e35 2920 2a20 6478 202b 2062 6f75 6e64  .5) * dx + bound
-0001da70: 735b 305d 5b30 5d0a 2020 2020 7920 3d20  s[0][0].    y = 
-0001da80: 2869 202b 2030 2e35 2920 2a20 6479 202b  (i + 0.5) * dy +
-0001da90: 2062 6f75 6e64 735b 305d 5b31 5d0a 2020   bounds[0][1].  
-0001daa0: 2020 7265 7475 726e 2078 2c20 790a 0a0a    return x, y...
-0001dab0: 6465 6620 5f65 7870 616e 645f 7261 7374  def _expand_rast
-0001dac0: 6572 2872 6173 7465 722c 2064 6973 7461  er(raster, dista
-0001dad0: 6e63 653d 2834 2c20 3229 293a 0a20 2020  nce=(4, 2)):.   
-0001dae0: 2022 2222 4578 7061 6e64 7320 616c 6c20   """Expands all 
-0001daf0: 626c 6163 6b20 2831 2920 7069 7865 6c73  black (1) pixels
-0001db00: 2069 6e20 7468 6520 7261 7374 6572 2222   in the raster""
-0001db10: 220a 2020 2020 7472 793a 0a20 2020 2020  ".    try:.     
-0001db20: 2020 2066 726f 6d20 736b 696d 6167 6520     from skimage 
-0001db30: 696d 706f 7274 2064 7261 772c 206d 6f72  import draw, mor
-0001db40: 7068 6f6c 6f67 790a 2020 2020 6578 6365  phology.    exce
-0001db50: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
-0001db60: 2020 2020 2020 7261 6973 6520 496d 706f        raise Impo
-0001db70: 7274 4572 726f 7228 0a20 2020 2020 2020  rtError(.       
-0001db80: 2020 2020 2022 5468 6520 6669 6c6c 2066       "The fill f
-0001db90: 756e 6374 696f 6e20 7265 7175 6972 6573  unction requires
-0001dba0: 2074 6865 206d 6f64 756c 6520 220a 2020   the module ".  
-0001dbb0: 2020 2020 2020 2020 2020 2722 7363 696b            '"scik
-0001dbc0: 6974 2d69 6d61 6765 2220 746f 206f 7065  it-image" to ope
-0001dbd0: 7261 7465 2e20 2050 6c65 6173 6520 7265  rate.  Please re
-0001dbe0: 7472 7920 270a 2020 2020 2020 2020 2020  try '.          
-0001dbf0: 2020 2261 6674 6572 2069 6e73 7461 6c6c    "after install
-0001dc00: 696e 6720 7363 696b 6974 2d69 6d61 6765  ing scikit-image
-0001dc10: 3a5c 6e5c 6e22 0a20 2020 2020 2020 2020  :\n\n".         
-0001dc20: 2020 2022 2420 7069 7020 696e 7374 616c     "$ pip instal
-0001dc30: 6c20 2d2d 7570 6772 6164 6520 7363 696b  l --upgrade scik
-0001dc40: 6974 2d69 6d61 6765 220a 2020 2020 2020  it-image".      
-0001dc50: 2020 290a 2020 2020 6966 2064 6973 7461    ).    if dista
-0001dc60: 6e63 655b 305d 203c 3d20 302e 3520 616e  nce[0] <= 0.5 an
-0001dc70: 6420 6469 7374 616e 6365 5b31 5d20 3c3d  d distance[1] <=
-0001dc80: 2030 2e35 3a0a 2020 2020 2020 2020 7265   0.5:.        re
-0001dc90: 7475 726e 2072 6173 7465 720a 0a20 2020  turn raster..   
-0001dca0: 206e 756d 5f70 6978 656c 7320 3d20 6e70   num_pixels = np
-0001dcb0: 2e61 7272 6179 286e 702e 6365 696c 2864  .array(np.ceil(d
-0001dcc0: 6973 7461 6e63 6529 2c20 6474 7970 653d  istance), dtype=
-0001dcd0: 696e 7429 0a20 2020 206e 6569 6768 626f  int).    neighbo
-0001dce0: 7268 6f6f 6420 3d20 6e70 2e7a 6572 6f73  rhood = np.zeros
-0001dcf0: 280a 2020 2020 2020 2020 286e 756d 5f70  (.        (num_p
-0001dd00: 6978 656c 735b 315d 202a 2032 202b 2031  ixels[1] * 2 + 1
-0001dd10: 2c20 6e75 6d5f 7069 7865 6c73 5b30 5d20  , num_pixels[0] 
-0001dd20: 2a20 3220 2b20 3129 2c20 6474 7970 653d  * 2 + 1), dtype=
-0001dd30: 6e70 2e62 6f6f 6c0a 2020 2020 290a 2020  np.bool.    ).  
-0001dd40: 2020 7272 2c20 6363 203d 2064 7261 772e    rr, cc = draw.
-0001dd50: 656c 6c69 7073 6528 0a20 2020 2020 2020  ellipse(.       
-0001dd60: 206e 756d 5f70 6978 656c 735b 315d 2c20   num_pixels[1], 
-0001dd70: 6e75 6d5f 7069 7865 6c73 5b30 5d2c 2064  num_pixels[0], d
-0001dd80: 6973 7461 6e63 655b 315d 202b 2030 2e35  istance[1] + 0.5
-0001dd90: 2c20 6469 7374 616e 6365 5b30 5d20 2b20  , distance[0] + 
-0001dda0: 302e 350a 2020 2020 290a 2020 2020 6e65  0.5.    ).    ne
-0001ddb0: 6967 6862 6f72 686f 6f64 5b72 722c 2063  ighborhood[rr, c
-0001ddc0: 635d 203d 2031 0a0a 2020 2020 7265 7475  c] = 1..    retu
-0001ddd0: 726e 206d 6f72 7068 6f6c 6f67 792e 6269  rn morphology.bi
-0001dde0: 6e61 7279 5f64 696c 6174 696f 6e28 696d  nary_dilation(im
-0001ddf0: 6167 653d 7261 7374 6572 2c20 7365 6c65  age=raster, sele
-0001de00: 6d3d 6e65 6967 6862 6f72 686f 6f64 290a  m=neighborhood).
-0001de10: 0a0a 6465 6620 5f66 696c 6c5f 6365 6c6c  ..def _fill_cell
-0001de20: 5f72 6563 7461 6e67 6c65 280a 2020 2020  _rectangle(.    
-0001de30: 7369 7a65 3d28 3230 2c20 3230 292c 0a20  size=(20, 20),. 
-0001de40: 2020 206c 6179 6572 733d 2830 2c20 312c     layers=(0, 1,
-0001de50: 2033 292c 0a20 2020 2064 656e 7369 7469   3),.    densiti
-0001de60: 6573 3d28 302e 352c 2030 2e32 352c 2030  es=(0.5, 0.25, 0
-0001de70: 2e37 292c 0a20 2020 2069 6e76 6572 7465  .7),.    inverte
-0001de80: 643d 2846 616c 7365 2c20 4661 6c73 652c  d=(False, False,
-0001de90: 2046 616c 7365 292c 0a29 3a0a 2020 2020   False),.):.    
-0001dea0: 2222 2243 7265 6174 6573 2061 2073 696e  """Creates a sin
-0001deb0: 676c 6520 4465 7669 6365 206f 6e20 6d75  gle Device on mu
-0001dec0: 6c74 6970 6c65 206c 6179 6572 7320 746f  ltiple layers to
-0001ded0: 2062 6520 7573 6564 2061 7320 6669 6c6c   be used as fill
-0001dee0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0001def0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001df00: 2020 2020 7369 7a65 203a 2061 7272 6179      size : array
-0001df10: 2d6c 696b 6520 6f66 2069 6e74 206f 7220  -like of int or 
-0001df20: 666c 6f61 740a 2020 2020 2020 2020 782c  float.        x,
-0001df30: 2079 2064 696d 656e 7369 6f6e 7320 6f66   y dimensions of
-0001df40: 2074 6865 2066 696c 6c20 6172 6561 2066   the fill area f
-0001df50: 6f72 2061 6c6c 206c 6179 6572 732e 0a20  or all layers.. 
-0001df60: 2020 206c 6179 6572 7320 3a20 696e 742c     layers : int,
-0001df70: 2061 7272 6179 2d6c 696b 655b 325d 2c20   array-like[2], 
-0001df80: 6f72 2073 6574 0a20 2020 2020 2020 2053  or set.        S
-0001df90: 7065 6369 6669 6320 6c61 7965 7228 7329  pecific layer(s)
-0001dfa0: 2074 6f20 7075 7420 6669 6c6c 2063 656c   to put fill cel
-0001dfb0: 6c20 7265 6374 616e 676c 6520 6765 6f6d  l rectangle geom
-0001dfc0: 6574 7279 206f 6e2e 0a20 2020 2064 656e  etry on..    den
-0001dfd0: 7369 7469 6573 203a 2061 7272 6179 2d6c  sities : array-l
-0001dfe0: 696b 6520 6f66 2069 6e74 206f 7220 666c  ike of int or fl
-0001dff0: 6f61 740a 2020 2020 2020 2020 4669 6c6c  oat.        Fill
-0001e000: 2064 656e 7369 7469 6573 2066 6f72 2065   densities for e
-0001e010: 6163 6820 6c61 7965 7220 7370 6563 6966  ach layer specif
-0001e020: 6965 6420 696e 2060 606c 6179 6572 7360  ied in ``layers`
-0001e030: 602e 204d 7573 7420 6265 2074 6865 2073  `. Must be the s
-0001e040: 616d 650a 2020 2020 2020 2020 7369 7a65  ame.        size
-0001e050: 2061 7320 6060 6c61 7965 7273 6060 2e0a   as ``layers``..
-0001e060: 2020 2020 696e 7665 7274 6564 203a 2061      inverted : a
-0001e070: 7272 6179 2d6c 696b 6520 6f72 2062 6f6f  rray-like or boo
-0001e080: 6c0a 2020 2020 2020 2020 4966 2074 7275  l.        If tru
-0001e090: 652c 2069 6e76 6572 7473 2074 6865 2066  e, inverts the f
-0001e0a0: 696c 6c20 6172 6561 2066 6f72 2063 6f72  ill area for cor
-0001e0b0: 7265 7370 6f6e 6469 6e67 206c 6179 6572  responding layer
-0001e0c0: 2e20 4d75 7374 2062 6520 7468 650a 2020  . Must be the.  
-0001e0d0: 2020 2020 2020 7361 6d65 2073 697a 6520        same size 
-0001e0e0: 6173 2060 606c 6179 6572 7360 602e 0a0a  as ``layers``...
-0001e0f0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001e100: 2d2d 2d2d 2d2d 2d0a 2020 2020 4420 3a20  -------.    D : 
-0001e110: 4465 7669 6365 0a20 2020 2020 2020 2041  Device.        A
-0001e120: 2044 6576 6963 6520 636f 6e74 6169 6e69   Device containi
-0001e130: 6e67 2066 696c 6c65 6420 6365 6c6c 2072  ng filled cell r
-0001e140: 6563 7461 6e67 6c65 732e 0a20 2020 2022  ectangles..    "
-0001e150: 2222 0a20 2020 2044 203d 2044 6576 6963  "".    D = Devic
-0001e160: 6528 2266 696c 6c63 656c 6c22 290a 2020  e("fillcell").  
-0001e170: 2020 666f 7220 6c61 7965 722c 2064 656e    for layer, den
-0001e180: 7369 7479 2c20 696e 7620 696e 207a 6970  sity, inv in zip
-0001e190: 286c 6179 6572 732c 2064 656e 7369 7469  (layers, densiti
-0001e1a0: 6573 2c20 696e 7665 7274 6564 293a 0a20  es, inverted):. 
-0001e1b0: 2020 2020 2020 2072 6563 7461 6e67 6c65         rectangle
-0001e1c0: 5f73 697a 6520 3d20 6e70 2e61 7272 6179  _size = np.array
-0001e1d0: 2873 697a 6529 202a 2073 7172 7428 6465  (size) * sqrt(de
-0001e1e0: 6e73 6974 7929 0a20 2020 2020 2020 2023  nsity).        #
-0001e1f0: 2072 203d 2044 2e61 6464 5f72 6566 2872   r = D.add_ref(r
-0001e200: 6563 7461 6e67 6c65 2873 697a 6520 3d20  ectangle(size = 
-0001e210: 7265 6374 616e 676c 655f 7369 7a65 2c20  rectangle_size, 
-0001e220: 6c61 7965 7220 3d20 6c61 7965 7229 290a  layer = layer)).
-0001e230: 2020 2020 2020 2020 5220 3d20 7265 6374          R = rect
-0001e240: 616e 676c 6528 7369 7a65 3d72 6563 7461  angle(size=recta
-0001e250: 6e67 6c65 5f73 697a 652c 206c 6179 6572  ngle_size, layer
-0001e260: 3d6c 6179 6572 290a 2020 2020 2020 2020  =layer).        
-0001e270: 522e 6365 6e74 6572 203d 2028 302c 2030  R.center = (0, 0
-0001e280: 290a 2020 2020 2020 2020 6966 2069 6e76  ).        if inv
-0001e290: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
-0001e2a0: 2020 2020 2020 4120 3d20 7265 6374 616e        A = rectan
-0001e2b0: 676c 6528 7369 7a65 3d73 697a 6529 0a20  gle(size=size). 
-0001e2c0: 2020 2020 2020 2020 2020 2041 2e63 656e             A.cen
-0001e2d0: 7465 7220 3d20 2830 2c20 3029 0a20 2020  ter = (0, 0).   
-0001e2e0: 2020 2020 2020 2020 2041 203d 2041 2e67           A = A.g
-0001e2f0: 6574 5f70 6f6c 7967 6f6e 7328 290a 2020  et_polygons().  
-0001e300: 2020 2020 2020 2020 2020 4220 3d20 522e            B = R.
-0001e310: 6765 745f 706f 6c79 676f 6e73 2829 0a20  get_polygons(). 
-0001e320: 2020 2020 2020 2020 2020 2070 203d 2067             p = g
-0001e330: 6473 7079 2e62 6f6f 6c65 616e 2841 2c20  dspy.boolean(A, 
-0001e340: 422c 206f 7065 7261 7469 6f6e 3d22 6e6f  B, operation="no
-0001e350: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-0001e360: 442e 6164 645f 706f 6c79 676f 6e28 702c  D.add_polygon(p,
-0001e370: 206c 6179 6572 3d6c 6179 6572 290a 2020   layer=layer).  
-0001e380: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001e390: 2020 2020 2020 2020 442e 6164 645f 7265          D.add_re
-0001e3a0: 6628 5229 0a20 2020 2072 6574 7572 6e20  f(R).    return 
-0001e3b0: 440a 0a0a 6465 6620 5f6c 6f6f 705f 6f76  D...def _loop_ov
-0001e3c0: 6572 2876 6172 293a 0a20 2020 2022 2222  er(var):.    """
-0001e3d0: 4368 6563 6b73 2069 6620 6120 7661 7269  Checks if a vari
-0001e3e0: 6162 6c65 2069 7320 696e 2074 6865 2066  able is in the f
-0001e3f0: 6f72 6d20 6f66 2061 6e20 6974 6572 6162  orm of an iterab
-0001e400: 6c65 2028 6c69 7374 2f74 7570 6c65 290a  le (list/tuple).
-0001e410: 2020 2020 616e 6420 6966 206e 6f74 2c20      and if not, 
-0001e420: 7265 7475 726e 7320 6974 2061 7320 6120  returns it as a 
-0001e430: 6c69 7374 2e20 2055 7365 6675 6c20 666f  list.  Useful fo
-0001e440: 7220 616c 6c6f 7769 6e67 2061 7267 756d  r allowing argum
-0001e450: 656e 740a 2020 2020 696e 7075 7473 2074  ent.    inputs t
-0001e460: 6f20 6265 2065 6974 6865 7220 6c69 7374  o be either list
-0001e470: 7320 2865 2e67 2e20 5b31 2c20 332c 2034  s (e.g. [1, 3, 4
-0001e480: 5d29 206f 7220 7369 6e67 6c65 2d76 616c  ]) or single-val
-0001e490: 7565 6420 2865 2e67 2e20 3329 2e0a 0a20  ued (e.g. 3)... 
-0001e4a0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001e4b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001e4c0: 2076 6172 203a 2069 6e74 206f 7220 666c   var : int or fl
-0001e4d0: 6f61 7420 6f72 206c 6973 740a 2020 2020  oat or list.    
-0001e4e0: 2020 2020 5661 7269 6162 6c65 2074 6f20      Variable to 
-0001e4f0: 6368 6563 6b20 666f 7220 6974 6572 6162  check for iterab
-0001e500: 696c 6974 792e 0a0a 2020 2020 5265 7475  ility...    Retu
-0001e510: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001e520: 2020 2020 7661 7220 3a20 6c69 7374 0a20      var : list. 
-0001e530: 2020 2020 2020 2056 6172 6961 626c 6520         Variable 
-0001e540: 636f 6e76 6572 7465 6420 746f 206c 6973  converted to lis
-0001e550: 7420 6966 2073 696e 676c 652d 7661 6c75  t if single-valu
-0001e560: 6564 2069 6e70 7574 2e0a 2020 2020 2222  ed input..    ""
-0001e570: 220a 0a20 2020 2069 6620 6861 7361 7474  "..    if hasatt
-0001e580: 7228 7661 722c 2022 5f5f 6974 6572 5f5f  r(var, "__iter__
-0001e590: 2229 3a0a 2020 2020 2020 2020 7265 7475  "):.        retu
-0001e5a0: 726e 2076 6172 0a20 2020 2065 6c73 653a  rn var.    else:
-0001e5b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001e5c0: 5b76 6172 5d0a 0a0a 6465 6620 6669 6c6c  [var]...def fill
-0001e5d0: 5f72 6563 7461 6e67 6c65 280a 2020 2020  _rectangle(.    
-0001e5e0: 442c 0a20 2020 2066 696c 6c5f 7369 7a65  D,.    fill_size
-0001e5f0: 3d28 3430 2c20 3130 292c 0a20 2020 2061  =(40, 10),.    a
-0001e600: 766f 6964 5f6c 6179 6572 733d 2261 6c6c  void_layers="all
-0001e610: 222c 0a20 2020 2069 6e63 6c75 6465 5f6c  ",.    include_l
-0001e620: 6179 6572 733d 4e6f 6e65 2c0a 2020 2020  ayers=None,.    
-0001e630: 6d61 7267 696e 3d31 3030 2c0a 2020 2020  margin=100,.    
-0001e640: 6669 6c6c 5f6c 6179 6572 733d 2830 2c20  fill_layers=(0, 
-0001e650: 312c 2033 292c 0a20 2020 2066 696c 6c5f  1, 3),.    fill_
-0001e660: 6465 6e73 6974 6965 733d 2830 2e35 2c20  densities=(0.5, 
-0001e670: 302e 3235 2c20 302e 3729 2c0a 2020 2020  0.25, 0.7),.    
-0001e680: 6669 6c6c 5f69 6e76 6572 7465 643d 4e6f  fill_inverted=No
-0001e690: 6e65 2c0a 2020 2020 6262 6f78 3d4e 6f6e  ne,.    bbox=Non
-0001e6a0: 652c 0a29 3a0a 2020 2020 2222 2243 7265  e,.):.    """Cre
-0001e6b0: 6174 6573 2061 2072 6563 7461 6e67 756c  ates a rectangul
-0001e6c0: 6172 2066 696c 6c20 7061 7474 6572 6e20  ar fill pattern 
-0001e6d0: 616e 6420 6669 6c6c 7320 616c 6c20 656d  and fills all em
-0001e6e0: 7074 7920 6172 6561 730a 2020 2020 696e  pty areas.    in
-0001e6f0: 2074 6865 2069 6e70 7574 2064 6576 6963   the input devic
-0001e700: 6520 440a 0a20 2020 2050 6172 616d 6574  e D..    Paramet
-0001e710: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0001e720: 2d2d 0a20 2020 2044 203a 2044 6576 6963  --.    D : Devic
-0001e730: 650a 2020 2020 2020 2020 4465 7669 6365  e.        Device
-0001e740: 2074 6f20 6265 2066 696c 6c65 640a 2020   to be filled.  
-0001e750: 2020 6669 6c6c 5f73 697a 6520 3a20 6172    fill_size : ar
-0001e760: 7261 792d 6c69 6b65 5b32 5d0a 2020 2020  ray-like[2].    
-0001e770: 2020 2020 5265 6374 616e 6775 6c61 7220      Rectangular 
-0001e780: 7369 7a65 206f 6620 7468 6520 6669 6c6c  size of the fill
-0001e790: 2065 6c65 6d65 6e74 0a20 2020 2061 766f   element.    avo
-0001e7a0: 6964 5f6c 6179 6572 7320 3a20 2761 6c6c  id_layers : 'all
-0001e7b0: 2720 6f72 206c 6973 7420 6f66 206c 6179  ' or list of lay
-0001e7c0: 6572 730a 2020 2020 2020 2020 4c61 7965  ers.        Laye
-0001e7d0: 7273 2074 6f20 6265 2061 766f 6964 6564  rs to be avoided
-0001e7e0: 2028 6e6f 7420 6669 6c6c 6564 2920 696e   (not filled) in
-0001e7f0: 2044 0a20 2020 2069 6e63 6c75 6465 5f6c   D.    include_l
-0001e800: 6179 6572 7320 3a0a 2020 2020 2020 2020  ayers :.        
-0001e810: 4c61 7965 7273 2074 6f20 6265 2069 6e63  Layers to be inc
-0001e820: 6c75 6465 6420 2866 696c 6c65 6429 2069  luded (filled) i
-0001e830: 6e20 442c 2073 7570 6572 6365 6465 7320  n D, supercedes 
-0001e840: 6176 6f69 645f 6c61 7965 7273 0a20 2020  avoid_layers.   
-0001e850: 206d 6172 6769 6e20 3a20 696e 7420 6f72   margin : int or
-0001e860: 2066 6c6f 6174 0a20 2020 2020 2020 204d   float.        M
-0001e870: 6172 6769 6e20 7370 6163 696e 6720 6172  argin spacing ar
-0001e880: 6f75 6e64 2061 766f 6964 6564 2061 7265  ound avoided are
-0001e890: 6173 202d 2d20 6669 6c6c 2077 696c 6c20  as -- fill will 
-0001e8a0: 6e6f 7420 636f 6d65 2077 6974 6869 6e0a  not come within.
-0001e8b0: 2020 2020 2020 2020 606d 6172 6769 6e60          `margin`
-0001e8c0: 206f 6620 7468 6520 6765 6f6d 6574 7279   of the geometry
-0001e8d0: 2069 6e20 440a 2020 2020 6669 6c6c 5f6c   in D.    fill_l
-0001e8e0: 6179 6572 7320 3a20 6c69 7374 206f 6620  ayers : list of 
-0001e8f0: 6c61 7965 7273 0a20 2020 2020 2020 2044  layers.        D
-0001e900: 6566 696e 6573 2074 6865 2066 696c 6c20  efines the fill 
-0001e910: 7061 7474 6572 6e20 6c61 7965 7273 0a20  pattern layers. 
-0001e920: 2020 2066 696c 6c5f 6465 6e73 6974 6965     fill_densitie
-0001e930: 7320 3a20 666c 6f61 7420 6265 7477 6565  s : float betwee
-0001e940: 6e20 3020 616e 6420 310a 2020 2020 2020  n 0 and 1.      
-0001e950: 2020 4465 6669 6e65 7320 7468 6520 6669    Defines the fi
-0001e960: 6c6c 2070 6174 7465 726e 2064 656e 7369  ll pattern densi
-0001e970: 7479 2028 312e 3020 3d3d 2066 756c 6c79  ty (1.0 == fully
-0001e980: 2066 696c 6c65 6429 0a20 2020 2066 696c   filled).    fil
-0001e990: 6c5f 696e 7665 7274 6564 203a 2062 6f6f  l_inverted : boo
-0001e9a0: 6c0a 2020 2020 2020 2020 496e 7665 7274  l.        Invert
-0001e9b0: 7320 7468 6520 6669 6c6c 2070 6174 7465  s the fill patte
-0001e9c0: 726e 0a20 2020 2062 626f 7820 3a20 6172  rn.    bbox : ar
-0001e9d0: 7261 792d 6c69 6b65 5b32 5d5b 325d 0a20  ray-like[2][2]. 
-0001e9e0: 2020 2020 2020 204c 696d 6974 2074 6865         Limit the
-0001e9f0: 2066 696c 6c20 7061 7474 6572 6e20 746f   fill pattern to
-0001ea00: 2074 6865 2061 7265 6120 6465 6669 6e65   the area define
-0001ea10: 6420 6279 2074 6869 7320 626f 756e 6469  d by this boundi
-0001ea20: 6e67 2062 6f78 0a0a 2020 2020 5265 7475  ng box..    Retu
-0001ea30: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001ea40: 2020 2020 4620 3a20 4465 7669 6365 0a0a      F : Device..
-0001ea50: 2020 2020 2222 220a 2020 2020 2320 4372      """.    # Cr
-0001ea60: 6561 7465 2074 6865 2066 696c 6c20 6365  eate the fill ce
-0001ea70: 6c6c 2e0a 2020 2020 2320 4966 2066 696c  ll..    # If fil
-0001ea80: 6c5f 696e 7665 7274 6564 2069 7320 6e6f  l_inverted is no
-0001ea90: 7420 7370 6563 6966 6965 642c 2061 7373  t specified, ass
-0001eaa0: 756d 6520 616c 6c20 4661 6c73 650a 2020  ume all False.  
-0001eab0: 2020 6669 6c6c 5f6c 6179 6572 7320 3d20    fill_layers = 
-0001eac0: 5f6c 6f6f 705f 6f76 6572 2866 696c 6c5f  _loop_over(fill_
-0001ead0: 6c61 7965 7273 290a 2020 2020 6669 6c6c  layers).    fill
-0001eae0: 5f64 656e 7369 7469 6573 203d 205f 6c6f  _densities = _lo
-0001eaf0: 6f70 5f6f 7665 7228 6669 6c6c 5f64 656e  op_over(fill_den
-0001eb00: 7369 7469 6573 290a 2020 2020 6966 2066  sities).    if f
-0001eb10: 696c 6c5f 696e 7665 7274 6564 2069 7320  ill_inverted is 
-0001eb20: 4e6f 6e65 3a0a 2020 2020 2020 2020 6669  None:.        fi
-0001eb30: 6c6c 5f69 6e76 6572 7465 6420 3d20 5b46  ll_inverted = [F
-0001eb40: 616c 7365 5d20 2a20 6c65 6e28 6669 6c6c  alse] * len(fill
-0001eb50: 5f6c 6179 6572 7329 0a20 2020 2066 696c  _layers).    fil
-0001eb60: 6c5f 696e 7665 7274 6564 203d 205f 6c6f  l_inverted = _lo
-0001eb70: 6f70 5f6f 7665 7228 6669 6c6c 5f69 6e76  op_over(fill_inv
-0001eb80: 6572 7465 6429 0a20 2020 2069 6620 6c65  erted).    if le
-0001eb90: 6e28 6669 6c6c 5f6c 6179 6572 7329 2021  n(fill_layers) !
-0001eba0: 3d20 6c65 6e28 6669 6c6c 5f64 656e 7369  = len(fill_densi
-0001ebb0: 7469 6573 293a 0a20 2020 2020 2020 2072  ties):.        r
-0001ebc0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0001ebd0: 0a20 2020 2020 2020 2020 2020 2022 5b50  .            "[P
-0001ebe0: 4849 444c 5d20 7068 6964 6c2e 6765 6f6d  HIDL] phidl.geom
-0001ebf0: 6574 7279 2e66 696c 6c5f 7265 6374 616e  etry.fill_rectan
-0001ec00: 676c 6528 2920 220a 2020 2020 2020 2020  gle() ".        
-0001ec10: 2020 2020 2260 6669 6c6c 5f6c 6179 6572      "`fill_layer
-0001ec20: 7360 2061 6e64 2060 6669 6c6c 5f64 656e  s` and `fill_den
-0001ec30: 7369 7469 6573 6020 7061 7261 6d65 7465  sities` paramete
-0001ec40: 7273 2022 0a20 2020 2020 2020 2020 2020  rs ".           
-0001ec50: 2022 6d75 7374 2062 6520 6c69 7374 7320   "must be lists 
-0001ec60: 6f66 2074 6865 2073 616d 6520 6c65 6e67  of the same leng
-0001ec70: 7468 220a 2020 2020 2020 2020 290a 2020  th".        ).  
-0001ec80: 2020 6966 206c 656e 2866 696c 6c5f 6c61    if len(fill_la
-0001ec90: 7965 7273 2920 213d 206c 656e 2866 696c  yers) != len(fil
-0001eca0: 6c5f 696e 7665 7274 6564 293a 0a20 2020  l_inverted):.   
-0001ecb0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001ecc0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0001ecd0: 2020 2022 5b50 4849 444c 5d20 7068 6964     "[PHIDL] phid
-0001ece0: 6c2e 6765 6f6d 6574 7279 2e66 696c 6c5f  l.geometry.fill_
-0001ecf0: 7265 6374 616e 676c 6528 2920 220a 2020  rectangle() ".  
-0001ed00: 2020 2020 2020 2020 2020 2260 6669 6c6c            "`fill
-0001ed10: 5f6c 6179 6572 7360 2061 6e64 2060 6669  _layers` and `fi
-0001ed20: 6c6c 5f69 6e76 6572 7465 6460 2070 6172  ll_inverted` par
-0001ed30: 616d 6574 6572 7320 6d75 7374 2022 0a20  ameters must ". 
-0001ed40: 2020 2020 2020 2020 2020 2022 6265 206c             "be l
-0001ed50: 6973 7473 206f 6620 7468 6520 7361 6d65  ists of the same
-0001ed60: 206c 656e 6774 6822 0a20 2020 2020 2020   length".       
-0001ed70: 2029 0a0a 2020 2020 6669 6c6c 5f63 656c   )..    fill_cel
-0001ed80: 6c20 3d20 5f66 696c 6c5f 6365 6c6c 5f72  l = _fill_cell_r
-0001ed90: 6563 7461 6e67 6c65 280a 2020 2020 2020  ectangle(.      
-0001eda0: 2020 7369 7a65 3d66 696c 6c5f 7369 7a65    size=fill_size
-0001edb0: 2c0a 2020 2020 2020 2020 6c61 7965 7273  ,.        layers
-0001edc0: 3d66 696c 6c5f 6c61 7965 7273 2c0a 2020  =fill_layers,.  
-0001edd0: 2020 2020 2020 6465 6e73 6974 6965 733d        densities=
-0001ede0: 6669 6c6c 5f64 656e 7369 7469 6573 2c0a  fill_densities,.
-0001edf0: 2020 2020 2020 2020 696e 7665 7274 6564          inverted
-0001ee00: 3d66 696c 6c5f 696e 7665 7274 6564 2c0a  =fill_inverted,.
-0001ee10: 2020 2020 290a 2020 2020 4620 3d20 4465      ).    F = De
-0001ee20: 7669 6365 286e 616d 653d 2266 696c 6c5f  vice(name="fill_
-0001ee30: 7061 7474 6572 6e22 290a 0a20 2020 2069  pattern")..    i
-0001ee40: 6620 6176 6f69 645f 6c61 7965 7273 203d  f avoid_layers =
-0001ee50: 3d20 2261 6c6c 223a 0a20 2020 2020 2020  = "all":.       
-0001ee60: 2065 7863 6c75 6465 5f70 6f6c 7973 203d   exclude_polys =
-0001ee70: 2044 2e67 6574 5f70 6f6c 7967 6f6e 7328   D.get_polygons(
-0001ee80: 6279 5f73 7065 633d 4661 6c73 652c 2064  by_spec=False, d
-0001ee90: 6570 7468 3d4e 6f6e 6529 0a20 2020 2065  epth=None).    e
-0001eea0: 6c73 653a 0a20 2020 2020 2020 2061 766f  lse:.        avo
-0001eeb0: 6964 5f6c 6179 6572 7320 3d20 5b5f 7061  id_layers = [_pa
-0001eec0: 7273 655f 6c61 7965 7228 6c29 2066 6f72  rse_layer(l) for
-0001eed0: 206c 2069 6e20 5f6c 6f6f 705f 6f76 6572   l in _loop_over
-0001eee0: 2861 766f 6964 5f6c 6179 6572 7329 5d0a  (avoid_layers)].
-0001eef0: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
-0001ef00: 706f 6c79 7320 3d20 442e 6765 745f 706f  polys = D.get_po
-0001ef10: 6c79 676f 6e73 2862 795f 7370 6563 3d54  lygons(by_spec=T
-0001ef20: 7275 652c 2064 6570 7468 3d4e 6f6e 6529  rue, depth=None)
-0001ef30: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-0001ef40: 5f70 6f6c 7973 203d 207b 0a20 2020 2020  _polys = {.     
-0001ef50: 2020 2020 2020 206b 6579 3a20 6578 636c         key: excl
-0001ef60: 7564 655f 706f 6c79 735b 6b65 795d 2066  ude_polys[key] f
-0001ef70: 6f72 206b 6579 2069 6e20 6578 636c 7564  or key in exclud
-0001ef80: 655f 706f 6c79 7320 6966 206b 6579 2069  e_polys if key i
-0001ef90: 6e20 6176 6f69 645f 6c61 7965 7273 0a20  n avoid_layers. 
-0001efa0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0001efb0: 2065 7863 6c75 6465 5f70 6f6c 7973 203d   exclude_polys =
-0001efc0: 2069 7465 7274 6f6f 6c73 2e63 6861 696e   itertools.chain
-0001efd0: 2e66 726f 6d5f 6974 6572 6162 6c65 2865  .from_iterable(e
-0001efe0: 7863 6c75 6465 5f70 6f6c 7973 2e76 616c  xclude_polys.val
-0001eff0: 7565 7328 2929 0a0a 2020 2020 6966 2069  ues())..    if i
-0001f000: 6e63 6c75 6465 5f6c 6179 6572 7320 6973  nclude_layers is
-0001f010: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-0001f020: 6e63 6c75 6465 5f70 6f6c 7973 203d 205b  nclude_polys = [
-0001f030: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-0001f040: 2020 2020 696e 636c 7564 655f 6c61 7965      include_laye
-0001f050: 7273 203d 205b 5f70 6172 7365 5f6c 6179  rs = [_parse_lay
-0001f060: 6572 286c 2920 666f 7220 6c20 696e 205f  er(l) for l in _
-0001f070: 6c6f 6f70 5f6f 7665 7228 696e 636c 7564  loop_over(includ
-0001f080: 655f 6c61 7965 7273 295d 0a20 2020 2020  e_layers)].     
-0001f090: 2020 2069 6e63 6c75 6465 5f70 6f6c 7973     include_polys
-0001f0a0: 203d 2044 2e67 6574 5f70 6f6c 7967 6f6e   = D.get_polygon
-0001f0b0: 7328 6279 5f73 7065 633d 5472 7565 2c20  s(by_spec=True, 
-0001f0c0: 6465 7074 683d 4e6f 6e65 290a 2020 2020  depth=None).    
-0001f0d0: 2020 2020 696e 636c 7564 655f 706f 6c79      include_poly
-0001f0e0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-0001f0f0: 2020 6b65 793a 2069 6e63 6c75 6465 5f70    key: include_p
-0001f100: 6f6c 7973 5b6b 6579 5d20 666f 7220 6b65  olys[key] for ke
-0001f110: 7920 696e 2069 6e63 6c75 6465 5f70 6f6c  y in include_pol
-0001f120: 7973 2069 6620 6b65 7920 696e 2069 6e63  ys if key in inc
-0001f130: 6c75 6465 5f6c 6179 6572 730a 2020 2020  lude_layers.    
-0001f140: 2020 2020 7d0a 2020 2020 2020 2020 696e      }.        in
-0001f150: 636c 7564 655f 706f 6c79 7320 3d20 6974  clude_polys = it
-0001f160: 6572 746f 6f6c 732e 6368 6169 6e2e 6672  ertools.chain.fr
-0001f170: 6f6d 5f69 7465 7261 626c 6528 696e 636c  om_iterable(incl
-0001f180: 7564 655f 706f 6c79 732e 7661 6c75 6573  ude_polys.values
-0001f190: 2829 290a 0a20 2020 2069 6620 6262 6f78  ())..    if bbox
-0001f1a0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001f1b0: 2020 6262 6f78 203d 2044 2e62 626f 780a    bbox = D.bbox.
-0001f1c0: 0a20 2020 2072 6173 7465 7220 3d20 5f72  .    raster = _r
-0001f1d0: 6173 7465 7269 7a65 5f70 6f6c 7967 6f6e  asterize_polygon
-0001f1e0: 7328 0a20 2020 2020 2020 2070 6f6c 7967  s(.        polyg
-0001f1f0: 6f6e 733d 6578 636c 7564 655f 706f 6c79  ons=exclude_poly
-0001f200: 732c 2062 6f75 6e64 733d 6262 6f78 2c20  s, bounds=bbox, 
-0001f210: 6478 3d66 696c 6c5f 7369 7a65 5b30 5d2c  dx=fill_size[0],
-0001f220: 2064 793d 6669 6c6c 5f73 697a 655b 315d   dy=fill_size[1]
-0001f230: 0a20 2020 2029 0a20 2020 2072 6173 7465  .    ).    raste
-0001f240: 7220 3d20 7261 7374 6572 2026 207e 5f72  r = raster & ~_r
-0001f250: 6173 7465 7269 7a65 5f70 6f6c 7967 6f6e  asterize_polygon
-0001f260: 7328 0a20 2020 2020 2020 2070 6f6c 7967  s(.        polyg
-0001f270: 6f6e 733d 696e 636c 7564 655f 706f 6c79  ons=include_poly
-0001f280: 732c 2062 6f75 6e64 733d 6262 6f78 2c20  s, bounds=bbox, 
-0001f290: 6478 3d66 696c 6c5f 7369 7a65 5b30 5d2c  dx=fill_size[0],
-0001f2a0: 2064 793d 6669 6c6c 5f73 697a 655b 315d   dy=fill_size[1]
-0001f2b0: 0a20 2020 2029 0a20 2020 2072 6173 7465  .    ).    raste
-0001f2c0: 7220 3d20 5f65 7870 616e 645f 7261 7374  r = _expand_rast
-0001f2d0: 6572 2872 6173 7465 722c 2064 6973 7461  er(raster, dista
-0001f2e0: 6e63 653d 6d61 7267 696e 202f 206e 702e  nce=margin / np.
-0001f2f0: 6172 7261 7928 6669 6c6c 5f73 697a 6529  array(fill_size)
-0001f300: 290a 0a20 2020 2066 6f72 2069 2069 6e20  )..    for i in 
-0001f310: 7261 6e67 6528 6e70 2e73 697a 6528 7261  range(np.size(ra
-0001f320: 7374 6572 2c20 3029 293a 0a20 2020 2020  ster, 0)):.     
-0001f330: 2020 2073 7562 5f72 6173 7465 7273 203d     sub_rasters =
-0001f340: 205b 6c69 7374 2867 2920 666f 7220 6b2c   [list(g) for k,
-0001f350: 2067 2069 6e20 6974 6572 746f 6f6c 732e   g in itertools.
-0001f360: 6772 6f75 7062 7928 7261 7374 6572 5b69  groupby(raster[i
-0001f370: 5d29 5d0a 2020 2020 2020 2020 6a20 3d20  ])].        j = 
-0001f380: 300a 2020 2020 2020 2020 666f 7220 7320  0.        for s 
-0001f390: 696e 2073 7562 5f72 6173 7465 7273 3a0a  in sub_rasters:.
-0001f3a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001f3b0: 5b30 5d20 3d3d 2030 3a0a 2020 2020 2020  [0] == 0:.      
-0001f3c0: 2020 2020 2020 2020 2020 782c 2079 203d            x, y =
-0001f3d0: 205f 7261 7374 6572 5f69 6e64 6578 5f74   _raster_index_t
-0001f3e0: 6f5f 636f 6f72 6473 2869 2c20 6a2c 2062  o_coords(i, j, b
-0001f3f0: 626f 782c 2066 696c 6c5f 7369 7a65 5b30  box, fill_size[0
-0001f400: 5d2c 2066 696c 6c5f 7369 7a65 5b31 5d29  ], fill_size[1])
-0001f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f420: 2023 2046 2e61 6464 2867 6473 7079 2e43   # F.add(gdspy.C
-0001f430: 656c 6c41 7272 6179 2872 6566 5f63 656c  ellArray(ref_cel
-0001f440: 6c20 3d20 6669 6c6c 5f63 656c 6c2c 0a20  l = fill_cell,. 
-0001f450: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f470: 2020 2020 2020 2063 6f6c 756d 6e73 203d         columns =
-0001f480: 206c 656e 2873 292c 2072 6f77 7320 3d20   len(s), rows = 
-0001f490: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0001f4a0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001f4b0: 2020 2020 2020 2020 2020 2073 7061 6369             spaci
-0001f4c0: 6e67 203d 2066 696c 6c5f 7369 7a65 2c20  ng = fill_size, 
-0001f4d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001f4e0: 2020 2061 203d 2046 2e61 6464 5f61 7272     a = F.add_arr
-0001f4f0: 6179 2866 696c 6c5f 6365 6c6c 2c20 636f  ay(fill_cell, co
-0001f500: 6c75 6d6e 733d 6c65 6e28 7329 2c20 726f  lumns=len(s), ro
-0001f510: 7773 3d31 2c20 7370 6163 696e 673d 6669  ws=1, spacing=fi
-0001f520: 6c6c 5f73 697a 6529 0a20 2020 2020 2020  ll_size).       
-0001f530: 2020 2020 2020 2020 2061 2e6d 6f76 6528           a.move(
-0001f540: 2878 2c20 7929 290a 2020 2020 2020 2020  (x, y)).        
-0001f550: 2020 2020 6a20 2b3d 206c 656e 2873 290a      j += len(s).
-0001f560: 0a20 2020 2072 6574 7572 6e20 460a 0a0a  .    return F...
-0001f570: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
-0001f580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f5a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f5b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f5c0: 0a23 0a23 2050 686f 746f 6e69 6373 0a23  .#.# Photonics.#
-0001f5d0: 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .# =============
-0001f5e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f5f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000198e0: 6420 2861 7320 6966 206e 702e 7265 7368  d (as if np.resh
+000198f0: 6170 6528 2920 7765 7265 2072 756e 2077  ape() were run w
+00019900: 6974 6820 7368 6170 655b 3a3a 2d31 5d29  ith shape[::-1])
+00019910: 2e20 4966 206e 6f20 7368 6170 6520 6973  . If no shape is
+00019920: 2067 6976 656e 2061 6e64 2074 6865 0a20   given and the. 
+00019930: 2020 2020 2020 206c 6973 7420 6973 2031         list is 1
+00019940: 442c 2074 6865 206f 7574 7075 7420 6973  D, the output is
+00019950: 2061 7320 6966 206e 702e 7265 7368 6170   as if np.reshap
+00019960: 6520 7765 7265 2072 756e 2077 6974 6820  e were run with 
+00019970: 282d 312c 2073 697a 6520 6f66 206c 6973  (-1, size of lis
+00019980: 7429 2e0a 2020 2020 616c 6967 6e5f 7820  t)..    align_x 
+00019990: 3a20 7b27 7827 2c20 2778 6d69 6e27 2c20  : {'x', 'xmin', 
+000199a0: 2778 6d61 7827 7d0a 2020 2020 2020 2020  'xmax'}.        
+000199b0: 5768 6963 6820 6564 6765 2074 6f20 7065  Which edge to pe
+000199c0: 7266 6f72 6d20 7468 6520 7820 2863 6f6c  rform the x (col
+000199d0: 756d 6e29 2061 6c69 676e 6d65 6e74 2061  umn) alignment a
+000199e0: 6c6f 6e67 0a20 2020 2061 6c69 676e 5f79  long.    align_y
+000199f0: 203a 207b 2779 272c 2027 796d 696e 272c   : {'y', 'ymin',
+00019a00: 2027 796d 6178 277d 0a20 2020 2020 2020   'ymax'}.       
+00019a10: 2057 6869 6368 2065 6467 6520 746f 2070   Which edge to p
+00019a20: 6572 666f 726d 2074 6865 2079 2028 726f  erform the y (ro
+00019a30: 7729 2061 6c69 676e 6d65 6e74 2061 6c6f  w) alignment alo
+00019a40: 6e67 0a20 2020 2065 6467 655f 7820 3a20  ng.    edge_x : 
+00019a50: 7b27 7827 2c20 2778 6d69 6e27 2c20 2778  {'x', 'xmin', 'x
+00019a60: 6d61 7827 7d0a 2020 2020 2020 2020 5768  max'}.        Wh
+00019a70: 6963 6820 6564 6765 2074 6f20 7065 7266  ich edge to perf
+00019a80: 6f72 6d20 7468 6520 7820 2863 6f6c 756d  orm the x (colum
+00019a90: 6e29 2064 6973 7472 6962 7574 696f 6e20  n) distribution 
+00019aa0: 616c 6f6e 6720 2875 6e75 7365 6420 6966  along (unused if
+00019ab0: 0a20 2020 2020 2020 2073 6570 6172 6174  .        separat
+00019ac0: 696f 6e20 3d3d 2054 7275 6529 0a20 2020  ion == True).   
+00019ad0: 2065 6467 655f 7920 3a20 7b27 7927 2c20   edge_y : {'y', 
+00019ae0: 2779 6d69 6e27 2c20 2779 6d61 7827 7d0a  'ymin', 'ymax'}.
+00019af0: 2020 2020 2020 2020 5768 6963 6820 6564          Which ed
+00019b00: 6765 2074 6f20 7065 7266 6f72 6d20 7468  ge to perform th
+00019b10: 6520 7920 2872 6f77 2920 6469 7374 7269  e y (row) distri
+00019b20: 6275 7469 6f6e 2061 6c6f 6e67 2028 756e  bution along (un
+00019b30: 7573 6564 2069 660a 2020 2020 2020 2020  used if.        
+00019b40: 7365 7061 7261 7469 6f6e 203d 3d20 5472  separation == Tr
+00019b50: 7565 290a 0a20 2020 2052 6574 7572 6e73  ue)..    Returns
+00019b60: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00019b70: 2064 6576 6963 655f 6d61 7472 6978 203a   device_matrix :
+00019b80: 2044 6576 6963 650a 2020 2020 2020 2020   Device.        
+00019b90: 4120 4465 7669 6365 2063 6f6e 7461 696e  A Device contain
+00019ba0: 696e 6720 616c 6c20 7468 6520 4465 7669  ing all the Devi
+00019bb0: 6365 7320 696e 2060 6465 7669 6365 5f6c  ces in `device_l
+00019bc0: 6973 7460 2069 6e20 6120 6772 6964 2e0a  ist` in a grid..
+00019bd0: 2020 2020 2222 220a 0a20 2020 2064 6576      """..    dev
+00019be0: 6963 655f 6172 7261 7920 3d20 6e70 2e61  ice_array = np.a
+00019bf0: 7361 7272 6179 2864 6576 6963 655f 6c69  sarray(device_li
+00019c00: 7374 290a 2020 2020 7370 6163 696e 6720  st).    spacing 
+00019c10: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
+00019c20: 6f28 7370 6163 696e 672c 2032 290a 2020  o(spacing, 2).  
+00019c30: 2020 2320 4368 6563 6b20 6172 6775 6d65    # Check argume
+00019c40: 6e74 730a 2020 2020 6966 2064 6576 6963  nts.    if devic
+00019c50: 655f 6172 7261 792e 6e64 696d 206e 6f74  e_array.ndim not
+00019c60: 2069 6e20 2831 2c20 3229 3a0a 2020 2020   in (1, 2):.    
+00019c70: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00019c80: 7272 6f72 2822 5b50 4849 444c 5d20 6772  rror("[PHIDL] gr
+00019c90: 6964 2829 2054 6865 2064 6576 6963 655f  id() The device_
+00019ca0: 6c69 7374 206e 6565 6473 2074 6f20 6265  list needs to be
+00019cb0: 2031 4420 6f72 2032 442e 2229 0a20 2020   1D or 2D.").   
+00019cc0: 2069 6620 7368 6170 6520 6973 206e 6f74   if shape is not
+00019cd0: 204e 6f6e 6520 616e 6420 6c65 6e28 7368   None and len(sh
+00019ce0: 6170 6529 2021 3d20 323a 0a20 2020 2020  ape) != 2:.     
+00019cf0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00019d00: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00019d10: 2022 5b50 4849 444c 5d20 6772 6964 2829   "[PHIDL] grid()
+00019d20: 2073 6861 7065 2061 7267 756d 656e 7420   shape argument 
+00019d30: 6d75 7374 2062 6520 4e6f 6e65 206f 7222  must be None or"
+00019d40: 0a20 2020 2020 2020 2020 2020 202b 2022  .            + "
+00019d50: 2068 6176 6520 6120 6c65 6e67 7468 206f   have a length o
+00019d60: 6620 322c 2066 6f72 2065 7861 6d70 6c65  f 2, for example
+00019d70: 2073 6861 7065 3d28 342c 3629 220a 2020   shape=(4,6)".  
+00019d80: 2020 2020 2020 290a 0a20 2020 2023 2043        )..    # C
+00019d90: 6865 636b 2074 6861 7420 7368 6170 6520  heck that shape 
+00019da0: 6973 2076 616c 6964 2061 6e64 2072 6573  is valid and res
+00019db0: 6861 7065 2061 7272 6179 2069 6620 6e65  hape array if ne
+00019dc0: 6564 6564 0a20 2020 2069 6620 2873 6861  eded.    if (sha
+00019dd0: 7065 2069 7320 4e6f 6e65 2920 616e 6420  pe is None) and 
+00019de0: 2864 6576 6963 655f 6172 7261 792e 6e64  (device_array.nd
+00019df0: 696d 203d 3d20 3229 3a20 2023 2041 6c72  im == 2):  # Alr
+00019e00: 6561 6479 2069 6e20 6465 7369 7265 6420  eady in desired 
+00019e10: 7368 6170 650a 2020 2020 2020 2020 7368  shape.        sh
+00019e20: 6170 6520 3d20 6465 7669 6365 5f61 7272  ape = device_arr
+00019e30: 6179 2e73 6861 7065 0a20 2020 2065 6c69  ay.shape.    eli
+00019e40: 6620 2873 6861 7065 2069 7320 4e6f 6e65  f (shape is None
+00019e50: 2920 616e 6420 2864 6576 6963 655f 6172  ) and (device_ar
+00019e60: 7261 792e 6e64 696d 203d 3d20 3129 3a0a  ray.ndim == 1):.
+00019e70: 2020 2020 2020 2020 7368 6170 6520 3d20          shape = 
+00019e80: 282d 312c 2064 6576 6963 655f 6172 7261  (-1, device_arra
+00019e90: 792e 7369 7a65 290a 2020 2020 656c 6966  y.size).    elif
+00019ea0: 2030 203c 2073 6861 7065 5b30 5d20 2a20   0 < shape[0] * 
+00019eb0: 7368 6170 655b 315d 203c 2064 6576 6963  shape[1] < devic
+00019ec0: 655f 6172 7261 792e 7369 7a65 3a0a 2020  e_array.size:.  
+00019ed0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00019ee0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00019ef0: 2020 2020 225b 5048 4944 4c5d 2067 7269      "[PHIDL] gri
+00019f00: 6428 2920 5468 6520 7368 6170 6520 6973  d() The shape is
+00019f10: 2074 6f6f 2073 6d61 6c6c 2066 6f72 2061   too small for a
+00019f20: 6c6c 2074 6865 2069 7465 6d73 2069 6e20  ll the items in 
+00019f30: 6465 7669 6365 5f6c 6973 7422 0a20 2020  device_list".   
+00019f40: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+00019f50: 0a20 2020 2020 2020 2023 2043 6861 6e67  .        # Chang
+00019f60: 6520 2878 2c79 2920 7368 6170 6520 746f  e (x,y) shape to
+00019f70: 2028 792c 7829 2073 6861 7065 2074 6f20   (y,x) shape to 
+00019f80: 666f 6c6c 6f77 2064 6566 6175 6c74 2072  follow default r
+00019f90: 6f77 2c20 636f 6c75 6d6e 2066 6f72 6d61  ow, column forma
+00019fa0: 7420 696e 206e 702e 7265 7368 6170 650a  t in np.reshape.
+00019fb0: 2020 2020 2020 2020 7368 6170 6520 3d20          shape = 
+00019fc0: 7368 6170 655b 3a3a 2d31 5d0a 0a20 2020  shape[::-1]..   
+00019fd0: 2020 2020 2069 6620 6e70 2e6d 696e 2873       if np.min(s
+00019fe0: 6861 7065 2920 3d3d 202d 313a 0a20 2020  hape) == -1:.   
+00019ff0: 2020 2020 2020 2020 206d 6178 5f73 6861           max_sha
+0001a000: 7065 203d 206e 702e 6d61 7828 7368 6170  pe = np.max(shap
+0001a010: 6529 0a20 2020 2020 2020 2020 2020 206d  e).            m
+0001a020: 696e 5f64 6576 6963 6573 203d 2069 6e74  in_devices = int
+0001a030: 286e 702e 6365 696c 2864 6576 6963 655f  (np.ceil(device_
+0001a040: 6172 7261 792e 7369 7a65 202f 206d 6178  array.size / max
+0001a050: 5f73 6861 7065 2920 2a20 6d61 785f 7368  _shape) * max_sh
+0001a060: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
+0001a070: 2065 7874 7261 5f64 6576 6963 6573 203d   extra_devices =
+0001a080: 206d 696e 5f64 6576 6963 6573 202d 2064   min_devices - d
+0001a090: 6576 6963 655f 6172 7261 792e 7369 7a65  evice_array.size
+0001a0a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0001a0b0: 2020 2020 2020 2020 2020 2065 7874 7261             extra
+0001a0c0: 5f64 6576 6963 6573 203d 2073 6861 7065  _devices = shape
+0001a0d0: 5b30 5d20 2a20 7368 6170 655b 315d 202d  [0] * shape[1] -
+0001a0e0: 2064 6576 6963 655f 6172 7261 792e 7369   device_array.si
+0001a0f0: 7a65 0a20 2020 2020 2020 2069 6620 6578  ze.        if ex
+0001a100: 7472 615f 6465 7669 6365 7320 213d 2030  tra_devices != 0
+0001a110: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+0001a120: 7669 6365 5f61 7272 6179 203d 206e 702e  vice_array = np.
+0001a130: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+0001a140: 2020 2020 2020 2020 6465 7669 6365 5f61          device_a
+0001a150: 7272 6179 2c0a 2020 2020 2020 2020 2020  rray,.          
+0001a160: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+0001a170: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+0001a180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a190: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0001a1a0: 2020 2020 2a20 6578 7472 615f 6465 7669      * extra_devi
+0001a1b0: 6365 732c 0a20 2020 2020 2020 2020 2020  ces,.           
+0001a1c0: 2029 0a20 2020 2064 6576 6963 655f 6172   ).    device_ar
+0001a1d0: 7261 7920 3d20 6e70 2e72 6573 6861 7065  ray = np.reshape
+0001a1e0: 2864 6576 6963 655f 6172 7261 792c 2073  (device_array, s
+0001a1f0: 6861 7065 290a 0a20 2020 2023 2043 7265  hape)..    # Cre
+0001a200: 6174 6520 6120 626c 616e 6b20 4465 7669  ate a blank Devi
+0001a210: 6365 2061 6e64 2072 6566 6572 656e 6365  ce and reference
+0001a220: 2061 6c6c 2074 6865 2044 6576 6963 6573   all the Devices
+0001a230: 2069 6e20 6974 0a20 2020 2044 203d 2044   in it.    D = D
+0001a240: 6576 6963 6528 2267 7269 6422 290a 2020  evice("grid").  
+0001a250: 2020 7265 665f 6172 7261 7920 3d20 6e70    ref_array = np
+0001a260: 2e65 6d70 7479 2864 6576 6963 655f 6172  .empty(device_ar
+0001a270: 7261 792e 7368 6170 652c 2064 7479 7065  ray.shape, dtype
+0001a280: 3d6f 626a 6563 7429 0a20 2020 2064 756d  =object).    dum
+0001a290: 6d79 203d 2044 6576 6963 6528 290a 2020  my = Device().  
+0001a2a0: 2020 666f 7220 6964 782c 2064 2069 6e20    for idx, d in 
+0001a2b0: 6e70 2e6e 6465 6e75 6d65 7261 7465 2864  np.ndenumerate(d
+0001a2c0: 6576 6963 655f 6172 7261 7929 3a0a 2020  evice_array):.  
+0001a2d0: 2020 2020 2020 6966 2064 2069 7320 6e6f        if d is no
+0001a2e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001a2f0: 2020 2020 7265 665f 6172 7261 795b 6964      ref_array[id
+0001a300: 785d 203d 2044 203c 3c20 640a 2020 2020  x] = D << d.    
+0001a310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001a320: 2020 2020 2020 7265 665f 6172 7261 795b        ref_array[
+0001a330: 6964 785d 203d 2044 203c 3c20 6475 6d6d  idx] = D << dumm
+0001a340: 7920 2023 2043 7265 6174 6520 6475 6d6d  y  # Create dumm
+0001a350: 7920 6465 7669 6365 730a 0a20 2020 2072  y devices..    r
+0001a360: 6f77 7320 3d20 5b47 726f 7570 2872 6566  ows = [Group(ref
+0001a370: 5f61 7272 6179 5b6e 2c20 3a5d 2920 666f  _array[n, :]) fo
+0001a380: 7220 6e20 696e 2072 616e 6765 2872 6566  r n in range(ref
+0001a390: 5f61 7272 6179 2e73 6861 7065 5b30 5d29  _array.shape[0])
+0001a3a0: 5d0a 2020 2020 636f 6c73 203d 205b 4772  ].    cols = [Gr
+0001a3b0: 6f75 7028 7265 665f 6172 7261 795b 3a2c  oup(ref_array[:,
+0001a3c0: 206e 5d29 2066 6f72 206e 2069 6e20 7261   n]) for n in ra
+0001a3d0: 6e67 6528 7265 665f 6172 7261 792e 7368  nge(ref_array.sh
+0001a3e0: 6170 655b 315d 295d 0a0a 2020 2020 2320  ape[1])]..    # 
+0001a3f0: 416c 6967 6e20 726f 7773 2061 6e64 2063  Align rows and c
+0001a400: 6f6c 756d 6e73 2069 6e64 6570 656e 6465  olumns independe
+0001a410: 6e74 6c79 0a20 2020 2066 6f72 206e 2c20  ntly.    for n, 
+0001a420: 7220 696e 2065 6e75 6d65 7261 7465 2872  r in enumerate(r
+0001a430: 6f77 7329 3a0a 2020 2020 2020 2020 722e  ows):.        r.
+0001a440: 616c 6967 6e28 616c 6967 6e6d 656e 743d  align(alignment=
+0001a450: 616c 6967 6e5f 7929 0a20 2020 2066 6f72  align_y).    for
+0001a460: 206e 2c20 6320 696e 2065 6e75 6d65 7261   n, c in enumera
+0001a470: 7465 2863 6f6c 7329 3a0a 2020 2020 2020  te(cols):.      
+0001a480: 2020 632e 616c 6967 6e28 616c 6967 6e6d    c.align(alignm
+0001a490: 656e 743d 616c 6967 6e5f 7829 0a0a 2020  ent=align_x)..  
+0001a4a0: 2020 2320 4469 7374 7269 6275 7465 2072    # Distribute r
+0001a4b0: 6f77 7320 616e 6420 636f 6c75 6d6e 730a  ows and columns.
+0001a4c0: 2020 2020 4772 6f75 7028 636f 6c73 292e      Group(cols).
+0001a4d0: 6469 7374 7269 6275 7465 280a 2020 2020  distribute(.    
+0001a4e0: 2020 2020 6469 7265 6374 696f 6e3d 2278      direction="x
+0001a4f0: 222c 2073 7061 6369 6e67 3d73 7061 6369  ", spacing=spaci
+0001a500: 6e67 5b30 5d2c 2073 6570 6172 6174 696f  ng[0], separatio
+0001a510: 6e3d 7365 7061 7261 7469 6f6e 2c20 6564  n=separation, ed
+0001a520: 6765 3d65 6467 655f 780a 2020 2020 290a  ge=edge_x.    ).
+0001a530: 2020 2020 4772 6f75 7028 726f 7773 5b3a      Group(rows[:
+0001a540: 3a2d 315d 292e 6469 7374 7269 6275 7465  :-1]).distribute
+0001a550: 280a 2020 2020 2020 2020 6469 7265 6374  (.        direct
+0001a560: 696f 6e3d 2279 222c 2073 7061 6369 6e67  ion="y", spacing
+0001a570: 3d73 7061 6369 6e67 5b31 5d2c 2073 6570  =spacing[1], sep
+0001a580: 6172 6174 696f 6e3d 7365 7061 7261 7469  aration=separati
+0001a590: 6f6e 2c20 6564 6765 3d65 6467 655f 790a  on, edge=edge_y.
+0001a5a0: 2020 2020 290a 0a20 2020 2023 2072 6574      )..    # ret
+0001a5b0: 7572 6e20 6465 7669 6365 5f6d 6174 7269  urn device_matri
+0001a5c0: 780a 2020 2020 7265 7475 726e 2044 0a0a  x.    return D..
+0001a5d0: 0a64 6566 205f 7061 7261 6d65 7465 725f  .def _parameter_
+0001a5e0: 636f 6d62 696e 6174 696f 6e73 2870 6172  combinations(par
+0001a5f0: 616d 6574 6572 735f 6469 6374 293a 0a20  ameters_dict):. 
+0001a600: 2020 2022 2222 4372 6561 7465 7320 7061     """Creates pa
+0001a610: 7261 6d65 7465 7220 636f 6d62 696e 6174  rameter combinat
+0001a620: 696f 6e73 2066 726f 6d20 6120 6469 6374  ions from a dict
+0001a630: 2066 696c 6c65 6420 7769 7468 206c 6973   filled with lis
+0001a640: 7420 7661 6c75 6573 2c20 652e 672e 0a20  t values, e.g.. 
+0001a650: 2020 2070 6172 616d 6574 6572 735f 6469     parameters_di
+0001a660: 6374 203d 207b 0a20 2020 2020 2020 2027  ct = {.        '
+0001a670: 7769 6474 6827 203a 205b 302e 312c 302e  width' : [0.1,0.
+0001a680: 325d 2c0a 2020 2020 2020 2020 276c 656e  2],.        'len
+0001a690: 6774 6827 203a 205b 342c 352c 365d 2c0a  gth' : [4,5,6],.
+0001a6a0: 2020 2020 2020 2020 2768 6569 6768 7427          'height'
+0001a6b0: 203a 205b 3232 5d0a 2020 2020 2020 2020   : [22].        
+0001a6c0: 7d0a 2020 2020 5769 6c6c 2070 726f 6475  }.    Will produ
+0001a6d0: 6365 2061 206c 6973 7420 6f66 2064 6963  ce a list of dic
+0001a6e0: 7469 6f6e 6172 6965 732c 2065 6163 6820  tionaries, each 
+0001a6f0: 6f66 2077 6869 6368 2063 616e 2062 6520  of which can be 
+0001a700: 7573 6564 2061 7320 6b77 6172 6773 2069  used as kwargs i
+0001a710: 6e70 7574 3a0a 2020 2020 2020 2020 5b7b  nput:.        [{
+0001a720: 2768 6569 6768 7427 3a20 3232 2c20 276c  'height': 22, 'l
+0001a730: 656e 6774 6827 3a20 342c 2027 7769 6474  ength': 4, 'widt
+0001a740: 6827 3a20 302e 317d 2c0a 2020 2020 2020  h': 0.1},.      
+0001a750: 2020 207b 2768 6569 6768 7427 3a20 3232     {'height': 22
+0001a760: 2c20 276c 656e 6774 6827 3a20 352c 2027  , 'length': 5, '
+0001a770: 7769 6474 6827 3a20 302e 317d 2c0a 2020  width': 0.1},.  
+0001a780: 2020 2020 2020 207b 2768 6569 6768 7427         {'height'
+0001a790: 3a20 3232 2c20 276c 656e 6774 6827 3a20  : 22, 'length': 
+0001a7a0: 362c 2027 7769 6474 6827 3a20 302e 317d  6, 'width': 0.1}
+0001a7b0: 2c0a 2020 2020 2020 2020 207b 2768 6569  ,.         {'hei
+0001a7c0: 6768 7427 3a20 3232 2c20 276c 656e 6774  ght': 22, 'lengt
+0001a7d0: 6827 3a20 342c 2027 7769 6474 6827 3a20  h': 4, 'width': 
+0001a7e0: 302e 327d 2c0a 2020 2020 2020 2020 207b  0.2},.         {
+0001a7f0: 2768 6569 6768 7427 3a20 3232 2c20 276c  'height': 22, 'l
+0001a800: 656e 6774 6827 3a20 352c 2027 7769 6474  ength': 5, 'widt
+0001a810: 6827 3a20 302e 327d 2c0a 2020 2020 2020  h': 0.2},.      
+0001a820: 2020 207b 2768 6569 6768 7427 3a20 3232     {'height': 22
+0001a830: 2c20 276c 656e 6774 6827 3a20 362c 2027  , 'length': 6, '
+0001a840: 7769 6474 6827 3a20 302e 327d 5d22 2222  width': 0.2}]"""
+0001a850: 0a20 2020 2076 616c 7565 5f63 6f6d 6269  .    value_combi
+0001a860: 6e61 7469 6f6e 7320 3d20 6c69 7374 2869  nations = list(i
+0001a870: 7465 7274 6f6f 6c73 2e70 726f 6475 6374  tertools.product
+0001a880: 282a 7061 7261 6d65 7465 7273 5f64 6963  (*parameters_dic
+0001a890: 742e 7661 6c75 6573 2829 2929 0a20 2020  t.values())).   
+0001a8a0: 206b 6579 7320 3d20 6c69 7374 2870 6172   keys = list(par
+0001a8b0: 616d 6574 6572 735f 6469 6374 2e6b 6579  ameters_dict.key
+0001a8c0: 7328 2929 0a20 2020 2072 6574 7572 6e20  s()).    return 
+0001a8d0: 5b0a 2020 2020 2020 2020 7b6b 6579 735b  [.        {keys[
+0001a8e0: 6e5d 3a20 7661 6c75 6573 5b6e 5d20 666f  n]: values[n] fo
+0001a8f0: 7220 6e20 696e 2072 616e 6765 286c 656e  r n in range(len
+0001a900: 286b 6579 7329 297d 2066 6f72 2076 616c  (keys))} for val
+0001a910: 7565 7320 696e 2076 616c 7565 5f63 6f6d  ues in value_com
+0001a920: 6269 6e61 7469 6f6e 730a 2020 2020 5d0a  binations.    ].
+0001a930: 0a0a 6465 6620 5f67 656e 5f70 6172 616d  ..def _gen_param
+0001a940: 5f76 6172 6961 7469 6f6e 7328 0a20 2020  _variations(.   
+0001a950: 2066 756e 6374 696f 6e2c 2070 6172 616d   function, param
+0001a960: 5f76 6172 6961 7469 6f6e 732c 2070 6172  _variations, par
+0001a970: 616d 5f64 6566 6175 6c74 733d 7b7d 2c20  am_defaults={}, 
+0001a980: 7061 7261 6d5f 6f76 6572 7269 6465 3d7b  param_override={
+0001a990: 7d2c 206c 6162 656c 5f6c 6179 6572 3d32  }, label_layer=2
+0001a9a0: 3535 0a29 3a0a 2020 2020 2222 2254 616b  55.):.    """Tak
+0001a9b0: 6573 2065 2e67 2e0a 0a20 2020 2070 6172  es e.g...    par
+0001a9c0: 616d 5f76 6172 6961 7469 6f6e 7320 3d20  am_variations = 
+0001a9d0: 7b0a 2020 2020 2020 2020 2020 2020 2763  {.            'c
+0001a9e0: 6861 6e6e 656c 5f77 6964 7468 2720 3a20  hannel_width' : 
+0001a9f0: 5b31 2c32 2c33 5d0a 2020 2020 2020 2020  [1,2,3].        
+0001aa00: 2020 2020 2767 6174 655f 7769 6474 6827      'gate_width'
+0001aa10: 203a 205b 302e 312c 302e 322c 302e 345d   : [0.1,0.2,0.4]
+0001aa20: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+0001aa30: 2020 2020 2020 206f 7220 6571 7569 7661         or equiva
+0001aa40: 6c65 6e74 6c79 0a20 2020 2070 6172 616d  lently.    param
+0001aa50: 5f76 6172 6961 7469 6f6e 7320 3d20 6469  _variations = di
+0001aa60: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+0001aa70: 6368 616e 6e65 6c5f 7769 6474 6820 3d20  channel_width = 
+0001aa80: 5b31 2c32 2c33 5d2c 0a20 2020 2020 2020  [1,2,3],.       
+0001aa90: 2020 2020 2067 6174 655f 7769 6474 6820       gate_width 
+0001aaa0: 3d20 5b30 2e31 2c30 2e32 2c30 2e34 5d2c  = [0.1,0.2,0.4],
+0001aab0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0001aac0: 2020 2022 2222 0a20 2020 2070 6172 616d     """.    param
+0001aad0: 6574 6572 5f6c 6973 7420 3d20 5f70 6172  eter_list = _par
+0001aae0: 616d 6574 6572 5f63 6f6d 6269 6e61 7469  ameter_combinati
+0001aaf0: 6f6e 7328 7061 7261 6d5f 7661 7269 6174  ons(param_variat
+0001ab00: 696f 6e73 290a 0a20 2020 2044 5f6c 6973  ions)..    D_lis
+0001ab10: 7420 3d20 5b5d 0a20 2020 2066 6f72 2070  t = [].    for p
+0001ab20: 6172 616d 7320 696e 2070 6172 616d 6574  arams in paramet
+0001ab30: 6572 5f6c 6973 743a 0a20 2020 2020 2020  er_list:.       
+0001ab40: 206e 6577 5f70 6172 616d 7320 3d20 6469   new_params = di
+0001ab50: 6374 2829 0a20 2020 2020 2020 206e 6577  ct().        new
+0001ab60: 5f70 6172 616d 732e 7570 6461 7465 2870  _params.update(p
+0001ab70: 6172 616d 7329 0a20 2020 2020 2020 206e  arams).        n
+0001ab80: 6577 5f70 6172 616d 732e 7570 6461 7465  ew_params.update
+0001ab90: 2870 6172 616d 5f6f 7665 7272 6964 6529  (param_override)
+0001aba0: 0a20 2020 2020 2020 2044 5f6e 6577 203d  .        D_new =
+0001abb0: 206d 616b 655f 6465 7669 6365 2866 756e   make_device(fun
+0001abc0: 6374 696f 6e2c 2063 6f6e 6669 673d 7061  ction, config=pa
+0001abd0: 7261 6d5f 6465 6661 756c 7473 2c20 2a2a  ram_defaults, **
+0001abe0: 6e65 775f 7061 7261 6d73 290a 2020 2020  new_params).    
+0001abf0: 2020 2020 6c61 6265 6c5f 7465 7874 203d      label_text =
+0001ac00: 2022 220a 2020 2020 2020 2020 666f 7220   "".        for 
+0001ac10: 6e61 6d65 2c20 7661 6c75 6520 696e 2070  name, value in p
+0001ac20: 6172 616d 732e 6974 656d 7328 293a 0a20  arams.items():. 
+0001ac30: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0001ac40: 5f74 6578 7420 2b3d 2028 6622 7b6e 616d  _text += (f"{nam
+0001ac50: 657d 3d7b 7661 6c75 657d 2229 202b 2022  e}={value}") + "
+0001ac60: 5c6e 220a 2020 2020 2020 2020 6966 206c  \n".        if l
+0001ac70: 6162 656c 5f6c 6179 6572 2069 7320 6e6f  abel_layer is no
+0001ac80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001ac90: 2020 2020 445f 6e65 772e 6164 645f 6c61      D_new.add_la
+0001aca0: 6265 6c28 7465 7874 3d6c 6162 656c 5f74  bel(text=label_t
+0001acb0: 6578 742c 2070 6f73 6974 696f 6e3d 445f  ext, position=D_
+0001acc0: 6e65 772e 6365 6e74 6572 2c20 6c61 7965  new.center, laye
+0001acd0: 723d 6c61 6265 6c5f 6c61 7965 7229 0a0a  r=label_layer)..
+0001ace0: 2020 2020 2020 2020 445f 6c69 7374 2e61          D_list.a
+0001acf0: 7070 656e 6428 445f 6e65 7729 0a20 2020  ppend(D_new).   
+0001ad00: 2072 6574 7572 6e20 445f 6c69 7374 0a0a   return D_list..
+0001ad10: 0a64 6566 2067 7269 6473 7765 6570 280a  .def gridsweep(.
+0001ad20: 2020 2020 6675 6e63 7469 6f6e 2c0a 2020      function,.  
+0001ad30: 2020 7061 7261 6d5f 783d 7b22 7769 6474    param_x={"widt
+0001ad40: 6822 3a20 5b31 2c20 352c 2036 2c20 375d  h": [1, 5, 6, 7]
+0001ad50: 7d2c 0a20 2020 2070 6172 616d 5f79 3d7b  },.    param_y={
+0001ad60: 226c 656e 6774 6822 3a20 5b31 2e31 2c20  "length": [1.1, 
+0001ad70: 322c 2037 305d 7d2c 0a20 2020 2070 6172  2, 70]},.    par
+0001ad80: 616d 5f64 6566 6175 6c74 733d 7b7d 2c0a  am_defaults={},.
+0001ad90: 2020 2020 7061 7261 6d5f 6f76 6572 7269      param_overri
+0001ada0: 6465 3d7b 7d2c 0a20 2020 2073 7061 6369  de={},.    spaci
+0001adb0: 6e67 3d28 3530 2c20 3130 3029 2c0a 2020  ng=(50, 100),.  
+0001adc0: 2020 7365 7061 7261 7469 6f6e 3d54 7275    separation=Tru
+0001add0: 652c 0a20 2020 2061 6c69 676e 5f78 3d22  e,.    align_x="
+0001ade0: 7822 2c0a 2020 2020 616c 6967 6e5f 793d  x",.    align_y=
+0001adf0: 2279 222c 0a20 2020 2065 6467 655f 783d  "y",.    edge_x=
+0001ae00: 2278 222c 0a20 2020 2065 6467 655f 793d  "x",.    edge_y=
+0001ae10: 2279 6d69 6e22 2c0a 2020 2020 6c61 6265  "ymin",.    labe
+0001ae20: 6c5f 6c61 7965 723d 3235 352c 0a29 3a0a  l_layer=255,.):.
+0001ae30: 2020 2020 2222 2243 7265 6174 6573 2061      """Creates a
+0001ae40: 2070 6172 616d 6574 6572 2073 7765 6570   parameter sweep
+0001ae50: 206f 6620 6465 7669 6365 7320 616e 6420   of devices and 
+0001ae60: 706c 6163 6573 2074 6865 6d20 6f6e 2061  places them on a
+0001ae70: 2067 7269 6420 7769 7468 0a20 2020 206c   grid with.    l
+0001ae80: 6162 656c 7320 666f 7220 6561 6368 2064  abels for each d
+0001ae90: 6576 6963 652e 2046 6f72 2069 6e73 7461  evice. For insta
+0001aea0: 6e63 652c 2067 6976 656e 2061 2066 756e  nce, given a fun
+0001aeb0: 6374 696f 6e20 6465 6669 6e65 6420 6c69  ction defined li
+0001aec0: 6b65 0a20 2020 2060 6d79 7368 6170 6528  ke.    `myshape(
+0001aed0: 7769 6474 682c 2068 6569 6768 742c 206f  width, height, o
+0001aee0: 6666 7365 742c 206c 6179 6572 2960 2061  ffset, layer)` a
+0001aef0: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
+0001af00: 2070 6172 616d 6574 6572 733a 0a20 2020   parameters:.   
+0001af10: 2020 2020 2070 6172 616d 5f78 203d 207b       param_x = {
+0001af20: 2777 6964 7468 2720 3a20 205b 342c 2035  'width' :  [4, 5
+0001af30: 2c20 365d 2020 7d2c 0a20 2020 2020 2020  , 6]  },.       
+0001af40: 2070 6172 616d 5f79 203d 207b 2768 6569   param_y = {'hei
+0001af50: 6768 7427 203a 205b 372c 2039 5d2c 0a20  ght' : [7, 9],. 
+0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af70: 2020 276c 6179 6572 2720 3a20 205b 312c    'layer' :  [1,
+0001af80: 2032 2c20 335d 2020 7d2c 0a20 2020 2020   2, 3]  },.     
+0001af90: 2020 2070 6172 616d 5f64 6566 6175 6c74     param_default
+0001afa0: 7320 3d20 7b27 7363 616c 6527 203a 2031  s = {'scale' : 1
+0001afb0: 7d0a 0a20 2020 2067 7269 6473 7765 6570  }..    gridsweep
+0001afc0: 2829 2070 726f 6475 6365 2061 2067 7269  () produce a gri
+0001afd0: 6420 6f66 2064 6576 6963 6573 2077 6974  d of devices wit
+0001afe0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
+0001aff0: 6c61 796f 7574 2f70 6172 616d 6574 6572  layout/parameter
+0001b000: 733a 0a20 2020 2020 2020 2028 773d 342c  s:.        (w=4,
+0001b010: 2068 3d37 2c20 733d 312c 206c 3d31 2920   h=7, s=1, l=1) 
+0001b020: 2020 2028 773d 352c 2068 3d37 2c20 733d     (w=5, h=7, s=
+0001b030: 312c 206c 3d31 2920 2020 2028 773d 362c  1, l=1)    (w=6,
+0001b040: 2068 3d37 2c20 733d 312c 206c 3d31 290a   h=7, s=1, l=1).
+0001b050: 2020 2020 2020 2020 2877 3d34 2c20 683d          (w=4, h=
+0001b060: 372c 2073 3d31 2c20 6c3d 3229 2020 2020  7, s=1, l=2)    
+0001b070: 2877 3d35 2c20 683d 372c 2073 3d31 2c20  (w=5, h=7, s=1, 
+0001b080: 6c3d 3229 2020 2020 2877 3d36 2c20 683d  l=2)    (w=6, h=
+0001b090: 372c 2073 3d31 2c20 6c3d 3229 0a20 2020  7, s=1, l=2).   
+0001b0a0: 2020 2020 2028 773d 342c 2068 3d37 2c20       (w=4, h=7, 
+0001b0b0: 733d 312c 206c 3d33 2920 2020 2028 773d  s=1, l=3)    (w=
+0001b0c0: 352c 2068 3d37 2c20 733d 312c 206c 3d33  5, h=7, s=1, l=3
+0001b0d0: 2920 2020 2028 773d 362c 2068 3d37 2c20  )    (w=6, h=7, 
+0001b0e0: 733d 312c 206c 3d33 290a 2020 2020 2020  s=1, l=3).      
+0001b0f0: 2020 2877 3d34 2c20 683d 392c 2073 3d31    (w=4, h=9, s=1
+0001b100: 2c20 6c3d 3129 2020 2020 2877 3d35 2c20  , l=1)    (w=5, 
+0001b110: 683d 392c 2073 3d31 2c20 6c3d 3129 2020  h=9, s=1, l=1)  
+0001b120: 2020 2877 3d36 2c20 683d 392c 2073 3d31    (w=6, h=9, s=1
+0001b130: 2c20 6c3d 3129 0a20 2020 2020 2020 2028  , l=1).        (
+0001b140: 773d 342c 2068 3d39 2c20 733d 312c 206c  w=4, h=9, s=1, l
+0001b150: 3d32 2920 2020 2028 773d 352c 2068 3d39  =2)    (w=5, h=9
+0001b160: 2c20 733d 312c 206c 3d32 2920 2020 2028  , s=1, l=2)    (
+0001b170: 773d 362c 2068 3d39 2c20 733d 312c 206c  w=6, h=9, s=1, l
+0001b180: 3d32 290a 2020 2020 2020 2020 2877 3d34  =2).        (w=4
+0001b190: 2c20 683d 392c 2073 3d31 2c20 6c3d 3329  , h=9, s=1, l=3)
+0001b1a0: 2020 2020 2877 3d35 2c20 683d 392c 2073      (w=5, h=9, s
+0001b1b0: 3d31 2c20 6c3d 3329 2020 2020 2877 3d36  =1, l=3)    (w=6
+0001b1c0: 2c20 683d 392c 2073 3d31 2c20 6c3d 3329  , h=9, s=1, l=3)
+0001b1d0: 0a0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+0001b1e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0001b1f0: 0a20 2020 2066 756e 6374 696f 6e20 3a20  .    function : 
+0001b200: 6675 6e63 7469 6f6e 2074 6861 7420 7072  function that pr
+0001b210: 6f64 7563 6573 2061 2044 6576 6963 650a  oduces a Device.
+0001b220: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
+0001b230: 7469 6f6e 2077 6869 6368 2077 696c 6c20  tion which will 
+0001b240: 6265 2075 7365 6420 746f 2063 7265 6174  be used to creat
+0001b250: 6520 7468 6520 696e 6469 7669 6475 616c  e the individual
+0001b260: 2064 6576 6963 6573 2069 6e20 7468 650a   devices in the.
+0001b270: 2020 2020 2020 2020 6772 6964 2e20 204d          grid.  M
+0001b280: 7573 7420 6f6e 6c79 2072 6574 7572 6e20  ust only return 
+0001b290: 6120 7369 6e67 6c65 2044 6576 6963 6520  a single Device 
+0001b2a0: 2865 2e67 2e20 616e 7920 6f66 2074 6865  (e.g. any of the
+0001b2b0: 2066 756e 6374 696f 6e73 2069 6e0a 2020   functions in.  
+0001b2c0: 2020 2020 2020 7067 2e67 656f 6d65 7472        pg.geometr
+0001b2d0: 7929 0a20 2020 2070 6172 616d 5f78 203a  y).    param_x :
+0001b2e0: 2064 6963 740a 2020 2020 2020 2020 4120   dict.        A 
+0001b2f0: 6469 6374 696f 6e61 7279 206f 6620 6f6e  dictionary of on
+0001b300: 6520 6f72 206d 6f72 6520 7061 7261 6d65  e or more parame
+0001b310: 7465 7273 2074 6f20 7377 6565 7020 696e  ters to sweep in
+0001b320: 2074 6865 2078 2d64 6972 6563 7469 6f6e   the x-direction
+0001b330: 0a20 2020 2070 6172 616d 5f79 203a 2064  .    param_y : d
+0001b340: 6963 740a 2020 2020 2020 2020 4120 6469  ict.        A di
+0001b350: 6374 696f 6e61 7279 206f 6620 6f6e 6520  ctionary of one 
+0001b360: 6f72 206d 6f72 6520 7061 7261 6d65 7465  or more paramete
+0001b370: 7273 2074 6f20 7377 6565 7020 696e 2074  rs to sweep in t
+0001b380: 6865 2079 2d64 6972 6563 7469 6f6e 0a20  he y-direction. 
+0001b390: 2020 2070 6172 616d 5f64 6566 6175 6c74     param_default
+0001b3a0: 7320 3a20 6469 6374 0a20 2020 2020 2020  s : dict.       
+0001b3b0: 2044 6566 6175 6c74 2070 6172 616d 6574   Default paramet
+0001b3c0: 6572 7320 746f 2070 6173 7320 746f 2065  ers to pass to e
+0001b3d0: 7665 7279 2064 6576 6963 6520 696e 2074  very device in t
+0001b3e0: 6865 2067 7269 640a 2020 2020 7061 7261  he grid.    para
+0001b3f0: 6d5f 6f76 6572 7269 6465 203a 2064 6963  m_override : dic
+0001b400: 740a 2020 2020 2020 2020 5061 7261 6d65  t.        Parame
+0001b410: 7465 7273 2074 6861 7420 7769 6c6c 206f  ters that will o
+0001b420: 7665 7272 6964 6520 6070 6172 616d 5f64  verride `param_d
+0001b430: 6566 6175 6c74 7360 2c20 6571 7569 7661  efaults`, equiva
+0001b440: 6c65 6e74 2074 6f20 6368 616e 6769 6e67  lent to changing
+0001b450: 0a20 2020 2020 2020 2070 6172 616d 5f64  .        param_d
+0001b460: 6566 6175 6c74 7320 2875 7365 6675 6c20  efaults (useful 
+0001b470: 290a 2020 2020 7370 6163 696e 6720 3a20  ).    spacing : 
+0001b480: 696e 742c 2066 6c6f 6174 2c20 6f72 2061  int, float, or a
+0001b490: 7272 6179 2d6c 696b 655b 325d 206f 6620  rray-like[2] of 
+0001b4a0: 696e 7420 6f72 2066 6c6f 6174 0a20 2020  int or float.   
+0001b4b0: 2020 2020 2053 7061 6369 6e67 2062 6574       Spacing bet
+0001b4c0: 7765 656e 2061 646a 6163 656e 7420 656c  ween adjacent el
+0001b4d0: 656d 656e 7473 206f 6e20 7468 6520 6772  ements on the gr
+0001b4e0: 6964 2c20 6361 6e20 6265 2061 2074 7570  id, can be a tup
+0001b4f0: 6c65 2066 6f72 0a20 2020 2020 2020 2064  le for.        d
+0001b500: 6966 6665 7265 6e74 2064 6973 7461 6e63  ifferent distanc
+0001b510: 6573 2069 6e20 7769 6474 6820 616e 6420  es in width and 
+0001b520: 6865 6967 6874 2028 782c 7929 2e0a 2020  height (x,y)..  
+0001b530: 2020 7365 7061 7261 7469 6f6e 203a 2062    separation : b
+0001b540: 6f6f 6c0a 2020 2020 2020 2020 4966 2054  ool.        If T
+0001b550: 7275 652c 2067 7561 7261 6e74 6565 7320  rue, guarantees 
+0001b560: 656c 656d 656e 7473 2061 7265 2073 6570  elements are sep
+0001b570: 6172 6174 6564 2077 6974 6820 6120 6669  arated with a fi
+0001b580: 7865 6420 7370 6163 696e 670a 2020 2020  xed spacing.    
+0001b590: 2020 2020 6265 7477 6565 6e3b 2069 6620      between; if 
+0001b5a0: 4661 6c73 652c 2065 6c65 6d65 6e74 7320  False, elements 
+0001b5b0: 6172 6520 7370 6163 6564 2065 7665 6e6c  are spaced evenl
+0001b5c0: 7920 616c 6f6e 6720 6120 6772 6964 2e0a  y along a grid..
+0001b5d0: 2020 2020 7368 6170 6520 3a20 6172 7261      shape : arra
+0001b5e0: 792d 6c69 6b65 5b32 5d0a 2020 2020 2020  y-like[2].      
+0001b5f0: 2020 782c 2079 2073 6861 7065 206f 6620    x, y shape of 
+0001b600: 7468 6520 6772 6964 2028 7365 6520 6e70  the grid (see np
+0001b610: 2e72 6573 6861 7065 292e 2049 6620 6e6f  .reshape). If no
+0001b620: 2073 6861 7065 2069 7320 6769 7665 6e20   shape is given 
+0001b630: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
+0001b640: 6c69 7374 2069 7320 3144 2c20 7468 6520  list is 1D, the 
+0001b650: 6f75 7470 7574 2069 7320 6173 2069 6620  output is as if 
+0001b660: 6e70 2e72 6573 6861 7065 2077 6572 6520  np.reshape were 
+0001b670: 7275 6e20 7769 7468 2028 312c 202d 3129  run with (1, -1)
+0001b680: 2e0a 2020 2020 616c 6967 6e5f 7820 3a20  ..    align_x : 
+0001b690: 7b27 7827 2c20 2778 6d69 6e27 2c20 2778  {'x', 'xmin', 'x
+0001b6a0: 6d61 7827 7d0a 2020 2020 2020 2020 5768  max'}.        Wh
+0001b6b0: 6963 6820 6564 6765 2074 6f20 7065 7266  ich edge to perf
+0001b6c0: 6f72 6d20 7468 6520 7820 2863 6f6c 756d  orm the x (colum
+0001b6d0: 6e29 2061 6c69 676e 6d65 6e74 2061 6c6f  n) alignment alo
+0001b6e0: 6e67 0a20 2020 2061 6c69 676e 5f79 203a  ng.    align_y :
+0001b6f0: 207b 2779 272c 2027 796d 696e 272c 2027   {'y', 'ymin', '
+0001b700: 796d 6178 277d 0a20 2020 2020 2020 2057  ymax'}.        W
+0001b710: 6869 6368 2065 6467 6520 746f 2070 6572  hich edge to per
+0001b720: 666f 726d 2074 6865 2079 2028 726f 7729  form the y (row)
+0001b730: 2061 6c69 676e 6d65 6e74 2061 6c6f 6e67   alignment along
+0001b740: 0a20 2020 2065 6467 655f 7820 3a20 7b27  .    edge_x : {'
+0001b750: 7827 2c20 2778 6d69 6e27 2c20 2778 6d61  x', 'xmin', 'xma
+0001b760: 7827 7d0a 2020 2020 2020 2020 5768 6963  x'}.        Whic
+0001b770: 6820 6564 6765 2074 6f20 7065 7266 6f72  h edge to perfor
+0001b780: 6d20 7468 6520 7820 2863 6f6c 756d 6e29  m the x (column)
+0001b790: 2064 6973 7472 6962 7574 696f 6e20 616c   distribution al
+0001b7a0: 6f6e 6720 2875 6e75 7365 6420 6966 0a20  ong (unused if. 
+0001b7b0: 2020 2020 2020 2073 6570 6172 6174 696f         separatio
+0001b7c0: 6e20 3d3d 2054 7275 6529 0a20 2020 2065  n == True).    e
+0001b7d0: 6467 655f 7920 3a20 7b27 7927 2c20 2779  dge_y : {'y', 'y
+0001b7e0: 6d69 6e27 2c20 2779 6d61 7827 7d0a 2020  min', 'ymax'}.  
+0001b7f0: 2020 2020 2020 5768 6963 6820 6564 6765        Which edge
+0001b800: 2074 6f20 7065 7266 6f72 6d20 7468 6520   to perform the 
+0001b810: 7920 2872 6f77 2920 6469 7374 7269 6275  y (row) distribu
+0001b820: 7469 6f6e 2061 6c6f 6e67 2028 756e 7573  tion along (unus
+0001b830: 6564 2069 660a 2020 2020 2020 2020 7365  ed if.        se
+0001b840: 7061 7261 7469 6f6e 203d 3d20 5472 7565  paration == True
+0001b850: 290a 2020 2020 6c61 6265 6c5f 6c61 7965  ).    label_laye
+0001b860: 7220 3a20 4e6f 6e65 206f 7220 6c61 7965  r : None or laye
+0001b870: 720a 2020 2020 2020 2020 4966 206e 6f74  r.        If not
+0001b880: 204e 6f6e 652c 2077 696c 6c20 706c 6163   None, will plac
+0001b890: 6520 6120 6c61 6265 6c20 7468 6174 2064  e a label that d
+0001b8a0: 6573 6372 6962 6573 2074 6865 2070 6172  escribes the par
+0001b8b0: 616d 6574 6572 7320 6f6e 2074 6865 2064  ameters on the d
+0001b8c0: 6576 6963 650a 0a20 2020 2052 6574 7572  evice..    Retur
+0001b8d0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0001b8e0: 2020 2064 6576 6963 655f 6d61 7472 6978     device_matrix
+0001b8f0: 203a 2044 6576 6963 650a 2020 2020 2020   : Device.      
+0001b900: 2020 4120 4465 7669 6365 2063 6f6e 7461    A Device conta
+0001b910: 696e 696e 6720 616c 6c20 7468 6520 4465  ining all the De
+0001b920: 7669 6365 7320 696e 2060 6465 7669 6365  vices in `device
+0001b930: 5f6c 6973 7460 2069 6e20 6120 6772 6964  _list` in a grid
+0001b940: 2e0a 2020 2020 2222 220a 0a20 2020 2070  ..    """..    p
+0001b950: 6172 616d 5f76 6172 6961 7469 6f6e 7320  aram_variations 
+0001b960: 3d20 4f72 6465 7265 6444 6963 7428 290a  = OrderedDict().
+0001b970: 2020 2020 7061 7261 6d5f 7661 7269 6174      param_variat
+0001b980: 696f 6e73 2e75 7064 6174 6528 7061 7261  ions.update(para
+0001b990: 6d5f 7929 0a20 2020 2070 6172 616d 5f76  m_y).    param_v
+0001b9a0: 6172 6961 7469 6f6e 732e 7570 6461 7465  ariations.update
+0001b9b0: 2870 6172 616d 5f78 290a 0a20 2020 2044  (param_x)..    D
+0001b9c0: 5f6c 6973 7420 3d20 5f67 656e 5f70 6172  _list = _gen_par
+0001b9d0: 616d 5f76 6172 6961 7469 6f6e 7328 0a20  am_variations(. 
+0001b9e0: 2020 2020 2020 2066 756e 6374 696f 6e3d         function=
+0001b9f0: 6675 6e63 7469 6f6e 2c0a 2020 2020 2020  function,.      
+0001ba00: 2020 7061 7261 6d5f 7661 7269 6174 696f    param_variatio
+0001ba10: 6e73 3d70 6172 616d 5f76 6172 6961 7469  ns=param_variati
+0001ba20: 6f6e 732c 0a20 2020 2020 2020 2070 6172  ons,.        par
+0001ba30: 616d 5f64 6566 6175 6c74 733d 7061 7261  am_defaults=para
+0001ba40: 6d5f 6465 6661 756c 7473 2c0a 2020 2020  m_defaults,.    
+0001ba50: 2020 2020 7061 7261 6d5f 6f76 6572 7269      param_overri
+0001ba60: 6465 3d70 6172 616d 5f6f 7665 7272 6964  de=param_overrid
+0001ba70: 652c 0a20 2020 2020 2020 206c 6162 656c  e,.        label
+0001ba80: 5f6c 6179 6572 3d6c 6162 656c 5f6c 6179  _layer=label_lay
+0001ba90: 6572 2c0a 2020 2020 290a 0a20 2020 206e  er,.    )..    n
+0001baa0: 756d 5f78 5f70 6172 616d 6574 6572 7320  um_x_parameters 
+0001bab0: 3d20 6c65 6e28 5f70 6172 616d 6574 6572  = len(_parameter
+0001bac0: 5f63 6f6d 6269 6e61 7469 6f6e 7328 7061  _combinations(pa
+0001bad0: 7261 6d5f 7829 290a 2020 2020 6e75 6d5f  ram_x)).    num_
+0001bae0: 795f 7061 7261 6d65 7465 7273 203d 206c  y_parameters = l
+0001baf0: 656e 285f 7061 7261 6d65 7465 725f 636f  en(_parameter_co
+0001bb00: 6d62 696e 6174 696f 6e73 2870 6172 616d  mbinations(param
+0001bb10: 5f79 2929 0a20 2020 2044 203d 2067 7269  _y)).    D = gri
+0001bb20: 6428 0a20 2020 2020 2020 2044 5f6c 6973  d(.        D_lis
+0001bb30: 742c 0a20 2020 2020 2020 2073 7061 6369  t,.        spaci
+0001bb40: 6e67 3d73 7061 6369 6e67 2c0a 2020 2020  ng=spacing,.    
+0001bb50: 2020 2020 7365 7061 7261 7469 6f6e 3d73      separation=s
+0001bb60: 6570 6172 6174 696f 6e2c 0a20 2020 2020  eparation,.     
+0001bb70: 2020 2073 6861 7065 3d28 6e75 6d5f 785f     shape=(num_x_
+0001bb80: 7061 7261 6d65 7465 7273 2c20 6e75 6d5f  parameters, num_
+0001bb90: 795f 7061 7261 6d65 7465 7273 292c 0a20  y_parameters),. 
+0001bba0: 2020 2020 2020 2061 6c69 676e 5f78 3d61         align_x=a
+0001bbb0: 6c69 676e 5f78 2c0a 2020 2020 2020 2020  lign_x,.        
+0001bbc0: 616c 6967 6e5f 793d 616c 6967 6e5f 792c  align_y=align_y,
+0001bbd0: 0a20 2020 2020 2020 2065 6467 655f 783d  .        edge_x=
+0001bbe0: 6564 6765 5f78 2c0a 2020 2020 2020 2020  edge_x,.        
+0001bbf0: 6564 6765 5f79 3d65 6467 655f 792c 0a20  edge_y=edge_y,. 
+0001bc00: 2020 2029 0a0a 2020 2020 6c61 6265 6c5f     )..    label_
+0001bc10: 7465 7874 203d 207b 7d0a 2020 2020 6c61  text = {}.    la
+0001bc20: 6265 6c5f 7465 7874 2e75 7064 6174 6528  bel_text.update(
+0001bc30: 7061 7261 6d5f 6465 6661 756c 7473 290a  param_defaults).
+0001bc40: 2020 2020 6c61 6265 6c5f 7465 7874 2e75      label_text.u
+0001bc50: 7064 6174 6528 7061 7261 6d5f 6f76 6572  pdate(param_over
+0001bc60: 7269 6465 290a 2020 2020 6966 206c 6162  ride).    if lab
+0001bc70: 656c 5f6c 6179 6572 2069 7320 6e6f 7420  el_layer is not 
+0001bc80: 4e6f 6e65 3a0a 2020 2020 2020 2020 442e  None:.        D.
+0001bc90: 6164 645f 6c61 6265 6c28 7465 7874 3d73  add_label(text=s
+0001bca0: 7472 286c 6162 656c 5f74 6578 7429 2c20  tr(label_text), 
+0001bcb0: 706f 7369 7469 6f6e 3d28 442e 786d 696e  position=(D.xmin
+0001bcc0: 2c20 442e 796d 696e 292c 206c 6179 6572  , D.ymin), layer
+0001bcd0: 3d6c 6162 656c 5f6c 6179 6572 290a 0a20  =label_layer).. 
+0001bce0: 2020 2072 6574 7572 6e20 440a 0a0a 6465     return D...de
+0001bcf0: 6620 5f70 6163 6b5f 7369 6e67 6c65 5f62  f _pack_single_b
+0001bd00: 696e 280a 2020 2020 7265 6374 5f64 6963  in(.    rect_dic
+0001bd10: 742c 2061 7370 6563 745f 7261 7469 6f2c  t, aspect_ratio,
+0001bd20: 206d 6178 5f73 697a 652c 2073 6f72 745f   max_size, sort_
+0001bd30: 6279 5f61 7265 612c 2064 656e 7369 7479  by_area, density
+0001bd40: 2c20 7072 6563 6973 696f 6e2c 2076 6572  , precision, ver
+0001bd50: 626f 7365 0a29 3a0a 2020 2020 2222 2254  bose.):.    """T
+0001bd60: 616b 6573 2061 2060 7265 6374 5f64 6963  akes a `rect_dic
+0001bd70: 7460 2061 7267 756d 656e 7420 6f66 2074  t` argument of t
+0001bd80: 6865 2066 6f72 6d20 7b69 643a 2877 2c20  he form {id:(w, 
+0001bd90: 6829 7d20 616e 6420 7472 6965 7320 746f  h)} and tries to
+0001bda0: 0a20 2020 2070 6163 6b20 6974 2069 6e74  .    pack it int
+0001bdb0: 6f20 6120 6269 6e20 6173 2073 6d61 6c6c  o a bin as small
+0001bdc0: 2061 7320 706f 7373 6962 6c65 2077 6974   as possible wit
+0001bdd0: 6820 6173 7065 6374 2072 6174 696f 2060  h aspect ratio `
+0001bde0: 6173 7065 6374 5f72 6174 696f 602e 0a20  aspect_ratio`.. 
+0001bdf0: 2020 2057 696c 6c20 6974 6572 6174 6976     Will iterativ
+0001be00: 656c 7920 6772 6f77 2074 6865 2062 696e  ely grow the bin
+0001be10: 2073 697a 6520 756e 7469 6c20 6576 6572   size until ever
+0001be20: 7974 6869 6e67 2066 6974 7320 6f72 2074  ything fits or t
+0001be30: 6865 2062 696e 2073 697a 650a 2020 2020  he bin size.    
+0001be40: 7265 6163 6865 7320 606d 6178 5f73 697a  reaches `max_siz
+0001be50: 6560 2e20 5265 7475 726e 7320 6120 6469  e`. Returns a di
+0001be60: 6374 696f 6e61 7279 206f 6620 7468 6520  ctionary of the 
+0001be70: 7061 636b 6564 2072 6563 7461 6e67 6c65  packed rectangle
+0001be80: 736e 2069 6e20 7468 650a 2020 2020 666f  sn in the.    fo
+0001be90: 726d 207b 6964 3a28 782c 2079 2c20 772c  rm {id:(x, y, w,
+0001bea0: 2068 297d 2c20 616e 6420 6120 6469 6374   h)}, and a dict
+0001beb0: 696f 6e61 7279 206f 6620 7265 6d61 696e  ionary of remain
+0001bec0: 696e 6720 756e 7061 636b 6564 2072 6563  ing unpacked rec
+0001bed0: 7473 2e0a 2020 2020 2222 220a 2020 2020  ts..    """.    
+0001bee0: 7472 793a 0a20 2020 2020 2020 2069 6d70  try:.        imp
+0001bef0: 6f72 7420 7265 6374 7061 636b 0a20 2020  ort rectpack.   
+0001bf00: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0001bf10: 6e3a 0a20 2020 2020 2020 2072 6169 7365  n:.        raise
+0001bf20: 2049 6d70 6f72 7445 7272 6f72 280a 2020   ImportError(.  
+0001bf30: 2020 2020 2020 2020 2020 225b 5048 4944            "[PHID
+0001bf40: 4c5d 2054 6865 2070 6163 6b65 7228 2920  L] The packer() 
+0001bf50: 6675 6e63 7469 6f6e 2072 6571 7569 7265  function require
+0001bf60: 7320 7468 6520 220a 2020 2020 2020 2020  s the ".        
+0001bf70: 2020 2020 276d 6f64 756c 6520 2272 6563      'module "rec
+0001bf80: 7470 6163 6b22 2074 6f20 6f70 6572 6174  tpack" to operat
+0001bf90: 652e 2020 506c 6561 7365 2072 6574 7279  e.  Please retry
+0001bfa0: 2027 0a20 2020 2020 2020 2020 2020 2022   '.            "
+0001bfb0: 6166 7465 7220 696e 7374 616c 6c69 6e67  after installing
+0001bfc0: 2072 6563 7470 6163 6b3a 5c6e 5c6e 220a   rectpack:\n\n".
+0001bfd0: 2020 2020 2020 2020 2020 2020 2224 2070              "$ p
+0001bfe0: 6970 2069 6e73 7461 6c6c 2072 6563 7470  ip install rectp
+0001bff0: 6163 6b22 0a20 2020 2020 2020 2029 0a0a  ack".        )..
+0001c000: 2020 2020 2320 436f 6d70 7574 6520 746f      # Compute to
+0001c010: 7461 6c20 6172 6561 2061 6e64 2075 7365  tal area and use
+0001c020: 2069 7420 666f 7220 616e 2069 6e69 7469   it for an initi
+0001c030: 616c 2065 7374 696d 6174 6520 6f66 2074  al estimate of t
+0001c040: 6865 2062 696e 2073 697a 650a 2020 2020  he bin size.    
+0001c050: 746f 7461 6c5f 6172 6561 203d 2030 0a20  total_area = 0. 
+0001c060: 2020 2066 6f72 2072 2069 6e20 7265 6374     for r in rect
+0001c070: 5f64 6963 742e 7661 6c75 6573 2829 3a0a  _dict.values():.
+0001c080: 2020 2020 2020 2020 746f 7461 6c5f 6172          total_ar
+0001c090: 6561 202b 3d20 725b 305d 202a 2072 5b31  ea += r[0] * r[1
+0001c0a0: 5d0a 2020 2020 2320 4e6f 726d 616c 697a  ].    # Normaliz
+0001c0b0: 650a 2020 2020 6173 7065 6374 5f72 6174  e.    aspect_rat
+0001c0c0: 696f 203d 206e 702e 6173 6172 7261 7928  io = np.asarray(
+0001c0d0: 6173 7065 6374 5f72 6174 696f 2920 2f20  aspect_ratio) / 
+0001c0e0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2861  np.linalg.norm(a
+0001c0f0: 7370 6563 745f 7261 7469 6f29 0a0a 2020  spect_ratio)..  
+0001c100: 2020 2320 5365 7475 7020 7661 7269 6162    # Setup variab
+0001c110: 6c65 730a 2020 2020 626f 785f 7369 7a65  les.    box_size
+0001c120: 203d 206e 702e 6173 6172 7261 7928 6173   = np.asarray(as
+0001c130: 7065 6374 5f72 6174 696f 202a 206e 702e  pect_ratio * np.
+0001c140: 7371 7274 2874 6f74 616c 5f61 7265 6129  sqrt(total_area)
+0001c150: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+0001c160: 3634 290a 2020 2020 626f 785f 7369 7a65  64).    box_size
+0001c170: 203d 206e 702e 636c 6970 2862 6f78 5f73   = np.clip(box_s
+0001c180: 697a 652c 204e 6f6e 652c 206d 6178 5f73  ize, None, max_s
+0001c190: 697a 6529 0a20 2020 2069 6620 736f 7274  ize).    if sort
+0001c1a0: 5f62 795f 6172 6561 3a0a 2020 2020 2020  _by_area:.      
+0001c1b0: 2020 7270 5f73 6f72 7420 3d20 7265 6374    rp_sort = rect
+0001c1c0: 7061 636b 2e53 4f52 545f 4152 4541 0a20  pack.SORT_AREA. 
+0001c1d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001c1e0: 2072 705f 736f 7274 203d 2072 6563 7470   rp_sort = rectp
+0001c1f0: 6163 6b2e 534f 5254 5f4e 4f4e 450a 0a20  ack.SORT_NONE.. 
+0001c200: 2020 2023 2052 6570 6561 7465 646c 7920     # Repeatedly 
+0001c210: 7275 6e20 7468 6520 7265 6374 616e 676c  run the rectangl
+0001c220: 652d 7061 636b 696e 6720 616c 676f 7269  e-packing algori
+0001c230: 7468 6d20 7769 7468 2069 6e63 7265 6173  thm with increas
+0001c240: 696e 676c 7920 6c61 7267 6572 0a20 2020  ingly larger.   
+0001c250: 2023 2061 7265 6173 2075 6e74 696c 2065   # areas until e
+0001c260: 7665 7279 7468 696e 6720 6669 7473 206f  verything fits o
+0001c270: 7220 7765 2776 6520 7265 6163 6865 6420  r we've reached 
+0001c280: 7468 6520 6d61 7869 6d75 6d20 7369 7a65  the maximum size
+0001c290: 0a20 2020 2077 6869 6c65 2054 7275 653a  .    while True:
+0001c2a0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+0001c2b0: 6520 7468 6520 7061 636b 6572 206f 626a  e the packer obj
+0001c2c0: 6563 740a 2020 2020 2020 2020 7265 6374  ect.        rect
+0001c2d0: 5f70 6163 6b65 7220 3d20 7265 6374 7061  _packer = rectpa
+0001c2e0: 636b 2e6e 6577 5061 636b 6572 280a 2020  ck.newPacker(.  
+0001c2f0: 2020 2020 2020 2020 2020 6d6f 6465 3d72            mode=r
+0001c300: 6563 7470 6163 6b2e 5061 636b 696e 674d  ectpack.PackingM
+0001c310: 6f64 652e 4f66 666c 696e 652c 0a20 2020  ode.Offline,.   
+0001c320: 2020 2020 2020 2020 2070 6163 6b5f 616c           pack_al
+0001c330: 676f 3d72 6563 7470 6163 6b2e 4d61 7852  go=rectpack.MaxR
+0001c340: 6563 7473 426c 7366 2c0a 2020 2020 2020  ectsBlsf,.      
+0001c350: 2020 2020 2020 736f 7274 5f61 6c67 6f3d        sort_algo=
+0001c360: 7270 5f73 6f72 742c 0a20 2020 2020 2020  rp_sort,.       
+0001c370: 2020 2020 2062 696e 5f61 6c67 6f3d 7265       bin_algo=re
+0001c380: 6374 7061 636b 2e50 6163 6b69 6e67 4269  ctpack.PackingBi
+0001c390: 6e2e 4242 462c 0a20 2020 2020 2020 2020  n.BBF,.         
+0001c3a0: 2020 2072 6f74 6174 696f 6e3d 4661 6c73     rotation=Fals
+0001c3b0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+0001c3c0: 2020 2020 2020 2320 4164 6420 6561 6368        # Add each
+0001c3d0: 2072 6563 7461 6e67 6c65 2074 6f20 7468   rectangle to th
+0001c3e0: 6520 7061 636b 6572 2c20 6372 6561 7465  e packer, create
+0001c3f0: 2061 2073 696e 676c 6520 6269 6e2c 2061   a single bin, a
+0001c400: 6e64 2070 6163 6b0a 2020 2020 2020 2020  nd pack.        
+0001c410: 666f 7220 7269 642c 2072 2069 6e20 7265  for rid, r in re
+0001c420: 6374 5f64 6963 742e 6974 656d 7328 293a  ct_dict.items():
+0001c430: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+0001c440: 745f 7061 636b 6572 2e61 6464 5f72 6563  t_packer.add_rec
+0001c450: 7428 7769 6474 683d 725b 305d 2c20 6865  t(width=r[0], he
+0001c460: 6967 6874 3d72 5b31 5d2c 2072 6964 3d72  ight=r[1], rid=r
+0001c470: 6964 290a 2020 2020 2020 2020 7265 6374  id).        rect
+0001c480: 5f70 6163 6b65 722e 6164 645f 6269 6e28  _packer.add_bin(
+0001c490: 7769 6474 683d 626f 785f 7369 7a65 5b30  width=box_size[0
+0001c4a0: 5d2c 2068 6569 6768 743d 626f 785f 7369  ], height=box_si
+0001c4b0: 7a65 5b31 5d29 0a20 2020 2020 2020 2072  ze[1]).        r
+0001c4c0: 6563 745f 7061 636b 6572 2e70 6163 6b28  ect_packer.pack(
+0001c4d0: 290a 0a20 2020 2020 2020 2023 2041 646a  )..        # Adj
+0001c4e0: 7573 7420 7468 6520 626f 7820 7369 7a65  ust the box size
+0001c4f0: 2066 6f72 206e 6578 7420 7469 6d65 0a20   for next time. 
+0001c500: 2020 2020 2020 2062 6f78 5f73 697a 6520         box_size 
+0001c510: 2a3d 2064 656e 7369 7479 2020 2320 496e  *= density  # In
+0001c520: 6372 6561 7365 2061 7265 6120 746f 2074  crease area to t
+0001c530: 7279 2074 6f20 6669 740a 2020 2020 2020  ry to fit.      
+0001c540: 2020 626f 785f 7369 7a65 203d 206e 702e    box_size = np.
+0001c550: 636c 6970 2862 6f78 5f73 697a 652c 204e  clip(box_size, N
+0001c560: 6f6e 652c 206d 6178 5f73 697a 6529 0a20  one, max_size). 
+0001c570: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
+0001c580: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+0001c590: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+0001c5a0: 2020 2020 2020 2254 7279 696e 6720 746f        "Trying to
+0001c5b0: 2070 6163 6b20 696e 2062 696e 2073 697a   pack in bin siz
+0001c5c0: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+0001c5d0: 2020 2020 2228 2530 2e32 662c 2025 302e      "(%0.2f, %0.
+0001c5e0: 3266 2922 2025 2074 7570 6c65 2862 6f78  2f)" % tuple(box
+0001c5f0: 5f73 697a 6520 2a20 7072 6563 6973 696f  _size * precisio
+0001c600: 6e29 0a20 2020 2020 2020 2020 2020 2029  n).            )
+0001c610: 0a0a 2020 2020 2020 2020 2320 5175 6974  ..        # Quit
+0001c620: 2074 6865 206c 6f6f 7020 6966 2077 6527   the loop if we'
+0001c630: 7665 2070 6163 6b65 6420 616c 6c20 7468  ve packed all th
+0001c640: 6520 7265 6374 616e 676c 6573 0a20 2020  e rectangles.   
+0001c650: 2020 2020 2023 206f 7220 7265 6163 6865       # or reache
+0001c660: 6420 7468 6520 6d61 7820 7369 7a65 0a20  d the max size. 
+0001c670: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+0001c680: 6374 5f70 6163 6b65 722e 7265 6374 5f6c  ct_packer.rect_l
+0001c690: 6973 7428 2929 203d 3d20 6c65 6e28 7265  ist()) == len(re
+0001c6a0: 6374 5f64 6963 7429 3a0a 2020 2020 2020  ct_dict):.      
+0001c6b0: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+0001c6c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001c6d0: 2020 7072 696e 7428 2253 7563 6365 7373    print("Success
+0001c6e0: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
+0001c6f0: 6272 6561 6b0a 2020 2020 2020 2020 656c  break.        el
+0001c700: 6966 2061 6c6c 2862 6f78 5f73 697a 6520  if all(box_size 
+0001c710: 3e3d 206d 6178 5f73 697a 6529 3a0a 2020  >= max_size):.  
+0001c720: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+0001c730: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+0001c740: 2020 2020 2020 7072 696e 7428 2252 6561        print("Rea
+0001c750: 6368 6564 206d 6178 5f73 697a 652c 2063  ched max_size, c
+0001c760: 7265 6174 696e 6720 2220 2261 6e20 6164  reating " "an ad
+0001c770: 6469 7469 6f6e 616c 2062 696e 2229 0a20  ditional bin"). 
+0001c780: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0001c790: 0a0a 2020 2020 2320 5365 7061 7261 7465  ..    # Separate
+0001c7a0: 2070 6163 6b65 6420 6672 6f6d 2075 6e70   packed from unp
+0001c7b0: 6163 6b65 6420 7265 6374 616e 676c 6573  acked rectangles
+0001c7c0: 2c20 6d61 6b65 2064 6963 7473 206f 6620  , make dicts of 
+0001c7d0: 666f 726d 0a20 2020 2023 207b 6964 3a28  form.    # {id:(
+0001c7e0: 782c 792c 772c 6829 7d0a 2020 2020 7061  x,y,w,h)}.    pa
+0001c7f0: 636b 6564 5f72 6563 745f 6469 6374 203d  cked_rect_dict =
+0001c800: 207b 725b 2d31 5d3a 2072 5b3a 2d31 5d20   {r[-1]: r[:-1] 
+0001c810: 666f 7220 7220 696e 2072 6563 745f 7061  for r in rect_pa
+0001c820: 636b 6572 5b30 5d2e 7265 6374 5f6c 6973  cker[0].rect_lis
+0001c830: 7428 297d 0a20 2020 2075 6e70 6163 6b65  t()}.    unpacke
+0001c840: 645f 7265 6374 5f64 6963 7420 3d20 7b7d  d_rect_dict = {}
+0001c850: 0a20 2020 2066 6f72 206b 2c20 7620 696e  .    for k, v in
+0001c860: 2072 6563 745f 6469 6374 2e69 7465 6d73   rect_dict.items
+0001c870: 2829 3a0a 2020 2020 2020 2020 6966 206b  ():.        if k
+0001c880: 206e 6f74 2069 6e20 7061 636b 6564 5f72   not in packed_r
+0001c890: 6563 745f 6469 6374 3a0a 2020 2020 2020  ect_dict:.      
+0001c8a0: 2020 2020 2020 756e 7061 636b 6564 5f72        unpacked_r
+0001c8b0: 6563 745f 6469 6374 5b6b 5d20 3d20 760a  ect_dict[k] = v.
+0001c8c0: 0a20 2020 2072 6574 7572 6e20 2870 6163  .    return (pac
+0001c8d0: 6b65 645f 7265 6374 5f64 6963 742c 2075  ked_rect_dict, u
+0001c8e0: 6e70 6163 6b65 645f 7265 6374 5f64 6963  npacked_rect_dic
+0001c8f0: 7429 0a0a 0a64 6566 2070 6163 6b65 7228  t)...def packer(
+0001c900: 0a20 2020 2044 5f6c 6973 742c 0a20 2020  .    D_list,.   
+0001c910: 2073 7061 6369 6e67 3d31 302c 0a20 2020   spacing=10,.   
+0001c920: 2061 7370 6563 745f 7261 7469 6f3d 2831   aspect_ratio=(1
+0001c930: 2c20 3129 2c0a 2020 2020 6d61 785f 7369  , 1),.    max_si
+0001c940: 7a65 3d28 4e6f 6e65 2c20 4e6f 6e65 292c  ze=(None, None),
+0001c950: 0a20 2020 2073 6f72 745f 6279 5f61 7265  .    sort_by_are
+0001c960: 613d 5472 7565 2c0a 2020 2020 6465 6e73  a=True,.    dens
+0001c970: 6974 793d 312e 312c 0a20 2020 2070 7265  ity=1.1,.    pre
+0001c980: 6369 7369 6f6e 3d31 652d 322c 0a20 2020  cision=1e-2,.   
+0001c990: 2076 6572 626f 7365 3d46 616c 7365 2c0a   verbose=False,.
+0001c9a0: 293a 0a20 2020 2022 2222 5061 636b 7320  ):.    """Packs 
+0001c9b0: 6765 6f6d 6574 7269 6573 2074 6f67 6574  geometries toget
+0001c9c0: 6865 7220 696e 746f 2072 6563 7461 6e67  her into rectang
+0001c9d0: 756c 6172 2062 696e 732e 0a0a 2020 2020  ular bins...    
+0001c9e0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001c9f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 445f  ---------.    D_
+0001ca00: 6c69 7374 203a 2061 7272 6179 2d6c 696b  list : array-lik
+0001ca10: 6520 6f66 2044 6576 6963 6573 0a20 2020  e of Devices.   
+0001ca20: 2020 2020 2049 6e70 7574 2044 6576 6963       Input Devic
+0001ca30: 6573 2074 6f20 6265 2070 6163 6b65 642e  es to be packed.
+0001ca40: 0a20 2020 2073 7061 6369 6e67 203a 2069  .    spacing : i
+0001ca50: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
+0001ca60: 2020 2020 5468 6520 6d69 6e69 6d75 6d20      The minimum 
+0001ca70: 6469 7374 616e 6365 2062 6574 7765 656e  distance between
+0001ca80: 2061 646a 6163 656e 7420 7368 6170 6573   adjacent shapes
+0001ca90: 2e0a 2020 2020 6173 7065 6374 5f72 6174  ..    aspect_rat
+0001caa0: 696f 203a 2061 7272 6179 2d6c 696b 650a  io : array-like.
+0001cab0: 2020 2020 2020 2020 5468 6520 2877 6964          The (wid
+0001cac0: 7468 2c20 6865 6967 6874 2920 7261 7469  th, height) rati
+0001cad0: 6f20 6f66 2074 6865 2072 6563 7461 6e67  o of the rectang
+0001cae0: 756c 6172 2062 696e 2e0a 2020 2020 6d61  ular bin..    ma
+0001caf0: 785f 7369 7a65 203a 2061 7272 6179 2d6c  x_size : array-l
+0001cb00: 696b 650a 2020 2020 2020 2020 4c69 6d69  ike.        Limi
+0001cb10: 7473 2074 6865 2073 697a 6520 696e 746f  ts the size into
+0001cb20: 2077 6869 6368 2074 6865 2073 6861 7065   which the shape
+0001cb30: 7320 7769 6c6c 2062 6520 7061 636b 6564  s will be packed
+0001cb40: 2e0a 2020 2020 736f 7274 5f62 795f 6172  ..    sort_by_ar
+0001cb50: 6561 203a 2062 6f6f 6c0a 2020 2020 2020  ea : bool.      
+0001cb60: 2020 4966 2074 7275 652c 2070 7265 2d73    If true, pre-s
+0001cb70: 6f72 7473 2074 6865 2073 6861 7065 7320  orts the shapes 
+0001cb80: 6279 2061 7265 612e 0a20 2020 2064 656e  by area..    den
+0001cb90: 7369 7479 203a 2069 6e74 206f 7220 666c  sity : int or fl
+0001cba0: 6f61 740a 2020 2020 2020 2020 4465 6e73  oat.        Dens
+0001cbb0: 6974 7920 6f66 2070 6163 6b69 6e67 2e20  ity of packing. 
+0001cbc0: 5661 6c75 6573 2063 6c6f 7365 7220 746f  Values closer to
+0001cbd0: 2031 2070 6163 6b20 7469 6768 7465 7220   1 pack tighter 
+0001cbe0: 6275 7420 7265 7175 6972 6520 6d6f 7265  but require more
+0001cbf0: 0a20 2020 2020 2020 2063 6f6d 7075 7461  .        computa
+0001cc00: 7469 6f6e 2e0a 2020 2020 7072 6563 6973  tion..    precis
+0001cc10: 696f 6e20 3a20 666c 6f61 740a 2020 2020  ion : float.    
+0001cc20: 2020 2020 4465 7369 7265 6420 7072 6563      Desired prec
+0001cc30: 6973 696f 6e20 666f 7220 726f 756e 6469  ision for roundi
+0001cc40: 6e67 2076 6572 7465 7820 636f 6f72 6469  ng vertex coordi
+0001cc50: 6e61 7465 732e 0a20 2020 2076 6572 626f  nates..    verbo
+0001cc60: 7365 203a 2062 6f6f 6c0a 2020 2020 2020  se : bool.      
+0001cc70: 2020 5768 6574 6865 7220 746f 2064 6973    Whether to dis
+0001cc80: 706c 6179 2072 6573 756c 7473 206f 6620  play results of 
+0001cc90: 7061 636b 696e 6720 6174 7465 6d70 7473  packing attempts
+0001cca0: 0a0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001ccb0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2044     -------.    D
+0001ccc0: 5f70 6163 6b65 645f 6c69 7374 203a 2044  _packed_list : D
+0001ccd0: 6576 6963 6520 6f72 206c 6973 7420 6f66  evice or list of
+0001cce0: 2044 6576 6963 6573 0a20 2020 2020 2020   Devices.       
+0001ccf0: 2041 2044 6576 6963 6520 6f72 206c 6973   A Device or lis
+0001cd00: 7420 6f66 2044 6576 6963 6573 2063 6f6e  t of Devices con
+0001cd10: 7461 696e 696e 6720 616c 6c20 7468 6520  taining all the 
+0001cd20: 7061 636b 6564 2072 6563 7461 6e67 756c  packed rectangul
+0001cd30: 6172 0a20 2020 2020 2020 2062 696e 7320  ar.        bins 
+0001cd40: 6765 6e65 7261 7465 642e 0a0a 2020 2020  generated...    
+0001cd50: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+0001cd60: 2020 2020 4966 2061 206d 6178 2d73 697a      If a max-siz
+0001cd70: 6520 6973 2073 7065 6369 6669 6564 2c20  e is specified, 
+0001cd80: 7468 6520 6675 6e63 7469 6f6e 2077 696c  the function wil
+0001cd90: 6c20 6372 6561 7465 2061 7320 6d61 6e79  l create as many
+0001cda0: 2062 696e 7320 6173 0a20 2020 206e 6563   bins as.    nec
+0001cdb0: 6573 7361 7279 2074 6f20 7061 636b 2061  essary to pack a
+0001cdc0: 6c6c 2074 6865 2067 656f 6d65 7472 6965  ll the geometrie
+0001cdd0: 7320 616e 6420 7468 656e 2072 6574 7572  s and then retur
+0001cde0: 6e20 6120 6c69 7374 206f 6620 7468 650a  n a list of the.
+0001cdf0: 2020 2020 6669 6c6c 6564 2d62 696e 2044      filled-bin D
+0001ce00: 6576 6963 6573 2e0a 2020 2020 2222 220a  evices..    """.
+0001ce10: 2020 2020 6966 2064 656e 7369 7479 203c      if density <
+0001ce20: 2031 2e30 313a 0a20 2020 2020 2020 2072   1.01:.        r
+0001ce30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0001ce40: 0a20 2020 2020 2020 2020 2020 2022 5b50  .            "[P
+0001ce50: 4849 444c 5d20 7061 636b 6572 2829 2077  HIDL] packer() w
+0001ce60: 6173 2067 6976 656e 2061 2060 6465 6e73  as given a `dens
+0001ce70: 6974 7960 2061 7267 756d 656e 7420 220a  ity` argument ".
+0001ce80: 2020 2020 2020 2020 2020 2020 2274 6861              "tha
+0001ce90: 7420 6973 2074 6f6f 2073 6d61 6c6c 2e20  t is too small. 
+0001cea0: 2054 6865 2064 656e 7369 7479 2061 7267   The density arg
+0001ceb0: 756d 656e 7420 6d75 7374 2062 6520 220a  ument must be ".
+0001cec0: 2020 2020 2020 2020 2020 2020 223e 3d20              ">= 
+0001ced0: 312e 3031 220a 2020 2020 2020 2020 290a  1.01".        ).
+0001cee0: 0a20 2020 2023 2053 616e 7469 7a65 206d  .    # Santize m
+0001cef0: 6178 5f73 697a 6520 7661 7269 6162 6c65  ax_size variable
+0001cf00: 0a20 2020 206d 6178 5f73 697a 6520 3d20  .    max_size = 
+0001cf10: 5b6e 702e 696e 6620 6966 2076 2069 7320  [np.inf if v is 
+0001cf20: 4e6f 6e65 2065 6c73 6520 7620 666f 7220  None else v for 
+0001cf30: 7620 696e 206d 6178 5f73 697a 655d 0a20  v in max_size]. 
+0001cf40: 2020 206d 6178 5f73 697a 6520 3d20 6e70     max_size = np
+0001cf50: 2e61 7361 7272 6179 286d 6178 5f73 697a  .asarray(max_siz
+0001cf60: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+0001cf70: 7436 3429 2020 2320 496e 2063 6173 6520  t64)  # In case 
+0001cf80: 6974 2773 2069 6e74 6567 6572 730a 2020  it's integers.  
+0001cf90: 2020 6d61 785f 7369 7a65 203d 206d 6178    max_size = max
+0001cfa0: 5f73 697a 6520 2f20 7072 6563 6973 696f  _size / precisio
+0001cfb0: 6e0a 0a20 2020 2023 2043 6f6e 7665 7274  n..    # Convert
+0001cfc0: 2044 6576 6963 6573 2074 6f20 7265 6374   Devices to rect
+0001cfd0: 616e 676c 6573 0a20 2020 2072 6563 745f  angles.    rect_
+0001cfe0: 6469 6374 203d 207b 7d0a 2020 2020 666f  dict = {}.    fo
+0001cff0: 7220 6e2c 2044 2069 6e20 656e 756d 6572  r n, D in enumer
+0001d000: 6174 6528 445f 6c69 7374 293a 0a20 2020  ate(D_list):.   
+0001d010: 2020 2020 2077 2c20 6820 3d20 2844 2e73       w, h = (D.s
+0001d020: 697a 6520 2b20 7370 6163 696e 6729 202f  ize + spacing) /
+0001d030: 2070 7265 6369 7369 6f6e 0a20 2020 2020   precision.     
+0001d040: 2020 2077 2c20 6820 3d20 696e 7428 7729     w, h = int(w)
+0001d050: 2c20 696e 7428 6829 0a20 2020 2020 2020  , int(h).       
+0001d060: 2069 6620 2877 203e 206d 6178 5f73 697a   if (w > max_siz
+0001d070: 655b 305d 2920 6f72 2028 6820 3e20 6d61  e[0]) or (h > ma
+0001d080: 785f 7369 7a65 5b31 5d29 3a0a 2020 2020  x_size[1]):.    
+0001d090: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0001d0a0: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+0001d0b0: 2020 2020 2020 2020 2020 225b 5048 4944            "[PHID
+0001d0c0: 4c5d 2070 6163 6b65 7228 2920 6661 696c  L] packer() fail
+0001d0d0: 6564 2062 6563 6175 7365 206f 6e65 206f  ed because one o
+0001d0e0: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
+0001d0f0: 2020 2020 2274 6865 206f 626a 6563 7473      "the objects
+0001d100: 2069 6e20 6044 5f6c 6973 7460 2069 7320   in `D_list` is 
+0001d110: 6861 7320 616e 2078 206f 7220 220a 2020  has an x or ".  
+0001d120: 2020 2020 2020 2020 2020 2020 2020 2279                "y
+0001d130: 2064 696d 656e 7369 6f6e 206c 6172 6765   dimension large
+0001d140: 7220 7468 616e 2060 6d61 785f 7369 7a65  r than `max_size
+0001d150: 6020 616e 6420 220a 2020 2020 2020 2020  ` and ".        
+0001d160: 2020 2020 2020 2020 2273 6f20 6361 6e6e          "so cann
+0001d170: 6f74 2062 6520 7061 636b 6564 220a 2020  ot be packed".  
+0001d180: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001d190: 2020 2020 7265 6374 5f64 6963 745b 6e5d      rect_dict[n]
+0001d1a0: 203d 2028 772c 2068 290a 0a20 2020 2070   = (w, h)..    p
+0001d1b0: 6163 6b65 645f 6c69 7374 203d 205b 5d0a  acked_list = [].
+0001d1c0: 2020 2020 7768 696c 6520 6c65 6e28 7265      while len(re
+0001d1d0: 6374 5f64 6963 7429 203e 2030 3a0a 2020  ct_dict) > 0:.  
+0001d1e0: 2020 2020 2020 2870 6163 6b65 645f 7265        (packed_re
+0001d1f0: 6374 5f64 6963 742c 2072 6563 745f 6469  ct_dict, rect_di
+0001d200: 6374 2920 3d20 5f70 6163 6b5f 7369 6e67  ct) = _pack_sing
+0001d210: 6c65 5f62 696e 280a 2020 2020 2020 2020  le_bin(.        
+0001d220: 2020 2020 7265 6374 5f64 6963 742c 0a20      rect_dict,. 
+0001d230: 2020 2020 2020 2020 2020 2061 7370 6563             aspec
+0001d240: 745f 7261 7469 6f3d 6173 7065 6374 5f72  t_ratio=aspect_r
+0001d250: 6174 696f 2c0a 2020 2020 2020 2020 2020  atio,.          
+0001d260: 2020 6d61 785f 7369 7a65 3d6d 6178 5f73    max_size=max_s
+0001d270: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+0001d280: 2073 6f72 745f 6279 5f61 7265 613d 736f   sort_by_area=so
+0001d290: 7274 5f62 795f 6172 6561 2c0a 2020 2020  rt_by_area,.    
+0001d2a0: 2020 2020 2020 2020 6465 6e73 6974 793d          density=
+0001d2b0: 6465 6e73 6974 792c 0a20 2020 2020 2020  density,.       
+0001d2c0: 2020 2020 2070 7265 6369 7369 6f6e 3d70       precision=p
+0001d2d0: 7265 6369 7369 6f6e 2c0a 2020 2020 2020  recision,.      
+0001d2e0: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
+0001d2f0: 7262 6f73 652c 0a20 2020 2020 2020 2029  rbose,.        )
+0001d300: 0a20 2020 2020 2020 2070 6163 6b65 645f  .        packed_
+0001d310: 6c69 7374 2e61 7070 656e 6428 7061 636b  list.append(pack
+0001d320: 6564 5f72 6563 745f 6469 6374 290a 0a20  ed_rect_dict).. 
+0001d330: 2020 2044 5f70 6163 6b65 645f 6c69 7374     D_packed_list
+0001d340: 203d 205b 5d0a 2020 2020 666f 7220 7265   = [].    for re
+0001d350: 6374 5f64 6963 7420 696e 2070 6163 6b65  ct_dict in packe
+0001d360: 645f 6c69 7374 3a0a 2020 2020 2020 2020  d_list:.        
+0001d370: 445f 7061 636b 6564 203d 2044 6576 6963  D_packed = Devic
+0001d380: 6528 290a 2020 2020 2020 2020 666f 7220  e().        for 
+0001d390: 6e2c 2072 6563 7420 696e 2072 6563 745f  n, rect in rect_
+0001d3a0: 6469 6374 2e69 7465 6d73 2829 3a0a 2020  dict.items():.  
+0001d3b0: 2020 2020 2020 2020 2020 782c 2079 2c20            x, y, 
+0001d3c0: 772c 2068 203d 2072 6563 740a 2020 2020  w, h = rect.    
+0001d3d0: 2020 2020 2020 2020 7863 656e 7465 7220          xcenter 
+0001d3e0: 3d20 7820 2b20 7720 2f20 3220 2b20 7370  = x + w / 2 + sp
+0001d3f0: 6163 696e 6720 2f20 320a 2020 2020 2020  acing / 2.      
+0001d400: 2020 2020 2020 7963 656e 7465 7220 3d20        ycenter = 
+0001d410: 7920 2b20 6820 2f20 3220 2b20 7370 6163  y + h / 2 + spac
+0001d420: 696e 6720 2f20 320a 2020 2020 2020 2020  ing / 2.        
+0001d430: 2020 2020 6420 3d20 445f 7061 636b 6564      d = D_packed
+0001d440: 2e61 6464 5f72 6566 2844 5f6c 6973 745b  .add_ref(D_list[
+0001d450: 6e5d 290a 2020 2020 2020 2020 2020 2020  n]).            
+0001d460: 642e 6365 6e74 6572 203d 2028 7863 656e  d.center = (xcen
+0001d470: 7465 7220 2a20 7072 6563 6973 696f 6e2c  ter * precision,
+0001d480: 2079 6365 6e74 6572 202a 2070 7265 6369   ycenter * preci
+0001d490: 7369 6f6e 290a 2020 2020 2020 2020 445f  sion).        D_
+0001d4a0: 7061 636b 6564 5f6c 6973 742e 6170 7065  packed_list.appe
+0001d4b0: 6e64 2844 5f70 6163 6b65 6429 0a0a 2020  nd(D_packed)..  
+0001d4c0: 2020 7265 7475 726e 2044 5f70 6163 6b65    return D_packe
+0001d4d0: 645f 6c69 7374 0a0a 0a64 6566 205f 7261  d_list...def _ra
+0001d4e0: 7374 6572 697a 655f 706f 6c79 676f 6e73  sterize_polygons
+0001d4f0: 2870 6f6c 7967 6f6e 732c 2062 6f75 6e64  (polygons, bound
+0001d500: 733d 5b5b 2d31 3030 2c20 2d31 3030 5d2c  s=[[-100, -100],
+0001d510: 205b 3130 302c 2031 3030 5d5d 2c20 6478   [100, 100]], dx
+0001d520: 3d31 2c20 6479 3d31 293a 0a20 2020 2022  =1, dy=1):.    "
+0001d530: 2222 436f 6e76 6572 7473 2070 6f6c 7967  ""Converts polyg
+0001d540: 6f6e 7320 746f 2061 2062 6c61 636b 2f77  ons to a black/w
+0001d550: 6869 7465 2028 312f 3029 206d 6174 7269  hite (1/0) matri
+0001d560: 7822 2222 0a20 2020 2074 7279 3a0a 2020  x""".    try:.  
+0001d570: 2020 2020 2020 6672 6f6d 2073 6b69 6d61        from skima
+0001d580: 6765 2069 6d70 6f72 7420 6472 6177 0a20  ge import draw. 
+0001d590: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0001d5a0: 696f 6e3a 0a20 2020 2020 2020 2072 6169  ion:.        rai
+0001d5b0: 7365 2049 6d70 6f72 7445 7272 6f72 280a  se ImportError(.
+0001d5c0: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+0001d5d0: 2066 696c 6c20 6675 6e63 7469 6f6e 2072   fill function r
+0001d5e0: 6571 7569 7265 7320 7468 6520 6d6f 6475  equires the modu
+0001d5f0: 6c65 2022 0a20 2020 2020 2020 2020 2020  le ".           
+0001d600: 2027 2273 6369 6b69 742d 696d 6167 6522   '"scikit-image"
+0001d610: 2074 6f20 6f70 6572 6174 652e 2020 506c   to operate.  Pl
+0001d620: 6561 7365 2072 6574 7279 2027 0a20 2020  ease retry '.   
+0001d630: 2020 2020 2020 2020 2022 6166 7465 7220           "after 
+0001d640: 696e 7374 616c 6c69 6e67 2073 6369 6b69  installing sciki
+0001d650: 742d 696d 6167 653a 5c6e 5c6e 220a 2020  t-image:\n\n".  
+0001d660: 2020 2020 2020 2020 2020 2224 2070 6970            "$ pip
+0001d670: 2069 6e73 7461 6c6c 202d 2d75 7067 7261   install --upgra
+0001d680: 6465 2073 6369 6b69 742d 696d 6167 6522  de scikit-image"
+0001d690: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001d6a0: 2320 5072 6570 6172 6520 706f 6c79 676f  # Prepare polygo
+0001d6b0: 6e20 6172 7261 7920 6279 2073 6869 6674  n array by shift
+0001d6c0: 696e 6720 616c 6c20 706f 696e 7473 2069  ing all points i
+0001d6d0: 6e74 6f20 7468 6520 6669 7273 7420 7175  nto the first qu
+0001d6e0: 6164 7261 6e74 2061 6e64 0a20 2020 2023  adrant and.    #
+0001d6f0: 2073 6570 6172 6174 696e 6720 706f 696e   separating poin
+0001d700: 7473 2069 6e74 6f20 7820 616e 6420 7920  ts into x and y 
+0001d710: 6c69 7374 730a 2020 2020 7870 7473 203d  lists.    xpts =
+0001d720: 205b 5d0a 2020 2020 7970 7473 203d 205b   [].    ypts = [
+0001d730: 5d0a 2020 2020 666f 7220 7020 696e 2070  ].    for p in p
+0001d740: 6f6c 7967 6f6e 733a 0a20 2020 2020 2020  olygons:.       
+0001d750: 2070 5f61 7272 6179 203d 206e 702e 6173   p_array = np.as
+0001d760: 6172 7261 7928 7029 0a20 2020 2020 2020  array(p).       
+0001d770: 2078 203d 2070 5f61 7272 6179 5b3a 2c20   x = p_array[:, 
+0001d780: 305d 0a20 2020 2020 2020 2079 203d 2070  0].        y = p
+0001d790: 5f61 7272 6179 5b3a 2c20 315d 0a20 2020  _array[:, 1].   
+0001d7a0: 2020 2020 2078 7074 732e 6170 7065 6e64       xpts.append
+0001d7b0: 2828 7820 2d20 626f 756e 6473 5b30 5d5b  ((x - bounds[0][
+0001d7c0: 305d 2920 2f20 6478 202d 2030 2e35 290a  0]) / dx - 0.5).
+0001d7d0: 2020 2020 2020 2020 7970 7473 2e61 7070          ypts.app
+0001d7e0: 656e 6428 2879 202d 2062 6f75 6e64 735b  end((y - bounds[
+0001d7f0: 305d 5b31 5d29 202f 2064 7920 2d20 302e  0][1]) / dy - 0.
+0001d800: 3529 0a0a 2020 2020 2320 496e 6974 6961  5)..    # Initia
+0001d810: 6c69 7a65 2074 6865 2072 6173 7465 7220  lize the raster 
+0001d820: 6d61 7472 6978 2077 6527 6c6c 2062 6520  matrix we'll be 
+0001d830: 7772 6974 696e 6720 746f 0a20 2020 2078  writing to.    x
+0001d840: 7369 7a65 203d 2069 6e74 286e 702e 6365  size = int(np.ce
+0001d850: 696c 2862 6f75 6e64 735b 315d 5b30 5d20  il(bounds[1][0] 
+0001d860: 2d20 626f 756e 6473 5b30 5d5b 305d 2920  - bounds[0][0]) 
+0001d870: 2f20 6478 290a 2020 2020 7973 697a 6520  / dx).    ysize 
+0001d880: 3d20 696e 7428 6e70 2e63 6569 6c28 626f  = int(np.ceil(bo
+0001d890: 756e 6473 5b31 5d5b 315d 202d 2062 6f75  unds[1][1] - bou
+0001d8a0: 6e64 735b 305d 5b31 5d29 202f 2064 7929  nds[0][1]) / dy)
+0001d8b0: 0a20 2020 2072 6173 7465 7220 3d20 6e70  .    raster = np
+0001d8c0: 2e7a 6572 6f73 2828 7973 697a 652c 2078  .zeros((ysize, x
+0001d8d0: 7369 7a65 292c 2064 7479 7065 3d62 6f6f  size), dtype=boo
+0001d8e0: 6c29 0a0a 2020 2020 2320 544f 444f 3a20  l)..    # TODO: 
+0001d8f0: 5265 706c 6163 6520 706f 6c79 676f 6e5f  Replace polygon_
+0001d900: 7065 7269 6d65 7465 7220 7769 7468 2074  perimeter with t
+0001d910: 6865 2073 7570 6572 636f 7665 7220 7665  he supercover ve
+0001d920: 7273 696f 6e0a 2020 2020 666f 7220 6e20  rsion.    for n 
+0001d930: 696e 2072 616e 6765 286c 656e 2878 7074  in range(len(xpt
+0001d940: 7329 293a 0a20 2020 2020 2020 2072 722c  s)):.        rr,
+0001d950: 2063 6320 3d20 6472 6177 2e70 6f6c 7967   cc = draw.polyg
+0001d960: 6f6e 2879 7074 735b 6e5d 2c20 7870 7473  on(ypts[n], xpts
+0001d970: 5b6e 5d2c 2073 6861 7065 3d72 6173 7465  [n], shape=raste
+0001d980: 722e 7368 6170 6529 0a20 2020 2020 2020  r.shape).       
+0001d990: 2072 7270 2c20 6363 7020 3d20 6472 6177   rrp, ccp = draw
+0001d9a0: 2e70 6f6c 7967 6f6e 5f70 6572 696d 6574  .polygon_perimet
+0001d9b0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+0001d9c0: 7970 7473 5b6e 5d2c 2078 7074 735b 6e5d  ypts[n], xpts[n]
+0001d9d0: 2c20 7368 6170 653d 7261 7374 6572 2e73  , shape=raster.s
+0001d9e0: 6861 7065 2c20 636c 6970 3d46 616c 7365  hape, clip=False
+0001d9f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001da00: 2020 2072 6173 7465 725b 7272 2c20 6363     raster[rr, cc
+0001da10: 5d20 3d20 310a 2020 2020 2020 2020 7261  ] = 1.        ra
+0001da20: 7374 6572 5b72 7270 2c20 6363 705d 203d  ster[rrp, ccp] =
+0001da30: 2031 0a0a 2020 2020 7265 7475 726e 2072   1..    return r
+0001da40: 6173 7465 720a 0a0a 6465 6620 5f72 6173  aster...def _ras
+0001da50: 7465 725f 696e 6465 785f 746f 5f63 6f6f  ter_index_to_coo
+0001da60: 7264 7328 692c 206a 2c20 626f 756e 6473  rds(i, j, bounds
+0001da70: 3d5b 5b2d 3130 302c 202d 3130 305d 2c20  =[[-100, -100], 
+0001da80: 5b31 3030 2c20 3130 305d 5d2c 2064 783d  [100, 100]], dx=
+0001da90: 312c 2064 793d 3129 3a0a 2020 2020 2222  1, dy=1):.    ""
+0001daa0: 2243 6f6e 7665 7274 7320 2869 2c6a 2920  "Converts (i,j) 
+0001dab0: 696e 6465 7820 6f66 2072 6173 7465 7220  index of raster 
+0001dac0: 6d61 7472 6978 2074 6f20 7265 616c 2063  matrix to real c
+0001dad0: 6f6f 7264 696e 6174 6573 2222 220a 2020  oordinates""".  
+0001dae0: 2020 7820 3d20 286a 202b 2030 2e35 2920    x = (j + 0.5) 
+0001daf0: 2a20 6478 202b 2062 6f75 6e64 735b 305d  * dx + bounds[0]
+0001db00: 5b30 5d0a 2020 2020 7920 3d20 2869 202b  [0].    y = (i +
+0001db10: 2030 2e35 2920 2a20 6479 202b 2062 6f75   0.5) * dy + bou
+0001db20: 6e64 735b 305d 5b31 5d0a 2020 2020 7265  nds[0][1].    re
+0001db30: 7475 726e 2078 2c20 790a 0a0a 6465 6620  turn x, y...def 
+0001db40: 5f65 7870 616e 645f 7261 7374 6572 2872  _expand_raster(r
+0001db50: 6173 7465 722c 2064 6973 7461 6e63 653d  aster, distance=
+0001db60: 2834 2c20 3229 293a 0a20 2020 2022 2222  (4, 2)):.    """
+0001db70: 4578 7061 6e64 7320 616c 6c20 626c 6163  Expands all blac
+0001db80: 6b20 2831 2920 7069 7865 6c73 2069 6e20  k (1) pixels in 
+0001db90: 7468 6520 7261 7374 6572 2222 220a 2020  the raster""".  
+0001dba0: 2020 7472 793a 0a20 2020 2020 2020 2066    try:.        f
+0001dbb0: 726f 6d20 736b 696d 6167 6520 696d 706f  rom skimage impo
+0001dbc0: 7274 2064 7261 772c 206d 6f72 7068 6f6c  rt draw, morphol
+0001dbd0: 6f67 790a 2020 2020 6578 6365 7074 2045  ogy.    except E
+0001dbe0: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+0001dbf0: 2020 7261 6973 6520 496d 706f 7274 4572    raise ImportEr
+0001dc00: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0001dc10: 2022 5468 6520 6669 6c6c 2066 756e 6374   "The fill funct
+0001dc20: 696f 6e20 7265 7175 6972 6573 2074 6865  ion requires the
+0001dc30: 206d 6f64 756c 6520 220a 2020 2020 2020   module ".      
+0001dc40: 2020 2020 2020 2722 7363 696b 6974 2d69        '"scikit-i
+0001dc50: 6d61 6765 2220 746f 206f 7065 7261 7465  mage" to operate
+0001dc60: 2e20 2050 6c65 6173 6520 7265 7472 7920  .  Please retry 
+0001dc70: 270a 2020 2020 2020 2020 2020 2020 2261  '.            "a
+0001dc80: 6674 6572 2069 6e73 7461 6c6c 696e 6720  fter installing 
+0001dc90: 7363 696b 6974 2d69 6d61 6765 3a5c 6e5c  scikit-image:\n\
+0001dca0: 6e22 0a20 2020 2020 2020 2020 2020 2022  n".            "
+0001dcb0: 2420 7069 7020 696e 7374 616c 6c20 2d2d  $ pip install --
+0001dcc0: 7570 6772 6164 6520 7363 696b 6974 2d69  upgrade scikit-i
+0001dcd0: 6d61 6765 220a 2020 2020 2020 2020 290a  mage".        ).
+0001dce0: 2020 2020 6966 2064 6973 7461 6e63 655b      if distance[
+0001dcf0: 305d 203c 3d20 302e 3520 616e 6420 6469  0] <= 0.5 and di
+0001dd00: 7374 616e 6365 5b31 5d20 3c3d 2030 2e35  stance[1] <= 0.5
+0001dd10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001dd20: 2072 6173 7465 720a 0a20 2020 206e 756d   raster..    num
+0001dd30: 5f70 6978 656c 7320 3d20 6e70 2e61 7272  _pixels = np.arr
+0001dd40: 6179 286e 702e 6365 696c 2864 6973 7461  ay(np.ceil(dista
+0001dd50: 6e63 6529 2c20 6474 7970 653d 696e 7429  nce), dtype=int)
+0001dd60: 0a20 2020 206e 6569 6768 626f 7268 6f6f  .    neighborhoo
+0001dd70: 6420 3d20 6e70 2e7a 6572 6f73 2828 6e75  d = np.zeros((nu
+0001dd80: 6d5f 7069 7865 6c73 5b31 5d20 2a20 3220  m_pixels[1] * 2 
+0001dd90: 2b20 312c 206e 756d 5f70 6978 656c 735b  + 1, num_pixels[
+0001dda0: 305d 202a 2032 202b 2031 292c 2064 7479  0] * 2 + 1), dty
+0001ddb0: 7065 3d62 6f6f 6c29 0a20 2020 2072 722c  pe=bool).    rr,
+0001ddc0: 2063 6320 3d20 6472 6177 2e65 6c6c 6970   cc = draw.ellip
+0001ddd0: 7365 280a 2020 2020 2020 2020 6e75 6d5f  se(.        num_
+0001dde0: 7069 7865 6c73 5b31 5d2c 206e 756d 5f70  pixels[1], num_p
+0001ddf0: 6978 656c 735b 305d 2c20 6469 7374 616e  ixels[0], distan
+0001de00: 6365 5b31 5d20 2b20 302e 352c 2064 6973  ce[1] + 0.5, dis
+0001de10: 7461 6e63 655b 305d 202b 2030 2e35 0a20  tance[0] + 0.5. 
+0001de20: 2020 2029 0a20 2020 206e 6569 6768 626f     ).    neighbo
+0001de30: 7268 6f6f 645b 7272 2c20 6363 5d20 3d20  rhood[rr, cc] = 
+0001de40: 310a 0a20 2020 2072 6574 7572 6e20 6d6f  1..    return mo
+0001de50: 7270 686f 6c6f 6779 2e62 696e 6172 795f  rphology.binary_
+0001de60: 6469 6c61 7469 6f6e 2869 6d61 6765 3d72  dilation(image=r
+0001de70: 6173 7465 722c 2066 6f6f 7470 7269 6e74  aster, footprint
+0001de80: 3d6e 6569 6768 626f 7268 6f6f 6429 0a0a  =neighborhood)..
+0001de90: 0a64 6566 205f 6669 6c6c 5f63 656c 6c5f  .def _fill_cell_
+0001dea0: 7265 6374 616e 676c 6528 0a20 2020 2073  rectangle(.    s
+0001deb0: 697a 653d 2832 302c 2032 3029 2c0a 2020  ize=(20, 20),.  
+0001dec0: 2020 6c61 7965 7273 3d28 302c 2031 2c20    layers=(0, 1, 
+0001ded0: 3329 2c0a 2020 2020 6465 6e73 6974 6965  3),.    densitie
+0001dee0: 733d 2830 2e35 2c20 302e 3235 2c20 302e  s=(0.5, 0.25, 0.
+0001def0: 3729 2c0a 2020 2020 696e 7665 7274 6564  7),.    inverted
+0001df00: 3d28 4661 6c73 652c 2046 616c 7365 2c20  =(False, False, 
+0001df10: 4661 6c73 6529 2c0a 293a 0a20 2020 2022  False),.):.    "
+0001df20: 2222 4372 6561 7465 7320 6120 7369 6e67  ""Creates a sing
+0001df30: 6c65 2044 6576 6963 6520 6f6e 206d 756c  le Device on mul
+0001df40: 7469 706c 6520 6c61 7965 7273 2074 6f20  tiple layers to 
+0001df50: 6265 2075 7365 6420 6173 2066 696c 6c0a  be used as fill.
+0001df60: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001df70: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001df80: 2020 2073 697a 6520 3a20 6172 7261 792d     size : array-
+0001df90: 6c69 6b65 206f 6620 696e 7420 6f72 2066  like of int or f
+0001dfa0: 6c6f 6174 0a20 2020 2020 2020 2078 2c20  loat.        x, 
+0001dfb0: 7920 6469 6d65 6e73 696f 6e73 206f 6620  y dimensions of 
+0001dfc0: 7468 6520 6669 6c6c 2061 7265 6120 666f  the fill area fo
+0001dfd0: 7220 616c 6c20 6c61 7965 7273 2e0a 2020  r all layers..  
+0001dfe0: 2020 6c61 7965 7273 203a 2069 6e74 2c20    layers : int, 
+0001dff0: 6172 7261 792d 6c69 6b65 5b32 5d2c 206f  array-like[2], o
+0001e000: 7220 7365 740a 2020 2020 2020 2020 5370  r set.        Sp
+0001e010: 6563 6966 6963 206c 6179 6572 2873 2920  ecific layer(s) 
+0001e020: 746f 2070 7574 2066 696c 6c20 6365 6c6c  to put fill cell
+0001e030: 2072 6563 7461 6e67 6c65 2067 656f 6d65   rectangle geome
+0001e040: 7472 7920 6f6e 2e0a 2020 2020 6465 6e73  try on..    dens
+0001e050: 6974 6965 7320 3a20 6172 7261 792d 6c69  ities : array-li
+0001e060: 6b65 206f 6620 696e 7420 6f72 2066 6c6f  ke of int or flo
+0001e070: 6174 0a20 2020 2020 2020 2046 696c 6c20  at.        Fill 
+0001e080: 6465 6e73 6974 6965 7320 666f 7220 6561  densities for ea
+0001e090: 6368 206c 6179 6572 2073 7065 6369 6669  ch layer specifi
+0001e0a0: 6564 2069 6e20 6060 6c61 7965 7273 6060  ed in ``layers``
+0001e0b0: 2e20 4d75 7374 2062 6520 7468 6520 7361  . Must be the sa
+0001e0c0: 6d65 0a20 2020 2020 2020 2073 697a 6520  me.        size 
+0001e0d0: 6173 2060 606c 6179 6572 7360 602e 0a20  as ``layers``.. 
+0001e0e0: 2020 2069 6e76 6572 7465 6420 3a20 6172     inverted : ar
+0001e0f0: 7261 792d 6c69 6b65 206f 7220 626f 6f6c  ray-like or bool
+0001e100: 0a20 2020 2020 2020 2049 6620 7472 7565  .        If true
+0001e110: 2c20 696e 7665 7274 7320 7468 6520 6669  , inverts the fi
+0001e120: 6c6c 2061 7265 6120 666f 7220 636f 7272  ll area for corr
+0001e130: 6573 706f 6e64 696e 6720 6c61 7965 722e  esponding layer.
+0001e140: 204d 7573 7420 6265 2074 6865 0a20 2020   Must be the.   
+0001e150: 2020 2020 2073 616d 6520 7369 7a65 2061       same size a
+0001e160: 7320 6060 6c61 7965 7273 6060 2e0a 0a20  s ``layers``... 
+0001e170: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0001e180: 2d2d 2d2d 2d2d 0a20 2020 2044 203a 2044  ------.    D : D
+0001e190: 6576 6963 650a 2020 2020 2020 2020 4120  evice.        A 
+0001e1a0: 4465 7669 6365 2063 6f6e 7461 696e 696e  Device containin
+0001e1b0: 6720 6669 6c6c 6564 2063 656c 6c20 7265  g filled cell re
+0001e1c0: 6374 616e 676c 6573 2e0a 2020 2020 2222  ctangles..    ""
+0001e1d0: 220a 2020 2020 4420 3d20 4465 7669 6365  ".    D = Device
+0001e1e0: 2822 6669 6c6c 6365 6c6c 2229 0a20 2020  ("fillcell").   
+0001e1f0: 2066 6f72 206c 6179 6572 2c20 6465 6e73   for layer, dens
+0001e200: 6974 792c 2069 6e76 2069 6e20 7a69 7028  ity, inv in zip(
+0001e210: 6c61 7965 7273 2c20 6465 6e73 6974 6965  layers, densitie
+0001e220: 732c 2069 6e76 6572 7465 6429 3a0a 2020  s, inverted):.  
+0001e230: 2020 2020 2020 7265 6374 616e 676c 655f        rectangle_
+0001e240: 7369 7a65 203d 206e 702e 6172 7261 7928  size = np.array(
+0001e250: 7369 7a65 2920 2a20 7371 7274 2864 656e  size) * sqrt(den
+0001e260: 7369 7479 290a 2020 2020 2020 2020 2320  sity).        # 
+0001e270: 7220 3d20 442e 6164 645f 7265 6628 7265  r = D.add_ref(re
+0001e280: 6374 616e 676c 6528 7369 7a65 203d 2072  ctangle(size = r
+0001e290: 6563 7461 6e67 6c65 5f73 697a 652c 206c  ectangle_size, l
+0001e2a0: 6179 6572 203d 206c 6179 6572 2929 0a20  ayer = layer)). 
+0001e2b0: 2020 2020 2020 2052 203d 2072 6563 7461         R = recta
+0001e2c0: 6e67 6c65 2873 697a 653d 7265 6374 616e  ngle(size=rectan
+0001e2d0: 676c 655f 7369 7a65 2c20 6c61 7965 723d  gle_size, layer=
+0001e2e0: 6c61 7965 7229 0a20 2020 2020 2020 2052  layer).        R
+0001e2f0: 2e63 656e 7465 7220 3d20 2830 2c20 3029  .center = (0, 0)
+0001e300: 0a20 2020 2020 2020 2069 6620 696e 7620  .        if inv 
+0001e310: 6973 2054 7275 653a 0a20 2020 2020 2020  is True:.       
+0001e320: 2020 2020 2041 203d 2072 6563 7461 6e67       A = rectang
+0001e330: 6c65 2873 697a 653d 7369 7a65 290a 2020  le(size=size).  
+0001e340: 2020 2020 2020 2020 2020 412e 6365 6e74            A.cent
+0001e350: 6572 203d 2028 302c 2030 290a 2020 2020  er = (0, 0).    
+0001e360: 2020 2020 2020 2020 4120 3d20 412e 6765          A = A.ge
+0001e370: 745f 706f 6c79 676f 6e73 2829 0a20 2020  t_polygons().   
+0001e380: 2020 2020 2020 2020 2042 203d 2052 2e67           B = R.g
+0001e390: 6574 5f70 6f6c 7967 6f6e 7328 290a 2020  et_polygons().  
+0001e3a0: 2020 2020 2020 2020 2020 7020 3d20 6764            p = gd
+0001e3b0: 7370 792e 626f 6f6c 6561 6e28 412c 2042  spy.boolean(A, B
+0001e3c0: 2c20 6f70 6572 6174 696f 6e3d 226e 6f74  , operation="not
+0001e3d0: 2229 0a20 2020 2020 2020 2020 2020 2044  ").            D
+0001e3e0: 2e61 6464 5f70 6f6c 7967 6f6e 2870 2c20  .add_polygon(p, 
+0001e3f0: 6c61 7965 723d 6c61 7965 7229 0a20 2020  layer=layer).   
+0001e400: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001e410: 2020 2020 2020 2044 2e61 6464 5f72 6566         D.add_ref
+0001e420: 2852 290a 2020 2020 7265 7475 726e 2044  (R).    return D
+0001e430: 0a0a 0a64 6566 205f 6c6f 6f70 5f6f 7665  ...def _loop_ove
+0001e440: 7228 7661 7229 3a0a 2020 2020 2222 2243  r(var):.    """C
+0001e450: 6865 636b 7320 6966 2061 2076 6172 6961  hecks if a varia
+0001e460: 626c 6520 6973 2069 6e20 7468 6520 666f  ble is in the fo
+0001e470: 726d 206f 6620 616e 2069 7465 7261 626c  rm of an iterabl
+0001e480: 6520 286c 6973 742f 7475 706c 6529 0a20  e (list/tuple). 
+0001e490: 2020 2061 6e64 2069 6620 6e6f 742c 2072     and if not, r
+0001e4a0: 6574 7572 6e73 2069 7420 6173 2061 206c  eturns it as a l
+0001e4b0: 6973 742e 2020 5573 6566 756c 2066 6f72  ist.  Useful for
+0001e4c0: 2061 6c6c 6f77 696e 6720 6172 6775 6d65   allowing argume
+0001e4d0: 6e74 0a20 2020 2069 6e70 7574 7320 746f  nt.    inputs to
+0001e4e0: 2062 6520 6569 7468 6572 206c 6973 7473   be either lists
+0001e4f0: 2028 652e 672e 205b 312c 2033 2c20 345d   (e.g. [1, 3, 4]
+0001e500: 2920 6f72 2073 696e 676c 652d 7661 6c75  ) or single-valu
+0001e510: 6564 2028 652e 672e 2033 292e 0a0a 2020  ed (e.g. 3)...  
+0001e520: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0001e530: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001e540: 7661 7220 3a20 696e 7420 6f72 2066 6c6f  var : int or flo
+0001e550: 6174 206f 7220 6c69 7374 0a20 2020 2020  at or list.     
+0001e560: 2020 2056 6172 6961 626c 6520 746f 2063     Variable to c
+0001e570: 6865 636b 2066 6f72 2069 7465 7261 6269  heck for iterabi
+0001e580: 6c69 7479 2e0a 0a20 2020 2052 6574 7572  lity...    Retur
+0001e590: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0001e5a0: 2020 2076 6172 203a 206c 6973 740a 2020     var : list.  
+0001e5b0: 2020 2020 2020 5661 7269 6162 6c65 2063        Variable c
+0001e5c0: 6f6e 7665 7274 6564 2074 6f20 6c69 7374  onverted to list
+0001e5d0: 2069 6620 7369 6e67 6c65 2d76 616c 7565   if single-value
+0001e5e0: 6420 696e 7075 742e 0a20 2020 2022 2222  d input..    """
+0001e5f0: 0a0a 2020 2020 6966 2068 6173 6174 7472  ..    if hasattr
+0001e600: 2876 6172 2c20 225f 5f69 7465 725f 5f22  (var, "__iter__"
+0001e610: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001e620: 6e20 7661 720a 2020 2020 656c 7365 3a0a  n var.    else:.
+0001e630: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+0001e640: 7661 725d 0a0a 0a64 6566 2066 696c 6c5f  var]...def fill_
+0001e650: 7265 6374 616e 676c 6528 0a20 2020 2044  rectangle(.    D
+0001e660: 2c0a 2020 2020 6669 6c6c 5f73 697a 653d  ,.    fill_size=
+0001e670: 2834 302c 2031 3029 2c0a 2020 2020 6176  (40, 10),.    av
+0001e680: 6f69 645f 6c61 7965 7273 3d22 616c 6c22  oid_layers="all"
+0001e690: 2c0a 2020 2020 696e 636c 7564 655f 6c61  ,.    include_la
+0001e6a0: 7965 7273 3d4e 6f6e 652c 0a20 2020 206d  yers=None,.    m
+0001e6b0: 6172 6769 6e3d 3130 302c 0a20 2020 2066  argin=100,.    f
+0001e6c0: 696c 6c5f 6c61 7965 7273 3d28 302c 2031  ill_layers=(0, 1
+0001e6d0: 2c20 3329 2c0a 2020 2020 6669 6c6c 5f64  , 3),.    fill_d
+0001e6e0: 656e 7369 7469 6573 3d28 302e 352c 2030  ensities=(0.5, 0
+0001e6f0: 2e32 352c 2030 2e37 292c 0a20 2020 2066  .25, 0.7),.    f
+0001e700: 696c 6c5f 696e 7665 7274 6564 3d4e 6f6e  ill_inverted=Non
+0001e710: 652c 0a20 2020 2062 626f 783d 4e6f 6e65  e,.    bbox=None
+0001e720: 2c0a 293a 0a20 2020 2022 2222 4372 6561  ,.):.    """Crea
+0001e730: 7465 7320 6120 7265 6374 616e 6775 6c61  tes a rectangula
+0001e740: 7220 6669 6c6c 2070 6174 7465 726e 2061  r fill pattern a
+0001e750: 6e64 2066 696c 6c73 2061 6c6c 2065 6d70  nd fills all emp
+0001e760: 7479 2061 7265 6173 0a20 2020 2069 6e20  ty areas.    in 
+0001e770: 7468 6520 696e 7075 7420 6465 7669 6365  the input device
+0001e780: 2044 0a0a 2020 2020 5061 7261 6d65 7465   D..    Paramete
+0001e790: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+0001e7a0: 2d0a 2020 2020 4420 3a20 4465 7669 6365  -.    D : Device
+0001e7b0: 0a20 2020 2020 2020 2044 6576 6963 6520  .        Device 
+0001e7c0: 746f 2062 6520 6669 6c6c 6564 0a20 2020  to be filled.   
+0001e7d0: 2066 696c 6c5f 7369 7a65 203a 2061 7272   fill_size : arr
+0001e7e0: 6179 2d6c 696b 655b 325d 0a20 2020 2020  ay-like[2].     
+0001e7f0: 2020 2052 6563 7461 6e67 756c 6172 2073     Rectangular s
+0001e800: 697a 6520 6f66 2074 6865 2066 696c 6c20  ize of the fill 
+0001e810: 656c 656d 656e 740a 2020 2020 6176 6f69  element.    avoi
+0001e820: 645f 6c61 7965 7273 203a 2027 616c 6c27  d_layers : 'all'
+0001e830: 206f 7220 6c69 7374 206f 6620 6c61 7965   or list of laye
+0001e840: 7273 0a20 2020 2020 2020 204c 6179 6572  rs.        Layer
+0001e850: 7320 746f 2062 6520 6176 6f69 6465 6420  s to be avoided 
+0001e860: 286e 6f74 2066 696c 6c65 6429 2069 6e20  (not filled) in 
+0001e870: 440a 2020 2020 696e 636c 7564 655f 6c61  D.    include_la
+0001e880: 7965 7273 203a 0a20 2020 2020 2020 204c  yers :.        L
+0001e890: 6179 6572 7320 746f 2062 6520 696e 636c  ayers to be incl
+0001e8a0: 7564 6564 2028 6669 6c6c 6564 2920 696e  uded (filled) in
+0001e8b0: 2044 2c20 7375 7065 7263 6564 6573 2061   D, supercedes a
+0001e8c0: 766f 6964 5f6c 6179 6572 730a 2020 2020  void_layers.    
+0001e8d0: 6d61 7267 696e 203a 2069 6e74 206f 7220  margin : int or 
+0001e8e0: 666c 6f61 740a 2020 2020 2020 2020 4d61  float.        Ma
+0001e8f0: 7267 696e 2073 7061 6369 6e67 2061 726f  rgin spacing aro
+0001e900: 756e 6420 6176 6f69 6465 6420 6172 6561  und avoided area
+0001e910: 7320 2d2d 2066 696c 6c20 7769 6c6c 206e  s -- fill will n
+0001e920: 6f74 2063 6f6d 6520 7769 7468 696e 0a20  ot come within. 
+0001e930: 2020 2020 2020 2060 6d61 7267 696e 6020         `margin` 
+0001e940: 6f66 2074 6865 2067 656f 6d65 7472 7920  of the geometry 
+0001e950: 696e 2044 0a20 2020 2066 696c 6c5f 6c61  in D.    fill_la
+0001e960: 7965 7273 203a 206c 6973 7420 6f66 206c  yers : list of l
+0001e970: 6179 6572 730a 2020 2020 2020 2020 4465  ayers.        De
+0001e980: 6669 6e65 7320 7468 6520 6669 6c6c 2070  fines the fill p
+0001e990: 6174 7465 726e 206c 6179 6572 730a 2020  attern layers.  
+0001e9a0: 2020 6669 6c6c 5f64 656e 7369 7469 6573    fill_densities
+0001e9b0: 203a 2066 6c6f 6174 2062 6574 7765 656e   : float between
+0001e9c0: 2030 2061 6e64 2031 0a20 2020 2020 2020   0 and 1.       
+0001e9d0: 2044 6566 696e 6573 2074 6865 2066 696c   Defines the fil
+0001e9e0: 6c20 7061 7474 6572 6e20 6465 6e73 6974  l pattern densit
+0001e9f0: 7920 2831 2e30 203d 3d20 6675 6c6c 7920  y (1.0 == fully 
+0001ea00: 6669 6c6c 6564 290a 2020 2020 6669 6c6c  filled).    fill
+0001ea10: 5f69 6e76 6572 7465 6420 3a20 626f 6f6c  _inverted : bool
+0001ea20: 0a20 2020 2020 2020 2049 6e76 6572 7473  .        Inverts
+0001ea30: 2074 6865 2066 696c 6c20 7061 7474 6572   the fill patter
+0001ea40: 6e0a 2020 2020 6262 6f78 203a 2061 7272  n.    bbox : arr
+0001ea50: 6179 2d6c 696b 655b 325d 5b32 5d0a 2020  ay-like[2][2].  
+0001ea60: 2020 2020 2020 4c69 6d69 7420 7468 6520        Limit the 
+0001ea70: 6669 6c6c 2070 6174 7465 726e 2074 6f20  fill pattern to 
+0001ea80: 7468 6520 6172 6561 2064 6566 696e 6564  the area defined
+0001ea90: 2062 7920 7468 6973 2062 6f75 6e64 696e   by this boundin
+0001eaa0: 6720 626f 780a 0a20 2020 2052 6574 7572  g box..    Retur
+0001eab0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0001eac0: 2020 2046 203a 2044 6576 6963 650a 0a20     F : Device.. 
+0001ead0: 2020 2022 2222 0a20 2020 2023 2043 7265     """.    # Cre
+0001eae0: 6174 6520 7468 6520 6669 6c6c 2063 656c  ate the fill cel
+0001eaf0: 6c2e 0a20 2020 2023 2049 6620 6669 6c6c  l..    # If fill
+0001eb00: 5f69 6e76 6572 7465 6420 6973 206e 6f74  _inverted is not
+0001eb10: 2073 7065 6369 6669 6564 2c20 6173 7375   specified, assu
+0001eb20: 6d65 2061 6c6c 2046 616c 7365 0a20 2020  me all False.   
+0001eb30: 2066 696c 6c5f 6c61 7965 7273 203d 205f   fill_layers = _
+0001eb40: 6c6f 6f70 5f6f 7665 7228 6669 6c6c 5f6c  loop_over(fill_l
+0001eb50: 6179 6572 7329 0a20 2020 2066 696c 6c5f  ayers).    fill_
+0001eb60: 6465 6e73 6974 6965 7320 3d20 5f6c 6f6f  densities = _loo
+0001eb70: 705f 6f76 6572 2866 696c 6c5f 6465 6e73  p_over(fill_dens
+0001eb80: 6974 6965 7329 0a20 2020 2069 6620 6669  ities).    if fi
+0001eb90: 6c6c 5f69 6e76 6572 7465 6420 6973 204e  ll_inverted is N
+0001eba0: 6f6e 653a 0a20 2020 2020 2020 2066 696c  one:.        fil
+0001ebb0: 6c5f 696e 7665 7274 6564 203d 205b 4661  l_inverted = [Fa
+0001ebc0: 6c73 655d 202a 206c 656e 2866 696c 6c5f  lse] * len(fill_
+0001ebd0: 6c61 7965 7273 290a 2020 2020 6669 6c6c  layers).    fill
+0001ebe0: 5f69 6e76 6572 7465 6420 3d20 5f6c 6f6f  _inverted = _loo
+0001ebf0: 705f 6f76 6572 2866 696c 6c5f 696e 7665  p_over(fill_inve
+0001ec00: 7274 6564 290a 2020 2020 6966 206c 656e  rted).    if len
+0001ec10: 2866 696c 6c5f 6c61 7965 7273 2920 213d  (fill_layers) !=
+0001ec20: 206c 656e 2866 696c 6c5f 6465 6e73 6974   len(fill_densit
+0001ec30: 6965 7329 3a0a 2020 2020 2020 2020 7261  ies):.        ra
+0001ec40: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+0001ec50: 2020 2020 2020 2020 2020 2020 225b 5048              "[PH
+0001ec60: 4944 4c5d 2070 6869 646c 2e67 656f 6d65  IDL] phidl.geome
+0001ec70: 7472 792e 6669 6c6c 5f72 6563 7461 6e67  try.fill_rectang
+0001ec80: 6c65 2829 2022 0a20 2020 2020 2020 2020  le() ".         
+0001ec90: 2020 2022 6066 696c 6c5f 6c61 7965 7273     "`fill_layers
+0001eca0: 6020 616e 6420 6066 696c 6c5f 6465 6e73  ` and `fill_dens
+0001ecb0: 6974 6965 7360 2070 6172 616d 6574 6572  ities` parameter
+0001ecc0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+0001ecd0: 226d 7573 7420 6265 206c 6973 7473 206f  "must be lists o
+0001ece0: 6620 7468 6520 7361 6d65 206c 656e 6774  f the same lengt
+0001ecf0: 6822 0a20 2020 2020 2020 2029 0a20 2020  h".        ).   
+0001ed00: 2069 6620 6c65 6e28 6669 6c6c 5f6c 6179   if len(fill_lay
+0001ed10: 6572 7329 2021 3d20 6c65 6e28 6669 6c6c  ers) != len(fill
+0001ed20: 5f69 6e76 6572 7465 6429 3a0a 2020 2020  _inverted):.    
+0001ed30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001ed40: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0001ed50: 2020 225b 5048 4944 4c5d 2070 6869 646c    "[PHIDL] phidl
+0001ed60: 2e67 656f 6d65 7472 792e 6669 6c6c 5f72  .geometry.fill_r
+0001ed70: 6563 7461 6e67 6c65 2829 2022 0a20 2020  ectangle() ".   
+0001ed80: 2020 2020 2020 2020 2022 6066 696c 6c5f           "`fill_
+0001ed90: 6c61 7965 7273 6020 616e 6420 6066 696c  layers` and `fil
+0001eda0: 6c5f 696e 7665 7274 6564 6020 7061 7261  l_inverted` para
+0001edb0: 6d65 7465 7273 206d 7573 7420 220a 2020  meters must ".  
+0001edc0: 2020 2020 2020 2020 2020 2262 6520 6c69            "be li
+0001edd0: 7374 7320 6f66 2074 6865 2073 616d 6520  sts of the same 
+0001ede0: 6c65 6e67 7468 220a 2020 2020 2020 2020  length".        
+0001edf0: 290a 0a20 2020 2066 696c 6c5f 6365 6c6c  )..    fill_cell
+0001ee00: 203d 205f 6669 6c6c 5f63 656c 6c5f 7265   = _fill_cell_re
+0001ee10: 6374 616e 676c 6528 0a20 2020 2020 2020  ctangle(.       
+0001ee20: 2073 697a 653d 6669 6c6c 5f73 697a 652c   size=fill_size,
+0001ee30: 0a20 2020 2020 2020 206c 6179 6572 733d  .        layers=
+0001ee40: 6669 6c6c 5f6c 6179 6572 732c 0a20 2020  fill_layers,.   
+0001ee50: 2020 2020 2064 656e 7369 7469 6573 3d66       densities=f
+0001ee60: 696c 6c5f 6465 6e73 6974 6965 732c 0a20  ill_densities,. 
+0001ee70: 2020 2020 2020 2069 6e76 6572 7465 643d         inverted=
+0001ee80: 6669 6c6c 5f69 6e76 6572 7465 642c 0a20  fill_inverted,. 
+0001ee90: 2020 2029 0a20 2020 2046 203d 2044 6576     ).    F = Dev
+0001eea0: 6963 6528 6e61 6d65 3d22 6669 6c6c 5f70  ice(name="fill_p
+0001eeb0: 6174 7465 726e 2229 0a0a 2020 2020 6966  attern")..    if
+0001eec0: 2061 766f 6964 5f6c 6179 6572 7320 3d3d   avoid_layers ==
+0001eed0: 2022 616c 6c22 3a0a 2020 2020 2020 2020   "all":.        
+0001eee0: 6578 636c 7564 655f 706f 6c79 7320 3d20  exclude_polys = 
+0001eef0: 442e 6765 745f 706f 6c79 676f 6e73 2862  D.get_polygons(b
+0001ef00: 795f 7370 6563 3d46 616c 7365 2c20 6465  y_spec=False, de
+0001ef10: 7074 683d 4e6f 6e65 290a 2020 2020 656c  pth=None).    el
+0001ef20: 7365 3a0a 2020 2020 2020 2020 6176 6f69  se:.        avoi
+0001ef30: 645f 6c61 7965 7273 203d 205b 5f70 6172  d_layers = [_par
+0001ef40: 7365 5f6c 6179 6572 286c 2920 666f 7220  se_layer(l) for 
+0001ef50: 6c20 696e 205f 6c6f 6f70 5f6f 7665 7228  l in _loop_over(
+0001ef60: 6176 6f69 645f 6c61 7965 7273 295d 0a20  avoid_layers)]. 
+0001ef70: 2020 2020 2020 2065 7863 6c75 6465 5f70         exclude_p
+0001ef80: 6f6c 7973 203d 2044 2e67 6574 5f70 6f6c  olys = D.get_pol
+0001ef90: 7967 6f6e 7328 6279 5f73 7065 633d 5472  ygons(by_spec=Tr
+0001efa0: 7565 2c20 6465 7074 683d 4e6f 6e65 290a  ue, depth=None).
+0001efb0: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
+0001efc0: 706f 6c79 7320 3d20 7b0a 2020 2020 2020  polys = {.      
+0001efd0: 2020 2020 2020 6b65 793a 2065 7863 6c75        key: exclu
+0001efe0: 6465 5f70 6f6c 7973 5b6b 6579 5d20 666f  de_polys[key] fo
+0001eff0: 7220 6b65 7920 696e 2065 7863 6c75 6465  r key in exclude
+0001f000: 5f70 6f6c 7973 2069 6620 6b65 7920 696e  _polys if key in
+0001f010: 2061 766f 6964 5f6c 6179 6572 730a 2020   avoid_layers.  
+0001f020: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001f030: 6578 636c 7564 655f 706f 6c79 7320 3d20  exclude_polys = 
+0001f040: 6974 6572 746f 6f6c 732e 6368 6169 6e2e  itertools.chain.
+0001f050: 6672 6f6d 5f69 7465 7261 626c 6528 6578  from_iterable(ex
+0001f060: 636c 7564 655f 706f 6c79 732e 7661 6c75  clude_polys.valu
+0001f070: 6573 2829 290a 0a20 2020 2069 6620 696e  es())..    if in
+0001f080: 636c 7564 655f 6c61 7965 7273 2069 7320  clude_layers is 
+0001f090: 4e6f 6e65 3a0a 2020 2020 2020 2020 696e  None:.        in
+0001f0a0: 636c 7564 655f 706f 6c79 7320 3d20 5b5d  clude_polys = []
+0001f0b0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0001f0c0: 2020 2069 6e63 6c75 6465 5f6c 6179 6572     include_layer
+0001f0d0: 7320 3d20 5b5f 7061 7273 655f 6c61 7965  s = [_parse_laye
+0001f0e0: 7228 6c29 2066 6f72 206c 2069 6e20 5f6c  r(l) for l in _l
+0001f0f0: 6f6f 705f 6f76 6572 2869 6e63 6c75 6465  oop_over(include
+0001f100: 5f6c 6179 6572 7329 5d0a 2020 2020 2020  _layers)].      
+0001f110: 2020 696e 636c 7564 655f 706f 6c79 7320    include_polys 
+0001f120: 3d20 442e 6765 745f 706f 6c79 676f 6e73  = D.get_polygons
+0001f130: 2862 795f 7370 6563 3d54 7275 652c 2064  (by_spec=True, d
+0001f140: 6570 7468 3d4e 6f6e 6529 0a20 2020 2020  epth=None).     
+0001f150: 2020 2069 6e63 6c75 6465 5f70 6f6c 7973     include_polys
+0001f160: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001f170: 206b 6579 3a20 696e 636c 7564 655f 706f   key: include_po
+0001f180: 6c79 735b 6b65 795d 2066 6f72 206b 6579  lys[key] for key
+0001f190: 2069 6e20 696e 636c 7564 655f 706f 6c79   in include_poly
+0001f1a0: 7320 6966 206b 6579 2069 6e20 696e 636c  s if key in incl
+0001f1b0: 7564 655f 6c61 7965 7273 0a20 2020 2020  ude_layers.     
+0001f1c0: 2020 207d 0a20 2020 2020 2020 2069 6e63     }.        inc
+0001f1d0: 6c75 6465 5f70 6f6c 7973 203d 2069 7465  lude_polys = ite
+0001f1e0: 7274 6f6f 6c73 2e63 6861 696e 2e66 726f  rtools.chain.fro
+0001f1f0: 6d5f 6974 6572 6162 6c65 2869 6e63 6c75  m_iterable(inclu
+0001f200: 6465 5f70 6f6c 7973 2e76 616c 7565 7328  de_polys.values(
+0001f210: 2929 0a0a 2020 2020 6966 2062 626f 7820  ))..    if bbox 
+0001f220: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0001f230: 2062 626f 7820 3d20 442e 6262 6f78 0a0a   bbox = D.bbox..
+0001f240: 2020 2020 7261 7374 6572 203d 205f 7261      raster = _ra
+0001f250: 7374 6572 697a 655f 706f 6c79 676f 6e73  sterize_polygons
+0001f260: 280a 2020 2020 2020 2020 706f 6c79 676f  (.        polygo
+0001f270: 6e73 3d65 7863 6c75 6465 5f70 6f6c 7973  ns=exclude_polys
+0001f280: 2c20 626f 756e 6473 3d62 626f 782c 2064  , bounds=bbox, d
+0001f290: 783d 6669 6c6c 5f73 697a 655b 305d 2c20  x=fill_size[0], 
+0001f2a0: 6479 3d66 696c 6c5f 7369 7a65 5b31 5d0a  dy=fill_size[1].
+0001f2b0: 2020 2020 290a 2020 2020 7261 7374 6572      ).    raster
+0001f2c0: 203d 2072 6173 7465 7220 2620 7e5f 7261   = raster & ~_ra
+0001f2d0: 7374 6572 697a 655f 706f 6c79 676f 6e73  sterize_polygons
+0001f2e0: 280a 2020 2020 2020 2020 706f 6c79 676f  (.        polygo
+0001f2f0: 6e73 3d69 6e63 6c75 6465 5f70 6f6c 7973  ns=include_polys
+0001f300: 2c20 626f 756e 6473 3d62 626f 782c 2064  , bounds=bbox, d
+0001f310: 783d 6669 6c6c 5f73 697a 655b 305d 2c20  x=fill_size[0], 
+0001f320: 6479 3d66 696c 6c5f 7369 7a65 5b31 5d0a  dy=fill_size[1].
+0001f330: 2020 2020 290a 2020 2020 7261 7374 6572      ).    raster
+0001f340: 203d 205f 6578 7061 6e64 5f72 6173 7465   = _expand_raste
+0001f350: 7228 7261 7374 6572 2c20 6469 7374 616e  r(raster, distan
+0001f360: 6365 3d6d 6172 6769 6e20 2f20 6e70 2e61  ce=margin / np.a
+0001f370: 7272 6179 2866 696c 6c5f 7369 7a65 2929  rray(fill_size))
+0001f380: 0a0a 2020 2020 666f 7220 6920 696e 2072  ..    for i in r
+0001f390: 616e 6765 286e 702e 7369 7a65 2872 6173  ange(np.size(ras
+0001f3a0: 7465 722c 2030 2929 3a0a 2020 2020 2020  ter, 0)):.      
+0001f3b0: 2020 7375 625f 7261 7374 6572 7320 3d20    sub_rasters = 
+0001f3c0: 5b6c 6973 7428 6729 2066 6f72 206b 2c20  [list(g) for k, 
+0001f3d0: 6720 696e 2069 7465 7274 6f6f 6c73 2e67  g in itertools.g
+0001f3e0: 726f 7570 6279 2872 6173 7465 725b 695d  roupby(raster[i]
+0001f3f0: 295d 0a20 2020 2020 2020 206a 203d 2030  )].        j = 0
+0001f400: 0a20 2020 2020 2020 2066 6f72 2073 2069  .        for s i
+0001f410: 6e20 7375 625f 7261 7374 6572 733a 0a20  n sub_rasters:. 
+0001f420: 2020 2020 2020 2020 2020 2069 6620 735b             if s[
+0001f430: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
+0001f440: 2020 2020 2020 2020 2078 2c20 7920 3d20           x, y = 
+0001f450: 5f72 6173 7465 725f 696e 6465 785f 746f  _raster_index_to
+0001f460: 5f63 6f6f 7264 7328 692c 206a 2c20 6262  _coords(i, j, bb
+0001f470: 6f78 2c20 6669 6c6c 5f73 697a 655b 305d  ox, fill_size[0]
+0001f480: 2c20 6669 6c6c 5f73 697a 655b 315d 290a  , fill_size[1]).
+0001f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4a0: 2320 462e 6164 6428 6764 7370 792e 4365  # F.add(gdspy.Ce
+0001f4b0: 6c6c 4172 7261 7928 7265 665f 6365 6c6c  llArray(ref_cell
+0001f4c0: 203d 2066 696c 6c5f 6365 6c6c 2c0a 2020   = fill_cell,.  
+0001f4d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4f0: 2020 2020 2020 636f 6c75 6d6e 7320 3d20        columns = 
+0001f500: 6c65 6e28 7329 2c20 726f 7773 203d 2031  len(s), rows = 1
+0001f510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f520: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001f530: 2020 2020 2020 2020 2020 7370 6163 696e            spacin
+0001f540: 6720 3d20 6669 6c6c 5f73 697a 652c 2029  g = fill_size, )
+0001f550: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001f560: 2020 6120 3d20 462e 6164 645f 6172 7261    a = F.add_arra
+0001f570: 7928 6669 6c6c 5f63 656c 6c2c 2063 6f6c  y(fill_cell, col
+0001f580: 756d 6e73 3d6c 656e 2873 292c 2072 6f77  umns=len(s), row
+0001f590: 733d 312c 2073 7061 6369 6e67 3d66 696c  s=1, spacing=fil
+0001f5a0: 6c5f 7369 7a65 290a 2020 2020 2020 2020  l_size).        
+0001f5b0: 2020 2020 2020 2020 612e 6d6f 7665 2828          a.move((
+0001f5c0: 782c 2079 2929 0a20 2020 2020 2020 2020  x, y)).         
+0001f5d0: 2020 206a 202b 3d20 6c65 6e28 7329 0a0a     j += len(s)..
+0001f5e0: 2020 2020 7265 7475 726e 2046 0a0a 0a23      return F...#
+0001f5f0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
 0001f600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001f610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f620: 3d0a 0a0a 6465 6620 706f 6c79 676f 6e5f  =...def polygon_
-0001f630: 706f 7274 7328 7870 7473 3d5b 2d31 2c20  ports(xpts=[-1, 
-0001f640: 2d31 2c20 302c 2030 5d2c 2079 7074 733d  -1, 0, 0], ypts=
-0001f650: 5b30 2c20 312c 2031 2c20 305d 2c20 6c61  [0, 1, 1, 0], la
-0001f660: 7965 723d 3029 3a0a 2020 2020 2222 2243  yer=0):.    """C
-0001f670: 7265 6174 6573 2061 2070 6f6c 7967 6f6e  reates a polygon
-0001f680: 2077 6974 6820 706f 7274 7320 6f6e 2061   with ports on a
-0001f690: 6c6c 2065 6467 6573 2e0a 0a20 2020 2050  ll edges...    P
-0001f6a0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001f6b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2078 7074  --------.    xpt
-0001f6c0: 7320 3a20 6172 7261 792d 6c69 6b65 0a20  s : array-like. 
-0001f6d0: 2020 2020 2020 2078 2d63 6f6f 7264 696e         x-coordin
-0001f6e0: 6174 6520 7661 6c75 6573 206f 6620 7468  ate values of th
-0001f6f0: 6520 706f 6c79 676f 6e20 7665 7274 6963  e polygon vertic
-0001f700: 6573 2e0a 2020 2020 7970 7473 203a 2061  es..    ypts : a
-0001f710: 7272 6179 2d6c 696b 650a 2020 2020 2020  rray-like.      
-0001f720: 2020 792d 636f 6f72 6469 6e61 7465 2076    y-coordinate v
-0001f730: 616c 7565 7320 6f66 2074 6865 2070 6f6c  alues of the pol
-0001f740: 7967 6f6e 2076 6572 7469 6365 732e 0a20  ygon vertices.. 
-0001f750: 2020 206c 6179 6572 203a 2069 6e74 2c20     layer : int, 
-0001f760: 6172 7261 792d 6c69 6b65 5b32 5d2c 206f  array-like[2], o
-0001f770: 7220 7365 740a 2020 2020 2020 2020 5370  r set.        Sp
-0001f780: 6563 6966 6963 206c 6179 6572 2873 2920  ecific layer(s) 
-0001f790: 746f 2070 7574 2070 6f6c 7967 6f6e 2067  to put polygon g
-0001f7a0: 656f 6d65 7472 7920 6f6e 2e0a 0a20 2020  eometry on...   
-0001f7b0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-0001f7c0: 2d2d 2d2d 0a20 2020 2050 203a 2044 6576  ----.    P : Dev
-0001f7d0: 6963 650a 2020 2020 2020 2020 4120 4465  ice.        A De
-0001f7e0: 7669 6365 2063 6f6e 7461 696e 696e 6720  vice containing 
-0001f7f0: 6120 706f 6c79 676f 6e20 7769 7468 2070  a polygon with p
-0001f800: 6f72 7473 206f 6e20 616c 6c20 6564 6765  orts on all edge
-0001f810: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
-0001f820: 2072 6574 7572 6e73 2061 2070 6f6c 7967   returns a polyg
-0001f830: 6f6e 2077 6974 6820 706f 7274 7320 6f6e  on with ports on
-0001f840: 2061 6c6c 2065 6467 6573 0a20 2020 2050   all edges.    P
-0001f850: 203d 2044 6576 6963 6528 2270 6f6c 7967   = Device("polyg
-0001f860: 6f6e 2229 0a20 2020 2050 2e61 6464 5f70  on").    P.add_p
-0001f870: 6f6c 7967 6f6e 285b 7870 7473 2c20 7970  olygon([xpts, yp
-0001f880: 7473 5d2c 206c 6179 6572 3d6c 6179 6572  ts], layer=layer
-0001f890: 290a 2020 2020 6e20 3d20 6c65 6e28 7870  ).    n = len(xp
-0001f8a0: 7473 290a 2020 2020 7870 7473 2e61 7070  ts).    xpts.app
-0001f8b0: 656e 6428 7870 7473 5b30 5d29 0a20 2020  end(xpts[0]).   
-0001f8c0: 2079 7074 732e 6170 7065 6e64 2879 7074   ypts.append(ypt
-0001f8d0: 735b 305d 290a 2020 2020 2320 6465 7465  s[0]).    # dete
-0001f8e0: 726d 696e 6520 6966 2063 6c6f 636b 7769  rmine if clockwi
-0001f8f0: 7365 206f 7220 636f 756e 7465 7263 6c6f  se or counterclo
-0001f900: 636b 7769 7365 0a20 2020 2063 6320 3d20  ckwise.    cc = 
-0001f910: 300a 2020 2020 666f 7220 6920 696e 2072  0.    for i in r
-0001f920: 616e 6765 2830 2c20 6e29 3a0a 2020 2020  ange(0, n):.    
-0001f930: 2020 2020 6363 202b 3d20 2878 7074 735b      cc += (xpts[
-0001f940: 6920 2b20 315d 202d 2078 7074 735b 695d  i + 1] - xpts[i]
-0001f950: 2920 2a20 2879 7074 735b 6920 2b20 315d  ) * (ypts[i + 1]
-0001f960: 202b 2079 7074 735b 695d 290a 0a20 2020   + ypts[i])..   
-0001f970: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0001f980: 302c 206e 293a 0a20 2020 2020 2020 206d  0, n):.        m
-0001f990: 6964 706f 696e 745f 6e20 3d20 5b28 7870  idpoint_n = [(xp
-0001f9a0: 7473 5b69 202b 2031 5d20 2b20 7870 7473  ts[i + 1] + xpts
-0001f9b0: 5b69 5d29 202f 2032 2c20 2879 7074 735b  [i]) / 2, (ypts[
-0001f9c0: 6920 2b20 315d 202b 2079 7074 735b 695d  i + 1] + ypts[i]
-0001f9d0: 2920 2f20 325d 0a20 2020 2020 2020 206f  ) / 2].        o
-0001f9e0: 7269 656e 7461 7469 6f6e 5f6e 203d 2028  rientation_n = (
-0001f9f0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-0001fa00: 6172 6374 616e 3228 0a20 2020 2020 2020  arctan2(.       
-0001fa10: 2020 2020 2020 2020 206e 702e 7369 676e           np.sign
-0001fa20: 2863 6329 202a 2028 7870 7473 5b69 202b  (cc) * (xpts[i +
-0001fa30: 2031 5d20 2d20 7870 7473 5b69 5d29 2c0a   1] - xpts[i]),.
-0001fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa50: 6e70 2e73 6967 6e28 6363 2920 2a20 2879  np.sign(cc) * (y
-0001fa60: 7074 735b 695d 202d 2079 7074 735b 6920  pts[i] - ypts[i 
-0001fa70: 2b20 315d 292c 0a20 2020 2020 2020 2020  + 1]),.         
-0001fa80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001fa90: 202a 2031 3830 0a20 2020 2020 2020 2020   * 180.         
-0001faa0: 2020 202f 2070 690a 2020 2020 2020 2020     / pi.        
-0001fab0: 290a 2020 2020 2020 2020 7769 6474 685f  ).        width_
-0001fac0: 6e20 3d20 6e70 2e61 6273 280a 2020 2020  n = np.abs(.    
-0001fad0: 2020 2020 2020 2020 7371 7274 2828 7870          sqrt((xp
-0001fae0: 7473 5b69 202b 2031 5d20 2d20 7870 7473  ts[i + 1] - xpts
-0001faf0: 5b69 5d29 202a 2a20 3220 2b20 2879 7074  [i]) ** 2 + (ypt
-0001fb00: 735b 6920 2b20 315d 202d 2079 7074 735b  s[i + 1] - ypts[
-0001fb10: 695d 2920 2a2a 2032 290a 2020 2020 2020  i]) ** 2).      
-0001fb20: 2020 290a 2020 2020 2020 2020 502e 6164    ).        P.ad
-0001fb30: 645f 706f 7274 280a 2020 2020 2020 2020  d_port(.        
-0001fb40: 2020 2020 6e61 6d65 3d73 7472 2869 202b      name=str(i +
-0001fb50: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
-0001fb60: 206d 6964 706f 696e 743d 6d69 6470 6f69   midpoint=midpoi
-0001fb70: 6e74 5f6e 2c0a 2020 2020 2020 2020 2020  nt_n,.          
-0001fb80: 2020 7769 6474 683d 7769 6474 685f 6e2c    width=width_n,
-0001fb90: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
-0001fba0: 656e 7461 7469 6f6e 3d6f 7269 656e 7461  entation=orienta
-0001fbb0: 7469 6f6e 5f6e 2c0a 2020 2020 2020 2020  tion_n,.        
-0001fbc0: 290a 0a20 2020 2072 6574 7572 6e20 500a  )..    return P.
-0001fbd0: 0a0a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..# ============
-0001fbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fbf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fc00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fc10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fc20: 3d3d 0a23 2045 7861 6d70 6c65 2063 6f64  ==.# Example cod
-0001fc30: 650a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e.# ============
-0001fc40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fc50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+0001f640: 230a 2320 5068 6f74 6f6e 6963 730a 230a  #.# Photonics.#.
+0001f650: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+0001f660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f6a0: 0a0a 0a64 6566 2070 6f6c 7967 6f6e 5f70  ...def polygon_p
+0001f6b0: 6f72 7473 2878 7074 733d 5b2d 312c 202d  orts(xpts=[-1, -
+0001f6c0: 312c 2030 2c20 305d 2c20 7970 7473 3d5b  1, 0, 0], ypts=[
+0001f6d0: 302c 2031 2c20 312c 2030 5d2c 206c 6179  0, 1, 1, 0], lay
+0001f6e0: 6572 3d30 293a 0a20 2020 2022 2222 4372  er=0):.    """Cr
+0001f6f0: 6561 7465 7320 6120 706f 6c79 676f 6e20  eates a polygon 
+0001f700: 7769 7468 2070 6f72 7473 206f 6e20 616c  with ports on al
+0001f710: 6c20 6564 6765 732e 0a0a 2020 2020 5061  l edges...    Pa
+0001f720: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+0001f730: 2d2d 2d2d 2d2d 2d0a 2020 2020 7870 7473  -------.    xpts
+0001f740: 203a 2061 7272 6179 2d6c 696b 650a 2020   : array-like.  
+0001f750: 2020 2020 2020 782d 636f 6f72 6469 6e61        x-coordina
+0001f760: 7465 2076 616c 7565 7320 6f66 2074 6865  te values of the
+0001f770: 2070 6f6c 7967 6f6e 2076 6572 7469 6365   polygon vertice
+0001f780: 732e 0a20 2020 2079 7074 7320 3a20 6172  s..    ypts : ar
+0001f790: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
+0001f7a0: 2079 2d63 6f6f 7264 696e 6174 6520 7661   y-coordinate va
+0001f7b0: 6c75 6573 206f 6620 7468 6520 706f 6c79  lues of the poly
+0001f7c0: 676f 6e20 7665 7274 6963 6573 2e0a 2020  gon vertices..  
+0001f7d0: 2020 6c61 7965 7220 3a20 696e 742c 2061    layer : int, a
+0001f7e0: 7272 6179 2d6c 696b 655b 325d 2c20 6f72  rray-like[2], or
+0001f7f0: 2073 6574 0a20 2020 2020 2020 2053 7065   set.        Spe
+0001f800: 6369 6669 6320 6c61 7965 7228 7329 2074  cific layer(s) t
+0001f810: 6f20 7075 7420 706f 6c79 676f 6e20 6765  o put polygon ge
+0001f820: 6f6d 6574 7279 206f 6e2e 0a0a 2020 2020  ometry on...    
+0001f830: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0001f840: 2d2d 2d0a 2020 2020 5020 3a20 4465 7669  ---.    P : Devi
+0001f850: 6365 0a20 2020 2020 2020 2041 2044 6576  ce.        A Dev
+0001f860: 6963 6520 636f 6e74 6169 6e69 6e67 2061  ice containing a
+0001f870: 2070 6f6c 7967 6f6e 2077 6974 6820 706f   polygon with po
+0001f880: 7274 7320 6f6e 2061 6c6c 2065 6467 6573  rts on all edges
+0001f890: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
+0001f8a0: 7265 7475 726e 7320 6120 706f 6c79 676f  returns a polygo
+0001f8b0: 6e20 7769 7468 2070 6f72 7473 206f 6e20  n with ports on 
+0001f8c0: 616c 6c20 6564 6765 730a 2020 2020 5020  all edges.    P 
+0001f8d0: 3d20 4465 7669 6365 2822 706f 6c79 676f  = Device("polygo
+0001f8e0: 6e22 290a 2020 2020 502e 6164 645f 706f  n").    P.add_po
+0001f8f0: 6c79 676f 6e28 5b78 7074 732c 2079 7074  lygon([xpts, ypt
+0001f900: 735d 2c20 6c61 7965 723d 6c61 7965 7229  s], layer=layer)
+0001f910: 0a20 2020 206e 203d 206c 656e 2878 7074  .    n = len(xpt
+0001f920: 7329 0a20 2020 2078 7074 732e 6170 7065  s).    xpts.appe
+0001f930: 6e64 2878 7074 735b 305d 290a 2020 2020  nd(xpts[0]).    
+0001f940: 7970 7473 2e61 7070 656e 6428 7970 7473  ypts.append(ypts
+0001f950: 5b30 5d29 0a20 2020 2023 2064 6574 6572  [0]).    # deter
+0001f960: 6d69 6e65 2069 6620 636c 6f63 6b77 6973  mine if clockwis
+0001f970: 6520 6f72 2063 6f75 6e74 6572 636c 6f63  e or countercloc
+0001f980: 6b77 6973 650a 2020 2020 6363 203d 2030  kwise.    cc = 0
+0001f990: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+0001f9a0: 6e67 6528 302c 206e 293a 0a20 2020 2020  nge(0, n):.     
+0001f9b0: 2020 2063 6320 2b3d 2028 7870 7473 5b69     cc += (xpts[i
+0001f9c0: 202b 2031 5d20 2d20 7870 7473 5b69 5d29   + 1] - xpts[i])
+0001f9d0: 202a 2028 7970 7473 5b69 202b 2031 5d20   * (ypts[i + 1] 
+0001f9e0: 2b20 7970 7473 5b69 5d29 0a0a 2020 2020  + ypts[i])..    
+0001f9f0: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+0001fa00: 2c20 6e29 3a0a 2020 2020 2020 2020 6d69  , n):.        mi
+0001fa10: 6470 6f69 6e74 5f6e 203d 205b 2878 7074  dpoint_n = [(xpt
+0001fa20: 735b 6920 2b20 315d 202b 2078 7074 735b  s[i + 1] + xpts[
+0001fa30: 695d 2920 2f20 322c 2028 7970 7473 5b69  i]) / 2, (ypts[i
+0001fa40: 202b 2031 5d20 2b20 7970 7473 5b69 5d29   + 1] + ypts[i])
+0001fa50: 202f 2032 5d0a 2020 2020 2020 2020 6f72   / 2].        or
+0001fa60: 6965 6e74 6174 696f 6e5f 6e20 3d20 280a  ientation_n = (.
+0001fa70: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+0001fa80: 7263 7461 6e32 280a 2020 2020 2020 2020  rctan2(.        
+0001fa90: 2020 2020 2020 2020 6e70 2e73 6967 6e28          np.sign(
+0001faa0: 6363 2920 2a20 2878 7074 735b 6920 2b20  cc) * (xpts[i + 
+0001fab0: 315d 202d 2078 7074 735b 695d 292c 0a20  1] - xpts[i]),. 
+0001fac0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0001fad0: 702e 7369 676e 2863 6329 202a 2028 7970  p.sign(cc) * (yp
+0001fae0: 7473 5b69 5d20 2d20 7970 7473 5b69 202b  ts[i] - ypts[i +
+0001faf0: 2031 5d29 2c0a 2020 2020 2020 2020 2020   1]),.          
+0001fb00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001fb10: 2a20 3138 300a 2020 2020 2020 2020 2020  * 180.          
+0001fb20: 2020 2f20 7069 0a20 2020 2020 2020 2029    / pi.        )
+0001fb30: 0a20 2020 2020 2020 2077 6964 7468 5f6e  .        width_n
+0001fb40: 203d 206e 702e 6162 7328 0a20 2020 2020   = np.abs(.     
+0001fb50: 2020 2020 2020 2073 7172 7428 2878 7074         sqrt((xpt
+0001fb60: 735b 6920 2b20 315d 202d 2078 7074 735b  s[i + 1] - xpts[
+0001fb70: 695d 2920 2a2a 2032 202b 2028 7970 7473  i]) ** 2 + (ypts
+0001fb80: 5b69 202b 2031 5d20 2d20 7970 7473 5b69  [i + 1] - ypts[i
+0001fb90: 5d29 202a 2a20 3229 0a20 2020 2020 2020  ]) ** 2).       
+0001fba0: 2029 0a20 2020 2020 2020 2050 2e61 6464   ).        P.add
+0001fbb0: 5f70 6f72 7428 0a20 2020 2020 2020 2020  _port(.         
+0001fbc0: 2020 206e 616d 653d 7374 7228 6920 2b20     name=str(i + 
+0001fbd0: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
+0001fbe0: 6d69 6470 6f69 6e74 3d6d 6964 706f 696e  midpoint=midpoin
+0001fbf0: 745f 6e2c 0a20 2020 2020 2020 2020 2020  t_n,.           
+0001fc00: 2077 6964 7468 3d77 6964 7468 5f6e 2c0a   width=width_n,.
+0001fc10: 2020 2020 2020 2020 2020 2020 6f72 6965              orie
+0001fc20: 6e74 6174 696f 6e3d 6f72 6965 6e74 6174  ntation=orientat
+0001fc30: 696f 6e5f 6e2c 0a20 2020 2020 2020 2029  ion_n,.        )
+0001fc40: 0a0a 2020 2020 7265 7475 726e 2050 0a0a  ..    return P..
+0001fc50: 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .# =============
 0001fc60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001fc70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001fc80: 3d3d 0a0a 2320 5020 3d20 706f 6c79 676f  ==..# P = polygo
-0001fc90: 6e28 7870 7473 3d5b 2d31 2c2d 332c 2030  n(xpts=[-1,-3, 0
-0001fca0: 2c20 305d 2c20 7970 7473 203d 205b 302c  , 0], ypts = [0,
-0001fcb0: 2031 2c20 322c 2030 5d2c 206c 6179 6572   1, 2, 0], layer
-0001fcc0: 203d 2033 290a 2320 7175 6963 6b70 6c6f   = 3).# quickplo
-0001fcd0: 7428 5029 0a0a 0a40 6465 7669 6365 5f6c  t(P)...@device_l
-0001fce0: 7275 5f63 6163 6865 0a64 6566 2067 7261  ru_cache.def gra
-0001fcf0: 7469 6e67 280a 2020 2020 6e75 6d5f 7065  ting(.    num_pe
-0001fd00: 7269 6f64 733d 3230 2c0a 2020 2020 7065  riods=20,.    pe
-0001fd10: 7269 6f64 3d30 2e37 352c 0a20 2020 2066  riod=0.75,.    f
-0001fd20: 696c 6c5f 6661 6374 6f72 3d30 2e35 2c0a  ill_factor=0.5,.
-0001fd30: 2020 2020 7769 6474 685f 6772 6174 696e      width_gratin
-0001fd40: 673d 352c 0a20 2020 206c 656e 6774 685f  g=5,.    length_
-0001fd50: 7461 7065 723d 3130 2c0a 2020 2020 7769  taper=10,.    wi
-0001fd60: 6474 683d 302e 342c 0a20 2020 2070 6172  dth=0.4,.    par
-0001fd70: 7469 616c 5f65 7463 683d 4661 6c73 652c  tial_etch=False,
-0001fd80: 0a29 3a0a 2020 2020 2222 2253 696d 706c  .):.    """Simpl
-0001fd90: 6520 6772 6174 696e 6720 7374 7275 6374  e grating struct
-0001fda0: 7572 6520 666f 7220 7068 6f74 6f6e 6963  ure for photonic
-0001fdb0: 730a 0a20 2020 2050 6172 616d 6574 6572  s..    Parameter
-0001fdc0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001fdd0: 0a20 2020 206e 756d 5f70 6572 696f 6473  .    num_periods
-0001fde0: 203a 2069 6e74 0a20 2020 2020 2020 204e   : int.        N
-0001fdf0: 756d 6265 7220 6f66 2067 7261 7469 6e67  umber of grating
-0001fe00: 732e 0a20 2020 2070 6572 696f 6420 3a20  s..    period : 
-0001fe10: 696e 7420 6f72 2066 6c6f 6174 0a20 2020  int or float.   
-0001fe20: 2020 2020 2044 6973 7461 6e63 6520 6265       Distance be
-0001fe30: 7477 6565 6e20 6772 6174 696e 6773 2e0a  tween gratings..
-0001fe40: 2020 2020 6669 6c6c 5f66 6163 746f 7220      fill_factor 
-0001fe50: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
-0001fe60: 2020 2020 2020 2054 6869 636b 6e65 7373         Thickness
-0001fe70: 206f 6620 7468 6520 6772 6174 696e 6773   of the gratings
-0001fe80: 2e0a 2020 2020 7769 6474 685f 6772 6174  ..    width_grat
-0001fe90: 696e 6720 3a20 696e 7420 6f72 2066 6c6f  ing : int or flo
-0001fea0: 6174 0a20 2020 2020 2020 2057 6964 7468  at.        Width
-0001feb0: 206f 6620 7468 6520 6772 6174 696e 6773   of the gratings
-0001fec0: 2e0a 2020 2020 6c65 6e67 7468 5f74 6170  ..    length_tap
-0001fed0: 6572 203a 2069 6e74 206f 7220 666c 6f61  er : int or floa
-0001fee0: 740a 2020 2020 2020 2020 4c65 6e67 7468  t.        Length
-0001fef0: 206f 6620 7468 6520 7461 7065 7220 7365   of the taper se
-0001ff00: 6374 696f 6e2e 0a20 2020 2077 6964 7468  ction..    width
-0001ff10: 203a 2069 6e74 206f 7220 666c 6f61 740a   : int or float.
-0001ff20: 2020 2020 2020 2020 5769 6474 6820 6f66          Width of
-0001ff30: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
-0001ff40: 7461 7065 7220 7365 6374 696f 6e2e 0a20  taper section.. 
-0001ff50: 2020 2070 6172 7469 616c 5f65 7463 6820     partial_etch 
-0001ff60: 3a20 626f 6f6c 0a20 2020 2020 2020 2049  : bool.        I
-0001ff70: 6620 5472 7565 2c20 6d61 6b65 7320 616e  f True, makes an
-0001ff80: 2075 6e74 6170 6572 6564 2c20 7061 7274   untapered, part
-0001ff90: 6961 6c6c 792d 6574 6368 6564 2067 7261  ially-etched gra
-0001ffa0: 7469 6e67 2e0a 0a20 2020 2052 6574 7572  ting...    Retur
-0001ffb0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0001ffc0: 2020 2047 203a 2044 6576 6963 650a 2020     G : Device.  
-0001ffd0: 2020 2020 2020 4120 4465 7669 6365 2063        A Device c
-0001ffe0: 6f6e 7461 696e 696e 6720 6120 6669 6265  ontaining a fibe
-0001fff0: 7220 6772 6174 696e 6720 6765 6f6d 6574  r grating geomet
-00020000: 7279 2e0a 2020 2020 2222 220a 2020 2020  ry..    """.    
-00020010: 2320 7265 7475 726e 7320 6120 6669 6265  # returns a fibe
-00020020: 7220 6772 6174 696e 670a 2020 2020 4720  r grating.    G 
-00020030: 3d20 4465 7669 6365 2822 6772 6174 696e  = Device("gratin
-00020040: 6722 290a 0a20 2020 2023 206d 616b 6520  g")..    # make 
-00020050: 7468 6520 6465 6570 2065 7463 6865 6420  the deep etched 
-00020060: 6772 6174 696e 670a 2020 2020 6966 2070  grating.    if p
-00020070: 6172 7469 616c 5f65 7463 6820 6973 2046  artial_etch is F
-00020080: 616c 7365 3a0a 2020 2020 2020 2020 2320  alse:.        # 
-00020090: 6d61 6b65 2074 6865 2067 7261 7469 6e67  make the grating
-000200a0: 2074 6565 7468 0a20 2020 2020 2020 2066   teeth.        f
-000200b0: 6f72 2069 2069 6e20 7261 6e67 6528 6e75  or i in range(nu
-000200c0: 6d5f 7065 7269 6f64 7329 3a0a 2020 2020  m_periods):.    
-000200d0: 2020 2020 2020 2020 6367 7261 7469 6e67          cgrating
-000200e0: 203d 2047 2e61 6464 5f72 6566 280a 2020   = G.add_ref(.  
-000200f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00020100: 6d70 6173 7328 7369 7a65 3d5b 7065 7269  mpass(size=[peri
-00020110: 6f64 202a 2066 696c 6c5f 6661 6374 6f72  od * fill_factor
-00020120: 2c20 7769 6474 685f 6772 6174 696e 675d  , width_grating]
-00020130: 2c20 6c61 7965 723d 3029 0a20 2020 2020  , layer=0).     
-00020140: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00020150: 2020 2020 2063 6772 6174 696e 672e 7820       cgrating.x 
-00020160: 2b3d 2069 202a 2070 6572 696f 640a 0a20  += i * period.. 
-00020170: 2020 2020 2020 2023 206d 616b 6520 7468         # make th
-00020180: 6520 7461 7065 720a 2020 2020 2020 2020  e taper.        
-00020190: 7467 7261 7469 6e67 203d 2047 2e61 6464  tgrating = G.add
-000201a0: 5f72 6566 280a 2020 2020 2020 2020 2020  _ref(.          
-000201b0: 2020 7461 7065 7228 0a20 2020 2020 2020    taper(.       
-000201c0: 2020 2020 2020 2020 206c 656e 6774 683d           length=
-000201d0: 6c65 6e67 7468 5f74 6170 6572 2c0a 2020  length_taper,.  
-000201e0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-000201f0: 6474 6831 3d77 6964 7468 5f67 7261 7469  dth1=width_grati
-00020200: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-00020210: 2020 2020 7769 6474 6832 3d77 6964 7468      width2=width
-00020220: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020230: 2020 706f 7274 3d4e 6f6e 652c 0a20 2020    port=None,.   
-00020240: 2020 2020 2020 2020 2020 2020 206c 6179               lay
-00020250: 6572 3d30 2c0a 2020 2020 2020 2020 2020  er=0,.          
-00020260: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-00020270: 2020 2020 2020 7467 7261 7469 6e67 2e78        tgrating.x
-00020280: 6d69 6e20 3d20 6367 7261 7469 6e67 2e78  min = cgrating.x
-00020290: 6d61 780a 2020 2020 2020 2020 2320 6465  max.        # de
-000202a0: 6669 6e65 2074 6865 2070 6f72 7420 6f66  fine the port of
-000202b0: 2074 6865 2067 7261 7469 6e67 0a20 2020   the grating.   
-000202c0: 2020 2020 2070 203d 2047 2e61 6464 5f70       p = G.add_p
-000202d0: 6f72 7428 706f 7274 3d74 6772 6174 696e  ort(port=tgratin
-000202e0: 672e 706f 7274 735b 325d 2c20 6e61 6d65  g.ports[2], name
-000202f0: 3d31 290a 2020 2020 2320 6d61 6b65 2061  =1).    # make a
-00020300: 2070 6172 7469 616c 6c79 2065 7463 6865   partially etche
-00020310: 6420 6772 6174 696e 670a 2020 2020 6966  d grating.    if
-00020320: 2070 6172 7469 616c 5f65 7463 6820 6973   partial_etch is
-00020330: 2054 7275 653a 0a20 2020 2020 2020 2023   True:.        #
-00020340: 2068 6172 6420 636f 6465 6420 6f76 6572   hard coded over
-00020350: 6c61 700a 2020 2020 2020 2020 7061 7274  lap.        part
-00020360: 6574 6368 5f6f 7665 7268 616e 6720 3d20  etch_overhang = 
-00020370: 350a 2020 2020 2020 2020 2320 6d61 6b65  5.        # make
-00020380: 2074 6865 2065 7463 6865 6420 6172 6561   the etched area
-00020390: 7320 286f 7070 6f73 6974 6520 746f 2074  s (opposite to t
-000203a0: 6565 7468 290a 2020 2020 2020 2020 666f  eeth).        fo
-000203b0: 7220 6920 696e 2072 616e 6765 286e 756d  r i in range(num
-000203c0: 5f70 6572 696f 6473 293a 0a20 2020 2020  _periods):.     
-000203d0: 2020 2020 2020 2063 6772 6174 696e 6720         cgrating 
-000203e0: 3d20 472e 6164 645f 7265 6628 0a20 2020  = G.add_ref(.   
-000203f0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-00020400: 7061 7373 280a 2020 2020 2020 2020 2020  pass(.          
-00020410: 2020 2020 2020 2020 2020 7369 7a65 3d5b            size=[
-00020420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020430: 2020 2020 2020 2020 2070 6572 696f 6420           period 
-00020440: 2a20 2831 202d 2066 696c 6c5f 6661 6374  * (1 - fill_fact
-00020450: 6f72 292c 0a20 2020 2020 2020 2020 2020  or),.           
-00020460: 2020 2020 2020 2020 2020 2020 2077 6964               wid
-00020470: 7468 5f67 7261 7469 6e67 202b 2070 6172  th_grating + par
-00020480: 7465 7463 685f 6f76 6572 6861 6e67 202a  tetch_overhang *
-00020490: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
-000204a0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000204b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000204c0: 6179 6572 3d31 2c0a 2020 2020 2020 2020  ayer=1,.        
-000204d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000204e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000204f0: 2020 2020 6367 7261 7469 6e67 2e78 202b      cgrating.x +
-00020500: 3d20 6920 2a20 7065 7269 6f64 0a20 2020  = i * period.   
-00020510: 2020 2020 2023 2064 6566 696e 6520 7468       # define th
-00020520: 6520 706f 7274 206f 6620 7468 6520 6772  e port of the gr
-00020530: 6174 696e 670a 2020 2020 2020 2020 7020  ating.        p 
-00020540: 3d20 472e 6164 645f 706f 7274 2870 6f72  = G.add_port(por
-00020550: 743d 6367 7261 7469 6e67 2e70 6f72 7473  t=cgrating.ports
-00020560: 5b22 4522 5d2c 206e 616d 653d 3129 0a20  ["E"], name=1). 
-00020570: 2020 2020 2020 2070 2e6d 6964 706f 696e         p.midpoin
-00020580: 7420 3d20 702e 6d69 6470 6f69 6e74 202b  t = p.midpoint +
-00020590: 206e 702e 6172 7261 7928 5b28 3120 2d20   np.array([(1 - 
-000205a0: 6669 6c6c 5f66 6163 746f 7229 202a 2070  fill_factor) * p
-000205b0: 6572 696f 642c 2030 5d29 0a0a 2020 2020  eriod, 0])..    
-000205c0: 2020 2020 2320 6472 6177 2074 6865 2064      # draw the d
-000205d0: 6565 7020 6574 6368 6564 2073 7175 6172  eep etched squar
-000205e0: 6520 6172 6f75 6e64 2074 6865 2067 7261  e around the gra
-000205f0: 7469 6e67 0a20 2020 2020 2020 2047 2e61  ting.        G.a
-00020600: 6464 5f72 6566 2820 2023 2064 6565 7062  dd_ref(  # deepb
-00020610: 6f78 0a20 2020 2020 2020 2020 2020 2063  ox.            c
-00020620: 6f6d 7061 7373 2873 697a 653d 5b6e 756d  ompass(size=[num
-00020630: 5f70 6572 696f 6473 202a 2070 6572 696f  _periods * perio
-00020640: 642c 2077 6964 7468 5f67 7261 7469 6e67  d, width_grating
-00020650: 5d2c 206c 6179 6572 3d30 290a 2020 2020  ], layer=0).    
-00020660: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00020670: 2047 0a0a 0a23 203d 3d3d 3d3d 3d3d 3d3d   G...# =========
-00020680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000206a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000206b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000206c0: 3d3d 3d3d 3d0a 2320 4578 616d 706c 6520  =====.# Example 
-000206d0: 636f 6465 0a23 203d 3d3d 3d3d 3d3d 3d3d  code.# =========
-000206e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000206f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fc80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fc90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fca0: 3d0a 2320 4578 616d 706c 6520 636f 6465  =.# Example code
+0001fcb0: 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .# =============
+0001fcc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fcd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fcf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001fd00: 3d0a 0a23 2050 203d 2070 6f6c 7967 6f6e  =..# P = polygon
+0001fd10: 2878 7074 733d 5b2d 312c 2d33 2c20 302c  (xpts=[-1,-3, 0,
+0001fd20: 2030 5d2c 2079 7074 7320 3d20 5b30 2c20   0], ypts = [0, 
+0001fd30: 312c 2032 2c20 305d 2c20 6c61 7965 7220  1, 2, 0], layer 
+0001fd40: 3d20 3329 0a23 2071 7569 636b 706c 6f74  = 3).# quickplot
+0001fd50: 2850 290a 0a0a 4064 6576 6963 655f 6c72  (P)...@device_lr
+0001fd60: 755f 6361 6368 650a 6465 6620 6772 6174  u_cache.def grat
+0001fd70: 696e 6728 0a20 2020 206e 756d 5f70 6572  ing(.    num_per
+0001fd80: 696f 6473 3d32 302c 0a20 2020 2070 6572  iods=20,.    per
+0001fd90: 696f 643d 302e 3735 2c0a 2020 2020 6669  iod=0.75,.    fi
+0001fda0: 6c6c 5f66 6163 746f 723d 302e 352c 0a20  ll_factor=0.5,. 
+0001fdb0: 2020 2077 6964 7468 5f67 7261 7469 6e67     width_grating
+0001fdc0: 3d35 2c0a 2020 2020 6c65 6e67 7468 5f74  =5,.    length_t
+0001fdd0: 6170 6572 3d31 302c 0a20 2020 2077 6964  aper=10,.    wid
+0001fde0: 7468 3d30 2e34 2c0a 2020 2020 7061 7274  th=0.4,.    part
+0001fdf0: 6961 6c5f 6574 6368 3d46 616c 7365 2c0a  ial_etch=False,.
+0001fe00: 293a 0a20 2020 2022 2222 5369 6d70 6c65  ):.    """Simple
+0001fe10: 2067 7261 7469 6e67 2073 7472 7563 7475   grating structu
+0001fe20: 7265 2066 6f72 2070 686f 746f 6e69 6373  re for photonics
+0001fe30: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001fe40: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001fe50: 2020 2020 6e75 6d5f 7065 7269 6f64 7320      num_periods 
+0001fe60: 3a20 696e 740a 2020 2020 2020 2020 4e75  : int.        Nu
+0001fe70: 6d62 6572 206f 6620 6772 6174 696e 6773  mber of gratings
+0001fe80: 2e0a 2020 2020 7065 7269 6f64 203a 2069  ..    period : i
+0001fe90: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
+0001fea0: 2020 2020 4469 7374 616e 6365 2062 6574      Distance bet
+0001feb0: 7765 656e 2067 7261 7469 6e67 732e 0a20  ween gratings.. 
+0001fec0: 2020 2066 696c 6c5f 6661 6374 6f72 203a     fill_factor :
+0001fed0: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
+0001fee0: 2020 2020 2020 5468 6963 6b6e 6573 7320        Thickness 
+0001fef0: 6f66 2074 6865 2067 7261 7469 6e67 732e  of the gratings.
+0001ff00: 0a20 2020 2077 6964 7468 5f67 7261 7469  .    width_grati
+0001ff10: 6e67 203a 2069 6e74 206f 7220 666c 6f61  ng : int or floa
+0001ff20: 740a 2020 2020 2020 2020 5769 6474 6820  t.        Width 
+0001ff30: 6f66 2074 6865 2067 7261 7469 6e67 732e  of the gratings.
+0001ff40: 0a20 2020 206c 656e 6774 685f 7461 7065  .    length_tape
+0001ff50: 7220 3a20 696e 7420 6f72 2066 6c6f 6174  r : int or float
+0001ff60: 0a20 2020 2020 2020 204c 656e 6774 6820  .        Length 
+0001ff70: 6f66 2074 6865 2074 6170 6572 2073 6563  of the taper sec
+0001ff80: 7469 6f6e 2e0a 2020 2020 7769 6474 6820  tion..    width 
+0001ff90: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
+0001ffa0: 2020 2020 2020 2057 6964 7468 206f 6620         Width of 
+0001ffb0: 7468 6520 656e 6420 6f66 2074 6865 2074  the end of the t
+0001ffc0: 6170 6572 2073 6563 7469 6f6e 2e0a 2020  aper section..  
+0001ffd0: 2020 7061 7274 6961 6c5f 6574 6368 203a    partial_etch :
+0001ffe0: 2062 6f6f 6c0a 2020 2020 2020 2020 4966   bool.        If
+0001fff0: 2054 7275 652c 206d 616b 6573 2061 6e20   True, makes an 
+00020000: 756e 7461 7065 7265 642c 2070 6172 7469  untapered, parti
+00020010: 616c 6c79 2d65 7463 6865 6420 6772 6174  ally-etched grat
+00020020: 696e 672e 0a0a 2020 2020 5265 7475 726e  ing...    Return
+00020030: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00020040: 2020 4720 3a20 4465 7669 6365 0a20 2020    G : Device.   
+00020050: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
+00020060: 6e74 6169 6e69 6e67 2061 2066 6962 6572  ntaining a fiber
+00020070: 2067 7261 7469 6e67 2067 656f 6d65 7472   grating geometr
+00020080: 792e 0a20 2020 2022 2222 0a20 2020 2023  y..    """.    #
+00020090: 2072 6574 7572 6e73 2061 2066 6962 6572   returns a fiber
+000200a0: 2067 7261 7469 6e67 0a20 2020 2047 203d   grating.    G =
+000200b0: 2044 6576 6963 6528 2267 7261 7469 6e67   Device("grating
+000200c0: 2229 0a0a 2020 2020 2320 6d61 6b65 2074  ")..    # make t
+000200d0: 6865 2064 6565 7020 6574 6368 6564 2067  he deep etched g
+000200e0: 7261 7469 6e67 0a20 2020 2069 6620 7061  rating.    if pa
+000200f0: 7274 6961 6c5f 6574 6368 2069 7320 4661  rtial_etch is Fa
+00020100: 6c73 653a 0a20 2020 2020 2020 2023 206d  lse:.        # m
+00020110: 616b 6520 7468 6520 6772 6174 696e 6720  ake the grating 
+00020120: 7465 6574 680a 2020 2020 2020 2020 666f  teeth.        fo
+00020130: 7220 6920 696e 2072 616e 6765 286e 756d  r i in range(num
+00020140: 5f70 6572 696f 6473 293a 0a20 2020 2020  _periods):.     
+00020150: 2020 2020 2020 2063 6772 6174 696e 6720         cgrating 
+00020160: 3d20 472e 6164 645f 7265 6628 0a20 2020  = G.add_ref(.   
+00020170: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00020180: 7061 7373 2873 697a 653d 5b70 6572 696f  pass(size=[perio
+00020190: 6420 2a20 6669 6c6c 5f66 6163 746f 722c  d * fill_factor,
+000201a0: 2077 6964 7468 5f67 7261 7469 6e67 5d2c   width_grating],
+000201b0: 206c 6179 6572 3d30 290a 2020 2020 2020   layer=0).      
+000201c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000201d0: 2020 2020 6367 7261 7469 6e67 2e78 202b      cgrating.x +
+000201e0: 3d20 6920 2a20 7065 7269 6f64 0a0a 2020  = i * period..  
+000201f0: 2020 2020 2020 2320 6d61 6b65 2074 6865        # make the
+00020200: 2074 6170 6572 0a20 2020 2020 2020 2074   taper.        t
+00020210: 6772 6174 696e 6720 3d20 472e 6164 645f  grating = G.add_
+00020220: 7265 6628 0a20 2020 2020 2020 2020 2020  ref(.           
+00020230: 2074 6170 6572 280a 2020 2020 2020 2020   taper(.        
+00020240: 2020 2020 2020 2020 6c65 6e67 7468 3d6c          length=l
+00020250: 656e 6774 685f 7461 7065 722c 0a20 2020  ength_taper,.   
+00020260: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00020270: 7468 313d 7769 6474 685f 6772 6174 696e  th1=width_gratin
+00020280: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+00020290: 2020 2077 6964 7468 323d 7769 6474 682c     width2=width,
+000202a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000202b0: 2070 6f72 743d 4e6f 6e65 2c0a 2020 2020   port=None,.    
+000202c0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+000202d0: 723d 302c 0a20 2020 2020 2020 2020 2020  r=0,.           
+000202e0: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
+000202f0: 2020 2020 2074 6772 6174 696e 672e 786d       tgrating.xm
+00020300: 696e 203d 2063 6772 6174 696e 672e 786d  in = cgrating.xm
+00020310: 6178 0a20 2020 2020 2020 2023 2064 6566  ax.        # def
+00020320: 696e 6520 7468 6520 706f 7274 206f 6620  ine the port of 
+00020330: 7468 6520 6772 6174 696e 670a 2020 2020  the grating.    
+00020340: 2020 2020 7020 3d20 472e 6164 645f 706f      p = G.add_po
+00020350: 7274 2870 6f72 743d 7467 7261 7469 6e67  rt(port=tgrating
+00020360: 2e70 6f72 7473 5b32 5d2c 206e 616d 653d  .ports[2], name=
+00020370: 3129 0a20 2020 2023 206d 616b 6520 6120  1).    # make a 
+00020380: 7061 7274 6961 6c6c 7920 6574 6368 6564  partially etched
+00020390: 2067 7261 7469 6e67 0a20 2020 2069 6620   grating.    if 
+000203a0: 7061 7274 6961 6c5f 6574 6368 2069 7320  partial_etch is 
+000203b0: 5472 7565 3a0a 2020 2020 2020 2020 2320  True:.        # 
+000203c0: 6861 7264 2063 6f64 6564 206f 7665 726c  hard coded overl
+000203d0: 6170 0a20 2020 2020 2020 2070 6172 7465  ap.        parte
+000203e0: 7463 685f 6f76 6572 6861 6e67 203d 2035  tch_overhang = 5
+000203f0: 0a20 2020 2020 2020 2023 206d 616b 6520  .        # make 
+00020400: 7468 6520 6574 6368 6564 2061 7265 6173  the etched areas
+00020410: 2028 6f70 706f 7369 7465 2074 6f20 7465   (opposite to te
+00020420: 6574 6829 0a20 2020 2020 2020 2066 6f72  eth).        for
+00020430: 2069 2069 6e20 7261 6e67 6528 6e75 6d5f   i in range(num_
+00020440: 7065 7269 6f64 7329 3a0a 2020 2020 2020  periods):.      
+00020450: 2020 2020 2020 6367 7261 7469 6e67 203d        cgrating =
+00020460: 2047 2e61 6464 5f72 6566 280a 2020 2020   G.add_ref(.    
+00020470: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00020480: 6173 7328 0a20 2020 2020 2020 2020 2020  ass(.           
+00020490: 2020 2020 2020 2020 2073 697a 653d 5b0a           size=[.
+000204a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000204b0: 2020 2020 2020 2020 7065 7269 6f64 202a          period *
+000204c0: 2028 3120 2d20 6669 6c6c 5f66 6163 746f   (1 - fill_facto
+000204d0: 7229 2c0a 2020 2020 2020 2020 2020 2020  r),.            
+000204e0: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+000204f0: 685f 6772 6174 696e 6720 2b20 7061 7274  h_grating + part
+00020500: 6574 6368 5f6f 7665 7268 616e 6720 2a20  etch_overhang * 
+00020510: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00020520: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00020530: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00020540: 7965 723d 312c 0a20 2020 2020 2020 2020  yer=1,.         
+00020550: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00020560: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00020570: 2020 2063 6772 6174 696e 672e 7820 2b3d     cgrating.x +=
+00020580: 2069 202a 2070 6572 696f 640a 2020 2020   i * period.    
+00020590: 2020 2020 2320 6465 6669 6e65 2074 6865      # define the
+000205a0: 2070 6f72 7420 6f66 2074 6865 2067 7261   port of the gra
+000205b0: 7469 6e67 0a20 2020 2020 2020 2070 203d  ting.        p =
+000205c0: 2047 2e61 6464 5f70 6f72 7428 706f 7274   G.add_port(port
+000205d0: 3d63 6772 6174 696e 672e 706f 7274 735b  =cgrating.ports[
+000205e0: 2245 225d 2c20 6e61 6d65 3d31 290a 2020  "E"], name=1).  
+000205f0: 2020 2020 2020 702e 6d69 6470 6f69 6e74        p.midpoint
+00020600: 203d 2070 2e6d 6964 706f 696e 7420 2b20   = p.midpoint + 
+00020610: 6e70 2e61 7272 6179 285b 2831 202d 2066  np.array([(1 - f
+00020620: 696c 6c5f 6661 6374 6f72 2920 2a20 7065  ill_factor) * pe
+00020630: 7269 6f64 2c20 305d 290a 0a20 2020 2020  riod, 0])..     
+00020640: 2020 2023 2064 7261 7720 7468 6520 6465     # draw the de
+00020650: 6570 2065 7463 6865 6420 7371 7561 7265  ep etched square
+00020660: 2061 726f 756e 6420 7468 6520 6772 6174   around the grat
+00020670: 696e 670a 2020 2020 2020 2020 472e 6164  ing.        G.ad
+00020680: 645f 7265 6628 2020 2320 6465 6570 626f  d_ref(  # deepbo
+00020690: 780a 2020 2020 2020 2020 2020 2020 636f  x.            co
+000206a0: 6d70 6173 7328 7369 7a65 3d5b 6e75 6d5f  mpass(size=[num_
+000206b0: 7065 7269 6f64 7320 2a20 7065 7269 6f64  periods * period
+000206c0: 2c20 7769 6474 685f 6772 6174 696e 675d  , width_grating]
+000206d0: 2c20 6c61 7965 723d 3029 0a20 2020 2020  , layer=0).     
+000206e0: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+000206f0: 470a 0a0a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  G...# ==========
 00020700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00020710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020720: 3d3d 3d3d 3d0a 0a23 2047 203d 2067 7261  =====..# G = gra
-00020730: 7469 6e67 286e 756d 5f70 6572 696f 6473  ting(num_periods
-00020740: 203d 2032 302c 2070 6572 696f 6420 3d20   = 20, period = 
-00020750: 302e 3735 2c20 6669 6c6c 5f66 6163 746f  0.75, fill_facto
-00020760: 7220 3d20 302e 352c 0a23 2020 2020 2020  r = 0.5,.#      
-00020770: 2020 2020 2020 2077 6964 7468 5f67 7261         width_gra
-00020780: 7469 6e67 203d 2032 302c 206c 656e 6774  ting = 20, lengt
-00020790: 685f 7461 7065 7220 3d20 3130 2c20 7769  h_taper = 10, wi
-000207a0: 6474 6820 3d20 302e 342c 0a23 2020 2020  dth = 0.4,.#    
-000207b0: 2020 2020 2020 2020 2070 6172 7469 616c           partial
-000207c0: 5f65 7463 6820 3d20 4661 6c73 6529 0a23  _etch = False).#
-000207d0: 2071 7569 636b 706c 6f74 2847 290a 0a0a   quickplot(G)...
-000207e0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
-000207f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020800: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020830: 0a23 0a23 2054 6573 7420 5374 7275 6374  .#.# Test Struct
-00020840: 7572 6573 0a23 0a23 203d 3d3d 3d3d 3d3d  ures.#.# =======
-00020850: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020860: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020740: 3d3d 3d3d 0a23 2045 7861 6d70 6c65 2063  ====.# Example c
+00020750: 6f64 650a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  ode.# ==========
+00020760: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000207a0: 3d3d 3d3d 0a0a 2320 4720 3d20 6772 6174  ====..# G = grat
+000207b0: 696e 6728 6e75 6d5f 7065 7269 6f64 7320  ing(num_periods 
+000207c0: 3d20 3230 2c20 7065 7269 6f64 203d 2030  = 20, period = 0
+000207d0: 2e37 352c 2066 696c 6c5f 6661 6374 6f72  .75, fill_factor
+000207e0: 203d 2030 2e35 2c0a 2320 2020 2020 2020   = 0.5,.#       
+000207f0: 2020 2020 2020 7769 6474 685f 6772 6174        width_grat
+00020800: 696e 6720 3d20 3230 2c20 6c65 6e67 7468  ing = 20, length
+00020810: 5f74 6170 6572 203d 2031 302c 2077 6964  _taper = 10, wid
+00020820: 7468 203d 2030 2e34 2c0a 2320 2020 2020  th = 0.4,.#     
+00020830: 2020 2020 2020 2020 7061 7274 6961 6c5f          partial_
+00020840: 6574 6368 203d 2046 616c 7365 290a 2320  etch = False).# 
+00020850: 7175 6963 6b70 6c6f 7428 4729 0a0a 0a23  quickplot(G)...#
+00020860: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
 00020870: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00020880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00020890: 3d3d 3d3d 3d3d 3d0a 0a23 2056 6961 2052  =======..# Via R
-000208a0: 6f75 7465 202d 2d2d 2d2d 2d2d 2d2d 2d2d  oute -----------
-000208b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000208c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 6465  -------------.de
-000208d0: 6620 5f76 6961 5f69 7465 7261 626c 6528  f _via_iterable(
-000208e0: 0a20 2020 2076 6961 5f73 7061 6369 6e67  .    via_spacing
-000208f0: 2c20 7769 7265 5f77 6964 7468 2c20 7769  , wire_width, wi
-00020900: 7269 6e67 315f 6c61 7965 722c 2077 6972  ring1_layer, wir
-00020910: 696e 6732 5f6c 6179 6572 2c20 7669 615f  ing2_layer, via_
-00020920: 6c61 7965 722c 2076 6961 5f77 6964 7468  layer, via_width
-00020930: 0a29 3a0a 2020 2020 2222 2248 656c 7065  .):.    """Helpe
-00020940: 7220 6675 6e63 7469 6f6e 2066 6f72 2074  r function for t
-00020950: 6573 745f 7669 610a 0a20 2020 2050 6172  est_via..    Par
-00020960: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00020970: 2d2d 2d2d 2d2d 0a20 2020 2076 6961 5f73  ------.    via_s
-00020980: 7061 6369 6e67 203a 2069 6e74 206f 7220  pacing : int or 
-00020990: 666c 6f61 740a 2020 2020 2020 2020 4469  float.        Di
-000209a0: 7374 616e 6365 2062 6574 7765 656e 2076  stance between v
-000209b0: 6961 732e 0a20 2020 2077 6972 655f 7769  ias..    wire_wi
-000209c0: 6474 6820 3a20 696e 7420 6f72 2066 6c6f  dth : int or flo
-000209d0: 6174 0a20 2020 2020 2020 2054 6865 2077  at.        The w
-000209e0: 6964 7468 206f 6620 7468 6520 7769 7265  idth of the wire
-000209f0: 732e 0a20 2020 2077 6972 696e 6731 5f6c  s..    wiring1_l
-00020a00: 6179 6572 203a 2069 6e74 0a20 2020 2020  ayer : int.     
-00020a10: 2020 2053 7065 6369 6669 6320 6c61 7965     Specific laye
-00020a20: 7220 746f 2070 7574 2074 6865 2074 6f70  r to put the top
-00020a30: 2077 6972 696e 6720 6f6e 2e0a 2020 2020   wiring on..    
-00020a40: 7769 7269 6e67 325f 6c61 7965 7220 3a20  wiring2_layer : 
-00020a50: 696e 740a 2020 2020 2020 2020 5370 6563  int.        Spec
-00020a60: 6966 6963 206c 6179 6572 2074 6f20 7075  ific layer to pu
-00020a70: 7420 7468 6520 626f 7474 6f6d 2077 6972  t the bottom wir
-00020a80: 696e 6720 6f6e 2e0a 2020 2020 7669 615f  ing on..    via_
-00020a90: 6c61 7965 7220 3a20 696e 740a 2020 2020  layer : int.    
-00020aa0: 2020 2020 5370 6563 6966 6963 206c 6179      Specific lay
-00020ab0: 6572 2074 6f20 7075 7420 7468 6520 7669  er to put the vi
-00020ac0: 6173 206f 6e2e 0a20 2020 2076 6961 5f77  as on..    via_w
-00020ad0: 6964 7468 203a 2069 6e74 206f 7220 666c  idth : int or fl
-00020ae0: 6f61 740a 2020 2020 2020 2020 4469 616d  oat.        Diam
-00020af0: 6574 6572 206f 6620 7468 6520 7669 6173  eter of the vias
-00020b00: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-00020b10: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2056     -------.    V
-00020b20: 4920 3a20 4465 7669 6365 0a0a 2020 2020  I : Device..    
-00020b30: 2222 220a 2020 2020 5649 203d 2044 6576  """.    VI = Dev
-00020b40: 6963 6528 2274 6573 745f 7669 615f 6974  ice("test_via_it
-00020b50: 6572 2229 0a20 2020 2077 6972 6531 203d  er").    wire1 =
-00020b60: 2056 492e 6164 645f 7265 6628 636f 6d70   VI.add_ref(comp
-00020b70: 6173 7328 7369 7a65 3d28 7669 615f 7370  ass(size=(via_sp
-00020b80: 6163 696e 672c 2077 6972 655f 7769 6474  acing, wire_widt
-00020b90: 6829 2c20 6c61 7965 723d 7769 7269 6e67  h), layer=wiring
-00020ba0: 315f 6c61 7965 7229 290a 2020 2020 7769  1_layer)).    wi
-00020bb0: 7265 3220 3d20 5649 2e61 6464 5f72 6566  re2 = VI.add_ref
-00020bc0: 2863 6f6d 7061 7373 2873 697a 653d 2876  (compass(size=(v
-00020bd0: 6961 5f73 7061 6369 6e67 2c20 7769 7265  ia_spacing, wire
-00020be0: 5f77 6964 7468 292c 206c 6179 6572 3d77  _width), layer=w
-00020bf0: 6972 696e 6732 5f6c 6179 6572 2929 0a20  iring2_layer)). 
-00020c00: 2020 2076 6961 3120 3d20 5649 2e61 6464     via1 = VI.add
-00020c10: 5f72 6566 2863 6f6d 7061 7373 2873 697a  _ref(compass(siz
-00020c20: 653d 2876 6961 5f77 6964 7468 2c20 7669  e=(via_width, vi
-00020c30: 615f 7769 6474 6829 2c20 6c61 7965 723d  a_width), layer=
-00020c40: 7669 615f 6c61 7965 7229 290a 2020 2020  via_layer)).    
-00020c50: 7669 6132 203d 2056 492e 6164 645f 7265  via2 = VI.add_re
-00020c60: 6628 636f 6d70 6173 7328 7369 7a65 3d28  f(compass(size=(
-00020c70: 7669 615f 7769 6474 682c 2076 6961 5f77  via_width, via_w
-00020c80: 6964 7468 292c 206c 6179 6572 3d76 6961  idth), layer=via
-00020c90: 5f6c 6179 6572 2929 0a20 2020 2077 6972  _layer)).    wir
-00020ca0: 6531 2e63 6f6e 6e65 6374 2870 6f72 743d  e1.connect(port=
-00020cb0: 2245 222c 2064 6573 7469 6e61 7469 6f6e  "E", destination
-00020cc0: 3d77 6972 6532 2e70 6f72 7473 5b22 5722  =wire2.ports["W"
-00020cd0: 5d2c 206f 7665 726c 6170 3d77 6972 655f  ], overlap=wire_
-00020ce0: 7769 6474 6829 0a20 2020 2076 6961 312e  width).    via1.
-00020cf0: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
-00020d00: 2070 6f72 743d 2257 222c 2064 6573 7469   port="W", desti
-00020d10: 6e61 7469 6f6e 3d77 6972 6531 2e70 6f72  nation=wire1.por
-00020d20: 7473 5b22 4522 5d2c 206f 7665 726c 6170  ts["E"], overlap
-00020d30: 3d28 7769 7265 5f77 6964 7468 202b 2076  =(wire_width + v
-00020d40: 6961 5f77 6964 7468 2920 2f20 320a 2020  ia_width) / 2.  
-00020d50: 2020 290a 2020 2020 7669 6132 2e63 6f6e    ).    via2.con
-00020d60: 6e65 6374 280a 2020 2020 2020 2020 706f  nect(.        po
-00020d70: 7274 3d22 5722 2c20 6465 7374 696e 6174  rt="W", destinat
-00020d80: 696f 6e3d 7769 7265 322e 706f 7274 735b  ion=wire2.ports[
-00020d90: 2245 225d 2c20 6f76 6572 6c61 703d 2877  "E"], overlap=(w
-00020da0: 6972 655f 7769 6474 6820 2b20 7669 615f  ire_width + via_
-00020db0: 7769 6474 6829 202f 2032 0a20 2020 2029  width) / 2.    )
-00020dc0: 0a20 2020 2056 492e 6164 645f 706f 7274  .    VI.add_port
-00020dd0: 286e 616d 653d 2257 222c 2070 6f72 743d  (name="W", port=
-00020de0: 7769 7265 312e 706f 7274 735b 2257 225d  wire1.ports["W"]
-00020df0: 290a 2020 2020 5649 2e61 6464 5f70 6f72  ).    VI.add_por
-00020e00: 7428 6e61 6d65 3d22 4522 2c20 706f 7274  t(name="E", port
-00020e10: 3d77 6972 6532 2e70 6f72 7473 5b22 4522  =wire2.ports["E"
-00020e20: 5d29 0a20 2020 2056 492e 6164 645f 706f  ]).    VI.add_po
-00020e30: 7274 280a 2020 2020 2020 2020 6e61 6d65  rt(.        name
-00020e40: 3d22 5322 2c0a 2020 2020 2020 2020 6d69  ="S",.        mi
-00020e50: 6470 6f69 6e74 3d5b 2831 202a 2077 6972  dpoint=[(1 * wir
-00020e60: 655f 7769 6474 6829 202b 2077 6972 655f  e_width) + wire_
-00020e70: 7769 6474 6820 2f20 322c 202d 7769 7265  width / 2, -wire
-00020e80: 5f77 6964 7468 202f 2032 5d2c 0a20 2020  _width / 2],.   
-00020e90: 2020 2020 2077 6964 7468 3d77 6972 655f       width=wire_
-00020ea0: 7769 6474 682c 0a20 2020 2020 2020 206f  width,.        o
-00020eb0: 7269 656e 7461 7469 6f6e 3d2d 3930 2c0a  rientation=-90,.
-00020ec0: 2020 2020 290a 2020 2020 5649 2e61 6464      ).    VI.add
-00020ed0: 5f70 6f72 7428 0a20 2020 2020 2020 206e  _port(.        n
-00020ee0: 616d 653d 224e 222c 0a20 2020 2020 2020  ame="N",.       
-00020ef0: 206d 6964 706f 696e 743d 5b28 3120 2a20   midpoint=[(1 * 
-00020f00: 7769 7265 5f77 6964 7468 2920 2b20 7769  wire_width) + wi
-00020f10: 7265 5f77 6964 7468 202f 2032 2c20 7769  re_width / 2, wi
-00020f20: 7265 5f77 6964 7468 202f 2032 5d2c 0a20  re_width / 2],. 
-00020f30: 2020 2020 2020 2077 6964 7468 3d77 6972         width=wir
-00020f40: 655f 7769 6474 682c 0a20 2020 2020 2020  e_width,.       
-00020f50: 206f 7269 656e 7461 7469 6f6e 3d39 302c   orientation=90,
-00020f60: 0a20 2020 2029 0a0a 2020 2020 7265 7475  .    )..    retu
-00020f70: 726e 2056 490a 0a0a 6465 6620 7465 7374  rn VI...def test
-00020f80: 5f76 6961 280a 2020 2020 6e75 6d5f 7669  _via(.    num_vi
-00020f90: 6173 3d31 3030 2c0a 2020 2020 7769 7265  as=100,.    wire
-00020fa0: 5f77 6964 7468 3d31 302c 0a20 2020 2076  _width=10,.    v
-00020fb0: 6961 5f77 6964 7468 3d31 352c 0a20 2020  ia_width=15,.   
-00020fc0: 2076 6961 5f73 7061 6369 6e67 3d34 302c   via_spacing=40,
-00020fd0: 0a20 2020 2070 6164 5f73 697a 653d 2833  .    pad_size=(3
-00020fe0: 3030 2c20 3330 3029 2c0a 2020 2020 6d69  00, 300),.    mi
-00020ff0: 6e5f 7061 645f 7370 6163 696e 673d 302c  n_pad_spacing=0,
-00021000: 0a20 2020 2070 6164 5f6c 6179 6572 3d30  .    pad_layer=0
-00021010: 2c0a 2020 2020 7769 7269 6e67 315f 6c61  ,.    wiring1_la
-00021020: 7965 723d 312c 0a20 2020 2077 6972 696e  yer=1,.    wirin
-00021030: 6732 5f6c 6179 6572 3d32 2c0a 2020 2020  g2_layer=2,.    
-00021040: 7669 615f 6c61 7965 723d 332c 0a29 3a0a  via_layer=3,.):.
-00021050: 2020 2020 2222 2256 6961 2063 6861 696e      """Via chain
-00021060: 2074 6573 7420 7374 7275 6374 7572 650a   test structure.
-00021070: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00021080: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00021090: 2020 206e 756d 5f76 6961 7320 3a20 696e     num_vias : in
-000210a0: 740a 2020 2020 2020 2020 5468 6520 746f  t.        The to
-000210b0: 7461 6c20 6e75 6d62 6572 206f 6620 7265  tal number of re
-000210c0: 7175 6573 7465 6420 7669 6173 2028 6d75  quested vias (mu
-000210d0: 7374 2062 6520 616e 2065 7665 6e20 6e75  st be an even nu
-000210e0: 6d62 6572 292e 0a20 2020 2077 6972 655f  mber)..    wire_
-000210f0: 7769 6474 6820 3a20 696e 7420 6f72 2066  width : int or f
-00021100: 6c6f 6174 0a20 2020 2020 2020 2054 6865  loat.        The
-00021110: 2077 6964 7468 206f 6620 7468 6520 7769   width of the wi
-00021120: 7265 732e 0a20 2020 2076 6961 5f77 6964  res..    via_wid
-00021130: 7468 203a 2069 6e74 206f 7220 666c 6f61  th : int or floa
-00021140: 740a 2020 2020 2020 2020 4469 616d 6574  t.        Diamet
-00021150: 6572 206f 6620 7468 6520 7669 6173 2e0a  er of the vias..
-00021160: 2020 2020 7669 615f 7370 6163 696e 6720      via_spacing 
-00021170: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
-00021180: 2020 2020 2020 2044 6973 7461 6e63 6520         Distance 
-00021190: 6265 7477 6565 6e20 7669 6173 2e0a 2020  between vias..  
-000211a0: 2020 7061 645f 7369 7a65 203a 2061 7272    pad_size : arr
-000211b0: 6179 2d6c 696b 655b 325d 0a20 2020 2020  ay-like[2].     
-000211c0: 2020 2028 7769 6474 682c 2068 6569 6768     (width, heigh
-000211d0: 7429 206f 6620 7468 6520 7061 6473 2e0a  t) of the pads..
-000211e0: 2020 2020 6d69 6e5f 7061 645f 7370 6163      min_pad_spac
-000211f0: 696e 6720 3a20 696e 7420 6f72 2066 6c6f  ing : int or flo
-00021200: 6174 0a20 2020 2020 2020 2044 6566 696e  at.        Defin
-00021210: 6573 2074 6865 206d 696e 696d 756d 2064  es the minimum d
-00021220: 6973 7461 6e63 6520 6265 7477 6565 6e20  istance between 
-00021230: 7468 6520 7477 6f20 7061 6473 2e0a 2020  the two pads..  
-00021240: 2020 7061 645f 6c61 7965 7220 3a20 696e    pad_layer : in
-00021250: 740a 2020 2020 2020 2020 5370 6563 6966  t.        Specif
-00021260: 6963 206c 6179 6572 2074 6f20 7075 7420  ic layer to put 
-00021270: 7468 6520 7061 6473 206f 6e2e 0a20 2020  the pads on..   
-00021280: 2077 6972 696e 6731 5f6c 6179 6572 203a   wiring1_layer :
-00021290: 2069 6e74 0a20 2020 2020 2020 2053 7065   int.        Spe
-000212a0: 6369 6669 6320 6c61 7965 7220 746f 2070  cific layer to p
-000212b0: 7574 2074 6865 2074 6f70 2077 6972 696e  ut the top wirin
-000212c0: 6720 6f6e 2e0a 2020 2020 7769 7269 6e67  g on..    wiring
-000212d0: 325f 6c61 7965 7220 3a20 696e 740a 2020  2_layer : int.  
-000212e0: 2020 2020 2020 5370 6563 6966 6963 206c        Specific l
-000212f0: 6179 6572 2074 6f20 7075 7420 7468 6520  ayer to put the 
-00021300: 626f 7474 6f6d 2077 6972 696e 6720 6f6e  bottom wiring on
-00021310: 2e0a 2020 2020 7669 615f 6c61 7965 7220  ..    via_layer 
-00021320: 3a20 696e 740a 2020 2020 2020 2020 5370  : int.        Sp
-00021330: 6563 6966 6963 206c 6179 6572 2074 6f20  ecific layer to 
-00021340: 7075 7420 7468 6520 7669 6173 206f 6e2e  put the vias on.
-00021350: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00021360: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 5652    -------.    VR
-00021370: 203a 2044 6576 6963 650a 2020 2020 2020   : Device.      
-00021380: 2020 4120 4465 7669 6365 2063 6f6e 7461    A Device conta
-00021390: 696e 696e 6720 7468 6520 7465 7374 2076  ining the test v
-000213a0: 6961 2073 7472 7563 7475 7265 732e 0a0a  ia structures...
-000213b0: 2020 2020 5573 6167 650a 2020 2020 2d2d      Usage.    --
-000213c0: 2d2d 2d0a 2020 2020 4361 6c6c 2076 6961  ---.    Call via
-000213d0: 5f72 6f75 7465 5f74 6573 745f 7374 7275  _route_test_stru
-000213e0: 6374 7572 6528 2920 6279 2069 6e64 6963  cture() by indic
-000213f0: 6174 696e 6720 7468 6520 6e75 6d62 6572  ating the number
-00021400: 206f 6620 7669 6173 2079 6f75 2077 616e   of vias you wan
-00021410: 740a 2020 2020 6472 6177 6e2e 2059 6f75  t.    drawn. You
-00021420: 2063 616e 2061 6c73 6f20 6368 616e 6765   can also change
-00021430: 2074 6865 206f 7468 6572 2070 6172 616d   the other param
-00021440: 6574 6572 7320 686f 7765 7665 7220 6966  eters however if
-00021450: 2079 6f75 2064 6f20 6e6f 740a 2020 2020   you do not.    
-00021460: 7370 6563 6966 6979 2061 2076 616c 7565  specifiy a value
-00021470: 2066 6f72 2061 2070 6172 616d 6574 6572   for a parameter
-00021480: 2069 7420 7769 6c6c 206a 7573 7420 7573   it will just us
-00021490: 6520 7468 6520 6465 6661 756c 7420 7661  e the default va
-000214a0: 6c75 650a 2020 2020 4578 3a3a 0a0a 2020  lue.    Ex::..  
-000214b0: 2020 2020 2020 7669 615f 726f 7574 655f        via_route_
-000214c0: 7465 7374 5f73 7472 7563 7475 7265 286e  test_structure(n
-000214d0: 756d 5f76 6961 733d 3534 290a 0a20 2020  um_vias=54)..   
-000214e0: 202d 206f 7220 2d3a 3a0a 0a20 2020 2020   - or -::..     
-000214f0: 2020 2076 6961 5f72 6f75 7465 5f74 6573     via_route_tes
-00021500: 745f 7374 7275 6374 7572 6528 6e75 6d5f  t_structure(num_
-00021510: 7669 6173 3d31 322c 2070 6164 5f73 697a  vias=12, pad_siz
-00021520: 653d 2831 3030 2c31 3030 292c 7769 7265  e=(100,100),wire
-00021530: 5f77 6964 7468 3d38 290a 0a20 2020 2065  _width=8)..    e
-00021540: 783a 2076 6961 5f72 6f75 7465 2835 342c  x: via_route(54,
-00021550: 206d 696e 5f70 6164 5f73 7061 6369 6e67   min_pad_spacing
-00021560: 3d33 3030 290a 2020 2020 2222 220a 2020  =300).    """.  
-00021570: 2020 5652 203d 2044 6576 6963 6528 2274    VR = Device("t
-00021580: 6573 745f 7669 6122 290a 2020 2020 7061  est_via").    pa
-00021590: 6431 203d 2056 522e 6164 645f 7265 6628  d1 = VR.add_ref(
-000215a0: 7265 6374 616e 676c 6528 7369 7a65 3d70  rectangle(size=p
-000215b0: 6164 5f73 697a 652c 206c 6179 6572 3d70  ad_size, layer=p
-000215c0: 6164 5f6c 6179 6572 2929 0a20 2020 2070  ad_layer)).    p
-000215d0: 6164 315f 6f76 6572 6c61 7920 3d20 5652  ad1_overlay = VR
-000215e0: 2e61 6464 5f72 6566 2872 6563 7461 6e67  .add_ref(rectang
-000215f0: 6c65 2873 697a 653d 7061 645f 7369 7a65  le(size=pad_size
-00021600: 2c20 6c61 7965 723d 7769 7269 6e67 315f  , layer=wiring1_
-00021610: 6c61 7965 7229 290a 2020 2020 7061 6432  layer)).    pad2
-00021620: 203d 2056 522e 6164 645f 7265 6628 7265   = VR.add_ref(re
-00021630: 6374 616e 676c 6528 7369 7a65 3d70 6164  ctangle(size=pad
-00021640: 5f73 697a 652c 206c 6179 6572 3d70 6164  _size, layer=pad
-00021650: 5f6c 6179 6572 2929 0a20 2020 2070 6164  _layer)).    pad
-00021660: 325f 6f76 6572 6c61 7920 3d20 5652 2e61  2_overlay = VR.a
-00021670: 6464 5f72 6566 2872 6563 7461 6e67 6c65  dd_ref(rectangle
-00021680: 2873 697a 653d 7061 645f 7369 7a65 2c20  (size=pad_size, 
-00021690: 6c61 7965 723d 7769 7269 6e67 315f 6c61  layer=wiring1_la
-000216a0: 7965 7229 290a 2020 2020 6e75 6220 3d20  yer)).    nub = 
-000216b0: 5652 2e61 6464 5f72 6566 2863 6f6d 7061  VR.add_ref(compa
-000216c0: 7373 2873 697a 653d 2833 202a 2077 6972  ss(size=(3 * wir
-000216d0: 655f 7769 6474 682c 2077 6972 655f 7769  e_width, wire_wi
-000216e0: 6474 6829 2c20 6c61 7965 723d 7061 645f  dth), layer=pad_
-000216f0: 6c61 7965 7229 290a 2020 2020 6e75 625f  layer)).    nub_
-00021700: 6f76 6572 6c61 7920 3d20 5652 2e61 6464  overlay = VR.add
-00021710: 5f72 6566 280a 2020 2020 2020 2020 636f  _ref(.        co
-00021720: 6d70 6173 7328 7369 7a65 3d28 3320 2a20  mpass(size=(3 * 
-00021730: 7769 7265 5f77 6964 7468 2c20 7769 7265  wire_width, wire
-00021740: 5f77 6964 7468 292c 206c 6179 6572 3d77  _width), layer=w
-00021750: 6972 696e 6731 5f6c 6179 6572 290a 2020  iring1_layer).  
-00021760: 2020 290a 2020 2020 6865 6164 203d 2056    ).    head = V
-00021770: 522e 6164 645f 7265 6628 636f 6d70 6173  R.add_ref(compas
-00021780: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
-00021790: 7468 2c20 7769 7265 5f77 6964 7468 292c  th, wire_width),
-000217a0: 206c 6179 6572 3d70 6164 5f6c 6179 6572   layer=pad_layer
-000217b0: 2929 0a20 2020 2068 6561 645f 6f76 6572  )).    head_over
-000217c0: 6c61 7920 3d20 5652 2e61 6464 5f72 6566  lay = VR.add_ref
-000217d0: 280a 2020 2020 2020 2020 636f 6d70 6173  (.        compas
-000217e0: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
-000217f0: 7468 2c20 7769 7265 5f77 6964 7468 292c  th, wire_width),
-00021800: 206c 6179 6572 3d77 6972 696e 6731 5f6c   layer=wiring1_l
-00021810: 6179 6572 290a 2020 2020 290a 2020 2020  ayer).    ).    
-00021820: 6e75 622e 796d 6178 203d 2070 6164 312e  nub.ymax = pad1.
-00021830: 796d 6178 202d 2035 0a20 2020 206e 7562  ymax - 5.    nub
-00021840: 2e78 6d69 6e20 3d20 7061 6431 2e78 6d61  .xmin = pad1.xma
-00021850: 780a 2020 2020 6e75 625f 6f76 6572 6c61  x.    nub_overla
-00021860: 792e 796d 6178 203d 2070 6164 312e 796d  y.ymax = pad1.ym
-00021870: 6178 202d 2035 0a20 2020 206e 7562 5f6f  ax - 5.    nub_o
-00021880: 7665 726c 6179 2e78 6d69 6e20 3d20 7061  verlay.xmin = pa
-00021890: 6431 2e78 6d61 780a 2020 2020 6865 6164  d1.xmax.    head
-000218a0: 2e63 6f6e 6e65 6374 2870 6f72 743d 2257  .connect(port="W
-000218b0: 222c 2064 6573 7469 6e61 7469 6f6e 3d6e  ", destination=n
-000218c0: 7562 2e70 6f72 7473 5b22 4522 5d29 0a20  ub.ports["E"]). 
-000218d0: 2020 2068 6561 645f 6f76 6572 6c61 792e     head_overlay.
-000218e0: 636f 6e6e 6563 7428 706f 7274 3d22 5722  connect(port="W"
-000218f0: 2c20 6465 7374 696e 6174 696f 6e3d 6e75  , destination=nu
-00021900: 625f 6f76 6572 6c61 792e 706f 7274 735b  b_overlay.ports[
-00021910: 2245 225d 290a 2020 2020 7061 6431 5f6f  "E"]).    pad1_o
-00021920: 7665 726c 6179 2e78 6d69 6e20 3d20 7061  verlay.xmin = pa
-00021930: 6431 2e78 6d69 6e0a 2020 2020 7061 6431  d1.xmin.    pad1
-00021940: 5f6f 7665 726c 6179 2e79 6d69 6e20 3d20  _overlay.ymin = 
-00021950: 7061 6431 2e79 6d69 6e0a 0a20 2020 206f  pad1.ymin..    o
-00021960: 6c64 5f70 6f72 7420 3d20 6865 6164 2e70  ld_port = head.p
-00021970: 6f72 7473 5b22 5322 5d0a 2020 2020 636f  orts["S"].    co
-00021980: 756e 7420 3d20 300a 2020 2020 7769 6474  unt = 0.    widt
-00021990: 685f 7669 615f 6974 6572 203d 2032 202a  h_via_iter = 2 *
-000219a0: 2076 6961 5f73 7061 6369 6e67 202d 2032   via_spacing - 2
-000219b0: 202a 2077 6972 655f 7769 6474 680a 0a20   * wire_width.. 
-000219c0: 2020 2070 6164 322e 786d 696e 203d 2070     pad2.xmin = p
-000219d0: 6164 312e 786d 6178 202b 206d 696e 5f70  ad1.xmax + min_p
-000219e0: 6164 5f73 7061 6369 6e67 0a20 2020 2075  ad_spacing.    u
-000219f0: 7020 3d20 4661 6c73 650a 2020 2020 646f  p = False.    do
-00021a00: 776e 203d 2054 7275 650a 2020 2020 6564  wn = True.    ed
-00021a10: 6765 203d 2054 7275 650a 2020 2020 6375  ge = True.    cu
-00021a20: 7272 656e 745f 7769 6474 6820 3d20 3320  rrent_width = 3 
-00021a30: 2a20 7769 7265 5f77 6964 7468 202b 2077  * wire_width + w
-00021a40: 6972 655f 7769 6474 6820 2023 2077 6964  ire_width  # wid
-00021a50: 7468 206f 6620 6e75 6220 616e 6420 3120  th of nub and 1 
-00021a60: 6f76 6572 6c61 700a 2020 2020 6f62 6a5f  overlap.    obj_
-00021a70: 6f6c 6420 3d20 6865 6164 0a20 2020 206f  old = head.    o
-00021a80: 626a 203d 2068 6561 640a 2020 2020 7669  bj = head.    vi
-00021a90: 615f 6974 6572 6162 6c65 203d 205f 7669  a_iterable = _vi
-00021aa0: 615f 6974 6572 6162 6c65 280a 2020 2020  a_iterable(.    
-00021ab0: 2020 2020 7669 615f 7370 6163 696e 672c      via_spacing,
-00021ac0: 2077 6972 655f 7769 6474 682c 2077 6972   wire_width, wir
-00021ad0: 696e 6731 5f6c 6179 6572 2c20 7769 7269  ing1_layer, wiri
-00021ae0: 6e67 325f 6c61 7965 722c 2076 6961 5f6c  ng2_layer, via_l
-00021af0: 6179 6572 2c20 7669 615f 7769 6474 680a  ayer, via_width.
-00021b00: 2020 2020 290a 2020 2020 7768 696c 6520      ).    while 
-00021b10: 2863 6f75 6e74 202b 2032 2920 3c3d 206e  (count + 2) <= n
-00021b20: 756d 5f76 6961 733a 0a20 2020 2020 2020  um_vias:.       
-00021b30: 206f 626a 203d 2056 522e 6164 645f 7265   obj = VR.add_re
-00021b40: 6628 7669 615f 6974 6572 6162 6c65 290a  f(via_iterable).
-00021b50: 2020 2020 2020 2020 6f62 6a2e 636f 6e6e          obj.conn
-00021b60: 6563 7428 706f 7274 3d22 5722 2c20 6465  ect(port="W", de
-00021b70: 7374 696e 6174 696f 6e3d 6f6c 645f 706f  stination=old_po
-00021b80: 7274 2c20 6f76 6572 6c61 703d 7769 7265  rt, overlap=wire
-00021b90: 5f77 6964 7468 290a 2020 2020 2020 2020  _width).        
-00021ba0: 6f6c 645f 706f 7274 203d 206f 626a 2e70  old_port = obj.p
-00021bb0: 6f72 7473 5b22 4522 5d0a 2020 2020 2020  orts["E"].      
-00021bc0: 2020 6564 6765 203d 2046 616c 7365 0a20    edge = False. 
-00021bd0: 2020 2020 2020 2069 6620 6f62 6a2e 796d         if obj.ym
-00021be0: 6178 203e 2070 6164 312e 796d 6178 3a0a  ax > pad1.ymax:.
-00021bf0: 2020 2020 2020 2020 2020 2020 6f62 6a2e              obj.
-00021c00: 636f 6e6e 6563 7428 706f 7274 3d22 5722  connect(port="W"
-00021c10: 2c20 6465 7374 696e 6174 696f 6e3d 6f62  , destination=ob
-00021c20: 6a5f 6f6c 642e 706f 7274 735b 2253 225d  j_old.ports["S"]
-00021c30: 2c20 6f76 6572 6c61 703d 7769 7265 5f77  , overlap=wire_w
-00021c40: 6964 7468 290a 2020 2020 2020 2020 2020  idth).          
-00021c50: 2020 6f6c 645f 706f 7274 203d 206f 626a    old_port = obj
-00021c60: 2e70 6f72 7473 5b22 5322 5d0a 2020 2020  .ports["S"].    
-00021c70: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00021c80: 7769 6474 6820 2b3d 2077 6964 7468 5f76  width += width_v
-00021c90: 6961 5f69 7465 720a 2020 2020 2020 2020  ia_iter.        
-00021ca0: 2020 2020 646f 776e 203d 2054 7275 650a      down = True.
-00021cb0: 2020 2020 2020 2020 2020 2020 7570 203d              up =
-00021cc0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00021cd0: 2020 2065 6467 6520 3d20 5472 7565 0a0a     edge = True..
-00021ce0: 2020 2020 2020 2020 656c 6966 206f 626a          elif obj
-00021cf0: 2e79 6d69 6e20 3c20 7061 6431 2e79 6d69  .ymin < pad1.ymi
-00021d00: 6e3a 0a20 2020 2020 2020 2020 2020 206f  n:.            o
-00021d10: 626a 2e63 6f6e 6e65 6374 2870 6f72 743d  bj.connect(port=
-00021d20: 2257 222c 2064 6573 7469 6e61 7469 6f6e  "W", destination
-00021d30: 3d6f 626a 5f6f 6c64 2e70 6f72 7473 5b22  =obj_old.ports["
-00021d40: 4e22 5d2c 206f 7665 726c 6170 3d77 6972  N"], overlap=wir
-00021d50: 655f 7769 6474 6829 0a20 2020 2020 2020  e_width).       
-00021d60: 2020 2020 206f 6c64 5f70 6f72 7420 3d20       old_port = 
-00021d70: 6f62 6a2e 706f 7274 735b 224e 225d 0a20  obj.ports["N"]. 
-00021d80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00021d90: 6e74 5f77 6964 7468 202b 3d20 7769 6474  nt_width += widt
-00021da0: 685f 7669 615f 6974 6572 0a20 2020 2020  h_via_iter.     
-00021db0: 2020 2020 2020 2075 7020 3d20 5472 7565         up = True
-00021dc0: 0a20 2020 2020 2020 2020 2020 2064 6f77  .            dow
-00021dd0: 6e20 3d20 4661 6c73 650a 2020 2020 2020  n = False.      
-00021de0: 2020 2020 2020 6564 6765 203d 2054 7275        edge = Tru
-00021df0: 650a 2020 2020 2020 2020 636f 756e 7420  e.        count 
-00021e00: 3d20 636f 756e 7420 2b20 320a 2020 2020  = count + 2.    
-00021e10: 2020 2020 6f62 6a5f 6f6c 6420 3d20 6f62      obj_old = ob
-00021e20: 6a0a 0a20 2020 2069 6620 280a 2020 2020  j..    if (.    
-00021e30: 2020 2020 6375 7272 656e 745f 7769 6474      current_widt
-00021e40: 6820 3c20 6d69 6e5f 7061 645f 7370 6163  h < min_pad_spac
-00021e50: 696e 670a 2020 2020 2020 2020 616e 6420  ing.        and 
-00021e60: 286d 696e 5f70 6164 5f73 7061 6369 6e67  (min_pad_spacing
-00021e70: 202d 2063 7572 7265 6e74 5f77 6964 7468   - current_width
-00021e80: 2920 3e20 3320 2a20 7769 7265 5f77 6964  ) > 3 * wire_wid
-00021e90: 7468 0a20 2020 2029 3a0a 2020 2020 2020  th.    ):.      
-00021ea0: 2020 7461 696c 203d 2056 522e 6164 645f    tail = VR.add_
-00021eb0: 7265 6628 0a20 2020 2020 2020 2020 2020  ref(.           
-00021ec0: 2063 6f6d 7061 7373 280a 2020 2020 2020   compass(.      
-00021ed0: 2020 2020 2020 2020 2020 7369 7a65 3d28            size=(
+00020890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000208a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+000208b0: 230a 2320 5465 7374 2053 7472 7563 7475  #.# Test Structu
+000208c0: 7265 730a 230a 2320 3d3d 3d3d 3d3d 3d3d  res.#.# ========
+000208d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000208e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000208f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020900: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00020910: 3d3d 3d3d 3d3d 0a0a 2320 5669 6120 526f  ======..# Via Ro
+00020920: 7574 6520 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ute ------------
+00020930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00020940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a64 6566  ------------.def
+00020950: 205f 7669 615f 6974 6572 6162 6c65 280a   _via_iterable(.
+00020960: 2020 2020 7669 615f 7370 6163 696e 672c      via_spacing,
+00020970: 2077 6972 655f 7769 6474 682c 2077 6972   wire_width, wir
+00020980: 696e 6731 5f6c 6179 6572 2c20 7769 7269  ing1_layer, wiri
+00020990: 6e67 325f 6c61 7965 722c 2076 6961 5f6c  ng2_layer, via_l
+000209a0: 6179 6572 2c20 7669 615f 7769 6474 680a  ayer, via_width.
+000209b0: 293a 0a20 2020 2022 2222 4865 6c70 6572  ):.    """Helper
+000209c0: 2066 756e 6374 696f 6e20 666f 7220 7465   function for te
+000209d0: 7374 5f76 6961 0a0a 2020 2020 5061 7261  st_via..    Para
+000209e0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+000209f0: 2d2d 2d2d 2d0a 2020 2020 7669 615f 7370  -----.    via_sp
+00020a00: 6163 696e 6720 3a20 696e 7420 6f72 2066  acing : int or f
+00020a10: 6c6f 6174 0a20 2020 2020 2020 2044 6973  loat.        Dis
+00020a20: 7461 6e63 6520 6265 7477 6565 6e20 7669  tance between vi
+00020a30: 6173 2e0a 2020 2020 7769 7265 5f77 6964  as..    wire_wid
+00020a40: 7468 203a 2069 6e74 206f 7220 666c 6f61  th : int or floa
+00020a50: 740a 2020 2020 2020 2020 5468 6520 7769  t.        The wi
+00020a60: 6474 6820 6f66 2074 6865 2077 6972 6573  dth of the wires
+00020a70: 2e0a 2020 2020 7769 7269 6e67 315f 6c61  ..    wiring1_la
+00020a80: 7965 7220 3a20 696e 740a 2020 2020 2020  yer : int.      
+00020a90: 2020 5370 6563 6966 6963 206c 6179 6572    Specific layer
+00020aa0: 2074 6f20 7075 7420 7468 6520 746f 7020   to put the top 
+00020ab0: 7769 7269 6e67 206f 6e2e 0a20 2020 2077  wiring on..    w
+00020ac0: 6972 696e 6732 5f6c 6179 6572 203a 2069  iring2_layer : i
+00020ad0: 6e74 0a20 2020 2020 2020 2053 7065 6369  nt.        Speci
+00020ae0: 6669 6320 6c61 7965 7220 746f 2070 7574  fic layer to put
+00020af0: 2074 6865 2062 6f74 746f 6d20 7769 7269   the bottom wiri
+00020b00: 6e67 206f 6e2e 0a20 2020 2076 6961 5f6c  ng on..    via_l
+00020b10: 6179 6572 203a 2069 6e74 0a20 2020 2020  ayer : int.     
+00020b20: 2020 2053 7065 6369 6669 6320 6c61 7965     Specific laye
+00020b30: 7220 746f 2070 7574 2074 6865 2076 6961  r to put the via
+00020b40: 7320 6f6e 2e0a 2020 2020 7669 615f 7769  s on..    via_wi
+00020b50: 6474 6820 3a20 696e 7420 6f72 2066 6c6f  dth : int or flo
+00020b60: 6174 0a20 2020 2020 2020 2044 6961 6d65  at.        Diame
+00020b70: 7465 7220 6f66 2074 6865 2076 6961 732e  ter of the vias.
+00020b80: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00020b90: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 5649    -------.    VI
+00020ba0: 203a 2044 6576 6963 650a 0a20 2020 2022   : Device..    "
+00020bb0: 2222 0a20 2020 2056 4920 3d20 4465 7669  "".    VI = Devi
+00020bc0: 6365 2822 7465 7374 5f76 6961 5f69 7465  ce("test_via_ite
+00020bd0: 7222 290a 2020 2020 7769 7265 3120 3d20  r").    wire1 = 
+00020be0: 5649 2e61 6464 5f72 6566 2863 6f6d 7061  VI.add_ref(compa
+00020bf0: 7373 2873 697a 653d 2876 6961 5f73 7061  ss(size=(via_spa
+00020c00: 6369 6e67 2c20 7769 7265 5f77 6964 7468  cing, wire_width
+00020c10: 292c 206c 6179 6572 3d77 6972 696e 6731  ), layer=wiring1
+00020c20: 5f6c 6179 6572 2929 0a20 2020 2077 6972  _layer)).    wir
+00020c30: 6532 203d 2056 492e 6164 645f 7265 6628  e2 = VI.add_ref(
+00020c40: 636f 6d70 6173 7328 7369 7a65 3d28 7669  compass(size=(vi
+00020c50: 615f 7370 6163 696e 672c 2077 6972 655f  a_spacing, wire_
+00020c60: 7769 6474 6829 2c20 6c61 7965 723d 7769  width), layer=wi
+00020c70: 7269 6e67 325f 6c61 7965 7229 290a 2020  ring2_layer)).  
+00020c80: 2020 7669 6131 203d 2056 492e 6164 645f    via1 = VI.add_
+00020c90: 7265 6628 636f 6d70 6173 7328 7369 7a65  ref(compass(size
+00020ca0: 3d28 7669 615f 7769 6474 682c 2076 6961  =(via_width, via
+00020cb0: 5f77 6964 7468 292c 206c 6179 6572 3d76  _width), layer=v
+00020cc0: 6961 5f6c 6179 6572 2929 0a20 2020 2076  ia_layer)).    v
+00020cd0: 6961 3220 3d20 5649 2e61 6464 5f72 6566  ia2 = VI.add_ref
+00020ce0: 2863 6f6d 7061 7373 2873 697a 653d 2876  (compass(size=(v
+00020cf0: 6961 5f77 6964 7468 2c20 7669 615f 7769  ia_width, via_wi
+00020d00: 6474 6829 2c20 6c61 7965 723d 7669 615f  dth), layer=via_
+00020d10: 6c61 7965 7229 290a 2020 2020 7769 7265  layer)).    wire
+00020d20: 312e 636f 6e6e 6563 7428 706f 7274 3d22  1.connect(port="
+00020d30: 4522 2c20 6465 7374 696e 6174 696f 6e3d  E", destination=
+00020d40: 7769 7265 322e 706f 7274 735b 2257 225d  wire2.ports["W"]
+00020d50: 2c20 6f76 6572 6c61 703d 7769 7265 5f77  , overlap=wire_w
+00020d60: 6964 7468 290a 2020 2020 7669 6131 2e63  idth).    via1.c
+00020d70: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+00020d80: 706f 7274 3d22 5722 2c20 6465 7374 696e  port="W", destin
+00020d90: 6174 696f 6e3d 7769 7265 312e 706f 7274  ation=wire1.port
+00020da0: 735b 2245 225d 2c20 6f76 6572 6c61 703d  s["E"], overlap=
+00020db0: 2877 6972 655f 7769 6474 6820 2b20 7669  (wire_width + vi
+00020dc0: 615f 7769 6474 6829 202f 2032 0a20 2020  a_width) / 2.   
+00020dd0: 2029 0a20 2020 2076 6961 322e 636f 6e6e   ).    via2.conn
+00020de0: 6563 7428 0a20 2020 2020 2020 2070 6f72  ect(.        por
+00020df0: 743d 2257 222c 2064 6573 7469 6e61 7469  t="W", destinati
+00020e00: 6f6e 3d77 6972 6532 2e70 6f72 7473 5b22  on=wire2.ports["
+00020e10: 4522 5d2c 206f 7665 726c 6170 3d28 7769  E"], overlap=(wi
+00020e20: 7265 5f77 6964 7468 202b 2076 6961 5f77  re_width + via_w
+00020e30: 6964 7468 2920 2f20 320a 2020 2020 290a  idth) / 2.    ).
+00020e40: 2020 2020 5649 2e61 6464 5f70 6f72 7428      VI.add_port(
+00020e50: 6e61 6d65 3d22 5722 2c20 706f 7274 3d77  name="W", port=w
+00020e60: 6972 6531 2e70 6f72 7473 5b22 5722 5d29  ire1.ports["W"])
+00020e70: 0a20 2020 2056 492e 6164 645f 706f 7274  .    VI.add_port
+00020e80: 286e 616d 653d 2245 222c 2070 6f72 743d  (name="E", port=
+00020e90: 7769 7265 322e 706f 7274 735b 2245 225d  wire2.ports["E"]
+00020ea0: 290a 2020 2020 5649 2e61 6464 5f70 6f72  ).    VI.add_por
+00020eb0: 7428 0a20 2020 2020 2020 206e 616d 653d  t(.        name=
+00020ec0: 2253 222c 0a20 2020 2020 2020 206d 6964  "S",.        mid
+00020ed0: 706f 696e 743d 5b28 3120 2a20 7769 7265  point=[(1 * wire
+00020ee0: 5f77 6964 7468 2920 2b20 7769 7265 5f77  _width) + wire_w
+00020ef0: 6964 7468 202f 2032 2c20 2d77 6972 655f  idth / 2, -wire_
+00020f00: 7769 6474 6820 2f20 325d 2c0a 2020 2020  width / 2],.    
+00020f10: 2020 2020 7769 6474 683d 7769 7265 5f77      width=wire_w
+00020f20: 6964 7468 2c0a 2020 2020 2020 2020 6f72  idth,.        or
+00020f30: 6965 6e74 6174 696f 6e3d 2d39 302c 0a20  ientation=-90,. 
+00020f40: 2020 2029 0a20 2020 2056 492e 6164 645f     ).    VI.add_
+00020f50: 706f 7274 280a 2020 2020 2020 2020 6e61  port(.        na
+00020f60: 6d65 3d22 4e22 2c0a 2020 2020 2020 2020  me="N",.        
+00020f70: 6d69 6470 6f69 6e74 3d5b 2831 202a 2077  midpoint=[(1 * w
+00020f80: 6972 655f 7769 6474 6829 202b 2077 6972  ire_width) + wir
+00020f90: 655f 7769 6474 6820 2f20 322c 2077 6972  e_width / 2, wir
+00020fa0: 655f 7769 6474 6820 2f20 325d 2c0a 2020  e_width / 2],.  
+00020fb0: 2020 2020 2020 7769 6474 683d 7769 7265        width=wire
+00020fc0: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
+00020fd0: 6f72 6965 6e74 6174 696f 6e3d 3930 2c0a  orientation=90,.
+00020fe0: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
+00020ff0: 6e20 5649 0a0a 0a64 6566 2074 6573 745f  n VI...def test_
+00021000: 7669 6128 0a20 2020 206e 756d 5f76 6961  via(.    num_via
+00021010: 733d 3130 302c 0a20 2020 2077 6972 655f  s=100,.    wire_
+00021020: 7769 6474 683d 3130 2c0a 2020 2020 7669  width=10,.    vi
+00021030: 615f 7769 6474 683d 3135 2c0a 2020 2020  a_width=15,.    
+00021040: 7669 615f 7370 6163 696e 673d 3430 2c0a  via_spacing=40,.
+00021050: 2020 2020 7061 645f 7369 7a65 3d28 3330      pad_size=(30
+00021060: 302c 2033 3030 292c 0a20 2020 206d 696e  0, 300),.    min
+00021070: 5f70 6164 5f73 7061 6369 6e67 3d30 2c0a  _pad_spacing=0,.
+00021080: 2020 2020 7061 645f 6c61 7965 723d 302c      pad_layer=0,
+00021090: 0a20 2020 2077 6972 696e 6731 5f6c 6179  .    wiring1_lay
+000210a0: 6572 3d31 2c0a 2020 2020 7769 7269 6e67  er=1,.    wiring
+000210b0: 325f 6c61 7965 723d 322c 0a20 2020 2076  2_layer=2,.    v
+000210c0: 6961 5f6c 6179 6572 3d33 2c0a 293a 0a20  ia_layer=3,.):. 
+000210d0: 2020 2022 2222 5669 6120 6368 6169 6e20     """Via chain 
+000210e0: 7465 7374 2073 7472 7563 7475 7265 0a0a  test structure..
+000210f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00021100: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00021110: 2020 6e75 6d5f 7669 6173 203a 2069 6e74    num_vias : int
+00021120: 0a20 2020 2020 2020 2054 6865 2074 6f74  .        The tot
+00021130: 616c 206e 756d 6265 7220 6f66 2072 6571  al number of req
+00021140: 7565 7374 6564 2076 6961 7320 286d 7573  uested vias (mus
+00021150: 7420 6265 2061 6e20 6576 656e 206e 756d  t be an even num
+00021160: 6265 7229 2e0a 2020 2020 7769 7265 5f77  ber)..    wire_w
+00021170: 6964 7468 203a 2069 6e74 206f 7220 666c  idth : int or fl
+00021180: 6f61 740a 2020 2020 2020 2020 5468 6520  oat.        The 
+00021190: 7769 6474 6820 6f66 2074 6865 2077 6972  width of the wir
+000211a0: 6573 2e0a 2020 2020 7669 615f 7769 6474  es..    via_widt
+000211b0: 6820 3a20 696e 7420 6f72 2066 6c6f 6174  h : int or float
+000211c0: 0a20 2020 2020 2020 2044 6961 6d65 7465  .        Diamete
+000211d0: 7220 6f66 2074 6865 2076 6961 732e 0a20  r of the vias.. 
+000211e0: 2020 2076 6961 5f73 7061 6369 6e67 203a     via_spacing :
+000211f0: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
+00021200: 2020 2020 2020 4469 7374 616e 6365 2062        Distance b
+00021210: 6574 7765 656e 2076 6961 732e 0a20 2020  etween vias..   
+00021220: 2070 6164 5f73 697a 6520 3a20 6172 7261   pad_size : arra
+00021230: 792d 6c69 6b65 5b32 5d0a 2020 2020 2020  y-like[2].      
+00021240: 2020 2877 6964 7468 2c20 6865 6967 6874    (width, height
+00021250: 2920 6f66 2074 6865 2070 6164 732e 0a20  ) of the pads.. 
+00021260: 2020 206d 696e 5f70 6164 5f73 7061 6369     min_pad_spaci
+00021270: 6e67 203a 2069 6e74 206f 7220 666c 6f61  ng : int or floa
+00021280: 740a 2020 2020 2020 2020 4465 6669 6e65  t.        Define
+00021290: 7320 7468 6520 6d69 6e69 6d75 6d20 6469  s the minimum di
+000212a0: 7374 616e 6365 2062 6574 7765 656e 2074  stance between t
+000212b0: 6865 2074 776f 2070 6164 732e 0a20 2020  he two pads..   
+000212c0: 2070 6164 5f6c 6179 6572 203a 2069 6e74   pad_layer : int
+000212d0: 0a20 2020 2020 2020 2053 7065 6369 6669  .        Specifi
+000212e0: 6320 6c61 7965 7220 746f 2070 7574 2074  c layer to put t
+000212f0: 6865 2070 6164 7320 6f6e 2e0a 2020 2020  he pads on..    
+00021300: 7769 7269 6e67 315f 6c61 7965 7220 3a20  wiring1_layer : 
+00021310: 696e 740a 2020 2020 2020 2020 5370 6563  int.        Spec
+00021320: 6966 6963 206c 6179 6572 2074 6f20 7075  ific layer to pu
+00021330: 7420 7468 6520 746f 7020 7769 7269 6e67  t the top wiring
+00021340: 206f 6e2e 0a20 2020 2077 6972 696e 6732   on..    wiring2
+00021350: 5f6c 6179 6572 203a 2069 6e74 0a20 2020  _layer : int.   
+00021360: 2020 2020 2053 7065 6369 6669 6320 6c61       Specific la
+00021370: 7965 7220 746f 2070 7574 2074 6865 2062  yer to put the b
+00021380: 6f74 746f 6d20 7769 7269 6e67 206f 6e2e  ottom wiring on.
+00021390: 0a20 2020 2076 6961 5f6c 6179 6572 203a  .    via_layer :
+000213a0: 2069 6e74 0a20 2020 2020 2020 2053 7065   int.        Spe
+000213b0: 6369 6669 6320 6c61 7965 7220 746f 2070  cific layer to p
+000213c0: 7574 2074 6865 2076 6961 7320 6f6e 2e0a  ut the vias on..
+000213d0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+000213e0: 202d 2d2d 2d2d 2d2d 0a20 2020 2056 5220   -------.    VR 
+000213f0: 3a20 4465 7669 6365 0a20 2020 2020 2020  : Device.       
+00021400: 2041 2044 6576 6963 6520 636f 6e74 6169   A Device contai
+00021410: 6e69 6e67 2074 6865 2074 6573 7420 7669  ning the test vi
+00021420: 6120 7374 7275 6374 7572 6573 2e0a 0a20  a structures... 
+00021430: 2020 2055 7361 6765 0a20 2020 202d 2d2d     Usage.    ---
+00021440: 2d2d 0a20 2020 2043 616c 6c20 7669 615f  --.    Call via_
+00021450: 726f 7574 655f 7465 7374 5f73 7472 7563  route_test_struc
+00021460: 7475 7265 2829 2062 7920 696e 6469 6361  ture() by indica
+00021470: 7469 6e67 2074 6865 206e 756d 6265 7220  ting the number 
+00021480: 6f66 2076 6961 7320 796f 7520 7761 6e74  of vias you want
+00021490: 0a20 2020 2064 7261 776e 2e20 596f 7520  .    drawn. You 
+000214a0: 6361 6e20 616c 736f 2063 6861 6e67 6520  can also change 
+000214b0: 7468 6520 6f74 6865 7220 7061 7261 6d65  the other parame
+000214c0: 7465 7273 2068 6f77 6576 6572 2069 6620  ters however if 
+000214d0: 796f 7520 646f 206e 6f74 0a20 2020 2073  you do not.    s
+000214e0: 7065 6369 6669 7920 6120 7661 6c75 6520  pecifiy a value 
+000214f0: 666f 7220 6120 7061 7261 6d65 7465 7220  for a parameter 
+00021500: 6974 2077 696c 6c20 6a75 7374 2075 7365  it will just use
+00021510: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
+00021520: 7565 0a20 2020 2045 783a 3a0a 0a20 2020  ue.    Ex::..   
+00021530: 2020 2020 2076 6961 5f72 6f75 7465 5f74       via_route_t
+00021540: 6573 745f 7374 7275 6374 7572 6528 6e75  est_structure(nu
+00021550: 6d5f 7669 6173 3d35 3429 0a0a 2020 2020  m_vias=54)..    
+00021560: 2d20 6f72 202d 3a3a 0a0a 2020 2020 2020  - or -::..      
+00021570: 2020 7669 615f 726f 7574 655f 7465 7374    via_route_test
+00021580: 5f73 7472 7563 7475 7265 286e 756d 5f76  _structure(num_v
+00021590: 6961 733d 3132 2c20 7061 645f 7369 7a65  ias=12, pad_size
+000215a0: 3d28 3130 302c 3130 3029 2c77 6972 655f  =(100,100),wire_
+000215b0: 7769 6474 683d 3829 0a0a 2020 2020 6578  width=8)..    ex
+000215c0: 3a20 7669 615f 726f 7574 6528 3534 2c20  : via_route(54, 
+000215d0: 6d69 6e5f 7061 645f 7370 6163 696e 673d  min_pad_spacing=
+000215e0: 3330 3029 0a20 2020 2022 2222 0a20 2020  300).    """.   
+000215f0: 2056 5220 3d20 4465 7669 6365 2822 7465   VR = Device("te
+00021600: 7374 5f76 6961 2229 0a20 2020 2070 6164  st_via").    pad
+00021610: 3120 3d20 5652 2e61 6464 5f72 6566 2872  1 = VR.add_ref(r
+00021620: 6563 7461 6e67 6c65 2873 697a 653d 7061  ectangle(size=pa
+00021630: 645f 7369 7a65 2c20 6c61 7965 723d 7061  d_size, layer=pa
+00021640: 645f 6c61 7965 7229 290a 2020 2020 7061  d_layer)).    pa
+00021650: 6431 5f6f 7665 726c 6179 203d 2056 522e  d1_overlay = VR.
+00021660: 6164 645f 7265 6628 7265 6374 616e 676c  add_ref(rectangl
+00021670: 6528 7369 7a65 3d70 6164 5f73 697a 652c  e(size=pad_size,
+00021680: 206c 6179 6572 3d77 6972 696e 6731 5f6c   layer=wiring1_l
+00021690: 6179 6572 2929 0a20 2020 2070 6164 3220  ayer)).    pad2 
+000216a0: 3d20 5652 2e61 6464 5f72 6566 2872 6563  = VR.add_ref(rec
+000216b0: 7461 6e67 6c65 2873 697a 653d 7061 645f  tangle(size=pad_
+000216c0: 7369 7a65 2c20 6c61 7965 723d 7061 645f  size, layer=pad_
+000216d0: 6c61 7965 7229 290a 2020 2020 7061 6432  layer)).    pad2
+000216e0: 5f6f 7665 726c 6179 203d 2056 522e 6164  _overlay = VR.ad
+000216f0: 645f 7265 6628 7265 6374 616e 676c 6528  d_ref(rectangle(
+00021700: 7369 7a65 3d70 6164 5f73 697a 652c 206c  size=pad_size, l
+00021710: 6179 6572 3d77 6972 696e 6731 5f6c 6179  ayer=wiring1_lay
+00021720: 6572 2929 0a20 2020 206e 7562 203d 2056  er)).    nub = V
+00021730: 522e 6164 645f 7265 6628 636f 6d70 6173  R.add_ref(compas
+00021740: 7328 7369 7a65 3d28 3320 2a20 7769 7265  s(size=(3 * wire
+00021750: 5f77 6964 7468 2c20 7769 7265 5f77 6964  _width, wire_wid
+00021760: 7468 292c 206c 6179 6572 3d70 6164 5f6c  th), layer=pad_l
+00021770: 6179 6572 2929 0a20 2020 206e 7562 5f6f  ayer)).    nub_o
+00021780: 7665 726c 6179 203d 2056 522e 6164 645f  verlay = VR.add_
+00021790: 7265 6628 0a20 2020 2020 2020 2063 6f6d  ref(.        com
+000217a0: 7061 7373 2873 697a 653d 2833 202a 2077  pass(size=(3 * w
+000217b0: 6972 655f 7769 6474 682c 2077 6972 655f  ire_width, wire_
+000217c0: 7769 6474 6829 2c20 6c61 7965 723d 7769  width), layer=wi
+000217d0: 7269 6e67 315f 6c61 7965 7229 0a20 2020  ring1_layer).   
+000217e0: 2029 0a20 2020 2068 6561 6420 3d20 5652   ).    head = VR
+000217f0: 2e61 6464 5f72 6566 2863 6f6d 7061 7373  .add_ref(compass
+00021800: 2873 697a 653d 2877 6972 655f 7769 6474  (size=(wire_widt
+00021810: 682c 2077 6972 655f 7769 6474 6829 2c20  h, wire_width), 
+00021820: 6c61 7965 723d 7061 645f 6c61 7965 7229  layer=pad_layer)
+00021830: 290a 2020 2020 6865 6164 5f6f 7665 726c  ).    head_overl
+00021840: 6179 203d 2056 522e 6164 645f 7265 6628  ay = VR.add_ref(
+00021850: 0a20 2020 2020 2020 2063 6f6d 7061 7373  .        compass
+00021860: 2873 697a 653d 2877 6972 655f 7769 6474  (size=(wire_widt
+00021870: 682c 2077 6972 655f 7769 6474 6829 2c20  h, wire_width), 
+00021880: 6c61 7965 723d 7769 7269 6e67 315f 6c61  layer=wiring1_la
+00021890: 7965 7229 0a20 2020 2029 0a20 2020 206e  yer).    ).    n
+000218a0: 7562 2e79 6d61 7820 3d20 7061 6431 2e79  ub.ymax = pad1.y
+000218b0: 6d61 7820 2d20 350a 2020 2020 6e75 622e  max - 5.    nub.
+000218c0: 786d 696e 203d 2070 6164 312e 786d 6178  xmin = pad1.xmax
+000218d0: 0a20 2020 206e 7562 5f6f 7665 726c 6179  .    nub_overlay
+000218e0: 2e79 6d61 7820 3d20 7061 6431 2e79 6d61  .ymax = pad1.yma
+000218f0: 7820 2d20 350a 2020 2020 6e75 625f 6f76  x - 5.    nub_ov
+00021900: 6572 6c61 792e 786d 696e 203d 2070 6164  erlay.xmin = pad
+00021910: 312e 786d 6178 0a20 2020 2068 6561 642e  1.xmax.    head.
+00021920: 636f 6e6e 6563 7428 706f 7274 3d22 5722  connect(port="W"
+00021930: 2c20 6465 7374 696e 6174 696f 6e3d 6e75  , destination=nu
+00021940: 622e 706f 7274 735b 2245 225d 290a 2020  b.ports["E"]).  
+00021950: 2020 6865 6164 5f6f 7665 726c 6179 2e63    head_overlay.c
+00021960: 6f6e 6e65 6374 2870 6f72 743d 2257 222c  onnect(port="W",
+00021970: 2064 6573 7469 6e61 7469 6f6e 3d6e 7562   destination=nub
+00021980: 5f6f 7665 726c 6179 2e70 6f72 7473 5b22  _overlay.ports["
+00021990: 4522 5d29 0a20 2020 2070 6164 315f 6f76  E"]).    pad1_ov
+000219a0: 6572 6c61 792e 786d 696e 203d 2070 6164  erlay.xmin = pad
+000219b0: 312e 786d 696e 0a20 2020 2070 6164 315f  1.xmin.    pad1_
+000219c0: 6f76 6572 6c61 792e 796d 696e 203d 2070  overlay.ymin = p
+000219d0: 6164 312e 796d 696e 0a0a 2020 2020 6f6c  ad1.ymin..    ol
+000219e0: 645f 706f 7274 203d 2068 6561 642e 706f  d_port = head.po
+000219f0: 7274 735b 2253 225d 0a20 2020 2063 6f75  rts["S"].    cou
+00021a00: 6e74 203d 2030 0a20 2020 2077 6964 7468  nt = 0.    width
+00021a10: 5f76 6961 5f69 7465 7220 3d20 3220 2a20  _via_iter = 2 * 
+00021a20: 7669 615f 7370 6163 696e 6720 2d20 3220  via_spacing - 2 
+00021a30: 2a20 7769 7265 5f77 6964 7468 0a0a 2020  * wire_width..  
+00021a40: 2020 7061 6432 2e78 6d69 6e20 3d20 7061    pad2.xmin = pa
+00021a50: 6431 2e78 6d61 7820 2b20 6d69 6e5f 7061  d1.xmax + min_pa
+00021a60: 645f 7370 6163 696e 670a 2020 2020 7570  d_spacing.    up
+00021a70: 203d 2046 616c 7365 0a20 2020 2064 6f77   = False.    dow
+00021a80: 6e20 3d20 5472 7565 0a20 2020 2065 6467  n = True.    edg
+00021a90: 6520 3d20 5472 7565 0a20 2020 2063 7572  e = True.    cur
+00021aa0: 7265 6e74 5f77 6964 7468 203d 2033 202a  rent_width = 3 *
+00021ab0: 2077 6972 655f 7769 6474 6820 2b20 7769   wire_width + wi
+00021ac0: 7265 5f77 6964 7468 2020 2320 7769 6474  re_width  # widt
+00021ad0: 6820 6f66 206e 7562 2061 6e64 2031 206f  h of nub and 1 o
+00021ae0: 7665 726c 6170 0a20 2020 206f 626a 5f6f  verlap.    obj_o
+00021af0: 6c64 203d 2068 6561 640a 2020 2020 6f62  ld = head.    ob
+00021b00: 6a20 3d20 6865 6164 0a20 2020 2076 6961  j = head.    via
+00021b10: 5f69 7465 7261 626c 6520 3d20 5f76 6961  _iterable = _via
+00021b20: 5f69 7465 7261 626c 6528 0a20 2020 2020  _iterable(.     
+00021b30: 2020 2076 6961 5f73 7061 6369 6e67 2c20     via_spacing, 
+00021b40: 7769 7265 5f77 6964 7468 2c20 7769 7269  wire_width, wiri
+00021b50: 6e67 315f 6c61 7965 722c 2077 6972 696e  ng1_layer, wirin
+00021b60: 6732 5f6c 6179 6572 2c20 7669 615f 6c61  g2_layer, via_la
+00021b70: 7965 722c 2076 6961 5f77 6964 7468 0a20  yer, via_width. 
+00021b80: 2020 2029 0a20 2020 2077 6869 6c65 2028     ).    while (
+00021b90: 636f 756e 7420 2b20 3229 203c 3d20 6e75  count + 2) <= nu
+00021ba0: 6d5f 7669 6173 3a0a 2020 2020 2020 2020  m_vias:.        
+00021bb0: 6f62 6a20 3d20 5652 2e61 6464 5f72 6566  obj = VR.add_ref
+00021bc0: 2876 6961 5f69 7465 7261 626c 6529 0a20  (via_iterable). 
+00021bd0: 2020 2020 2020 206f 626a 2e63 6f6e 6e65         obj.conne
+00021be0: 6374 2870 6f72 743d 2257 222c 2064 6573  ct(port="W", des
+00021bf0: 7469 6e61 7469 6f6e 3d6f 6c64 5f70 6f72  tination=old_por
+00021c00: 742c 206f 7665 726c 6170 3d77 6972 655f  t, overlap=wire_
+00021c10: 7769 6474 6829 0a20 2020 2020 2020 206f  width).        o
+00021c20: 6c64 5f70 6f72 7420 3d20 6f62 6a2e 706f  ld_port = obj.po
+00021c30: 7274 735b 2245 225d 0a20 2020 2020 2020  rts["E"].       
+00021c40: 2065 6467 6520 3d20 4661 6c73 650a 2020   edge = False.  
+00021c50: 2020 2020 2020 6966 206f 626a 2e79 6d61        if obj.yma
+00021c60: 7820 3e20 7061 6431 2e79 6d61 783a 0a20  x > pad1.ymax:. 
+00021c70: 2020 2020 2020 2020 2020 206f 626a 2e63             obj.c
+00021c80: 6f6e 6e65 6374 2870 6f72 743d 2257 222c  onnect(port="W",
+00021c90: 2064 6573 7469 6e61 7469 6f6e 3d6f 626a   destination=obj
+00021ca0: 5f6f 6c64 2e70 6f72 7473 5b22 5322 5d2c  _old.ports["S"],
+00021cb0: 206f 7665 726c 6170 3d77 6972 655f 7769   overlap=wire_wi
+00021cc0: 6474 6829 0a20 2020 2020 2020 2020 2020  dth).           
+00021cd0: 206f 6c64 5f70 6f72 7420 3d20 6f62 6a2e   old_port = obj.
+00021ce0: 706f 7274 735b 2253 225d 0a20 2020 2020  ports["S"].     
+00021cf0: 2020 2020 2020 2063 7572 7265 6e74 5f77         current_w
+00021d00: 6964 7468 202b 3d20 7769 6474 685f 7669  idth += width_vi
+00021d10: 615f 6974 6572 0a20 2020 2020 2020 2020  a_iter.         
+00021d20: 2020 2064 6f77 6e20 3d20 5472 7565 0a20     down = True. 
+00021d30: 2020 2020 2020 2020 2020 2075 7020 3d20             up = 
+00021d40: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00021d50: 2020 6564 6765 203d 2054 7275 650a 0a20    edge = True.. 
+00021d60: 2020 2020 2020 2065 6c69 6620 6f62 6a2e         elif obj.
+00021d70: 796d 696e 203c 2070 6164 312e 796d 696e  ymin < pad1.ymin
+00021d80: 3a0a 2020 2020 2020 2020 2020 2020 6f62  :.            ob
+00021d90: 6a2e 636f 6e6e 6563 7428 706f 7274 3d22  j.connect(port="
+00021da0: 5722 2c20 6465 7374 696e 6174 696f 6e3d  W", destination=
+00021db0: 6f62 6a5f 6f6c 642e 706f 7274 735b 224e  obj_old.ports["N
+00021dc0: 225d 2c20 6f76 6572 6c61 703d 7769 7265  "], overlap=wire
+00021dd0: 5f77 6964 7468 290a 2020 2020 2020 2020  _width).        
+00021de0: 2020 2020 6f6c 645f 706f 7274 203d 206f      old_port = o
+00021df0: 626a 2e70 6f72 7473 5b22 4e22 5d0a 2020  bj.ports["N"].  
+00021e00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00021e10: 745f 7769 6474 6820 2b3d 2077 6964 7468  t_width += width
+00021e20: 5f76 6961 5f69 7465 720a 2020 2020 2020  _via_iter.      
+00021e30: 2020 2020 2020 7570 203d 2054 7275 650a        up = True.
+00021e40: 2020 2020 2020 2020 2020 2020 646f 776e              down
+00021e50: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00021e60: 2020 2020 2065 6467 6520 3d20 5472 7565       edge = True
+00021e70: 0a20 2020 2020 2020 2063 6f75 6e74 203d  .        count =
+00021e80: 2063 6f75 6e74 202b 2032 0a20 2020 2020   count + 2.     
+00021e90: 2020 206f 626a 5f6f 6c64 203d 206f 626a     obj_old = obj
+00021ea0: 0a0a 2020 2020 6966 2028 0a20 2020 2020  ..    if (.     
+00021eb0: 2020 2063 7572 7265 6e74 5f77 6964 7468     current_width
+00021ec0: 203c 206d 696e 5f70 6164 5f73 7061 6369   < min_pad_spaci
+00021ed0: 6e67 0a20 2020 2020 2020 2061 6e64 2028  ng.        and (
 00021ee0: 6d69 6e5f 7061 645f 7370 6163 696e 6720  min_pad_spacing 
-00021ef0: 2d20 6375 7272 656e 745f 7769 6474 6820  - current_width 
-00021f00: 2b20 7769 7265 5f77 6964 7468 2c20 7769  + wire_width, wi
-00021f10: 7265 5f77 6964 7468 292c 0a20 2020 2020  re_width),.     
-00021f20: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00021f30: 3d77 6972 696e 6731 5f6c 6179 6572 2c0a  =wiring1_layer,.
-00021f40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00021f50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00021f60: 7461 696c 5f6f 7665 726c 6179 203d 2056  tail_overlay = V
-00021f70: 522e 6164 645f 7265 6628 0a20 2020 2020  R.add_ref(.     
-00021f80: 2020 2020 2020 2063 6f6d 7061 7373 280a         compass(.
-00021f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021fa0: 7369 7a65 3d28 6d69 6e5f 7061 645f 7370  size=(min_pad_sp
-00021fb0: 6163 696e 6720 2d20 6375 7272 656e 745f  acing - current_
-00021fc0: 7769 6474 6820 2b20 7769 7265 5f77 6964  width + wire_wid
-00021fd0: 7468 2c20 7769 7265 5f77 6964 7468 292c  th, wire_width),
-00021fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ff0: 206c 6179 6572 3d70 6164 5f6c 6179 6572   layer=pad_layer
-00022000: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00022010: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00022020: 7365 3a0a 2020 2020 2020 2020 7461 696c  se:.        tail
-00022030: 203d 2056 522e 6164 645f 7265 6628 0a20   = VR.add_ref(. 
-00022040: 2020 2020 2020 2020 2020 2063 6f6d 7061             compa
-00022050: 7373 2873 697a 653d 2833 202a 2077 6972  ss(size=(3 * wir
-00022060: 655f 7769 6474 682c 2077 6972 655f 7769  e_width, wire_wi
-00022070: 6474 6829 2c20 6c61 7965 723d 7769 7269  dth), layer=wiri
-00022080: 6e67 315f 6c61 7965 7229 0a20 2020 2020  ng1_layer).     
-00022090: 2020 2029 0a20 2020 2020 2020 2074 6169     ).        tai
-000220a0: 6c5f 6f76 6572 6c61 7920 3d20 5652 2e61  l_overlay = VR.a
-000220b0: 6464 5f72 6566 280a 2020 2020 2020 2020  dd_ref(.        
-000220c0: 2020 2020 636f 6d70 6173 7328 7369 7a65      compass(size
-000220d0: 3d28 3320 2a20 7769 7265 5f77 6964 7468  =(3 * wire_width
-000220e0: 2c20 7769 7265 5f77 6964 7468 292c 206c  , wire_width), l
-000220f0: 6179 6572 3d77 6972 696e 6731 5f6c 6179  ayer=wiring1_lay
-00022100: 6572 290a 2020 2020 2020 2020 290a 0a20  er).        ).. 
-00022110: 2020 2069 6620 7570 2061 6e64 206e 6f74     if up and not
-00022120: 2065 6467 653a 0a20 2020 2020 2020 2074   edge:.        t
-00022130: 6169 6c2e 636f 6e6e 6563 7428 706f 7274  ail.connect(port
-00022140: 3d22 5722 2c20 6465 7374 696e 6174 696f  ="W", destinatio
-00022150: 6e3d 6f62 6a2e 706f 7274 735b 2253 225d  n=obj.ports["S"]
-00022160: 2c20 6f76 6572 6c61 703d 7769 7265 5f77  , overlap=wire_w
-00022170: 6964 7468 290a 2020 2020 2020 2020 7461  idth).        ta
-00022180: 696c 5f6f 7665 726c 6179 2e63 6f6e 6e65  il_overlay.conne
-00022190: 6374 2870 6f72 743d 2257 222c 2064 6573  ct(port="W", des
-000221a0: 7469 6e61 7469 6f6e 3d6f 626a 2e70 6f72  tination=obj.por
-000221b0: 7473 5b22 5322 5d2c 206f 7665 726c 6170  ts["S"], overlap
-000221c0: 3d77 6972 655f 7769 6474 6829 0a20 2020  =wire_width).   
-000221d0: 2065 6c69 6620 646f 776e 2061 6e64 206e   elif down and n
-000221e0: 6f74 2065 6467 653a 0a20 2020 2020 2020  ot edge:.       
-000221f0: 2074 6169 6c2e 636f 6e6e 6563 7428 706f   tail.connect(po
-00022200: 7274 3d22 5722 2c20 6465 7374 696e 6174  rt="W", destinat
-00022210: 696f 6e3d 6f62 6a2e 706f 7274 735b 224e  ion=obj.ports["N
-00022220: 225d 2c20 6f76 6572 6c61 703d 7769 7265  "], overlap=wire
-00022230: 5f77 6964 7468 290a 2020 2020 2020 2020  _width).        
-00022240: 7461 696c 5f6f 7665 726c 6179 2e63 6f6e  tail_overlay.con
-00022250: 6e65 6374 2870 6f72 743d 2257 222c 2064  nect(port="W", d
-00022260: 6573 7469 6e61 7469 6f6e 3d6f 626a 2e70  estination=obj.p
-00022270: 6f72 7473 5b22 4e22 5d2c 206f 7665 726c  orts["N"], overl
-00022280: 6170 3d77 6972 655f 7769 6474 6829 0a20  ap=wire_width). 
-00022290: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000222a0: 2074 6169 6c2e 636f 6e6e 6563 7428 706f   tail.connect(po
-000222b0: 7274 3d22 5722 2c20 6465 7374 696e 6174  rt="W", destinat
-000222c0: 696f 6e3d 6f62 6a2e 706f 7274 735b 2245  ion=obj.ports["E
-000222d0: 225d 2c20 6f76 6572 6c61 703d 7769 7265  "], overlap=wire
-000222e0: 5f77 6964 7468 290a 2020 2020 2020 2020  _width).        
-000222f0: 7461 696c 5f6f 7665 726c 6179 2e63 6f6e  tail_overlay.con
-00022300: 6e65 6374 2870 6f72 743d 2257 222c 2064  nect(port="W", d
-00022310: 6573 7469 6e61 7469 6f6e 3d6f 626a 2e70  estination=obj.p
-00022320: 6f72 7473 5b22 4522 5d2c 206f 7665 726c  orts["E"], overl
-00022330: 6170 3d77 6972 655f 7769 6474 6829 0a0a  ap=wire_width)..
-00022340: 2020 2020 7061 6432 2e78 6d69 6e20 3d20      pad2.xmin = 
-00022350: 7461 696c 2e78 6d61 780a 2020 2020 7061  tail.xmax.    pa
-00022360: 6432 5f6f 7665 726c 6179 2e78 6d69 6e20  d2_overlay.xmin 
-00022370: 3d20 7061 6432 2e78 6d69 6e0a 2020 2020  = pad2.xmin.    
-00022380: 7061 6432 5f6f 7665 726c 6179 2e79 6d69  pad2_overlay.ymi
-00022390: 6e20 3d20 7061 6432 2e79 6d69 6e0a 0a20  n = pad2.ymin.. 
-000223a0: 2020 2072 6574 7572 6e20 5652 0a0a 0a64     return VR...d
-000223b0: 6566 2074 6573 745f 636f 6d62 280a 2020  ef test_comb(.  
-000223c0: 2020 7061 645f 7369 7a65 3d28 3230 302c    pad_size=(200,
-000223d0: 2032 3030 292c 0a20 2020 2077 6972 655f   200),.    wire_
-000223e0: 7769 6474 683d 312c 0a20 2020 2077 6972  width=1,.    wir
-000223f0: 655f 6761 703d 332c 0a20 2020 2063 6f6d  e_gap=3,.    com
-00022400: 625f 6c61 7965 723d 302c 0a20 2020 206f  b_layer=0,.    o
-00022410: 7665 726c 6170 5f7a 6967 7a61 675f 6c61  verlap_zigzag_la
-00022420: 7965 723d 312c 0a20 2020 2063 6f6d 625f  yer=1,.    comb_
-00022430: 7061 645f 6c61 7965 723d 322c 0a20 2020  pad_layer=2,.   
-00022440: 2063 6f6d 625f 676e 645f 6c61 7965 723d   comb_gnd_layer=
-00022450: 332c 0a20 2020 206f 7665 726c 6170 5f70  3,.    overlap_p
-00022460: 6164 5f6c 6179 6572 3d34 2c0a 293a 0a20  ad_layer=4,.):. 
-00022470: 2020 2022 2222 4f76 6572 6c61 7020 636f     """Overlap co
-00022480: 6d62 2074 6573 7420 7374 7275 6374 7572  mb test structur
-00022490: 6520 666f 7220 6368 6563 6b69 6e67 2077  e for checking w
-000224a0: 6865 7468 6572 2074 776f 206c 6179 6572  hether two layer
-000224b0: 730a 2020 2020 6172 6520 656c 6563 7472  s.    are electr
-000224c0: 6963 616c 6c79 2069 736f 6c61 7465 640a  ically isolated.
-000224d0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-000224e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000224f0: 2020 2070 6164 5f73 697a 6520 3a20 6172     pad_size : ar
-00022500: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
-00022510: 2078 2061 6e64 2079 2064 696d 656e 7369   x and y dimensi
-00022520: 6f6e 7320 6f66 2074 6865 2063 6f6d 6220  ons of the comb 
-00022530: 7061 6473 2e0a 2020 2020 7769 7265 5f77  pads..    wire_w
-00022540: 6964 7468 203a 2069 6e74 206f 7220 666c  idth : int or fl
-00022550: 6f61 740a 2020 2020 2020 2020 5769 6474  oat.        Widt
-00022560: 6820 6f66 2074 6865 2074 6573 7420 636f  h of the test co
-00022570: 6d62 2074 6565 7468 2e0a 2020 2020 7769  mb teeth..    wi
-00022580: 7265 5f67 6170 203a 2069 6e74 206f 7220  re_gap : int or 
-00022590: 666c 6f61 740a 2020 2020 2020 2020 5369  float.        Si
-000225a0: 7a65 206f 6620 7468 6520 6761 7020 6265  ze of the gap be
-000225b0: 7477 6565 6e20 636f 6d62 2074 6565 7468  tween comb teeth
-000225c0: 2e0a 2020 2020 636f 6d62 5f6c 6179 6572  ..    comb_layer
-000225d0: 203a 2069 6e74 2c20 6172 7261 792d 6c69   : int, array-li
-000225e0: 6b65 5b32 5d2c 206f 7220 7365 740a 2020  ke[2], or set.  
-000225f0: 2020 2020 2020 5370 6563 6966 6963 206c        Specific l
-00022600: 6179 6572 2873 2920 746f 2070 7574 2063  ayer(s) to put c
-00022610: 6f6d 6220 6765 6f6d 6574 7279 206f 6e2e  omb geometry on.
-00022620: 0a20 2020 206f 7665 726c 6170 5f7a 6967  .    overlap_zig
-00022630: 7a61 675f 6c61 7965 7220 3a20 696e 742c  zag_layer : int,
-00022640: 2061 7272 6179 2d6c 696b 655b 325d 2c20   array-like[2], 
-00022650: 6f72 2073 6574 0a20 2020 2020 2020 2053  or set.        S
-00022660: 7065 6369 6669 6320 6c61 7965 7228 7329  pecific layer(s)
-00022670: 2074 6f20 7075 7420 6f76 6572 6c61 7020   to put overlap 
-00022680: 7a69 677a 6167 2067 656f 6d65 7472 7920  zigzag geometry 
-00022690: 6f6e 2e0a 2020 2020 636f 6d62 5f70 6164  on..    comb_pad
-000226a0: 5f6c 6179 6572 203a 2069 6e74 2c20 6172  _layer : int, ar
-000226b0: 7261 792d 6c69 6b65 5b32 5d2c 206f 7220  ray-like[2], or 
-000226c0: 7365 740a 2020 2020 2020 2020 5370 6563  set.        Spec
-000226d0: 6966 6963 206c 6179 6572 2873 2920 746f  ific layer(s) to
-000226e0: 2070 7574 2063 6f6d 6220 7061 6473 206f   put comb pads o
-000226f0: 6e2e 0a20 2020 2063 6f6d 625f 676e 645f  n..    comb_gnd_
-00022700: 6c61 7965 7220 3a20 696e 742c 2061 7272  layer : int, arr
-00022710: 6179 2d6c 696b 655b 325d 2c20 6f72 2073  ay-like[2], or s
-00022720: 6574 0a20 2020 2020 2020 2053 7065 6369  et.        Speci
-00022730: 6669 6320 6c61 7965 7228 7329 2074 6f20  fic layer(s) to 
-00022740: 7075 7420 7468 6520 636f 6d62 2067 726f  put the comb gro
-00022750: 756e 6420 6f6e 2e0a 2020 2020 6f76 6572  und on..    over
-00022760: 6c61 705f 7061 645f 6c61 7965 7220 3a20  lap_pad_layer : 
-00022770: 696e 742c 2061 7272 6179 2d6c 696b 655b  int, array-like[
-00022780: 325d 2c20 6f72 2073 6574 0a20 2020 2020  2], or set.     
-00022790: 2020 2053 7065 6369 6669 6320 6c61 7965     Specific laye
-000227a0: 7228 7329 2074 6f20 7075 7420 6f76 6572  r(s) to put over
-000227b0: 6c61 7020 7061 6473 206f 6e2e 0a0a 2020  lap pads on...  
-000227c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000227d0: 2d2d 2d2d 2d0a 2020 2020 4349 203a 2044  -----.    CI : D
-000227e0: 6576 6963 650a 2020 2020 2020 2020 4120  evice.        A 
-000227f0: 4465 7669 6365 2063 6f6e 7461 696e 696e  Device containin
-00022800: 6720 6120 7465 7374 2063 6f6d 6220 6765  g a test comb ge
-00022810: 6f6d 6574 7279 2e0a 0a20 2020 204e 6f74  ometry...    Not
-00022820: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
-00022830: 2043 616c 6c20 636f 6d62 5f69 6e73 756c   Call comb_insul
-00022840: 6174 696f 6e5f 7465 7374 5f73 7472 7563  ation_test_struc
-00022850: 7475 7265 2829 2077 6974 6820 616e 7920  ture() with any 
-00022860: 6f66 2074 6865 2070 6172 616d 6574 6572  of the parameter
-00022870: 7320 7368 6f77 6e0a 2020 2020 6265 6c6f  s shown.    belo
-00022880: 7720 7768 6963 6820 796f 7527 6420 6c69  w which you'd li
-00022890: 6b65 2074 6f20 6368 616e 6765 2e20 596f  ke to change. Yo
-000228a0: 7520 6f6e 6c79 206e 6565 6420 746f 2073  u only need to s
-000228b0: 7570 706c 7920 7468 6520 7061 7261 6d65  upply the parame
-000228c0: 7465 7273 0a20 2020 2077 6869 6368 2079  ters.    which y
-000228d0: 6f75 2069 6e74 656e 6420 6f6e 2063 6861  ou intend on cha
-000228e0: 6e67 696e 6720 596f 7520 6361 6e20 616c  nging You can al
-000228f0: 7465 726e 6174 6976 656c 7920 6361 6c6c  ternatively call
-00022900: 2069 7420 7769 7468 206e 6f0a 2020 2020   it with no.    
-00022910: 7061 7261 6d65 7465 7273 2061 6e64 2069  parameters and i
-00022920: 7420 7769 6c6c 2074 616b 6520 616c 6c20  t will take all 
-00022930: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
-00022940: 6573 2073 686f 776e 2062 656c 6f77 2e0a  es shown below..
-00022950: 0a20 2020 2045 783a 3a0a 2020 2020 2020  .    Ex::.      
-00022960: 2020 636f 6d62 5f69 6e73 756c 6174 696f    comb_insulatio
-00022970: 6e5f 7465 7374 5f73 7472 7563 7475 7265  n_test_structure
-00022980: 2870 6164 5f73 697a 653d 2831 3735 2c31  (pad_size=(175,1
-00022990: 3735 292c 2077 6972 655f 7769 6474 683d  75), wire_width=
-000229a0: 322c 2077 6972 655f 6761 703d 3529 0a20  2, wire_gap=5). 
-000229b0: 2020 202d 206f 7220 2d3a 3a0a 2020 2020     - or -::.    
-000229c0: 2020 2020 636f 6d62 5f69 6e73 756c 6174      comb_insulat
-000229d0: 696f 6e5f 7465 7374 5f73 7472 7563 7475  ion_test_structu
-000229e0: 7265 2829 0a20 2020 2022 2222 0a20 2020  re().    """.   
-000229f0: 2043 4920 3d20 4465 7669 6365 2822 7465   CI = Device("te
-00022a00: 7374 5f63 6f6d 6222 290a 0a20 2020 2023  st_comb")..    #
-00022a10: 2069 6620 636f 6d62 5f70 6164 5f6c 6179   if comb_pad_lay
-00022a20: 6572 2069 7320 4e6f 6e65 3a20 636f 6d62  er is None: comb
-00022a30: 5f70 6164 5f6c 6179 6572 203d 2063 6f6d  _pad_layer = com
-00022a40: 625f 6c61 7965 720a 2020 2020 2320 6966  b_layer.    # if
-00022a50: 2063 6f6d 625f 676e 645f 6c61 7965 7220   comb_gnd_layer 
-00022a60: 6973 204e 6f6e 653a 2063 6f6d 625f 676e  is None: comb_gn
-00022a70: 645f 6c61 7965 7220 3d20 636f 6d62 5f6c  d_layer = comb_l
-00022a80: 6179 6572 0a20 2020 2023 2069 6620 6f76  ayer.    # if ov
-00022a90: 6572 6c61 705f 7061 645f 6c61 7965 7220  erlap_pad_layer 
-00022aa0: 6973 204e 6f6e 653a 206f 7665 726c 6170  is None: overlap
-00022ab0: 5f70 6164 5f6c 6179 6572 203d 206f 7665  _pad_layer = ove
-00022ac0: 726c 6170 5f7a 6967 7a61 675f 6c61 7965  rlap_zigzag_laye
-00022ad0: 720a 2020 2020 7769 7265 5f73 7061 6369  r.    wire_spaci
-00022ae0: 6e67 203d 2077 6972 655f 7769 6474 6820  ng = wire_width 
-00022af0: 2b20 7769 7265 5f67 6170 202a 2032 0a0a  + wire_gap * 2..
-00022b00: 2020 2020 2320 7061 6420 6f76 6572 6c61      # pad overla
-00022b10: 7973 0a20 2020 206f 7665 726c 6179 5f70  ys.    overlay_p
-00022b20: 6164 6220 3d20 4349 2e61 6464 5f72 6566  adb = CI.add_ref
-00022b30: 280a 2020 2020 2020 2020 7265 6374 616e  (.        rectan
-00022b40: 676c 6528 0a20 2020 2020 2020 2020 2020  gle(.           
-00022b50: 2073 697a 653d 2870 6164 5f73 697a 655b   size=(pad_size[
-00022b60: 305d 202a 2039 202f 2031 302c 2070 6164  0] * 9 / 10, pad
-00022b70: 5f73 697a 655b 315d 202a 2039 202f 2031  _size[1] * 9 / 1
-00022b80: 3029 2c20 6c61 7965 723d 6f76 6572 6c61  0), layer=overla
-00022b90: 705f 7061 645f 6c61 7965 720a 2020 2020  p_pad_layer.    
-00022ba0: 2020 2020 290a 2020 2020 290a 2020 2020      ).    ).    
-00022bb0: 6f76 6572 6c61 795f 7061 646c 203d 2043  overlay_padl = C
-00022bc0: 492e 6164 645f 7265 6628 0a20 2020 2020  I.add_ref(.     
-00022bd0: 2020 2072 6563 7461 6e67 6c65 280a 2020     rectangle(.  
-00022be0: 2020 2020 2020 2020 2020 7369 7a65 3d28            size=(
-00022bf0: 7061 645f 7369 7a65 5b30 5d20 2a20 3920  pad_size[0] * 9 
-00022c00: 2f20 3130 2c20 7061 645f 7369 7a65 5b31  / 10, pad_size[1
-00022c10: 5d20 2a20 3920 2f20 3130 292c 206c 6179  ] * 9 / 10), lay
-00022c20: 6572 3d63 6f6d 625f 7061 645f 6c61 7965  er=comb_pad_laye
-00022c30: 720a 2020 2020 2020 2020 290a 2020 2020  r.        ).    
-00022c40: 290a 2020 2020 6f76 6572 6c61 795f 7061  ).    overlay_pa
-00022c50: 6474 203d 2043 492e 6164 645f 7265 6628  dt = CI.add_ref(
-00022c60: 0a20 2020 2020 2020 2072 6563 7461 6e67  .        rectang
-00022c70: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00022c80: 7369 7a65 3d28 7061 645f 7369 7a65 5b30  size=(pad_size[0
-00022c90: 5d20 2a20 3920 2f20 3130 2c20 7061 645f  ] * 9 / 10, pad_
-00022ca0: 7369 7a65 5b31 5d20 2a20 3920 2f20 3130  size[1] * 9 / 10
-00022cb0: 292c 206c 6179 6572 3d63 6f6d 625f 7061  ), layer=comb_pa
-00022cc0: 645f 6c61 7965 720a 2020 2020 2020 2020  d_layer.        
-00022cd0: 290a 2020 2020 290a 2020 2020 6f76 6572  ).    ).    over
-00022ce0: 6c61 795f 7061 6472 203d 2043 492e 6164  lay_padr = CI.ad
-00022cf0: 645f 7265 6628 0a20 2020 2020 2020 2072  d_ref(.        r
-00022d00: 6563 7461 6e67 6c65 280a 2020 2020 2020  ectangle(.      
-00022d10: 2020 2020 2020 7369 7a65 3d28 7061 645f        size=(pad_
-00022d20: 7369 7a65 5b30 5d20 2a20 3920 2f20 3130  size[0] * 9 / 10
-00022d30: 2c20 7061 645f 7369 7a65 5b31 5d20 2a20  , pad_size[1] * 
-00022d40: 3920 2f20 3130 292c 206c 6179 6572 3d63  9 / 10), layer=c
-00022d50: 6f6d 625f 676e 645f 6c61 7965 720a 2020  omb_gnd_layer.  
-00022d60: 2020 2020 2020 290a 2020 2020 290a 2020        ).    ).  
-00022d70: 2020 6f76 6572 6c61 795f 7061 646c 2e78    overlay_padl.x
-00022d80: 6d69 6e20 3d20 300a 2020 2020 6f76 6572  min = 0.    over
-00022d90: 6c61 795f 7061 646c 2e79 6d69 6e20 3d20  lay_padl.ymin = 
-00022da0: 300a 2020 2020 6f76 6572 6c61 795f 7061  0.    overlay_pa
-00022db0: 6462 2e79 6d61 7820 3d20 300a 2020 2020  db.ymax = 0.    
-00022dc0: 6f76 6572 6c61 795f 7061 6462 2e78 6d69  overlay_padb.xmi
-00022dd0: 6e20 3d20 6f76 6572 6c61 795f 7061 646c  n = overlay_padl
-00022de0: 2e78 6d61 7820 2b20 7061 645f 7369 7a65  .xmax + pad_size
-00022df0: 5b31 5d20 2f20 350a 2020 2020 6f76 6572  [1] / 5.    over
-00022e00: 6c61 795f 7061 6472 2e79 6d69 6e20 3d20  lay_padr.ymin = 
-00022e10: 6f76 6572 6c61 795f 7061 646c 2e79 6d69  overlay_padl.ymi
-00022e20: 6e0a 2020 2020 6f76 6572 6c61 795f 7061  n.    overlay_pa
-00022e30: 6472 2e78 6d69 6e20 3d20 6f76 6572 6c61  dr.xmin = overla
-00022e40: 795f 7061 6462 2e78 6d61 7820 2b20 7061  y_padb.xmax + pa
-00022e50: 645f 7369 7a65 5b31 5d20 2f20 350a 2020  d_size[1] / 5.  
-00022e60: 2020 6f76 6572 6c61 795f 7061 6474 2e78    overlay_padt.x
-00022e70: 6d69 6e20 3d20 6f76 6572 6c61 795f 7061  min = overlay_pa
-00022e80: 646c 2e78 6d61 7820 2b20 7061 645f 7369  dl.xmax + pad_si
-00022e90: 7a65 5b31 5d20 2f20 350a 2020 2020 6f76  ze[1] / 5.    ov
-00022ea0: 6572 6c61 795f 7061 6474 2e79 6d69 6e20  erlay_padt.ymin 
-00022eb0: 3d20 6f76 6572 6c61 795f 7061 646c 2e79  = overlay_padl.y
-00022ec0: 6d61 780a 0a20 2020 2023 2070 6164 730a  max..    # pads.
-00022ed0: 2020 2020 7061 646c 203d 2043 492e 6164      padl = CI.ad
-00022ee0: 645f 7265 6628 7265 6374 616e 676c 6528  d_ref(rectangle(
-00022ef0: 7369 7a65 3d70 6164 5f73 697a 652c 206c  size=pad_size, l
-00022f00: 6179 6572 3d63 6f6d 625f 6c61 7965 7229  ayer=comb_layer)
-00022f10: 290a 2020 2020 7061 6474 203d 2043 492e  ).    padt = CI.
-00022f20: 6164 645f 7265 6628 7265 6374 616e 676c  add_ref(rectangl
-00022f30: 6528 7369 7a65 3d70 6164 5f73 697a 652c  e(size=pad_size,
-00022f40: 206c 6179 6572 3d63 6f6d 625f 6c61 7965   layer=comb_laye
-00022f50: 7229 290a 2020 2020 7061 6472 203d 2043  r)).    padr = C
-00022f60: 492e 6164 645f 7265 6628 7265 6374 616e  I.add_ref(rectan
-00022f70: 676c 6528 7369 7a65 3d70 6164 5f73 697a  gle(size=pad_siz
-00022f80: 652c 206c 6179 6572 3d63 6f6d 625f 6c61  e, layer=comb_la
-00022f90: 7965 7229 290a 2020 2020 7061 6462 203d  yer)).    padb =
-00022fa0: 2043 492e 6164 645f 7265 6628 7265 6374   CI.add_ref(rect
-00022fb0: 616e 676c 6528 7369 7a65 3d70 6164 5f73  angle(size=pad_s
-00022fc0: 697a 652c 206c 6179 6572 3d6f 7665 726c  ize, layer=overl
-00022fd0: 6170 5f7a 6967 7a61 675f 6c61 7965 7229  ap_zigzag_layer)
-00022fe0: 290a 2020 2020 7061 646c 5f6e 7562 203d  ).    padl_nub =
-00022ff0: 2043 492e 6164 645f 7265 6628 0a20 2020   CI.add_ref(.   
-00023000: 2020 2020 2072 6563 7461 6e67 6c65 2873       rectangle(s
-00023010: 697a 653d 2870 6164 5f73 697a 655b 305d  ize=(pad_size[0]
-00023020: 202f 2034 2c20 7061 645f 7369 7a65 5b31   / 4, pad_size[1
-00023030: 5d20 2f20 3229 2c20 6c61 7965 723d 636f  ] / 2), layer=co
-00023040: 6d62 5f6c 6179 6572 290a 2020 2020 290a  mb_layer).    ).
-00023050: 2020 2020 7061 6472 5f6e 7562 203d 2043      padr_nub = C
-00023060: 492e 6164 645f 7265 6628 0a20 2020 2020  I.add_ref(.     
-00023070: 2020 2072 6563 7461 6e67 6c65 2873 697a     rectangle(siz
-00023080: 653d 2870 6164 5f73 697a 655b 305d 202f  e=(pad_size[0] /
-00023090: 2034 2c20 7061 645f 7369 7a65 5b31 5d20   4, pad_size[1] 
-000230a0: 2f20 3229 2c20 6c61 7965 723d 636f 6d62  / 2), layer=comb
-000230b0: 5f6c 6179 6572 290a 2020 2020 290a 2020  _layer).    ).  
-000230c0: 2020 7061 646c 2e78 6d69 6e20 3d20 6f76    padl.xmin = ov
-000230d0: 6572 6c61 795f 7061 646c 2e78 6d69 6e0a  erlay_padl.xmin.
-000230e0: 2020 2020 7061 646c 2e63 656e 7465 7220      padl.center 
-000230f0: 3d20 5b70 6164 6c2e 6365 6e74 6572 5b30  = [padl.center[0
-00023100: 5d2c 206f 7665 726c 6179 5f70 6164 6c2e  ], overlay_padl.
-00023110: 6365 6e74 6572 5b31 5d5d 0a20 2020 2070  center[1]].    p
-00023120: 6164 742e 796d 6178 203d 206f 7665 726c  adt.ymax = overl
-00023130: 6179 5f70 6164 742e 796d 6178 0a20 2020  ay_padt.ymax.   
-00023140: 2070 6164 742e 6365 6e74 6572 203d 205b   padt.center = [
-00023150: 6f76 6572 6c61 795f 7061 6474 2e63 656e  overlay_padt.cen
-00023160: 7465 725b 305d 2c20 7061 6474 2e63 656e  ter[0], padt.cen
-00023170: 7465 725b 315d 5d0a 2020 2020 7061 6472  ter[1]].    padr
-00023180: 2e78 6d61 7820 3d20 6f76 6572 6c61 795f  .xmax = overlay_
-00023190: 7061 6472 2e78 6d61 780a 2020 2020 7061  padr.xmax.    pa
-000231a0: 6472 2e63 656e 7465 7220 3d20 5b70 6164  dr.center = [pad
-000231b0: 722e 6365 6e74 6572 5b30 5d2c 206f 7665  r.center[0], ove
-000231c0: 726c 6179 5f70 6164 722e 6365 6e74 6572  rlay_padr.center
-000231d0: 5b31 5d5d 0a20 2020 2070 6164 622e 796d  [1]].    padb.ym
-000231e0: 696e 203d 206f 7665 726c 6179 5f70 6164  in = overlay_pad
-000231f0: 622e 796d 696e 0a20 2020 2070 6164 622e  b.ymin.    padb.
-00023200: 6365 6e74 6572 203d 205b 6f76 6572 6c61  center = [overla
-00023210: 795f 7061 6462 2e63 656e 7465 725b 305d  y_padb.center[0]
-00023220: 2c20 7061 6462 2e63 656e 7465 725b 315d  , padb.center[1]
-00023230: 5d0a 2020 2020 7061 646c 5f6e 7562 2e78  ].    padl_nub.x
-00023240: 6d69 6e20 3d20 7061 646c 2e78 6d61 780a  min = padl.xmax.
-00023250: 2020 2020 7061 646c 5f6e 7562 2e63 656e      padl_nub.cen
-00023260: 7465 7220 3d20 5b70 6164 6c5f 6e75 622e  ter = [padl_nub.
-00023270: 6365 6e74 6572 5b30 5d2c 2070 6164 6c2e  center[0], padl.
-00023280: 6365 6e74 6572 5b31 5d5d 0a20 2020 2070  center[1]].    p
-00023290: 6164 725f 6e75 622e 786d 6178 203d 2070  adr_nub.xmax = p
-000232a0: 6164 722e 786d 696e 0a20 2020 2070 6164  adr.xmin.    pad
-000232b0: 725f 6e75 622e 6365 6e74 6572 203d 205b  r_nub.center = [
-000232c0: 7061 6472 5f6e 7562 2e63 656e 7465 725b  padr_nub.center[
-000232d0: 305d 2c20 7061 6472 2e63 656e 7465 725b  0], padr.center[
-000232e0: 315d 5d0a 0a20 2020 2023 2063 6f6e 6e65  1]]..    # conne
-000232f0: 6374 6564 207a 6967 0a20 2020 2068 6561  cted zig.    hea
-00023300: 6420 3d20 4349 2e61 6464 5f72 6566 2863  d = CI.add_ref(c
-00023310: 6f6d 7061 7373 2873 697a 653d 2870 6164  ompass(size=(pad
-00023320: 5f73 697a 655b 305d 202f 2031 322c 2077  _size[0] / 12, w
-00023330: 6972 655f 7769 6474 6829 2c20 6c61 7965  ire_width), laye
-00023340: 723d 636f 6d62 5f6c 6179 6572 2929 0a20  r=comb_layer)). 
-00023350: 2020 2068 6561 642e 786d 696e 203d 2070     head.xmin = p
-00023360: 6164 6c5f 6e75 622e 786d 6178 0a20 2020  adl_nub.xmax.   
-00023370: 2068 6561 642e 796d 6178 203d 2070 6164   head.ymax = pad
-00023380: 6c5f 6e75 622e 796d 6178 0a20 2020 2063  l_nub.ymax.    c
-00023390: 6f6e 6e65 6374 6f72 203d 2043 492e 6164  onnector = CI.ad
-000233a0: 645f 7265 6628 636f 6d70 6173 7328 7369  d_ref(compass(si
-000233b0: 7a65 3d28 7769 7265 5f77 6964 7468 2c20  ze=(wire_width, 
-000233c0: 7769 7265 5f77 6964 7468 292c 206c 6179  wire_width), lay
-000233d0: 6572 3d63 6f6d 625f 6c61 7965 7229 290a  er=comb_layer)).
-000233e0: 2020 2020 636f 6e6e 6563 746f 722e 636f      connector.co
-000233f0: 6e6e 6563 7428 706f 7274 3d22 5722 2c20  nnect(port="W", 
-00023400: 6465 7374 696e 6174 696f 6e3d 6865 6164  destination=head
-00023410: 2e70 6f72 7473 5b22 4522 5d29 0a20 2020  .ports["E"]).   
-00023420: 206f 6c64 5f70 6f72 7420 3d20 636f 6e6e   old_port = conn
-00023430: 6563 746f 722e 706f 7274 735b 2253 225d  ector.ports["S"]
-00023440: 0a20 2020 2074 6f70 203d 2054 7275 650a  .    top = True.
-00023450: 2020 2020 6f62 6a20 3d20 636f 6e6e 6563      obj = connec
-00023460: 746f 720a 2020 2020 7768 696c 6520 6f62  tor.    while ob
-00023470: 6a2e 786d 6178 202b 2070 6164 5f73 697a  j.xmax + pad_siz
-00023480: 655b 305d 202f 2031 3220 3c20 7061 6472  e[0] / 12 < padr
-00023490: 5f6e 7562 2e78 6d69 6e3a 0a20 2020 2020  _nub.xmin:.     
-000234a0: 2020 2023 206c 6f6e 6720 7a69 6720 7a61     # long zig za
-000234b0: 6720 7265 6374 616e 676c 650a 2020 2020  g rectangle.    
-000234c0: 2020 2020 6f62 6a20 3d20 4349 2e61 6464      obj = CI.add
-000234d0: 5f72 6566 280a 2020 2020 2020 2020 2020  _ref(.          
-000234e0: 2020 636f 6d70 6173 7328 0a20 2020 2020    compass(.     
-000234f0: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-00023500: 2870 6164 5f73 697a 655b 315d 202f 2032  (pad_size[1] / 2
-00023510: 202d 2032 202a 2077 6972 655f 7769 6474   - 2 * wire_widt
-00023520: 682c 2077 6972 655f 7769 6474 6829 2c20  h, wire_width), 
-00023530: 6c61 7965 723d 636f 6d62 5f6c 6179 6572  layer=comb_layer
-00023540: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00023550: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023560: 206f 626a 2e63 6f6e 6e65 6374 2870 6f72   obj.connect(por
-00023570: 743d 2257 222c 2064 6573 7469 6e61 7469  t="W", destinati
-00023580: 6f6e 3d6f 6c64 5f70 6f72 7429 0a20 2020  on=old_port).   
-00023590: 2020 2020 206f 6c64 5f70 6f72 7420 3d20       old_port = 
-000235a0: 6f62 6a2e 706f 7274 735b 2245 225d 0a20  obj.ports["E"]. 
-000235b0: 2020 2020 2020 2069 6620 746f 703a 0a20         if top:. 
-000235c0: 2020 2020 2020 2020 2020 2023 207a 6967             # zig
-000235d0: 207a 6167 2065 6467 6520 7265 6374 616e   zag edge rectan
-000235e0: 676c 650a 2020 2020 2020 2020 2020 2020  gle.            
-000235f0: 6f62 6a20 3d20 4349 2e61 6464 5f72 6566  obj = CI.add_ref
-00023600: 2863 6f6d 7061 7373 2873 697a 653d 2877  (compass(size=(w
-00023610: 6972 655f 7769 6474 682c 2077 6972 655f  ire_width, wire_
-00023620: 7769 6474 6829 2c20 6c61 7965 723d 636f  width), layer=co
-00023630: 6d62 5f6c 6179 6572 2929 0a20 2020 2020  mb_layer)).     
-00023640: 2020 2020 2020 206f 626a 2e63 6f6e 6e65         obj.conne
-00023650: 6374 2870 6f72 743d 224e 222c 2064 6573  ct(port="N", des
-00023660: 7469 6e61 7469 6f6e 3d6f 6c64 5f70 6f72  tination=old_por
-00023670: 7429 0a20 2020 2020 2020 2020 2020 2074  t).            t
-00023680: 6f70 203d 2046 616c 7365 0a20 2020 2020  op = False.     
-00023690: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000236a0: 2020 2020 2023 207a 6967 207a 6167 2065       # zig zag e
-000236b0: 6467 6520 7265 6374 616e 676c 650a 2020  dge rectangle.  
-000236c0: 2020 2020 2020 2020 2020 6f62 6a20 3d20            obj = 
-000236d0: 4349 2e61 6464 5f72 6566 2863 6f6d 7061  CI.add_ref(compa
-000236e0: 7373 2873 697a 653d 2877 6972 655f 7769  ss(size=(wire_wi
-000236f0: 6474 682c 2077 6972 655f 7769 6474 6829  dth, wire_width)
-00023700: 2c20 6c61 7965 723d 636f 6d62 5f6c 6179  , layer=comb_lay
-00023710: 6572 2929 0a20 2020 2020 2020 2020 2020  er)).           
-00023720: 206f 626a 2e63 6f6e 6e65 6374 2870 6f72   obj.connect(por
-00023730: 743d 2253 222c 2064 6573 7469 6e61 7469  t="S", destinati
-00023740: 6f6e 3d6f 6c64 5f70 6f72 7429 0a20 2020  on=old_port).   
-00023750: 2020 2020 2020 2020 2074 6f70 203d 2054           top = T
-00023760: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00023770: 2320 636f 6d62 2072 6563 7461 6e67 650a  # comb rectange.
-00023780: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-00023790: 203d 2043 492e 6164 645f 7265 6628 0a20   = CI.add_ref(. 
-000237a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000237b0: 6563 7461 6e67 6c65 280a 2020 2020 2020  ectangle(.      
-000237c0: 2020 2020 2020 2020 2020 2020 2020 7369                si
-000237d0: 7a65 3d28 0a20 2020 2020 2020 2020 2020  ze=(.           
-000237e0: 2020 2020 2020 2020 2020 2020 2028 7061               (pa
-000237f0: 6474 2e79 6d69 6e20 2d20 6865 6164 2e79  dt.ymin - head.y
-00023800: 6d61 7829 0a20 2020 2020 2020 2020 2020  max).           
-00023810: 2020 2020 2020 2020 2020 2020 202b 2070               + p
-00023820: 6164 5f73 697a 655b 315d 202f 2032 0a20  ad_size[1] / 2. 
-00023830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023840: 2020 2020 2020 202d 2028 7769 7265 5f73         - (wire_s
-00023850: 7061 6369 6e67 202b 2077 6972 655f 7769  pacing + wire_wi
-00023860: 6474 6829 202f 2032 2c0a 2020 2020 2020  dth) / 2,.      
-00023870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023880: 2020 7769 7265 5f77 6964 7468 2c0a 2020    wire_width,.  
-00023890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238a0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-000238b0: 2020 2020 2020 2020 206c 6179 6572 3d63           layer=c
-000238c0: 6f6d 625f 6c61 7965 722c 0a20 2020 2020  omb_layer,.     
-000238d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000238e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000238f0: 2020 2020 2020 2063 6f6d 622e 726f 7461         comb.rota
-00023900: 7465 2839 3029 0a20 2020 2020 2020 2020  te(90).         
-00023910: 2020 2063 6f6d 622e 796d 6178 203d 2070     comb.ymax = p
-00023920: 6164 742e 796d 696e 0a20 2020 2020 2020  adt.ymin.       
-00023930: 2020 2020 2063 6f6d 622e 786d 6178 203d       comb.xmax =
-00023940: 206f 626a 2e78 6d61 7820 2d20 2877 6972   obj.xmax - (wir
-00023950: 655f 7370 6163 696e 6720 2b20 7769 7265  e_spacing + wire
-00023960: 5f77 6964 7468 2920 2f20 320a 2020 2020  _width) / 2.    
-00023970: 2020 2020 6f6c 645f 706f 7274 203d 206f      old_port = o
-00023980: 626a 2e70 6f72 7473 5b22 4522 5d0a 2020  bj.ports["E"].  
-00023990: 2020 2020 2020 6f62 6a20 3d20 4349 2e61        obj = CI.a
-000239a0: 6464 5f72 6566 2863 6f6d 7061 7373 2873  dd_ref(compass(s
-000239b0: 697a 653d 2877 6972 655f 7370 6163 696e  ize=(wire_spacin
-000239c0: 672c 2077 6972 655f 7769 6474 6829 2c20  g, wire_width), 
-000239d0: 6c61 7965 723d 636f 6d62 5f6c 6179 6572  layer=comb_layer
-000239e0: 2929 0a20 2020 2020 2020 206f 626a 2e63  )).        obj.c
-000239f0: 6f6e 6e65 6374 2870 6f72 743d 2257 222c  onnect(port="W",
-00023a00: 2064 6573 7469 6e61 7469 6f6e 3d6f 6c64   destination=old
-00023a10: 5f70 6f72 7429 0a20 2020 2020 2020 206f  _port).        o
-00023a20: 6c64 5f70 6f72 7420 3d20 6f62 6a2e 706f  ld_port = obj.po
-00023a30: 7274 735b 2245 225d 0a20 2020 2020 2020  rts["E"].       
-00023a40: 206f 626a 203d 2043 492e 6164 645f 7265   obj = CI.add_re
-00023a50: 6628 636f 6d70 6173 7328 7369 7a65 3d28  f(compass(size=(
-00023a60: 7769 7265 5f77 6964 7468 2c20 7769 7265  wire_width, wire
-00023a70: 5f77 6964 7468 292c 206c 6179 6572 3d63  _width), layer=c
-00023a80: 6f6d 625f 6c61 7965 7229 290a 2020 2020  omb_layer)).    
-00023a90: 2020 2020 6f62 6a2e 636f 6e6e 6563 7428      obj.connect(
-00023aa0: 706f 7274 3d22 5722 2c20 6465 7374 696e  port="W", destin
-00023ab0: 6174 696f 6e3d 6f6c 645f 706f 7274 290a  ation=old_port).
-00023ac0: 2020 2020 2020 2020 6966 2074 6f70 3a0a          if top:.
-00023ad0: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
-00023ae0: 706f 7274 203d 206f 626a 2e70 6f72 7473  port = obj.ports
-00023af0: 5b22 5322 5d0a 2020 2020 2020 2020 656c  ["S"].        el
-00023b00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00023b10: 6f6c 645f 706f 7274 203d 206f 626a 2e70  old_port = obj.p
-00023b20: 6f72 7473 5b22 4e22 5d0a 2020 2020 6f6c  orts["N"].    ol
-00023b30: 645f 706f 7274 203d 206f 626a 2e70 6f72  d_port = obj.por
-00023b40: 7473 5b22 4522 5d0a 2020 2020 6966 2070  ts["E"].    if p
-00023b50: 6164 725f 6e75 622e 786d 696e 202d 206f  adr_nub.xmin - o
-00023b60: 626a 2e78 6d61 7820 3e20 303a 0a20 2020  bj.xmax > 0:.   
-00023b70: 2020 2020 2074 6169 6c20 3d20 4349 2e61       tail = CI.a
-00023b80: 6464 5f72 6566 280a 2020 2020 2020 2020  dd_ref(.        
-00023b90: 2020 2020 636f 6d70 6173 7328 7369 7a65      compass(size
-00023ba0: 3d28 7061 6472 5f6e 7562 2e78 6d69 6e20  =(padr_nub.xmin 
-00023bb0: 2d20 6f62 6a2e 786d 6178 2c20 7769 7265  - obj.xmax, wire
-00023bc0: 5f77 6964 7468 292c 206c 6179 6572 3d63  _width), layer=c
-00023bd0: 6f6d 625f 6c61 7965 7229 0a20 2020 2020  omb_layer).     
-00023be0: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
-00023bf0: 2020 2020 2020 2074 6169 6c20 3d20 4349         tail = CI
-00023c00: 2e61 6464 5f72 6566 2863 6f6d 7061 7373  .add_ref(compass
-00023c10: 2873 697a 653d 2877 6972 655f 7769 6474  (size=(wire_widt
-00023c20: 682c 2077 6972 655f 7769 6474 6829 2c20  h, wire_width), 
-00023c30: 6c61 7965 723d 636f 6d62 5f6c 6179 6572  layer=comb_layer
-00023c40: 2929 0a20 2020 2074 6169 6c2e 636f 6e6e  )).    tail.conn
-00023c50: 6563 7428 706f 7274 3d22 5722 2c20 6465  ect(port="W", de
-00023c60: 7374 696e 6174 696f 6e3d 6f6c 645f 706f  stination=old_po
-00023c70: 7274 290a 0a20 2020 2023 2064 6973 636f  rt)..    # disco
-00023c80: 6e6e 6563 7465 6420 7a69 670a 2020 2020  nnected zig.    
-00023c90: 6468 6561 6420 3d20 4349 2e61 6464 5f72  dhead = CI.add_r
-00023ca0: 6566 280a 2020 2020 2020 2020 636f 6d70  ef(.        comp
-00023cb0: 6173 7328 0a20 2020 2020 2020 2020 2020  ass(.           
-00023cc0: 2073 697a 653d 2870 6164 725f 6e75 622e   size=(padr_nub.
-00023cd0: 796d 696e 202d 2070 6164 622e 796d 6178  ymin - padb.ymax
-00023ce0: 202d 2077 6972 655f 7769 6474 682c 2077   - wire_width, w
-00023cf0: 6972 655f 7769 6474 6829 2c0a 2020 2020  ire_width),.    
-00023d00: 2020 2020 2020 2020 6c61 7965 723d 6f76          layer=ov
-00023d10: 6572 6c61 705f 7a69 677a 6167 5f6c 6179  erlap_zigzag_lay
-00023d20: 6572 2c0a 2020 2020 2020 2020 290a 2020  er,.        ).  
-00023d30: 2020 290a 2020 2020 6468 6561 642e 726f    ).    dhead.ro
-00023d40: 7461 7465 2839 3029 0a20 2020 2064 6865  tate(90).    dhe
-00023d50: 6164 2e79 6d69 6e20 3d20 7061 6462 2e79  ad.ymin = padb.y
-00023d60: 6d61 780a 2020 2020 6468 6561 642e 786d  max.    dhead.xm
-00023d70: 6178 203d 2074 6169 6c2e 786d 696e 202d  ax = tail.xmin -
-00023d80: 2028 7769 7265 5f73 7061 6369 6e67 202b   (wire_spacing +
-00023d90: 2077 6972 655f 7769 6474 6829 202f 2032   wire_width) / 2
-00023da0: 0a20 2020 2063 6f6e 6e65 6374 6f72 203d  .    connector =
-00023db0: 2043 492e 6164 645f 7265 6628 0a20 2020   CI.add_ref(.   
-00023dc0: 2020 2020 2063 6f6d 7061 7373 2873 697a       compass(siz
-00023dd0: 653d 2877 6972 655f 7769 6474 682c 2077  e=(wire_width, w
-00023de0: 6972 655f 7769 6474 6829 2c20 6c61 7965  ire_width), laye
-00023df0: 723d 6f76 6572 6c61 705f 7a69 677a 6167  r=overlap_zigzag
-00023e00: 5f6c 6179 6572 290a 2020 2020 290a 2020  _layer).    ).  
-00023e10: 2020 636f 6e6e 6563 746f 722e 636f 6e6e    connector.conn
-00023e20: 6563 7428 706f 7274 3d22 5322 2c20 6465  ect(port="S", de
-00023e30: 7374 696e 6174 696f 6e3d 6468 6561 642e  stination=dhead.
-00023e40: 706f 7274 735b 2245 225d 290a 2020 2020  ports["E"]).    
-00023e50: 6f6c 645f 706f 7274 203d 2063 6f6e 6e65  old_port = conne
-00023e60: 6374 6f72 2e70 6f72 7473 5b22 4e22 5d0a  ctor.ports["N"].
-00023e70: 2020 2020 7269 6768 7420 3d20 5472 7565      right = True
-00023e80: 0a20 2020 206f 626a 203d 2063 6f6e 6e65  .    obj = conne
-00023e90: 6374 6f72 0a20 2020 2077 6869 6c65 206f  ctor.    while o
-00023ea0: 626a 2e79 6d61 7820 2b20 7769 7265 5f73  bj.ymax + wire_s
-00023eb0: 7061 6369 6e67 202b 2077 6972 655f 7769  pacing + wire_wi
-00023ec0: 6474 6820 3c20 6865 6164 2e79 6d61 783a  dth < head.ymax:
-00023ed0: 0a20 2020 2020 2020 206f 626a 203d 2043  .        obj = C
-00023ee0: 492e 6164 645f 7265 6628 0a20 2020 2020  I.add_ref(.     
-00023ef0: 2020 2020 2020 2063 6f6d 7061 7373 2873         compass(s
-00023f00: 697a 653d 2877 6972 655f 7370 6163 696e  ize=(wire_spacin
-00023f10: 672c 2077 6972 655f 7769 6474 6829 2c20  g, wire_width), 
-00023f20: 6c61 7965 723d 6f76 6572 6c61 705f 7a69  layer=overlap_zi
-00023f30: 677a 6167 5f6c 6179 6572 290a 2020 2020  gzag_layer).    
-00023f40: 2020 2020 290a 2020 2020 2020 2020 6f62      ).        ob
-00023f50: 6a2e 636f 6e6e 6563 7428 706f 7274 3d22  j.connect(port="
-00023f60: 5722 2c20 6465 7374 696e 6174 696f 6e3d  W", destination=
-00023f70: 6f6c 645f 706f 7274 290a 2020 2020 2020  old_port).      
-00023f80: 2020 6f6c 645f 706f 7274 203d 206f 626a    old_port = obj
-00023f90: 2e70 6f72 7473 5b22 4522 5d0a 2020 2020  .ports["E"].    
-00023fa0: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
-00023fb0: 2020 2020 2020 2020 2020 6f62 6a20 3d20            obj = 
-00023fc0: 4349 2e61 6464 5f72 6566 280a 2020 2020  CI.add_ref(.    
-00023fd0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00023fe0: 6173 7328 7369 7a65 3d28 7769 7265 5f77  ass(size=(wire_w
-00023ff0: 6964 7468 2c20 7769 7265 5f77 6964 7468  idth, wire_width
-00024000: 292c 206c 6179 6572 3d6f 7665 726c 6170  ), layer=overlap
-00024010: 5f7a 6967 7a61 675f 6c61 7965 7229 0a20  _zigzag_layer). 
-00024020: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00024030: 2020 2020 2020 2020 206f 626a 2e63 6f6e           obj.con
-00024040: 6e65 6374 2870 6f72 743d 2257 222c 2064  nect(port="W", d
-00024050: 6573 7469 6e61 7469 6f6e 3d6f 6c64 5f70  estination=old_p
-00024060: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-00024070: 2072 6967 6874 203d 2046 616c 7365 0a20   right = False. 
-00024080: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00024090: 2020 2020 2020 2020 206f 626a 203d 2043           obj = C
-000240a0: 492e 6164 645f 7265 6628 0a20 2020 2020  I.add_ref(.     
-000240b0: 2020 2020 2020 2020 2020 2063 6f6d 7061             compa
-000240c0: 7373 2873 697a 653d 2877 6972 655f 7769  ss(size=(wire_wi
-000240d0: 6474 682c 2077 6972 655f 7769 6474 6829  dth, wire_width)
-000240e0: 2c20 6c61 7965 723d 6f76 6572 6c61 705f  , layer=overlap_
-000240f0: 7a69 677a 6167 5f6c 6179 6572 290a 2020  zigzag_layer).  
-00024100: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00024110: 2020 2020 2020 2020 6f62 6a2e 636f 6e6e          obj.conn
-00024120: 6563 7428 706f 7274 3d22 4522 2c20 6465  ect(port="E", de
-00024130: 7374 696e 6174 696f 6e3d 6f6c 645f 706f  stination=old_po
-00024140: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
-00024150: 7269 6768 7420 3d20 5472 7565 0a20 2020  right = True.   
-00024160: 2020 2020 206f 6c64 5f70 6f72 7420 3d20       old_port = 
-00024170: 6f62 6a2e 706f 7274 735b 224e 225d 0a20  obj.ports["N"]. 
-00024180: 2020 2020 2020 206f 626a 203d 2043 492e         obj = CI.
-00024190: 6164 645f 7265 6628 0a20 2020 2020 2020  add_ref(.       
-000241a0: 2020 2020 2063 6f6d 7061 7373 280a 2020       compass(.  
-000241b0: 2020 2020 2020 2020 2020 2020 2020 7369                si
-000241c0: 7a65 3d28 0a20 2020 2020 2020 2020 2020  ze=(.           
-000241d0: 2020 2020 2020 2020 2064 6865 6164 2e78           dhead.x
-000241e0: 6d69 6e20 2d20 2868 6561 642e 786d 6178  min - (head.xmax
-000241f0: 202b 2068 6561 642e 786d 696e 202b 2077   + head.xmin + w
-00024200: 6972 655f 7769 6474 6829 202f 2032 2c0a  ire_width) / 2,.
-00024210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024220: 2020 2020 7769 7265 5f77 6964 7468 2c0a      wire_width,.
-00024230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024240: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00024250: 2020 206c 6179 6572 3d6f 7665 726c 6170     layer=overlap
-00024260: 5f7a 6967 7a61 675f 6c61 7965 722c 0a20  _zigzag_layer,. 
-00024270: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00024280: 2020 2020 2029 0a20 2020 2020 2020 206f       ).        o
-00024290: 626a 2e63 6f6e 6e65 6374 2870 6f72 743d  bj.connect(port=
-000242a0: 2245 222c 2064 6573 7469 6e61 7469 6f6e  "E", destination
-000242b0: 3d6f 6c64 5f70 6f72 7429 0a20 2020 2020  =old_port).     
-000242c0: 2020 206f 6c64 5f70 6f72 7420 3d20 6f62     old_port = ob
-000242d0: 6a2e 706f 7274 735b 2257 225d 0a20 2020  j.ports["W"].   
-000242e0: 2020 2020 206f 626a 203d 2043 492e 6164       obj = CI.ad
-000242f0: 645f 7265 6628 0a20 2020 2020 2020 2020  d_ref(.         
-00024300: 2020 2063 6f6d 7061 7373 2873 697a 653d     compass(size=
-00024310: 2877 6972 655f 7769 6474 682c 2077 6972  (wire_width, wir
-00024320: 655f 7769 6474 6829 2c20 6c61 7965 723d  e_width), layer=
-00024330: 6f76 6572 6c61 705f 7a69 677a 6167 5f6c  overlap_zigzag_l
-00024340: 6179 6572 290a 2020 2020 2020 2020 290a  ayer).        ).
-00024350: 2020 2020 2020 2020 6f62 6a2e 636f 6e6e          obj.conn
-00024360: 6563 7428 706f 7274 3d22 5322 2c20 6465  ect(port="S", de
-00024370: 7374 696e 6174 696f 6e3d 6f6c 645f 706f  stination=old_po
-00024380: 7274 290a 2020 2020 2020 2020 6966 2072  rt).        if r
-00024390: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
-000243a0: 2020 6f6c 645f 706f 7274 203d 206f 626a    old_port = obj
-000243b0: 2e70 6f72 7473 5b22 5722 5d0a 2020 2020  .ports["W"].    
-000243c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000243d0: 2020 2020 2020 6f6c 645f 706f 7274 203d        old_port =
-000243e0: 206f 626a 2e70 6f72 7473 5b22 4522 5d0a   obj.ports["E"].
-000243f0: 0a20 2020 2072 6574 7572 6e20 4349 0a0a  .    return CI..
-00024400: 0a64 6566 205f 7465 7374 5f69 635f 7769  .def _test_ic_wi
-00024410: 7265 5f73 7465 7028 7468 6963 6b5f 7769  re_step(thick_wi
-00024420: 6474 683d 3130 2c20 7468 696e 5f77 6964  dth=10, thin_wid
-00024430: 7468 3d31 2c20 7769 7265 5f6c 6179 6572  th=1, wire_layer
-00024440: 3d32 293a 0a20 2020 2022 2222 4865 6c70  =2):.    """Help
-00024450: 6572 2066 756e 6374 696f 6e20 7573 6564  er function used
-00024460: 2074 6f20 6d61 6b65 2074 6865 2049 4320   to make the IC 
-00024470: 7374 6570 2077 6972 6520 7374 7275 6374  step wire struct
-00024480: 7572 652e 2222 220a 2020 2020 5753 3420  ure.""".    WS4 
-00024490: 3d20 4465 7669 6365 2822 7465 7374 5f69  = Device("test_i
-000244a0: 635f 7374 6570 2229 0a20 2020 2077 6972  c_step").    wir
-000244b0: 655f 7374 6570 6120 3d20 5753 342e 6164  e_stepa = WS4.ad
-000244c0: 645f 7265 6628 0a20 2020 2020 2020 206f  d_ref(.        o
-000244d0: 7074 696d 616c 5f73 7465 7028 7468 6963  ptimal_step(thic
-000244e0: 6b5f 7769 6474 6820 2f20 322c 2074 6869  k_width / 2, thi
-000244f0: 6e5f 7769 6474 6820 2f20 322c 206c 6179  n_width / 2, lay
-00024500: 6572 3d77 6972 655f 6c61 7965 7229 0a20  er=wire_layer). 
-00024510: 2020 2029 0a20 2020 2077 6972 655f 7374     ).    wire_st
-00024520: 6570 6220 3d20 5753 342e 6164 645f 7265  epb = WS4.add_re
-00024530: 6628 0a20 2020 2020 2020 206f 7074 696d  f(.        optim
-00024540: 616c 5f73 7465 7028 7468 696e 5f77 6964  al_step(thin_wid
-00024550: 7468 202f 2032 2c20 7468 6963 6b5f 7769  th / 2, thick_wi
-00024560: 6474 6820 2f20 322c 206c 6179 6572 3d77  dth / 2, layer=w
-00024570: 6972 655f 6c61 7965 7229 0a20 2020 2029  ire_layer).    )
-00024580: 0a20 2020 2077 6972 655f 7374 6570 6320  .    wire_stepc 
-00024590: 3d20 5753 342e 6164 645f 7265 6628 0a20  = WS4.add_ref(. 
-000245a0: 2020 2020 2020 206f 7074 696d 616c 5f73         optimal_s
-000245b0: 7465 7028 7468 6963 6b5f 7769 6474 6820  tep(thick_width 
-000245c0: 2f20 322c 2074 6869 6e5f 7769 6474 6820  / 2, thin_width 
-000245d0: 2f20 322c 206c 6179 6572 3d77 6972 655f  / 2, layer=wire_
-000245e0: 6c61 7965 7229 0a20 2020 2029 0a20 2020  layer).    ).   
-000245f0: 2077 6972 655f 7374 6570 6420 3d20 5753   wire_stepd = WS
-00024600: 342e 6164 645f 7265 6628 0a20 2020 2020  4.add_ref(.     
-00024610: 2020 206f 7074 696d 616c 5f73 7465 7028     optimal_step(
-00024620: 7468 696e 5f77 6964 7468 202f 2032 2c20  thin_width / 2, 
-00024630: 7468 6963 6b5f 7769 6474 6820 2f20 322c  thick_width / 2,
-00024640: 206c 6179 6572 3d77 6972 655f 6c61 7965   layer=wire_laye
-00024650: 7229 0a20 2020 2029 0a20 2020 2077 6972  r).    ).    wir
-00024660: 655f 7374 6570 622e 726f 7461 7465 2831  e_stepb.rotate(1
-00024670: 3830 290a 2020 2020 7769 7265 5f73 7465  80).    wire_ste
-00024680: 7062 2e78 6d69 6e20 3d20 7769 7265 5f73  pb.xmin = wire_s
-00024690: 7465 7061 2e78 6d69 6e0a 2020 2020 7769  tepa.xmin.    wi
-000246a0: 7265 5f73 7465 7063 2e72 6f74 6174 6528  re_stepc.rotate(
-000246b0: 3138 3029 0a20 2020 2077 6972 655f 7374  180).    wire_st
-000246c0: 6570 632e 786d 696e 203d 2077 6972 655f  epc.xmin = wire_
-000246d0: 7374 6570 612e 786d 6178 0a20 2020 2077  stepa.xmax.    w
-000246e0: 6972 655f 7374 6570 642e 786d 696e 203d  ire_stepd.xmin =
-000246f0: 2077 6972 655f 7374 6570 632e 786d 696e   wire_stepc.xmin
-00024700: 0a20 2020 2072 6574 7572 6e20 5753 340a  .    return WS4.
-00024710: 0a0a 6465 6620 7465 7374 5f69 6328 0a20  ..def test_ic(. 
-00024720: 2020 2077 6972 655f 7769 6474 6873 3d5b     wire_widths=[
-00024730: 302e 3235 2c20 302e 352c 2031 2c20 322c  0.25, 0.5, 1, 2,
-00024740: 2034 5d2c 0a20 2020 2077 6972 655f 7769   4],.    wire_wi
-00024750: 6474 6873 5f77 6964 653d 5b30 2e37 352c  dths_wide=[0.75,
-00024760: 2031 2e35 2c20 332c 2034 2c20 365d 2c0a   1.5, 3, 4, 6],.
-00024770: 2020 2020 7061 645f 7369 7a65 3d28 3230      pad_size=(20
-00024780: 302c 2032 3030 292c 0a20 2020 2070 6164  0, 200),.    pad
-00024790: 5f67 6170 3d37 352c 0a20 2020 2077 6972  _gap=75,.    wir
-000247a0: 655f 6c61 7965 723d 302c 0a20 2020 2070  e_layer=0,.    p
-000247b0: 6164 5f6c 6179 6572 3d31 2c0a 2020 2020  ad_layer=1,.    
-000247c0: 676e 645f 6c61 7965 723d 312c 0a29 3a0a  gnd_layer=1,.):.
-000247d0: 2020 2020 2222 2243 7269 7469 6361 6c20      """Critical 
-000247e0: 6375 7272 656e 7420 7465 7374 2073 7472  current test str
-000247f0: 7563 7475 7265 2066 6f72 2073 7570 6572  ucture for super
-00024800: 636f 6e64 7563 7469 6e67 2077 6972 6573  conducting wires
-00024810: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00024820: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00024830: 0a20 2020 2077 6972 655f 7769 6474 6873  .    wire_widths
-00024840: 203a 2061 7272 6179 2d6c 696b 655b 4e5d   : array-like[N]
-00024850: 0a20 2020 2020 2020 2054 6865 2077 6964  .        The wid
-00024860: 7468 7320 6f66 2074 6865 2074 6869 6e6e  ths of the thinn
-00024870: 6573 7420 7061 7274 7320 6f66 2074 6865  est parts of the
-00024880: 2074 6573 7420 7769 7265 732e 0a20 2020   test wires..   
-00024890: 2077 6972 655f 7769 6474 6873 5f77 6964   wire_widths_wid
-000248a0: 6520 3a20 6172 7261 792d 6c69 6b65 5b4e  e : array-like[N
-000248b0: 5d0a 2020 2020 2020 2020 5468 6520 7769  ].        The wi
-000248c0: 6474 6873 206f 6620 7468 6520 7468 6963  dths of the thic
-000248d0: 6b65 7374 2070 6172 7473 206f 6620 7468  kest parts of th
-000248e0: 6520 7465 7374 2077 6972 6573 2e0a 2020  e test wires..  
-000248f0: 2020 7061 645f 7369 7a65 203a 2061 7272    pad_size : arr
-00024900: 6179 2d6c 696b 655b 325d 206f 6620 696e  ay-like[2] of in
-00024910: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-00024920: 2020 2028 7769 6474 682c 2068 6569 6768     (width, heigh
-00024930: 7429 206f 6620 7468 6520 7061 6473 2e0a  t) of the pads..
-00024940: 2020 2020 7061 645f 6761 7020 3a20 696e      pad_gap : in
-00024950: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-00024960: 2020 2044 6973 7461 6e63 6520 6265 7477     Distance betw
-00024970: 6565 6e20 7468 6520 7061 6473 2061 6e64  een the pads and
-00024980: 2074 6865 2067 726f 756e 6420 706c 616e   the ground plan
-00024990: 652e 0a20 2020 2077 6972 655f 6c61 7965  e..    wire_laye
-000249a0: 7220 3a20 696e 740a 2020 2020 2020 2020  r : int.        
-000249b0: 5370 6563 6966 6963 206c 6179 6572 2873  Specific layer(s
-000249c0: 2920 746f 2070 7574 2074 6865 2077 6972  ) to put the wir
-000249d0: 6573 206f 6e2e 0a20 2020 2070 6164 5f6c  es on..    pad_l
-000249e0: 6179 6572 203a 2069 6e74 0a20 2020 2020  ayer : int.     
-000249f0: 2020 2053 7065 6369 6669 6320 6c61 7965     Specific laye
-00024a00: 7228 7329 2074 6f20 7075 7420 7468 6520  r(s) to put the 
-00024a10: 7061 6473 206f 6e2e 0a20 2020 2067 6e64  pads on..    gnd
-00024a20: 5f6c 6179 6572 203a 2069 6e74 206f 7220  _layer : int or 
-00024a30: 4e6f 6e65 0a20 2020 2020 2020 2053 7065  None.        Spe
-00024a40: 6369 6669 6320 6c61 7965 7228 7329 2074  cific layer(s) t
-00024a50: 6f20 7075 7420 7468 6520 6772 6f75 6e64  o put the ground
-00024a60: 2070 6c61 6e65 206f 6e2e 0a0a 2020 2020   plane on...    
-00024a70: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00024a80: 2d2d 2d0a 2020 2020 4465 7669 6365 0a20  ---.    Device. 
-00024a90: 2020 2020 2020 2041 2044 6576 6963 6520         A Device 
-00024aa0: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
-00024ab0: 7269 7469 6361 6c2d 6375 7272 656e 7420  ritical-current 
-00024ac0: 7465 7374 2073 7472 7563 7475 7265 2e0a  test structure..
-00024ad0: 2020 2020 2222 220a 2020 2020 4943 5320      """.    ICS 
-00024ae0: 3d20 4465 7669 6365 2822 7465 7374 5f69  = Device("test_i
-00024af0: 6322 290a 0a20 2020 2023 2069 6620 676e  c")..    # if gn
-00024b00: 645f 6c61 7965 7220 6973 204e 6f6e 653a  d_layer is None:
-00024b10: 2067 6e64 5f6c 6179 6572 203d 2070 6164   gnd_layer = pad
-00024b20: 5f6c 6179 6572 0a20 2020 2074 7261 6e73  _layer.    trans
-00024b30: 6c61 7469 6f6e 203d 2030 0a20 2020 2070  lation = 0.    p
-00024b40: 6164 6220 3d20 4943 532e 6164 645f 7265  adb = ICS.add_re
-00024b50: 6628 0a20 2020 2020 2020 2072 6563 7461  f(.        recta
-00024b60: 6e67 6c65 280a 2020 2020 2020 2020 2020  ngle(.          
-00024b70: 2020 7369 7a65 3d28 6e70 2e73 697a 6528    size=(np.size(
-00024b80: 7769 7265 5f77 6964 7468 7329 202a 2028  wire_widths) * (
-00024b90: 7061 645f 7369 7a65 5b30 5d20 2a20 3620  pad_size[0] * 6 
-00024ba0: 2f20 3529 2c20 7061 645f 7369 7a65 5b31  / 5), pad_size[1
-00024bb0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00024bc0: 6c61 7965 723d 7769 7265 5f6c 6179 6572  layer=wire_layer
-00024bd0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00024be0: 290a 0a20 2020 2070 6164 625f 6f76 6572  )..    padb_over
-00024bf0: 6c61 7920 3d20 4943 532e 6164 645f 7265  lay = ICS.add_re
-00024c00: 6628 0a20 2020 2020 2020 2072 6563 7461  f(.        recta
-00024c10: 6e67 6c65 280a 2020 2020 2020 2020 2020  ngle(.          
-00024c20: 2020 7369 7a65 3d28 0a20 2020 2020 2020    size=(.       
-00024c30: 2020 2020 2020 2020 2028 6e70 2e73 697a           (np.siz
-00024c40: 6528 7769 7265 5f77 6964 7468 7329 202a  e(wire_widths) *
-00024c50: 2028 7061 645f 7369 7a65 5b30 5d20 2a20   (pad_size[0] * 
-00024c60: 3620 2f20 3529 2920 2a20 3920 2f20 3130  6 / 5)) * 9 / 10
-00024c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00024c80: 2020 7061 645f 7369 7a65 5b31 5d20 2a20    pad_size[1] * 
-00024c90: 3920 2f20 3130 2c0a 2020 2020 2020 2020  9 / 10,.        
-00024ca0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00024cb0: 2020 206c 6179 6572 3d67 6e64 5f6c 6179     layer=gnd_lay
-00024cc0: 6572 2c0a 2020 2020 2020 2020 290a 2020  er,.        ).  
-00024cd0: 2020 290a 2020 2020 7061 6462 5f6f 7665    ).    padb_ove
-00024ce0: 726c 6179 2e63 656e 7465 7220 3d20 7061  rlay.center = pa
-00024cf0: 6462 2e63 656e 7465 720a 2020 2020 7061  db.center.    pa
-00024d00: 6462 5f6f 7665 726c 6179 2e79 6d69 6e20  db_overlay.ymin 
-00024d10: 3d20 7061 6462 2e79 6d69 6e0a 2020 2020  = padb.ymin.    
-00024d20: 666f 7220 692c 2078 2069 6e20 656e 756d  for i, x in enum
-00024d30: 6572 6174 6528 7769 7265 5f77 6964 7468  erate(wire_width
-00024d40: 735f 7769 6465 293a 0a20 2020 2020 2020  s_wide):.       
-00024d50: 2070 6164 7420 3d20 4943 532e 6164 645f   padt = ICS.add_
-00024d60: 7265 6628 7265 6374 616e 676c 6528 7061  ref(rectangle(pa
-00024d70: 645f 7369 7a65 2c20 7769 7265 5f6c 6179  d_size, wire_lay
-00024d80: 6572 2929 0a20 2020 2020 2020 2070 6164  er)).        pad
-00024d90: 742e 786d 696e 203d 2070 6164 622e 786d  t.xmin = padb.xm
-00024da0: 696e 202b 2074 7261 6e73 6c61 7469 6f6e  in + translation
-00024db0: 0a20 2020 2020 2020 2070 6164 742e 796d  .        padt.ym
-00024dc0: 696e 203d 2070 6164 622e 796d 6178 202b  in = padb.ymax +
-00024dd0: 2070 6164 5f67 6170 0a20 2020 2020 2020   pad_gap.       
-00024de0: 2070 6164 745f 6f76 6572 6c61 7920 3d20   padt_overlay = 
-00024df0: 4943 532e 6164 645f 7265 6628 0a20 2020  ICS.add_ref(.   
-00024e00: 2020 2020 2020 2020 2072 6563 7461 6e67           rectang
-00024e10: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00024e20: 2020 2020 7369 7a65 3d28 7061 645f 7369      size=(pad_si
-00024e30: 7a65 5b30 5d20 2a20 3920 2f20 3130 2c20  ze[0] * 9 / 10, 
-00024e40: 7061 645f 7369 7a65 5b31 5d20 2a20 3920  pad_size[1] * 9 
-00024e50: 2f20 3130 292c 206c 6179 6572 3d70 6164  / 10), layer=pad
-00024e60: 5f6c 6179 6572 0a20 2020 2020 2020 2020  _layer.         
-00024e70: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
-00024e80: 2020 2020 2020 2070 6164 745f 6f76 6572         padt_over
-00024e90: 6c61 792e 6365 6e74 6572 203d 2070 6164  lay.center = pad
-00024ea0: 742e 6365 6e74 6572 0a20 2020 2020 2020  t.center.       
-00024eb0: 2070 6164 745f 6f76 6572 6c61 792e 796d   padt_overlay.ym
-00024ec0: 6178 203d 2070 6164 742e 796d 6178 0a20  ax = padt.ymax. 
-00024ed0: 2020 2020 2020 2064 6966 6665 7265 6e63         differenc
-00024ee0: 6520 3d20 7061 6474 2e79 6d69 6e20 2d20  e = padt.ymin - 
-00024ef0: 7061 6462 2e79 6d61 780a 2020 2020 2020  padb.ymax.      
-00024f00: 2020 7769 7265 5f73 7465 7020 3d20 4943    wire_step = IC
-00024f10: 532e 6164 645f 7265 6628 0a20 2020 2020  S.add_ref(.     
-00024f20: 2020 2020 2020 205f 7465 7374 5f69 635f         _test_ic_
-00024f30: 7769 7265 5f73 7465 7028 0a20 2020 2020  wire_step(.     
-00024f40: 2020 2020 2020 2020 2020 2077 6972 655f             wire_
-00024f50: 7769 6474 6873 5f77 6964 655b 695d 2c20  widths_wide[i], 
-00024f60: 7769 7265 5f77 6964 7468 735b 695d 2c20  wire_widths[i], 
-00024f70: 7769 7265 5f6c 6179 6572 3d77 6972 655f  wire_layer=wire_
-00024f80: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
-00024f90: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-00024fa0: 2020 2020 2020 7769 7265 5f73 7465 702e        wire_step.
-00024fb0: 726f 7461 7465 2839 3029 0a20 2020 2020  rotate(90).     
-00024fc0: 2020 2077 6972 655f 7374 6570 2e63 656e     wire_step.cen
-00024fd0: 7465 7220 3d20 2870 6164 742e 6365 6e74  ter = (padt.cent
-00024fe0: 6572 5b30 5d2c 2070 6164 622e 796d 6178  er[0], padb.ymax
-00024ff0: 202b 2064 6966 6665 7265 6e63 6520 2f20   + difference / 
-00025000: 3229 0a20 2020 2020 2020 2074 7261 6e73  2).        trans
-00025010: 6c61 7469 6f6e 203d 2074 7261 6e73 6c61  lation = transla
-00025020: 7469 6f6e 202b 2070 6164 5f73 697a 655b  tion + pad_size[
-00025030: 305d 202a 2031 3220 2f20 3130 0a20 2020  0] * 12 / 10.   
-00025040: 2020 2020 2063 6f6e 6e5f 7769 7265 5f74       conn_wire_t
-00025050: 6f70 203d 2049 4353 2e61 6464 5f72 6566  op = ICS.add_ref
-00025060: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00025070: 6374 616e 676c 6528 0a20 2020 2020 2020  ctangle(.       
-00025080: 2020 2020 2020 2020 2073 697a 653d 2877           size=(w
-00025090: 6972 655f 7769 6474 6873 5f77 6964 655b  ire_widths_wide[
-000250a0: 695d 2c20 7061 6474 2e79 6d69 6e20 2d20  i], padt.ymin - 
-000250b0: 7769 7265 5f73 7465 702e 796d 6178 292c  wire_step.ymax),
-000250c0: 206c 6179 6572 3d77 6972 655f 6c61 7965   layer=wire_laye
-000250d0: 720a 2020 2020 2020 2020 2020 2020 290a  r.            ).
-000250e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000250f0: 2020 636f 6e6e 5f77 6972 655f 626f 7474    conn_wire_bott
-00025100: 6f6d 203d 2049 4353 2e61 6464 5f72 6566  om = ICS.add_ref
-00025110: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00025120: 6374 616e 676c 6528 0a20 2020 2020 2020  ctangle(.       
-00025130: 2020 2020 2020 2020 2073 697a 653d 2877           size=(w
-00025140: 6972 655f 7769 6474 6873 5f77 6964 655b  ire_widths_wide[
-00025150: 695d 2c20 7769 7265 5f73 7465 702e 796d  i], wire_step.ym
-00025160: 696e 202d 2070 6164 622e 796d 6178 292c  in - padb.ymax),
-00025170: 206c 6179 6572 3d77 6972 655f 6c61 7965   layer=wire_laye
-00025180: 720a 2020 2020 2020 2020 2020 2020 290a  r.            ).
-00025190: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000251a0: 2020 636f 6e6e 5f77 6972 655f 746f 702e    conn_wire_top.
-000251b0: 796d 6178 203d 2070 6164 742e 796d 696e  ymax = padt.ymin
-000251c0: 0a20 2020 2020 2020 2063 6f6e 6e5f 7769  .        conn_wi
-000251d0: 7265 5f74 6f70 2e78 6d69 6e20 3d20 7769  re_top.xmin = wi
-000251e0: 7265 5f73 7465 702e 786d 696e 0a20 2020  re_step.xmin.   
-000251f0: 2020 2020 2063 6f6e 6e5f 7769 7265 5f62       conn_wire_b
-00025200: 6f74 746f 6d2e 796d 696e 203d 2070 6164  ottom.ymin = pad
-00025210: 622e 796d 6178 0a20 2020 2020 2020 2063  b.ymax.        c
-00025220: 6f6e 6e5f 7769 7265 5f62 6f74 746f 6d2e  onn_wire_bottom.
-00025230: 786d 696e 203d 2077 6972 655f 7374 6570  xmin = wire_step
-00025240: 2e78 6d69 6e0a 0a20 2020 2072 6574 7572  .xmin..    retur
-00025250: 6e20 4943 530a 0a0a 6465 6620 7465 7374  n ICS...def test
-00025260: 5f72 6573 280a 2020 2020 7061 645f 7369  _res(.    pad_si
-00025270: 7a65 3d5b 3530 2c20 3530 5d2c 206e 756d  ze=[50, 50], num
-00025280: 5f73 7175 6172 6573 3d31 3030 302c 2077  _squares=1000, w
-00025290: 6964 7468 3d31 2c20 7265 735f 6c61 7965  idth=1, res_laye
-000252a0: 723d 302c 2070 6164 5f6c 6179 6572 3d31  r=0, pad_layer=1
-000252b0: 2c20 676e 645f 6c61 7965 723d 320a 293a  , gnd_layer=2.):
-000252c0: 0a20 2020 2022 2222 4372 6561 7465 7320  .    """Creates 
-000252d0: 616e 2065 6666 6963 6965 6e74 2072 6573  an efficient res
-000252e0: 6f6e 6174 6f72 2073 7472 7563 7475 7265  onator structure
-000252f0: 2066 6f72 2061 2077 6166 6572 206c 6179   for a wafer lay
-00025300: 6f75 742e 0a0a 2020 2020 5061 7261 6d65  out...    Parame
-00025310: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00025320: 2d2d 2d0a 2020 2020 7061 645f 7369 7a65  ---.    pad_size
-00025330: 203a 2061 7272 6179 2d6c 696b 655b 325d   : array-like[2]
-00025340: 206f 6620 696e 7420 6f72 2066 6c6f 6174   of int or float
-00025350: 0a20 2020 2020 2020 2028 7769 6474 682c  .        (width,
-00025360: 2068 6569 6768 7429 206f 6620 7468 6520   height) of the 
-00025370: 7477 6f20 6d61 7463 6865 6420 696d 7065  two matched impe
-00025380: 6461 6e63 6520 7061 6473 2069 6e20 6d69  dance pads in mi
-00025390: 6372 6f6e 732e 0a20 2020 206e 756d 5f73  crons..    num_s
-000253a0: 7175 6172 6573 203a 2069 6e74 206f 7220  quares : int or 
-000253b0: 666c 6f61 740a 2020 2020 2020 2020 4e75  float.        Nu
-000253c0: 6d62 6572 206f 6620 7371 7561 7265 7320  mber of squares 
-000253d0: 636f 6d70 7269 7369 6e67 2074 6865 2072  comprising the r
-000253e0: 6573 6f6e 6174 6f72 2077 6972 652e 0a20  esonator wire.. 
-000253f0: 2020 2077 6964 7468 203a 2069 6e74 206f     width : int o
-00025400: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
-00025410: 5468 6520 7769 6474 6820 6f66 2074 6865  The width of the
-00025420: 2073 7175 6172 6573 2069 6e20 6d69 6372   squares in micr
-00025430: 6f6e 732e 0a20 2020 2072 6573 5f6c 6179  ons..    res_lay
-00025440: 6572 203a 2069 6e74 0a20 2020 2020 2020  er : int.       
-00025450: 2053 7065 6369 6669 6320 6c61 7965 7228   Specific layer(
-00025460: 7329 2074 6f20 7075 7420 7468 6520 7265  s) to put the re
-00025470: 736f 6e61 746f 7220 7374 7275 6374 7572  sonator structur
-00025480: 6520 6f6e 2e0a 2020 2020 7061 645f 6c61  e on..    pad_la
-00025490: 7965 7220 3a20 696e 7420 6f72 204e 6f6e  yer : int or Non
-000254a0: 650a 2020 2020 2020 2020 5370 6563 6966  e.        Specif
-000254b0: 6963 206c 6179 6572 2873 2920 746f 2070  ic layer(s) to p
-000254c0: 7574 2074 6865 2070 6164 7320 6f6e 2e0a  ut the pads on..
-000254d0: 2020 2020 676e 645f 6c61 7965 7220 3a20      gnd_layer : 
-000254e0: 2069 6e74 206f 7220 4e6f 6e65 0a20 2020   int or None.   
-000254f0: 2020 2020 2053 7065 6369 6669 6320 6c61       Specific la
-00025500: 7965 7228 7329 2074 6f20 7075 7420 7468  yer(s) to put th
-00025510: 6520 6772 6f75 6e64 2070 6c61 6e65 206f  e ground plane o
-00025520: 6e2e 0a0a 2020 2020 5265 7475 726e 730a  n...    Returns.
-00025530: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00025540: 5020 3a20 4465 7669 6365 0a20 2020 2020  P : Device.     
-00025550: 2020 2041 2044 6576 6963 6520 636f 6e74     A Device cont
-00025560: 6169 6e69 6e67 2061 6e20 6566 6669 6369  aining an effici
-00025570: 656e 7420 7265 736f 6e61 746f 7220 7374  ent resonator st
-00025580: 7275 6374 7572 652e 0a20 2020 2022 2222  ructure..    """
-00025590: 0a20 2020 2078 203d 2070 6164 5f73 697a  .    x = pad_siz
-000255a0: 655b 305d 0a20 2020 207a 203d 2070 6164  e[0].    z = pad
-000255b0: 5f73 697a 655b 315d 0a0a 2020 2020 2320  _size[1]..    # 
-000255c0: 4368 6563 6b69 6e67 2076 616c 6964 6974  Checking validit
-000255d0: 7920 6f66 2069 6e70 7574 0a20 2020 2069  y of input.    i
-000255e0: 6620 7820 3c3d 2030 206f 7220 7a20 3c3d  f x <= 0 or z <=
-000255f0: 2030 3a0a 2020 2020 2020 2020 7261 6973   0:.        rais
-00025600: 6520 5661 6c75 6545 7272 6f72 2822 5061  e ValueError("Pa
-00025610: 6420 6d75 7374 2068 6176 6520 706f 7369  d must have posi
-00025620: 7469 7665 2c20 7265 616c 2064 696d 656e  tive, real dimen
-00025630: 7369 6f6e 7322 290a 2020 2020 656c 6966  sions").    elif
-00025640: 2077 6964 7468 203e 207a 3a0a 2020 2020   width > z:.    
-00025650: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00025660: 7272 6f72 2822 5769 6474 6820 6f66 2063  rror("Width of c
-00025670: 656c 6c20 6361 6e6e 6f74 2062 6520 6772  ell cannot be gr
-00025680: 6561 7465 7220 7468 616e 2068 6569 6768  eater than heigh
-00025690: 7420 6f66 2070 6164 2229 0a20 2020 2065  t of pad").    e
-000256a0: 6c69 6620 6e75 6d5f 7371 7561 7265 7320  lif num_squares 
-000256b0: 3c3d 2030 3a0a 2020 2020 2020 2020 7261  <= 0:.        ra
-000256c0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-000256d0: 4e75 6d62 6572 206f 6620 7371 7561 7265  Number of square
-000256e0: 7320 6d75 7374 2062 6520 6120 706f 7369  s must be a posi
-000256f0: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-00025700: 2229 0a20 2020 2065 6c69 6620 7769 6474  ").    elif widt
-00025710: 6820 3c3d 2030 3a0a 2020 2020 2020 2020  h <= 0:.        
-00025720: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00025730: 2822 5769 6474 6820 6f66 2063 656c 6c20  ("Width of cell 
-00025740: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-00025750: 7665 2072 6561 6c20 6e75 6d62 6572 2229  ve real number")
-00025760: 0a0a 2020 2020 2320 5065 7266 6f72 6d69  ..    # Performi
-00025770: 6e67 2070 7265 6c69 6d69 6e61 7279 2063  ng preliminary c
-00025780: 616c 6375 6c61 7469 6f6e 730a 2020 2020  alculations.    
-00025790: 6e75 6d5f 726f 7773 203d 2069 6e74 286e  num_rows = int(n
-000257a0: 702e 666c 6f6f 7228 7a20 2f20 2832 202a  p.floor(z / (2 *
-000257b0: 2077 6964 7468 2929 290a 2020 2020 6966   width))).    if
-000257c0: 206e 756d 5f72 6f77 7320 2520 3220 3d3d   num_rows % 2 ==
-000257d0: 2030 3a0a 2020 2020 2020 2020 6e75 6d5f   0:.        num_
-000257e0: 726f 7773 202d 3d20 310a 2020 2020 6e75  rows -= 1.    nu
-000257f0: 6d5f 636f 6c75 6d6e 7320 3d20 6e75 6d5f  m_columns = num_
-00025800: 726f 7773 202d 2031 0a20 2020 2073 7175  rows - 1.    squ
-00025810: 6172 6573 5f69 6e5f 726f 7720 3d20 286e  ares_in_row = (n
-00025820: 756d 5f73 7175 6172 6573 202d 206e 756d  um_squares - num
-00025830: 5f63 6f6c 756d 6e73 202d 2032 2920 2f20  _columns - 2) / 
-00025840: 6e75 6d5f 726f 7773 0a0a 2020 2020 2320  num_rows..    # 
-00025850: 436f 6d70 656e 7361 7469 6e67 2066 6f72  Compensating for
-00025860: 2077 6569 7264 2065 6467 6520 6361 7365   weird edge case
-00025870: 730a 2020 2020 6966 2073 7175 6172 6573  s.    if squares
-00025880: 5f69 6e5f 726f 7720 3c20 313a 0a20 2020  _in_row < 1:.   
-00025890: 2020 2020 206e 756d 5f72 6f77 7320 3d20       num_rows = 
-000258a0: 696e 7428 726f 756e 6428 6e75 6d5f 726f  int(round(num_ro
-000258b0: 7773 202f 2032 2920 2d20 3229 0a20 2020  ws / 2) - 2).   
-000258c0: 2020 2020 2073 7175 6172 6573 5f69 6e5f       squares_in_
-000258d0: 726f 7720 3d20 310a 2020 2020 6966 2077  row = 1.    if w
-000258e0: 6964 7468 202a 2032 203e 207a 3a0a 2020  idth * 2 > z:.  
-000258f0: 2020 2020 2020 6e75 6d5f 726f 7773 203d        num_rows =
-00025900: 2031 0a20 2020 2020 2020 2073 7175 6172   1.        squar
-00025910: 6573 5f69 6e5f 726f 7720 3d20 6e75 6d5f  es_in_row = num_
-00025920: 7371 7561 7265 7320 2d20 320a 0a20 2020  squares - 2..   
-00025930: 206c 656e 6774 685f 726f 7720 3d20 7371   length_row = sq
-00025940: 7561 7265 735f 696e 5f72 6f77 202a 2077  uares_in_row * w
-00025950: 6964 7468 0a0a 2020 2020 2320 4372 6561  idth..    # Crea
-00025960: 7469 6e67 2072 6f77 2f63 6f6c 756d 6e20  ting row/column 
-00025970: 636f 726e 6572 2063 6f6d 6269 6e61 7469  corner combinati
-00025980: 6f6e 2073 7472 7563 7475 7265 0a20 2020  on structure.   
-00025990: 2054 203d 2044 6576 6963 6528 290a 2020   T = Device().  
-000259a0: 2020 526f 7720 3d20 7265 6374 616e 676c    Row = rectangl
-000259b0: 6528 7369 7a65 3d28 6c65 6e67 7468 5f72  e(size=(length_r
-000259c0: 6f77 2c20 7769 6474 6829 2c20 6c61 7965  ow, width), laye
-000259d0: 723d 7265 735f 6c61 7965 7229 0a20 2020  r=res_layer).   
-000259e0: 2043 6f6c 203d 2072 6563 7461 6e67 6c65   Col = rectangle
-000259f0: 2873 697a 653d 2877 6964 7468 2c20 7769  (size=(width, wi
-00025a00: 6474 6829 2c20 6c61 7965 723d 7265 735f  dth), layer=res_
-00025a10: 6c61 7965 7229 0a0a 2020 2020 542e 6164  layer)..    T.ad
-00025a20: 645f 7265 6628 526f 7729 0a20 2020 2063  d_ref(Row).    c
-00025a30: 6f6c 203d 2054 2e61 6464 5f72 6566 2843  ol = T.add_ref(C
-00025a40: 6f6c 290a 2020 2020 636f 6c2e 6d6f 7665  ol).    col.move
-00025a50: 285b 6c65 6e67 7468 5f72 6f77 202d 2077  ([length_row - w
-00025a60: 6964 7468 2c20 2d77 6964 7468 5d29 0a0a  idth, -width])..
-00025a70: 2020 2020 2320 4372 6561 7469 6e67 2065      # Creating e
-00025a80: 6e74 6972 6520 7761 7665 6775 6964 6520  ntire waveguide 
-00025a90: 6e65 740a 2020 2020 4e20 3d20 4465 7669  net.    N = Devi
-00025aa0: 6365 2822 6e65 7422 290a 2020 2020 6e20  ce("net").    n 
-00025ab0: 3d20 310a 2020 2020 666f 7220 6920 696e  = 1.    for i in
-00025ac0: 2072 616e 6765 286e 756d 5f72 6f77 7329   range(num_rows)
-00025ad0: 3a0a 2020 2020 2020 2020 6966 2069 2021  :.        if i !
-00025ae0: 3d20 6e75 6d5f 726f 7773 202d 2031 3a0a  = num_rows - 1:.
-00025af0: 2020 2020 2020 2020 2020 2020 6420 3d20              d = 
-00025b00: 4e2e 6164 645f 7265 6628 5429 0a20 2020  N.add_ref(T).   
-00025b10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00025b20: 2020 2020 2020 2064 203d 204e 2e61 6464         d = N.add
-00025b30: 5f72 6566 2852 6f77 290a 2020 2020 2020  _ref(Row).      
-00025b40: 2020 6966 206e 2025 2032 203d 3d20 303a    if n % 2 == 0:
-00025b50: 0a20 2020 2020 2020 2020 2020 2064 2e6d  .            d.m
-00025b60: 6972 726f 7228 7031 3d28 642e 782c 2064  irror(p1=(d.x, d
-00025b70: 2e79 6d61 7829 2c20 7032 3d28 642e 782c  .ymax), p2=(d.x,
-00025b80: 2064 2e79 6d69 6e29 290a 2020 2020 2020   d.ymin)).      
-00025b90: 2020 642e 6d6f 7665 7928 2d28 6e20 2d20    d.movey(-(n - 
-00025ba0: 3129 202a 2054 2e79 7369 7a65 290a 2020  1) * T.ysize).  
-00025bb0: 2020 2020 2020 6e20 2b3d 2031 0a20 2020        n += 1.   
-00025bc0: 2064 203d 204e 2e61 6464 5f72 6566 2843   d = N.add_ref(C
-00025bd0: 6f6c 292e 6d6f 7665 7828 2d77 6964 7468  ol).movex(-width
-00025be0: 290a 2020 2020 6420 3d20 4e2e 6164 645f  ).    d = N.add_
-00025bf0: 7265 6628 436f 6c29 2e6d 6f76 6528 5b6c  ref(Col).move([l
-00025c00: 656e 6774 685f 726f 772c 202d 286e 202d  ength_row, -(n -
-00025c10: 2032 2920 2a20 542e 7973 697a 655d 290a   2) * T.ysize]).
-00025c20: 0a20 2020 2023 2043 7265 6174 696e 6720  .    # Creating 
-00025c30: 7061 6473 0a20 2020 2050 203d 2044 6576  pads.    P = Dev
-00025c40: 6963 6528 2274 6573 745f 7265 7322 290a  ice("test_res").
-00025c50: 2020 2020 5061 6431 203d 2072 6563 7461      Pad1 = recta
-00025c60: 6e67 6c65 2873 697a 653d 2878 2c20 7a29  ngle(size=(x, z)
-00025c70: 2c20 6c61 7965 723d 7061 645f 6c61 7965  , layer=pad_laye
-00025c80: 7229 0a20 2020 2050 6164 3220 3d20 7265  r).    Pad2 = re
-00025c90: 6374 616e 676c 6528 7369 7a65 3d28 7820  ctangle(size=(x 
-00025ca0: 2b20 352c 207a 292c 206c 6179 6572 3d70  + 5, z), layer=p
-00025cb0: 6164 5f6c 6179 6572 290a 2020 2020 476e  ad_layer).    Gn
-00025cc0: 6431 203d 206f 6666 7365 7428 5061 6431  d1 = offset(Pad1
-00025cd0: 2c20 6469 7374 616e 6365 3d2d 352c 206c  , distance=-5, l
-00025ce0: 6179 6572 3d67 6e64 5f6c 6179 6572 290a  ayer=gnd_layer).
-00025cf0: 2020 2020 476e 6432 203d 206f 6666 7365      Gnd2 = offse
-00025d00: 7428 5061 6432 2c20 6469 7374 616e 6365  t(Pad2, distance
-00025d10: 3d2d 352c 206c 6179 6572 3d67 6e64 5f6c  =-5, layer=gnd_l
-00025d20: 6179 6572 290a 2020 2020 7061 6431 203d  ayer).    pad1 =
-00025d30: 2050 2e61 6464 5f72 6566 2850 6164 3129   P.add_ref(Pad1)
-00025d40: 2e6d 6f76 6578 282d 7820 2d20 7769 6474  .movex(-x - widt
-00025d50: 6829 0a20 2020 2070 6164 3220 3d20 502e  h).    pad2 = P.
-00025d60: 6164 645f 7265 6628 5061 6431 292e 6d6f  add_ref(Pad1).mo
-00025d70: 7665 7828 6c65 6e67 7468 5f72 6f77 202b  vex(length_row +
-00025d80: 2077 6964 7468 290a 2020 2020 502e 6164   width).    P.ad
-00025d90: 645f 7265 6628 476e 6431 292e 6365 6e74  d_ref(Gnd1).cent
-00025da0: 6572 203d 2070 6164 312e 6365 6e74 6572  er = pad1.center
-00025db0: 2020 2320 676e 6431 0a20 2020 2067 6e64    # gnd1.    gnd
-00025dc0: 3220 3d20 502e 6164 645f 7265 6628 476e  2 = P.add_ref(Gn
-00025dd0: 6432 290a 2020 2020 502e 6164 645f 7265  d2).    P.add_re
-00025de0: 6628 4e29 2e79 203d 2070 6164 312e 7920  f(N).y = pad1.y 
-00025df0: 2023 206e 6574 730a 2020 2020 676e 6432   # nets.    gnd2
-00025e00: 2e63 656e 7465 7220 3d20 7061 6432 2e63  .center = pad2.c
-00025e10: 656e 7465 720a 2020 2020 676e 6432 2e6d  enter.    gnd2.m
-00025e20: 6f76 6578 2832 2e35 290a 0a20 2020 2072  ovex(2.5)..    r
-00025e30: 6574 7572 6e20 500a 0a0a 2320 3d3d 3d3d  eturn P...# ====
-00025e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025e60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025e70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025e80: 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 0a23 204f  ==========.#.# O
-00025e90: 7074 696d 616c 2063 7572 7265 6e74 2d63  ptimal current-c
-00025ea0: 726f 7764 696e 6720 7375 7065 7263 6f6e  rowding supercon
-00025eb0: 6475 6374 696e 6720 7374 7275 6374 7572  ducting structur
-00025ec0: 6573 0a23 0a23 203d 3d3d 3d3d 3d3d 3d3d  es.#.# =========
+00021ef0: 2d20 6375 7272 656e 745f 7769 6474 6829  - current_width)
+00021f00: 203e 2033 202a 2077 6972 655f 7769 6474   > 3 * wire_widt
+00021f10: 680a 2020 2020 293a 0a20 2020 2020 2020  h.    ):.       
+00021f20: 2074 6169 6c20 3d20 5652 2e61 6464 5f72   tail = VR.add_r
+00021f30: 6566 280a 2020 2020 2020 2020 2020 2020  ef(.            
+00021f40: 636f 6d70 6173 7328 0a20 2020 2020 2020  compass(.       
+00021f50: 2020 2020 2020 2020 2073 697a 653d 286d           size=(m
+00021f60: 696e 5f70 6164 5f73 7061 6369 6e67 202d  in_pad_spacing -
+00021f70: 2063 7572 7265 6e74 5f77 6964 7468 202b   current_width +
+00021f80: 2077 6972 655f 7769 6474 682c 2077 6972   wire_width, wir
+00021f90: 655f 7769 6474 6829 2c0a 2020 2020 2020  e_width),.      
+00021fa0: 2020 2020 2020 2020 2020 6c61 7965 723d            layer=
+00021fb0: 7769 7269 6e67 315f 6c61 7965 722c 0a20  wiring1_layer,. 
+00021fc0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00021fd0: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+00021fe0: 6169 6c5f 6f76 6572 6c61 7920 3d20 5652  ail_overlay = VR
+00021ff0: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00022000: 2020 2020 2020 636f 6d70 6173 7328 0a20        compass(. 
+00022010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022020: 697a 653d 286d 696e 5f70 6164 5f73 7061  ize=(min_pad_spa
+00022030: 6369 6e67 202d 2063 7572 7265 6e74 5f77  cing - current_w
+00022040: 6964 7468 202b 2077 6972 655f 7769 6474  idth + wire_widt
+00022050: 682c 2077 6972 655f 7769 6474 6829 2c0a  h, wire_width),.
+00022060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022070: 6c61 7965 723d 7061 645f 6c61 7965 722c  layer=pad_layer,
+00022080: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00022090: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+000220a0: 653a 0a20 2020 2020 2020 2074 6169 6c20  e:.        tail 
+000220b0: 3d20 5652 2e61 6464 5f72 6566 280a 2020  = VR.add_ref(.  
+000220c0: 2020 2020 2020 2020 2020 636f 6d70 6173            compas
+000220d0: 7328 7369 7a65 3d28 3320 2a20 7769 7265  s(size=(3 * wire
+000220e0: 5f77 6964 7468 2c20 7769 7265 5f77 6964  _width, wire_wid
+000220f0: 7468 292c 206c 6179 6572 3d77 6972 696e  th), layer=wirin
+00022100: 6731 5f6c 6179 6572 290a 2020 2020 2020  g1_layer).      
+00022110: 2020 290a 2020 2020 2020 2020 7461 696c    ).        tail
+00022120: 5f6f 7665 726c 6179 203d 2056 522e 6164  _overlay = VR.ad
+00022130: 645f 7265 6628 0a20 2020 2020 2020 2020  d_ref(.         
+00022140: 2020 2063 6f6d 7061 7373 2873 697a 653d     compass(size=
+00022150: 2833 202a 2077 6972 655f 7769 6474 682c  (3 * wire_width,
+00022160: 2077 6972 655f 7769 6474 6829 2c20 6c61   wire_width), la
+00022170: 7965 723d 7769 7269 6e67 315f 6c61 7965  yer=wiring1_laye
+00022180: 7229 0a20 2020 2020 2020 2029 0a0a 2020  r).        )..  
+00022190: 2020 6966 2075 7020 616e 6420 6e6f 7420    if up and not 
+000221a0: 6564 6765 3a0a 2020 2020 2020 2020 7461  edge:.        ta
+000221b0: 696c 2e63 6f6e 6e65 6374 2870 6f72 743d  il.connect(port=
+000221c0: 2257 222c 2064 6573 7469 6e61 7469 6f6e  "W", destination
+000221d0: 3d6f 626a 2e70 6f72 7473 5b22 5322 5d2c  =obj.ports["S"],
+000221e0: 206f 7665 726c 6170 3d77 6972 655f 7769   overlap=wire_wi
+000221f0: 6474 6829 0a20 2020 2020 2020 2074 6169  dth).        tai
+00022200: 6c5f 6f76 6572 6c61 792e 636f 6e6e 6563  l_overlay.connec
+00022210: 7428 706f 7274 3d22 5722 2c20 6465 7374  t(port="W", dest
+00022220: 696e 6174 696f 6e3d 6f62 6a2e 706f 7274  ination=obj.port
+00022230: 735b 2253 225d 2c20 6f76 6572 6c61 703d  s["S"], overlap=
+00022240: 7769 7265 5f77 6964 7468 290a 2020 2020  wire_width).    
+00022250: 656c 6966 2064 6f77 6e20 616e 6420 6e6f  elif down and no
+00022260: 7420 6564 6765 3a0a 2020 2020 2020 2020  t edge:.        
+00022270: 7461 696c 2e63 6f6e 6e65 6374 2870 6f72  tail.connect(por
+00022280: 743d 2257 222c 2064 6573 7469 6e61 7469  t="W", destinati
+00022290: 6f6e 3d6f 626a 2e70 6f72 7473 5b22 4e22  on=obj.ports["N"
+000222a0: 5d2c 206f 7665 726c 6170 3d77 6972 655f  ], overlap=wire_
+000222b0: 7769 6474 6829 0a20 2020 2020 2020 2074  width).        t
+000222c0: 6169 6c5f 6f76 6572 6c61 792e 636f 6e6e  ail_overlay.conn
+000222d0: 6563 7428 706f 7274 3d22 5722 2c20 6465  ect(port="W", de
+000222e0: 7374 696e 6174 696f 6e3d 6f62 6a2e 706f  stination=obj.po
+000222f0: 7274 735b 224e 225d 2c20 6f76 6572 6c61  rts["N"], overla
+00022300: 703d 7769 7265 5f77 6964 7468 290a 2020  p=wire_width).  
+00022310: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00022320: 7461 696c 2e63 6f6e 6e65 6374 2870 6f72  tail.connect(por
+00022330: 743d 2257 222c 2064 6573 7469 6e61 7469  t="W", destinati
+00022340: 6f6e 3d6f 626a 2e70 6f72 7473 5b22 4522  on=obj.ports["E"
+00022350: 5d2c 206f 7665 726c 6170 3d77 6972 655f  ], overlap=wire_
+00022360: 7769 6474 6829 0a20 2020 2020 2020 2074  width).        t
+00022370: 6169 6c5f 6f76 6572 6c61 792e 636f 6e6e  ail_overlay.conn
+00022380: 6563 7428 706f 7274 3d22 5722 2c20 6465  ect(port="W", de
+00022390: 7374 696e 6174 696f 6e3d 6f62 6a2e 706f  stination=obj.po
+000223a0: 7274 735b 2245 225d 2c20 6f76 6572 6c61  rts["E"], overla
+000223b0: 703d 7769 7265 5f77 6964 7468 290a 0a20  p=wire_width).. 
+000223c0: 2020 2070 6164 322e 786d 696e 203d 2074     pad2.xmin = t
+000223d0: 6169 6c2e 786d 6178 0a20 2020 2070 6164  ail.xmax.    pad
+000223e0: 325f 6f76 6572 6c61 792e 786d 696e 203d  2_overlay.xmin =
+000223f0: 2070 6164 322e 786d 696e 0a20 2020 2070   pad2.xmin.    p
+00022400: 6164 325f 6f76 6572 6c61 792e 796d 696e  ad2_overlay.ymin
+00022410: 203d 2070 6164 322e 796d 696e 0a0a 2020   = pad2.ymin..  
+00022420: 2020 7265 7475 726e 2056 520a 0a0a 6465    return VR...de
+00022430: 6620 7465 7374 5f63 6f6d 6228 0a20 2020  f test_comb(.   
+00022440: 2070 6164 5f73 697a 653d 2832 3030 2c20   pad_size=(200, 
+00022450: 3230 3029 2c0a 2020 2020 7769 7265 5f77  200),.    wire_w
+00022460: 6964 7468 3d31 2c0a 2020 2020 7769 7265  idth=1,.    wire
+00022470: 5f67 6170 3d33 2c0a 2020 2020 636f 6d62  _gap=3,.    comb
+00022480: 5f6c 6179 6572 3d30 2c0a 2020 2020 6f76  _layer=0,.    ov
+00022490: 6572 6c61 705f 7a69 677a 6167 5f6c 6179  erlap_zigzag_lay
+000224a0: 6572 3d31 2c0a 2020 2020 636f 6d62 5f70  er=1,.    comb_p
+000224b0: 6164 5f6c 6179 6572 3d32 2c0a 2020 2020  ad_layer=2,.    
+000224c0: 636f 6d62 5f67 6e64 5f6c 6179 6572 3d33  comb_gnd_layer=3
+000224d0: 2c0a 2020 2020 6f76 6572 6c61 705f 7061  ,.    overlap_pa
+000224e0: 645f 6c61 7965 723d 342c 0a29 3a0a 2020  d_layer=4,.):.  
+000224f0: 2020 2222 224f 7665 726c 6170 2063 6f6d    """Overlap com
+00022500: 6220 7465 7374 2073 7472 7563 7475 7265  b test structure
+00022510: 2066 6f72 2063 6865 636b 696e 6720 7768   for checking wh
+00022520: 6574 6865 7220 7477 6f20 6c61 7965 7273  ether two layers
+00022530: 0a20 2020 2061 7265 2065 6c65 6374 7269  .    are electri
+00022540: 6361 6c6c 7920 6973 6f6c 6174 6564 0a0a  cally isolated..
+00022550: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00022560: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00022570: 2020 7061 645f 7369 7a65 203a 2061 7272    pad_size : arr
+00022580: 6179 2d6c 696b 650a 2020 2020 2020 2020  ay-like.        
+00022590: 7820 616e 6420 7920 6469 6d65 6e73 696f  x and y dimensio
+000225a0: 6e73 206f 6620 7468 6520 636f 6d62 2070  ns of the comb p
+000225b0: 6164 732e 0a20 2020 2077 6972 655f 7769  ads..    wire_wi
+000225c0: 6474 6820 3a20 696e 7420 6f72 2066 6c6f  dth : int or flo
+000225d0: 6174 0a20 2020 2020 2020 2057 6964 7468  at.        Width
+000225e0: 206f 6620 7468 6520 7465 7374 2063 6f6d   of the test com
+000225f0: 6220 7465 6574 682e 0a20 2020 2077 6972  b teeth..    wir
+00022600: 655f 6761 7020 3a20 696e 7420 6f72 2066  e_gap : int or f
+00022610: 6c6f 6174 0a20 2020 2020 2020 2053 697a  loat.        Siz
+00022620: 6520 6f66 2074 6865 2067 6170 2062 6574  e of the gap bet
+00022630: 7765 656e 2063 6f6d 6220 7465 6574 682e  ween comb teeth.
+00022640: 0a20 2020 2063 6f6d 625f 6c61 7965 7220  .    comb_layer 
+00022650: 3a20 696e 742c 2061 7272 6179 2d6c 696b  : int, array-lik
+00022660: 655b 325d 2c20 6f72 2073 6574 0a20 2020  e[2], or set.   
+00022670: 2020 2020 2053 7065 6369 6669 6320 6c61       Specific la
+00022680: 7965 7228 7329 2074 6f20 7075 7420 636f  yer(s) to put co
+00022690: 6d62 2067 656f 6d65 7472 7920 6f6e 2e0a  mb geometry on..
+000226a0: 2020 2020 6f76 6572 6c61 705f 7a69 677a      overlap_zigz
+000226b0: 6167 5f6c 6179 6572 203a 2069 6e74 2c20  ag_layer : int, 
+000226c0: 6172 7261 792d 6c69 6b65 5b32 5d2c 206f  array-like[2], o
+000226d0: 7220 7365 740a 2020 2020 2020 2020 5370  r set.        Sp
+000226e0: 6563 6966 6963 206c 6179 6572 2873 2920  ecific layer(s) 
+000226f0: 746f 2070 7574 206f 7665 726c 6170 207a  to put overlap z
+00022700: 6967 7a61 6720 6765 6f6d 6574 7279 206f  igzag geometry o
+00022710: 6e2e 0a20 2020 2063 6f6d 625f 7061 645f  n..    comb_pad_
+00022720: 6c61 7965 7220 3a20 696e 742c 2061 7272  layer : int, arr
+00022730: 6179 2d6c 696b 655b 325d 2c20 6f72 2073  ay-like[2], or s
+00022740: 6574 0a20 2020 2020 2020 2053 7065 6369  et.        Speci
+00022750: 6669 6320 6c61 7965 7228 7329 2074 6f20  fic layer(s) to 
+00022760: 7075 7420 636f 6d62 2070 6164 7320 6f6e  put comb pads on
+00022770: 2e0a 2020 2020 636f 6d62 5f67 6e64 5f6c  ..    comb_gnd_l
+00022780: 6179 6572 203a 2069 6e74 2c20 6172 7261  ayer : int, arra
+00022790: 792d 6c69 6b65 5b32 5d2c 206f 7220 7365  y-like[2], or se
+000227a0: 740a 2020 2020 2020 2020 5370 6563 6966  t.        Specif
+000227b0: 6963 206c 6179 6572 2873 2920 746f 2070  ic layer(s) to p
+000227c0: 7574 2074 6865 2063 6f6d 6220 6772 6f75  ut the comb grou
+000227d0: 6e64 206f 6e2e 0a20 2020 206f 7665 726c  nd on..    overl
+000227e0: 6170 5f70 6164 5f6c 6179 6572 203a 2069  ap_pad_layer : i
+000227f0: 6e74 2c20 6172 7261 792d 6c69 6b65 5b32  nt, array-like[2
+00022800: 5d2c 206f 7220 7365 740a 2020 2020 2020  ], or set.      
+00022810: 2020 5370 6563 6966 6963 206c 6179 6572    Specific layer
+00022820: 2873 2920 746f 2070 7574 206f 7665 726c  (s) to put overl
+00022830: 6170 2070 6164 7320 6f6e 2e0a 0a20 2020  ap pads on...   
+00022840: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00022850: 2d2d 2d2d 0a20 2020 2043 4920 3a20 4465  ----.    CI : De
+00022860: 7669 6365 0a20 2020 2020 2020 2041 2044  vice.        A D
+00022870: 6576 6963 6520 636f 6e74 6169 6e69 6e67  evice containing
+00022880: 2061 2074 6573 7420 636f 6d62 2067 656f   a test comb geo
+00022890: 6d65 7472 792e 0a0a 2020 2020 4e6f 7465  metry...    Note
+000228a0: 730a 2020 2020 2d2d 2d2d 2d0a 2020 2020  s.    -----.    
+000228b0: 4361 6c6c 2063 6f6d 625f 696e 7375 6c61  Call comb_insula
+000228c0: 7469 6f6e 5f74 6573 745f 7374 7275 6374  tion_test_struct
+000228d0: 7572 6528 2920 7769 7468 2061 6e79 206f  ure() with any o
+000228e0: 6620 7468 6520 7061 7261 6d65 7465 7273  f the parameters
+000228f0: 2073 686f 776e 0a20 2020 2062 656c 6f77   shown.    below
+00022900: 2077 6869 6368 2079 6f75 2764 206c 696b   which you'd lik
+00022910: 6520 746f 2063 6861 6e67 652e 2059 6f75  e to change. You
+00022920: 206f 6e6c 7920 6e65 6564 2074 6f20 7375   only need to su
+00022930: 7070 6c79 2074 6865 2070 6172 616d 6574  pply the paramet
+00022940: 6572 730a 2020 2020 7768 6963 6820 796f  ers.    which yo
+00022950: 7520 696e 7465 6e64 206f 6e20 6368 616e  u intend on chan
+00022960: 6769 6e67 2059 6f75 2063 616e 2061 6c74  ging You can alt
+00022970: 6572 6e61 7469 7665 6c79 2063 616c 6c20  ernatively call 
+00022980: 6974 2077 6974 6820 6e6f 0a20 2020 2070  it with no.    p
+00022990: 6172 616d 6574 6572 7320 616e 6420 6974  arameters and it
+000229a0: 2077 696c 6c20 7461 6b65 2061 6c6c 2074   will take all t
+000229b0: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
+000229c0: 7320 7368 6f77 6e20 6265 6c6f 772e 0a0a  s shown below...
+000229d0: 2020 2020 4578 3a3a 0a20 2020 2020 2020      Ex::.       
+000229e0: 2063 6f6d 625f 696e 7375 6c61 7469 6f6e   comb_insulation
+000229f0: 5f74 6573 745f 7374 7275 6374 7572 6528  _test_structure(
+00022a00: 7061 645f 7369 7a65 3d28 3137 352c 3137  pad_size=(175,17
+00022a10: 3529 2c20 7769 7265 5f77 6964 7468 3d32  5), wire_width=2
+00022a20: 2c20 7769 7265 5f67 6170 3d35 290a 2020  , wire_gap=5).  
+00022a30: 2020 2d20 6f72 202d 3a3a 0a20 2020 2020    - or -::.     
+00022a40: 2020 2063 6f6d 625f 696e 7375 6c61 7469     comb_insulati
+00022a50: 6f6e 5f74 6573 745f 7374 7275 6374 7572  on_test_structur
+00022a60: 6528 290a 2020 2020 2222 220a 2020 2020  e().    """.    
+00022a70: 4349 203d 2044 6576 6963 6528 2274 6573  CI = Device("tes
+00022a80: 745f 636f 6d62 2229 0a0a 2020 2020 2320  t_comb")..    # 
+00022a90: 6966 2063 6f6d 625f 7061 645f 6c61 7965  if comb_pad_laye
+00022aa0: 7220 6973 204e 6f6e 653a 2063 6f6d 625f  r is None: comb_
+00022ab0: 7061 645f 6c61 7965 7220 3d20 636f 6d62  pad_layer = comb
+00022ac0: 5f6c 6179 6572 0a20 2020 2023 2069 6620  _layer.    # if 
+00022ad0: 636f 6d62 5f67 6e64 5f6c 6179 6572 2069  comb_gnd_layer i
+00022ae0: 7320 4e6f 6e65 3a20 636f 6d62 5f67 6e64  s None: comb_gnd
+00022af0: 5f6c 6179 6572 203d 2063 6f6d 625f 6c61  _layer = comb_la
+00022b00: 7965 720a 2020 2020 2320 6966 206f 7665  yer.    # if ove
+00022b10: 726c 6170 5f70 6164 5f6c 6179 6572 2069  rlap_pad_layer i
+00022b20: 7320 4e6f 6e65 3a20 6f76 6572 6c61 705f  s None: overlap_
+00022b30: 7061 645f 6c61 7965 7220 3d20 6f76 6572  pad_layer = over
+00022b40: 6c61 705f 7a69 677a 6167 5f6c 6179 6572  lap_zigzag_layer
+00022b50: 0a20 2020 2077 6972 655f 7370 6163 696e  .    wire_spacin
+00022b60: 6720 3d20 7769 7265 5f77 6964 7468 202b  g = wire_width +
+00022b70: 2077 6972 655f 6761 7020 2a20 320a 0a20   wire_gap * 2.. 
+00022b80: 2020 2023 2070 6164 206f 7665 726c 6179     # pad overlay
+00022b90: 730a 2020 2020 6f76 6572 6c61 795f 7061  s.    overlay_pa
+00022ba0: 6462 203d 2043 492e 6164 645f 7265 6628  db = CI.add_ref(
+00022bb0: 0a20 2020 2020 2020 2072 6563 7461 6e67  .        rectang
+00022bc0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00022bd0: 7369 7a65 3d28 7061 645f 7369 7a65 5b30  size=(pad_size[0
+00022be0: 5d20 2a20 3920 2f20 3130 2c20 7061 645f  ] * 9 / 10, pad_
+00022bf0: 7369 7a65 5b31 5d20 2a20 3920 2f20 3130  size[1] * 9 / 10
+00022c00: 292c 206c 6179 6572 3d6f 7665 726c 6170  ), layer=overlap
+00022c10: 5f70 6164 5f6c 6179 6572 0a20 2020 2020  _pad_layer.     
+00022c20: 2020 2029 0a20 2020 2029 0a20 2020 206f     ).    ).    o
+00022c30: 7665 726c 6179 5f70 6164 6c20 3d20 4349  verlay_padl = CI
+00022c40: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00022c50: 2020 7265 6374 616e 676c 6528 0a20 2020    rectangle(.   
+00022c60: 2020 2020 2020 2020 2073 697a 653d 2870           size=(p
+00022c70: 6164 5f73 697a 655b 305d 202a 2039 202f  ad_size[0] * 9 /
+00022c80: 2031 302c 2070 6164 5f73 697a 655b 315d   10, pad_size[1]
+00022c90: 202a 2039 202f 2031 3029 2c20 6c61 7965   * 9 / 10), laye
+00022ca0: 723d 636f 6d62 5f70 6164 5f6c 6179 6572  r=comb_pad_layer
+00022cb0: 0a20 2020 2020 2020 2029 0a20 2020 2029  .        ).    )
+00022cc0: 0a20 2020 206f 7665 726c 6179 5f70 6164  .    overlay_pad
+00022cd0: 7420 3d20 4349 2e61 6464 5f72 6566 280a  t = CI.add_ref(.
+00022ce0: 2020 2020 2020 2020 7265 6374 616e 676c          rectangl
+00022cf0: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
+00022d00: 697a 653d 2870 6164 5f73 697a 655b 305d  ize=(pad_size[0]
+00022d10: 202a 2039 202f 2031 302c 2070 6164 5f73   * 9 / 10, pad_s
+00022d20: 697a 655b 315d 202a 2039 202f 2031 3029  ize[1] * 9 / 10)
+00022d30: 2c20 6c61 7965 723d 636f 6d62 5f70 6164  , layer=comb_pad
+00022d40: 5f6c 6179 6572 0a20 2020 2020 2020 2029  _layer.        )
+00022d50: 0a20 2020 2029 0a20 2020 206f 7665 726c  .    ).    overl
+00022d60: 6179 5f70 6164 7220 3d20 4349 2e61 6464  ay_padr = CI.add
+00022d70: 5f72 6566 280a 2020 2020 2020 2020 7265  _ref(.        re
+00022d80: 6374 616e 676c 6528 0a20 2020 2020 2020  ctangle(.       
+00022d90: 2020 2020 2073 697a 653d 2870 6164 5f73       size=(pad_s
+00022da0: 697a 655b 305d 202a 2039 202f 2031 302c  ize[0] * 9 / 10,
+00022db0: 2070 6164 5f73 697a 655b 315d 202a 2039   pad_size[1] * 9
+00022dc0: 202f 2031 3029 2c20 6c61 7965 723d 636f   / 10), layer=co
+00022dd0: 6d62 5f67 6e64 5f6c 6179 6572 0a20 2020  mb_gnd_layer.   
+00022de0: 2020 2020 2029 0a20 2020 2029 0a20 2020       ).    ).   
+00022df0: 206f 7665 726c 6179 5f70 6164 6c2e 786d   overlay_padl.xm
+00022e00: 696e 203d 2030 0a20 2020 206f 7665 726c  in = 0.    overl
+00022e10: 6179 5f70 6164 6c2e 796d 696e 203d 2030  ay_padl.ymin = 0
+00022e20: 0a20 2020 206f 7665 726c 6179 5f70 6164  .    overlay_pad
+00022e30: 622e 796d 6178 203d 2030 0a20 2020 206f  b.ymax = 0.    o
+00022e40: 7665 726c 6179 5f70 6164 622e 786d 696e  verlay_padb.xmin
+00022e50: 203d 206f 7665 726c 6179 5f70 6164 6c2e   = overlay_padl.
+00022e60: 786d 6178 202b 2070 6164 5f73 697a 655b  xmax + pad_size[
+00022e70: 315d 202f 2035 0a20 2020 206f 7665 726c  1] / 5.    overl
+00022e80: 6179 5f70 6164 722e 796d 696e 203d 206f  ay_padr.ymin = o
+00022e90: 7665 726c 6179 5f70 6164 6c2e 796d 696e  verlay_padl.ymin
+00022ea0: 0a20 2020 206f 7665 726c 6179 5f70 6164  .    overlay_pad
+00022eb0: 722e 786d 696e 203d 206f 7665 726c 6179  r.xmin = overlay
+00022ec0: 5f70 6164 622e 786d 6178 202b 2070 6164  _padb.xmax + pad
+00022ed0: 5f73 697a 655b 315d 202f 2035 0a20 2020  _size[1] / 5.   
+00022ee0: 206f 7665 726c 6179 5f70 6164 742e 786d   overlay_padt.xm
+00022ef0: 696e 203d 206f 7665 726c 6179 5f70 6164  in = overlay_pad
+00022f00: 6c2e 786d 6178 202b 2070 6164 5f73 697a  l.xmax + pad_siz
+00022f10: 655b 315d 202f 2035 0a20 2020 206f 7665  e[1] / 5.    ove
+00022f20: 726c 6179 5f70 6164 742e 796d 696e 203d  rlay_padt.ymin =
+00022f30: 206f 7665 726c 6179 5f70 6164 6c2e 796d   overlay_padl.ym
+00022f40: 6178 0a0a 2020 2020 2320 7061 6473 0a20  ax..    # pads. 
+00022f50: 2020 2070 6164 6c20 3d20 4349 2e61 6464     padl = CI.add
+00022f60: 5f72 6566 2872 6563 7461 6e67 6c65 2873  _ref(rectangle(s
+00022f70: 697a 653d 7061 645f 7369 7a65 2c20 6c61  ize=pad_size, la
+00022f80: 7965 723d 636f 6d62 5f6c 6179 6572 2929  yer=comb_layer))
+00022f90: 0a20 2020 2070 6164 7420 3d20 4349 2e61  .    padt = CI.a
+00022fa0: 6464 5f72 6566 2872 6563 7461 6e67 6c65  dd_ref(rectangle
+00022fb0: 2873 697a 653d 7061 645f 7369 7a65 2c20  (size=pad_size, 
+00022fc0: 6c61 7965 723d 636f 6d62 5f6c 6179 6572  layer=comb_layer
+00022fd0: 2929 0a20 2020 2070 6164 7220 3d20 4349  )).    padr = CI
+00022fe0: 2e61 6464 5f72 6566 2872 6563 7461 6e67  .add_ref(rectang
+00022ff0: 6c65 2873 697a 653d 7061 645f 7369 7a65  le(size=pad_size
+00023000: 2c20 6c61 7965 723d 636f 6d62 5f6c 6179  , layer=comb_lay
+00023010: 6572 2929 0a20 2020 2070 6164 6220 3d20  er)).    padb = 
+00023020: 4349 2e61 6464 5f72 6566 2872 6563 7461  CI.add_ref(recta
+00023030: 6e67 6c65 2873 697a 653d 7061 645f 7369  ngle(size=pad_si
+00023040: 7a65 2c20 6c61 7965 723d 6f76 6572 6c61  ze, layer=overla
+00023050: 705f 7a69 677a 6167 5f6c 6179 6572 2929  p_zigzag_layer))
+00023060: 0a20 2020 2070 6164 6c5f 6e75 6220 3d20  .    padl_nub = 
+00023070: 4349 2e61 6464 5f72 6566 280a 2020 2020  CI.add_ref(.    
+00023080: 2020 2020 7265 6374 616e 676c 6528 7369      rectangle(si
+00023090: 7a65 3d28 7061 645f 7369 7a65 5b30 5d20  ze=(pad_size[0] 
+000230a0: 2f20 342c 2070 6164 5f73 697a 655b 315d  / 4, pad_size[1]
+000230b0: 202f 2032 292c 206c 6179 6572 3d63 6f6d   / 2), layer=com
+000230c0: 625f 6c61 7965 7229 0a20 2020 2029 0a20  b_layer).    ). 
+000230d0: 2020 2070 6164 725f 6e75 6220 3d20 4349     padr_nub = CI
+000230e0: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+000230f0: 2020 7265 6374 616e 676c 6528 7369 7a65    rectangle(size
+00023100: 3d28 7061 645f 7369 7a65 5b30 5d20 2f20  =(pad_size[0] / 
+00023110: 342c 2070 6164 5f73 697a 655b 315d 202f  4, pad_size[1] /
+00023120: 2032 292c 206c 6179 6572 3d63 6f6d 625f   2), layer=comb_
+00023130: 6c61 7965 7229 0a20 2020 2029 0a20 2020  layer).    ).   
+00023140: 2070 6164 6c2e 786d 696e 203d 206f 7665   padl.xmin = ove
+00023150: 726c 6179 5f70 6164 6c2e 786d 696e 0a20  rlay_padl.xmin. 
+00023160: 2020 2070 6164 6c2e 6365 6e74 6572 203d     padl.center =
+00023170: 205b 7061 646c 2e63 656e 7465 725b 305d   [padl.center[0]
+00023180: 2c20 6f76 6572 6c61 795f 7061 646c 2e63  , overlay_padl.c
+00023190: 656e 7465 725b 315d 5d0a 2020 2020 7061  enter[1]].    pa
+000231a0: 6474 2e79 6d61 7820 3d20 6f76 6572 6c61  dt.ymax = overla
+000231b0: 795f 7061 6474 2e79 6d61 780a 2020 2020  y_padt.ymax.    
+000231c0: 7061 6474 2e63 656e 7465 7220 3d20 5b6f  padt.center = [o
+000231d0: 7665 726c 6179 5f70 6164 742e 6365 6e74  verlay_padt.cent
+000231e0: 6572 5b30 5d2c 2070 6164 742e 6365 6e74  er[0], padt.cent
+000231f0: 6572 5b31 5d5d 0a20 2020 2070 6164 722e  er[1]].    padr.
+00023200: 786d 6178 203d 206f 7665 726c 6179 5f70  xmax = overlay_p
+00023210: 6164 722e 786d 6178 0a20 2020 2070 6164  adr.xmax.    pad
+00023220: 722e 6365 6e74 6572 203d 205b 7061 6472  r.center = [padr
+00023230: 2e63 656e 7465 725b 305d 2c20 6f76 6572  .center[0], over
+00023240: 6c61 795f 7061 6472 2e63 656e 7465 725b  lay_padr.center[
+00023250: 315d 5d0a 2020 2020 7061 6462 2e79 6d69  1]].    padb.ymi
+00023260: 6e20 3d20 6f76 6572 6c61 795f 7061 6462  n = overlay_padb
+00023270: 2e79 6d69 6e0a 2020 2020 7061 6462 2e63  .ymin.    padb.c
+00023280: 656e 7465 7220 3d20 5b6f 7665 726c 6179  enter = [overlay
+00023290: 5f70 6164 622e 6365 6e74 6572 5b30 5d2c  _padb.center[0],
+000232a0: 2070 6164 622e 6365 6e74 6572 5b31 5d5d   padb.center[1]]
+000232b0: 0a20 2020 2070 6164 6c5f 6e75 622e 786d  .    padl_nub.xm
+000232c0: 696e 203d 2070 6164 6c2e 786d 6178 0a20  in = padl.xmax. 
+000232d0: 2020 2070 6164 6c5f 6e75 622e 6365 6e74     padl_nub.cent
+000232e0: 6572 203d 205b 7061 646c 5f6e 7562 2e63  er = [padl_nub.c
+000232f0: 656e 7465 725b 305d 2c20 7061 646c 2e63  enter[0], padl.c
+00023300: 656e 7465 725b 315d 5d0a 2020 2020 7061  enter[1]].    pa
+00023310: 6472 5f6e 7562 2e78 6d61 7820 3d20 7061  dr_nub.xmax = pa
+00023320: 6472 2e78 6d69 6e0a 2020 2020 7061 6472  dr.xmin.    padr
+00023330: 5f6e 7562 2e63 656e 7465 7220 3d20 5b70  _nub.center = [p
+00023340: 6164 725f 6e75 622e 6365 6e74 6572 5b30  adr_nub.center[0
+00023350: 5d2c 2070 6164 722e 6365 6e74 6572 5b31  ], padr.center[1
+00023360: 5d5d 0a0a 2020 2020 2320 636f 6e6e 6563  ]]..    # connec
+00023370: 7465 6420 7a69 670a 2020 2020 6865 6164  ted zig.    head
+00023380: 203d 2043 492e 6164 645f 7265 6628 636f   = CI.add_ref(co
+00023390: 6d70 6173 7328 7369 7a65 3d28 7061 645f  mpass(size=(pad_
+000233a0: 7369 7a65 5b30 5d20 2f20 3132 2c20 7769  size[0] / 12, wi
+000233b0: 7265 5f77 6964 7468 292c 206c 6179 6572  re_width), layer
+000233c0: 3d63 6f6d 625f 6c61 7965 7229 290a 2020  =comb_layer)).  
+000233d0: 2020 6865 6164 2e78 6d69 6e20 3d20 7061    head.xmin = pa
+000233e0: 646c 5f6e 7562 2e78 6d61 780a 2020 2020  dl_nub.xmax.    
+000233f0: 6865 6164 2e79 6d61 7820 3d20 7061 646c  head.ymax = padl
+00023400: 5f6e 7562 2e79 6d61 780a 2020 2020 636f  _nub.ymax.    co
+00023410: 6e6e 6563 746f 7220 3d20 4349 2e61 6464  nnector = CI.add
+00023420: 5f72 6566 2863 6f6d 7061 7373 2873 697a  _ref(compass(siz
+00023430: 653d 2877 6972 655f 7769 6474 682c 2077  e=(wire_width, w
+00023440: 6972 655f 7769 6474 6829 2c20 6c61 7965  ire_width), laye
+00023450: 723d 636f 6d62 5f6c 6179 6572 2929 0a20  r=comb_layer)). 
+00023460: 2020 2063 6f6e 6e65 6374 6f72 2e63 6f6e     connector.con
+00023470: 6e65 6374 2870 6f72 743d 2257 222c 2064  nect(port="W", d
+00023480: 6573 7469 6e61 7469 6f6e 3d68 6561 642e  estination=head.
+00023490: 706f 7274 735b 2245 225d 290a 2020 2020  ports["E"]).    
+000234a0: 6f6c 645f 706f 7274 203d 2063 6f6e 6e65  old_port = conne
+000234b0: 6374 6f72 2e70 6f72 7473 5b22 5322 5d0a  ctor.ports["S"].
+000234c0: 2020 2020 746f 7020 3d20 5472 7565 0a20      top = True. 
+000234d0: 2020 206f 626a 203d 2063 6f6e 6e65 6374     obj = connect
+000234e0: 6f72 0a20 2020 2077 6869 6c65 206f 626a  or.    while obj
+000234f0: 2e78 6d61 7820 2b20 7061 645f 7369 7a65  .xmax + pad_size
+00023500: 5b30 5d20 2f20 3132 203c 2070 6164 725f  [0] / 12 < padr_
+00023510: 6e75 622e 786d 696e 3a0a 2020 2020 2020  nub.xmin:.      
+00023520: 2020 2320 6c6f 6e67 207a 6967 207a 6167    # long zig zag
+00023530: 2072 6563 7461 6e67 6c65 0a20 2020 2020   rectangle.     
+00023540: 2020 206f 626a 203d 2043 492e 6164 645f     obj = CI.add_
+00023550: 7265 6628 0a20 2020 2020 2020 2020 2020  ref(.           
+00023560: 2063 6f6d 7061 7373 280a 2020 2020 2020   compass(.      
+00023570: 2020 2020 2020 2020 2020 7369 7a65 3d28            size=(
+00023580: 7061 645f 7369 7a65 5b31 5d20 2f20 3220  pad_size[1] / 2 
+00023590: 2d20 3220 2a20 7769 7265 5f77 6964 7468  - 2 * wire_width
+000235a0: 2c20 7769 7265 5f77 6964 7468 292c 206c  , wire_width), l
+000235b0: 6179 6572 3d63 6f6d 625f 6c61 7965 720a  ayer=comb_layer.
+000235c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000235d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000235e0: 6f62 6a2e 636f 6e6e 6563 7428 706f 7274  obj.connect(port
+000235f0: 3d22 5722 2c20 6465 7374 696e 6174 696f  ="W", destinatio
+00023600: 6e3d 6f6c 645f 706f 7274 290a 2020 2020  n=old_port).    
+00023610: 2020 2020 6f6c 645f 706f 7274 203d 206f      old_port = o
+00023620: 626a 2e70 6f72 7473 5b22 4522 5d0a 2020  bj.ports["E"].  
+00023630: 2020 2020 2020 6966 2074 6f70 3a0a 2020        if top:.  
+00023640: 2020 2020 2020 2020 2020 2320 7a69 6720            # zig 
+00023650: 7a61 6720 6564 6765 2072 6563 7461 6e67  zag edge rectang
+00023660: 6c65 0a20 2020 2020 2020 2020 2020 206f  le.            o
+00023670: 626a 203d 2043 492e 6164 645f 7265 6628  bj = CI.add_ref(
+00023680: 636f 6d70 6173 7328 7369 7a65 3d28 7769  compass(size=(wi
+00023690: 7265 5f77 6964 7468 2c20 7769 7265 5f77  re_width, wire_w
+000236a0: 6964 7468 292c 206c 6179 6572 3d63 6f6d  idth), layer=com
+000236b0: 625f 6c61 7965 7229 290a 2020 2020 2020  b_layer)).      
+000236c0: 2020 2020 2020 6f62 6a2e 636f 6e6e 6563        obj.connec
+000236d0: 7428 706f 7274 3d22 4e22 2c20 6465 7374  t(port="N", dest
+000236e0: 696e 6174 696f 6e3d 6f6c 645f 706f 7274  ination=old_port
+000236f0: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
+00023700: 7020 3d20 4661 6c73 650a 2020 2020 2020  p = False.      
+00023710: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00023720: 2020 2020 2320 7a69 6720 7a61 6720 6564      # zig zag ed
+00023730: 6765 2072 6563 7461 6e67 6c65 0a20 2020  ge rectangle.   
+00023740: 2020 2020 2020 2020 206f 626a 203d 2043           obj = C
+00023750: 492e 6164 645f 7265 6628 636f 6d70 6173  I.add_ref(compas
+00023760: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
+00023770: 7468 2c20 7769 7265 5f77 6964 7468 292c  th, wire_width),
+00023780: 206c 6179 6572 3d63 6f6d 625f 6c61 7965   layer=comb_laye
+00023790: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
+000237a0: 6f62 6a2e 636f 6e6e 6563 7428 706f 7274  obj.connect(port
+000237b0: 3d22 5322 2c20 6465 7374 696e 6174 696f  ="S", destinatio
+000237c0: 6e3d 6f6c 645f 706f 7274 290a 2020 2020  n=old_port).    
+000237d0: 2020 2020 2020 2020 746f 7020 3d20 5472          top = Tr
+000237e0: 7565 0a20 2020 2020 2020 2020 2020 2023  ue.            #
+000237f0: 2063 6f6d 6220 7265 6374 616e 6765 0a20   comb rectange. 
+00023800: 2020 2020 2020 2020 2020 2063 6f6d 6220             comb 
+00023810: 3d20 4349 2e61 6464 5f72 6566 280a 2020  = CI.add_ref(.  
+00023820: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00023830: 6374 616e 676c 6528 0a20 2020 2020 2020  ctangle(.       
+00023840: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00023850: 653d 280a 2020 2020 2020 2020 2020 2020  e=(.            
+00023860: 2020 2020 2020 2020 2020 2020 2870 6164              (pad
+00023870: 742e 796d 696e 202d 2068 6561 642e 796d  t.ymin - head.ym
+00023880: 6178 290a 2020 2020 2020 2020 2020 2020  ax).            
+00023890: 2020 2020 2020 2020 2020 2020 2b20 7061              + pa
+000238a0: 645f 7369 7a65 5b31 5d20 2f20 320a 2020  d_size[1] / 2.  
+000238b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000238c0: 2020 2020 2020 2d20 2877 6972 655f 7370        - (wire_sp
+000238d0: 6163 696e 6720 2b20 7769 7265 5f77 6964  acing + wire_wid
+000238e0: 7468 2920 2f20 322c 0a20 2020 2020 2020  th) / 2,.       
+000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023900: 2077 6972 655f 7769 6474 682c 0a20 2020   wire_width,.   
+00023910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023920: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00023930: 2020 2020 2020 2020 6c61 7965 723d 636f          layer=co
+00023940: 6d62 5f6c 6179 6572 2c0a 2020 2020 2020  mb_layer,.      
+00023950: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00023960: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00023970: 2020 2020 2020 636f 6d62 2e72 6f74 6174        comb.rotat
+00023980: 6528 3930 290a 2020 2020 2020 2020 2020  e(90).          
+00023990: 2020 636f 6d62 2e79 6d61 7820 3d20 7061    comb.ymax = pa
+000239a0: 6474 2e79 6d69 6e0a 2020 2020 2020 2020  dt.ymin.        
+000239b0: 2020 2020 636f 6d62 2e78 6d61 7820 3d20      comb.xmax = 
+000239c0: 6f62 6a2e 786d 6178 202d 2028 7769 7265  obj.xmax - (wire
+000239d0: 5f73 7061 6369 6e67 202b 2077 6972 655f  _spacing + wire_
+000239e0: 7769 6474 6829 202f 2032 0a20 2020 2020  width) / 2.     
+000239f0: 2020 206f 6c64 5f70 6f72 7420 3d20 6f62     old_port = ob
+00023a00: 6a2e 706f 7274 735b 2245 225d 0a20 2020  j.ports["E"].   
+00023a10: 2020 2020 206f 626a 203d 2043 492e 6164       obj = CI.ad
+00023a20: 645f 7265 6628 636f 6d70 6173 7328 7369  d_ref(compass(si
+00023a30: 7a65 3d28 7769 7265 5f73 7061 6369 6e67  ze=(wire_spacing
+00023a40: 2c20 7769 7265 5f77 6964 7468 292c 206c  , wire_width), l
+00023a50: 6179 6572 3d63 6f6d 625f 6c61 7965 7229  ayer=comb_layer)
+00023a60: 290a 2020 2020 2020 2020 6f62 6a2e 636f  ).        obj.co
+00023a70: 6e6e 6563 7428 706f 7274 3d22 5722 2c20  nnect(port="W", 
+00023a80: 6465 7374 696e 6174 696f 6e3d 6f6c 645f  destination=old_
+00023a90: 706f 7274 290a 2020 2020 2020 2020 6f6c  port).        ol
+00023aa0: 645f 706f 7274 203d 206f 626a 2e70 6f72  d_port = obj.por
+00023ab0: 7473 5b22 4522 5d0a 2020 2020 2020 2020  ts["E"].        
+00023ac0: 6f62 6a20 3d20 4349 2e61 6464 5f72 6566  obj = CI.add_ref
+00023ad0: 2863 6f6d 7061 7373 2873 697a 653d 2877  (compass(size=(w
+00023ae0: 6972 655f 7769 6474 682c 2077 6972 655f  ire_width, wire_
+00023af0: 7769 6474 6829 2c20 6c61 7965 723d 636f  width), layer=co
+00023b00: 6d62 5f6c 6179 6572 2929 0a20 2020 2020  mb_layer)).     
+00023b10: 2020 206f 626a 2e63 6f6e 6e65 6374 2870     obj.connect(p
+00023b20: 6f72 743d 2257 222c 2064 6573 7469 6e61  ort="W", destina
+00023b30: 7469 6f6e 3d6f 6c64 5f70 6f72 7429 0a20  tion=old_port). 
+00023b40: 2020 2020 2020 2069 6620 746f 703a 0a20         if top:. 
+00023b50: 2020 2020 2020 2020 2020 206f 6c64 5f70             old_p
+00023b60: 6f72 7420 3d20 6f62 6a2e 706f 7274 735b  ort = obj.ports[
+00023b70: 2253 225d 0a20 2020 2020 2020 2065 6c73  "S"].        els
+00023b80: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+00023b90: 6c64 5f70 6f72 7420 3d20 6f62 6a2e 706f  ld_port = obj.po
+00023ba0: 7274 735b 224e 225d 0a20 2020 206f 6c64  rts["N"].    old
+00023bb0: 5f70 6f72 7420 3d20 6f62 6a2e 706f 7274  _port = obj.port
+00023bc0: 735b 2245 225d 0a20 2020 2069 6620 7061  s["E"].    if pa
+00023bd0: 6472 5f6e 7562 2e78 6d69 6e20 2d20 6f62  dr_nub.xmin - ob
+00023be0: 6a2e 786d 6178 203e 2030 3a0a 2020 2020  j.xmax > 0:.    
+00023bf0: 2020 2020 7461 696c 203d 2043 492e 6164      tail = CI.ad
+00023c00: 645f 7265 6628 0a20 2020 2020 2020 2020  d_ref(.         
+00023c10: 2020 2063 6f6d 7061 7373 2873 697a 653d     compass(size=
+00023c20: 2870 6164 725f 6e75 622e 786d 696e 202d  (padr_nub.xmin -
+00023c30: 206f 626a 2e78 6d61 782c 2077 6972 655f   obj.xmax, wire_
+00023c40: 7769 6474 6829 2c20 6c61 7965 723d 636f  width), layer=co
+00023c50: 6d62 5f6c 6179 6572 290a 2020 2020 2020  mb_layer).      
+00023c60: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+00023c70: 2020 2020 2020 7461 696c 203d 2043 492e        tail = CI.
+00023c80: 6164 645f 7265 6628 636f 6d70 6173 7328  add_ref(compass(
+00023c90: 7369 7a65 3d28 7769 7265 5f77 6964 7468  size=(wire_width
+00023ca0: 2c20 7769 7265 5f77 6964 7468 292c 206c  , wire_width), l
+00023cb0: 6179 6572 3d63 6f6d 625f 6c61 7965 7229  ayer=comb_layer)
+00023cc0: 290a 2020 2020 7461 696c 2e63 6f6e 6e65  ).    tail.conne
+00023cd0: 6374 2870 6f72 743d 2257 222c 2064 6573  ct(port="W", des
+00023ce0: 7469 6e61 7469 6f6e 3d6f 6c64 5f70 6f72  tination=old_por
+00023cf0: 7429 0a0a 2020 2020 2320 6469 7363 6f6e  t)..    # discon
+00023d00: 6e65 6374 6564 207a 6967 0a20 2020 2064  nected zig.    d
+00023d10: 6865 6164 203d 2043 492e 6164 645f 7265  head = CI.add_re
+00023d20: 6628 0a20 2020 2020 2020 2063 6f6d 7061  f(.        compa
+00023d30: 7373 280a 2020 2020 2020 2020 2020 2020  ss(.            
+00023d40: 7369 7a65 3d28 7061 6472 5f6e 7562 2e79  size=(padr_nub.y
+00023d50: 6d69 6e20 2d20 7061 6462 2e79 6d61 7820  min - padb.ymax 
+00023d60: 2d20 7769 7265 5f77 6964 7468 2c20 7769  - wire_width, wi
+00023d70: 7265 5f77 6964 7468 292c 0a20 2020 2020  re_width),.     
+00023d80: 2020 2020 2020 206c 6179 6572 3d6f 7665         layer=ove
+00023d90: 726c 6170 5f7a 6967 7a61 675f 6c61 7965  rlap_zigzag_laye
+00023da0: 722c 0a20 2020 2020 2020 2029 0a20 2020  r,.        ).   
+00023db0: 2029 0a20 2020 2064 6865 6164 2e72 6f74   ).    dhead.rot
+00023dc0: 6174 6528 3930 290a 2020 2020 6468 6561  ate(90).    dhea
+00023dd0: 642e 796d 696e 203d 2070 6164 622e 796d  d.ymin = padb.ym
+00023de0: 6178 0a20 2020 2064 6865 6164 2e78 6d61  ax.    dhead.xma
+00023df0: 7820 3d20 7461 696c 2e78 6d69 6e20 2d20  x = tail.xmin - 
+00023e00: 2877 6972 655f 7370 6163 696e 6720 2b20  (wire_spacing + 
+00023e10: 7769 7265 5f77 6964 7468 2920 2f20 320a  wire_width) / 2.
+00023e20: 2020 2020 636f 6e6e 6563 746f 7220 3d20      connector = 
+00023e30: 4349 2e61 6464 5f72 6566 280a 2020 2020  CI.add_ref(.    
+00023e40: 2020 2020 636f 6d70 6173 7328 7369 7a65      compass(size
+00023e50: 3d28 7769 7265 5f77 6964 7468 2c20 7769  =(wire_width, wi
+00023e60: 7265 5f77 6964 7468 292c 206c 6179 6572  re_width), layer
+00023e70: 3d6f 7665 726c 6170 5f7a 6967 7a61 675f  =overlap_zigzag_
+00023e80: 6c61 7965 7229 0a20 2020 2029 0a20 2020  layer).    ).   
+00023e90: 2063 6f6e 6e65 6374 6f72 2e63 6f6e 6e65   connector.conne
+00023ea0: 6374 2870 6f72 743d 2253 222c 2064 6573  ct(port="S", des
+00023eb0: 7469 6e61 7469 6f6e 3d64 6865 6164 2e70  tination=dhead.p
+00023ec0: 6f72 7473 5b22 4522 5d29 0a20 2020 206f  orts["E"]).    o
+00023ed0: 6c64 5f70 6f72 7420 3d20 636f 6e6e 6563  ld_port = connec
+00023ee0: 746f 722e 706f 7274 735b 224e 225d 0a20  tor.ports["N"]. 
+00023ef0: 2020 2072 6967 6874 203d 2054 7275 650a     right = True.
+00023f00: 2020 2020 6f62 6a20 3d20 636f 6e6e 6563      obj = connec
+00023f10: 746f 720a 2020 2020 7768 696c 6520 6f62  tor.    while ob
+00023f20: 6a2e 796d 6178 202b 2077 6972 655f 7370  j.ymax + wire_sp
+00023f30: 6163 696e 6720 2b20 7769 7265 5f77 6964  acing + wire_wid
+00023f40: 7468 203c 2068 6561 642e 796d 6178 3a0a  th < head.ymax:.
+00023f50: 2020 2020 2020 2020 6f62 6a20 3d20 4349          obj = CI
+00023f60: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00023f70: 2020 2020 2020 636f 6d70 6173 7328 7369        compass(si
+00023f80: 7a65 3d28 7769 7265 5f73 7061 6369 6e67  ze=(wire_spacing
+00023f90: 2c20 7769 7265 5f77 6964 7468 292c 206c  , wire_width), l
+00023fa0: 6179 6572 3d6f 7665 726c 6170 5f7a 6967  ayer=overlap_zig
+00023fb0: 7a61 675f 6c61 7965 7229 0a20 2020 2020  zag_layer).     
+00023fc0: 2020 2029 0a20 2020 2020 2020 206f 626a     ).        obj
+00023fd0: 2e63 6f6e 6e65 6374 2870 6f72 743d 2257  .connect(port="W
+00023fe0: 222c 2064 6573 7469 6e61 7469 6f6e 3d6f  ", destination=o
+00023ff0: 6c64 5f70 6f72 7429 0a20 2020 2020 2020  ld_port).       
+00024000: 206f 6c64 5f70 6f72 7420 3d20 6f62 6a2e   old_port = obj.
+00024010: 706f 7274 735b 2245 225d 0a20 2020 2020  ports["E"].     
+00024020: 2020 2069 6620 7269 6768 743a 0a20 2020     if right:.   
+00024030: 2020 2020 2020 2020 206f 626a 203d 2043           obj = C
+00024040: 492e 6164 645f 7265 6628 0a20 2020 2020  I.add_ref(.     
+00024050: 2020 2020 2020 2020 2020 2063 6f6d 7061             compa
+00024060: 7373 2873 697a 653d 2877 6972 655f 7769  ss(size=(wire_wi
+00024070: 6474 682c 2077 6972 655f 7769 6474 6829  dth, wire_width)
+00024080: 2c20 6c61 7965 723d 6f76 6572 6c61 705f  , layer=overlap_
+00024090: 7a69 677a 6167 5f6c 6179 6572 290a 2020  zigzag_layer).  
+000240a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000240b0: 2020 2020 2020 2020 6f62 6a2e 636f 6e6e          obj.conn
+000240c0: 6563 7428 706f 7274 3d22 5722 2c20 6465  ect(port="W", de
+000240d0: 7374 696e 6174 696f 6e3d 6f6c 645f 706f  stination=old_po
+000240e0: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
+000240f0: 7269 6768 7420 3d20 4661 6c73 650a 2020  right = False.  
+00024100: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00024110: 2020 2020 2020 2020 6f62 6a20 3d20 4349          obj = CI
+00024120: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00024130: 2020 2020 2020 2020 2020 636f 6d70 6173            compas
+00024140: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
+00024150: 7468 2c20 7769 7265 5f77 6964 7468 292c  th, wire_width),
+00024160: 206c 6179 6572 3d6f 7665 726c 6170 5f7a   layer=overlap_z
+00024170: 6967 7a61 675f 6c61 7965 7229 0a20 2020  igzag_layer).   
+00024180: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00024190: 2020 2020 2020 206f 626a 2e63 6f6e 6e65         obj.conne
+000241a0: 6374 2870 6f72 743d 2245 222c 2064 6573  ct(port="E", des
+000241b0: 7469 6e61 7469 6f6e 3d6f 6c64 5f70 6f72  tination=old_por
+000241c0: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
+000241d0: 6967 6874 203d 2054 7275 650a 2020 2020  ight = True.    
+000241e0: 2020 2020 6f6c 645f 706f 7274 203d 206f      old_port = o
+000241f0: 626a 2e70 6f72 7473 5b22 4e22 5d0a 2020  bj.ports["N"].  
+00024200: 2020 2020 2020 6f62 6a20 3d20 4349 2e61        obj = CI.a
+00024210: 6464 5f72 6566 280a 2020 2020 2020 2020  dd_ref(.        
+00024220: 2020 2020 636f 6d70 6173 7328 0a20 2020      compass(.   
+00024230: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00024240: 653d 280a 2020 2020 2020 2020 2020 2020  e=(.            
+00024250: 2020 2020 2020 2020 6468 6561 642e 786d          dhead.xm
+00024260: 696e 202d 2028 6865 6164 2e78 6d61 7820  in - (head.xmax 
+00024270: 2b20 6865 6164 2e78 6d69 6e20 2b20 7769  + head.xmin + wi
+00024280: 7265 5f77 6964 7468 2920 2f20 322c 0a20  re_width) / 2,. 
+00024290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000242a0: 2020 2077 6972 655f 7769 6474 682c 0a20     wire_width,. 
+000242b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000242c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000242d0: 2020 6c61 7965 723d 6f76 6572 6c61 705f    layer=overlap_
+000242e0: 7a69 677a 6167 5f6c 6179 6572 2c0a 2020  zigzag_layer,.  
+000242f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00024300: 2020 2020 290a 2020 2020 2020 2020 6f62      ).        ob
+00024310: 6a2e 636f 6e6e 6563 7428 706f 7274 3d22  j.connect(port="
+00024320: 4522 2c20 6465 7374 696e 6174 696f 6e3d  E", destination=
+00024330: 6f6c 645f 706f 7274 290a 2020 2020 2020  old_port).      
+00024340: 2020 6f6c 645f 706f 7274 203d 206f 626a    old_port = obj
+00024350: 2e70 6f72 7473 5b22 5722 5d0a 2020 2020  .ports["W"].    
+00024360: 2020 2020 6f62 6a20 3d20 4349 2e61 6464      obj = CI.add
+00024370: 5f72 6566 280a 2020 2020 2020 2020 2020  _ref(.          
+00024380: 2020 636f 6d70 6173 7328 7369 7a65 3d28    compass(size=(
+00024390: 7769 7265 5f77 6964 7468 2c20 7769 7265  wire_width, wire
+000243a0: 5f77 6964 7468 292c 206c 6179 6572 3d6f  _width), layer=o
+000243b0: 7665 726c 6170 5f7a 6967 7a61 675f 6c61  verlap_zigzag_la
+000243c0: 7965 7229 0a20 2020 2020 2020 2029 0a20  yer).        ). 
+000243d0: 2020 2020 2020 206f 626a 2e63 6f6e 6e65         obj.conne
+000243e0: 6374 2870 6f72 743d 2253 222c 2064 6573  ct(port="S", des
+000243f0: 7469 6e61 7469 6f6e 3d6f 6c64 5f70 6f72  tination=old_por
+00024400: 7429 0a20 2020 2020 2020 2069 6620 7269  t).        if ri
+00024410: 6768 743a 0a20 2020 2020 2020 2020 2020  ght:.           
+00024420: 206f 6c64 5f70 6f72 7420 3d20 6f62 6a2e   old_port = obj.
+00024430: 706f 7274 735b 2257 225d 0a20 2020 2020  ports["W"].     
+00024440: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00024450: 2020 2020 206f 6c64 5f70 6f72 7420 3d20       old_port = 
+00024460: 6f62 6a2e 706f 7274 735b 2245 225d 0a0a  obj.ports["E"]..
+00024470: 2020 2020 7265 7475 726e 2043 490a 0a0a      return CI...
+00024480: 6465 6620 5f74 6573 745f 6963 5f77 6972  def _test_ic_wir
+00024490: 655f 7374 6570 2874 6869 636b 5f77 6964  e_step(thick_wid
+000244a0: 7468 3d31 302c 2074 6869 6e5f 7769 6474  th=10, thin_widt
+000244b0: 683d 312c 2077 6972 655f 6c61 7965 723d  h=1, wire_layer=
+000244c0: 3229 3a0a 2020 2020 2222 2248 656c 7065  2):.    """Helpe
+000244d0: 7220 6675 6e63 7469 6f6e 2075 7365 6420  r function used 
+000244e0: 746f 206d 616b 6520 7468 6520 4943 2073  to make the IC s
+000244f0: 7465 7020 7769 7265 2073 7472 7563 7475  tep wire structu
+00024500: 7265 2e22 2222 0a20 2020 2057 5334 203d  re.""".    WS4 =
+00024510: 2044 6576 6963 6528 2274 6573 745f 6963   Device("test_ic
+00024520: 5f73 7465 7022 290a 2020 2020 7769 7265  _step").    wire
+00024530: 5f73 7465 7061 203d 2057 5334 2e61 6464  _stepa = WS4.add
+00024540: 5f72 6566 280a 2020 2020 2020 2020 6f70  _ref(.        op
+00024550: 7469 6d61 6c5f 7374 6570 2874 6869 636b  timal_step(thick
+00024560: 5f77 6964 7468 202f 2032 2c20 7468 696e  _width / 2, thin
+00024570: 5f77 6964 7468 202f 2032 2c20 6c61 7965  _width / 2, laye
+00024580: 723d 7769 7265 5f6c 6179 6572 290a 2020  r=wire_layer).  
+00024590: 2020 290a 2020 2020 7769 7265 5f73 7465    ).    wire_ste
+000245a0: 7062 203d 2057 5334 2e61 6464 5f72 6566  pb = WS4.add_ref
+000245b0: 280a 2020 2020 2020 2020 6f70 7469 6d61  (.        optima
+000245c0: 6c5f 7374 6570 2874 6869 6e5f 7769 6474  l_step(thin_widt
+000245d0: 6820 2f20 322c 2074 6869 636b 5f77 6964  h / 2, thick_wid
+000245e0: 7468 202f 2032 2c20 6c61 7965 723d 7769  th / 2, layer=wi
+000245f0: 7265 5f6c 6179 6572 290a 2020 2020 290a  re_layer).    ).
+00024600: 2020 2020 7769 7265 5f73 7465 7063 203d      wire_stepc =
+00024610: 2057 5334 2e61 6464 5f72 6566 280a 2020   WS4.add_ref(.  
+00024620: 2020 2020 2020 6f70 7469 6d61 6c5f 7374        optimal_st
+00024630: 6570 2874 6869 636b 5f77 6964 7468 202f  ep(thick_width /
+00024640: 2032 2c20 7468 696e 5f77 6964 7468 202f   2, thin_width /
+00024650: 2032 2c20 6c61 7965 723d 7769 7265 5f6c   2, layer=wire_l
+00024660: 6179 6572 290a 2020 2020 290a 2020 2020  ayer).    ).    
+00024670: 7769 7265 5f73 7465 7064 203d 2057 5334  wire_stepd = WS4
+00024680: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00024690: 2020 6f70 7469 6d61 6c5f 7374 6570 2874    optimal_step(t
+000246a0: 6869 6e5f 7769 6474 6820 2f20 322c 2074  hin_width / 2, t
+000246b0: 6869 636b 5f77 6964 7468 202f 2032 2c20  hick_width / 2, 
+000246c0: 6c61 7965 723d 7769 7265 5f6c 6179 6572  layer=wire_layer
+000246d0: 290a 2020 2020 290a 2020 2020 7769 7265  ).    ).    wire
+000246e0: 5f73 7465 7062 2e72 6f74 6174 6528 3138  _stepb.rotate(18
+000246f0: 3029 0a20 2020 2077 6972 655f 7374 6570  0).    wire_step
+00024700: 622e 786d 696e 203d 2077 6972 655f 7374  b.xmin = wire_st
+00024710: 6570 612e 786d 696e 0a20 2020 2077 6972  epa.xmin.    wir
+00024720: 655f 7374 6570 632e 726f 7461 7465 2831  e_stepc.rotate(1
+00024730: 3830 290a 2020 2020 7769 7265 5f73 7465  80).    wire_ste
+00024740: 7063 2e78 6d69 6e20 3d20 7769 7265 5f73  pc.xmin = wire_s
+00024750: 7465 7061 2e78 6d61 780a 2020 2020 7769  tepa.xmax.    wi
+00024760: 7265 5f73 7465 7064 2e78 6d69 6e20 3d20  re_stepd.xmin = 
+00024770: 7769 7265 5f73 7465 7063 2e78 6d69 6e0a  wire_stepc.xmin.
+00024780: 2020 2020 7265 7475 726e 2057 5334 0a0a      return WS4..
+00024790: 0a64 6566 2074 6573 745f 6963 280a 2020  .def test_ic(.  
+000247a0: 2020 7769 7265 5f77 6964 7468 733d 5b30    wire_widths=[0
+000247b0: 2e32 352c 2030 2e35 2c20 312c 2032 2c20  .25, 0.5, 1, 2, 
+000247c0: 345d 2c0a 2020 2020 7769 7265 5f77 6964  4],.    wire_wid
+000247d0: 7468 735f 7769 6465 3d5b 302e 3735 2c20  ths_wide=[0.75, 
+000247e0: 312e 352c 2033 2c20 342c 2036 5d2c 0a20  1.5, 3, 4, 6],. 
+000247f0: 2020 2070 6164 5f73 697a 653d 2832 3030     pad_size=(200
+00024800: 2c20 3230 3029 2c0a 2020 2020 7061 645f  , 200),.    pad_
+00024810: 6761 703d 3735 2c0a 2020 2020 7769 7265  gap=75,.    wire
+00024820: 5f6c 6179 6572 3d30 2c0a 2020 2020 7061  _layer=0,.    pa
+00024830: 645f 6c61 7965 723d 312c 0a20 2020 2067  d_layer=1,.    g
+00024840: 6e64 5f6c 6179 6572 3d31 2c0a 293a 0a20  nd_layer=1,.):. 
+00024850: 2020 2022 2222 4372 6974 6963 616c 2063     """Critical c
+00024860: 7572 7265 6e74 2074 6573 7420 7374 7275  urrent test stru
+00024870: 6374 7572 6520 666f 7220 7375 7065 7263  cture for superc
+00024880: 6f6e 6475 6374 696e 6720 7769 7265 732e  onducting wires.
+00024890: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+000248a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000248b0: 2020 2020 7769 7265 5f77 6964 7468 7320      wire_widths 
+000248c0: 3a20 6172 7261 792d 6c69 6b65 5b4e 5d0a  : array-like[N].
+000248d0: 2020 2020 2020 2020 5468 6520 7769 6474          The widt
+000248e0: 6873 206f 6620 7468 6520 7468 696e 6e65  hs of the thinne
+000248f0: 7374 2070 6172 7473 206f 6620 7468 6520  st parts of the 
+00024900: 7465 7374 2077 6972 6573 2e0a 2020 2020  test wires..    
+00024910: 7769 7265 5f77 6964 7468 735f 7769 6465  wire_widths_wide
+00024920: 203a 2061 7272 6179 2d6c 696b 655b 4e5d   : array-like[N]
+00024930: 0a20 2020 2020 2020 2054 6865 2077 6964  .        The wid
+00024940: 7468 7320 6f66 2074 6865 2074 6869 636b  ths of the thick
+00024950: 6573 7420 7061 7274 7320 6f66 2074 6865  est parts of the
+00024960: 2074 6573 7420 7769 7265 732e 0a20 2020   test wires..   
+00024970: 2070 6164 5f73 697a 6520 3a20 6172 7261   pad_size : arra
+00024980: 792d 6c69 6b65 5b32 5d20 6f66 2069 6e74  y-like[2] of int
+00024990: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
+000249a0: 2020 2877 6964 7468 2c20 6865 6967 6874    (width, height
+000249b0: 2920 6f66 2074 6865 2070 6164 732e 0a20  ) of the pads.. 
+000249c0: 2020 2070 6164 5f67 6170 203a 2069 6e74     pad_gap : int
+000249d0: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
+000249e0: 2020 4469 7374 616e 6365 2062 6574 7765    Distance betwe
+000249f0: 656e 2074 6865 2070 6164 7320 616e 6420  en the pads and 
+00024a00: 7468 6520 6772 6f75 6e64 2070 6c61 6e65  the ground plane
+00024a10: 2e0a 2020 2020 7769 7265 5f6c 6179 6572  ..    wire_layer
+00024a20: 203a 2069 6e74 0a20 2020 2020 2020 2053   : int.        S
+00024a30: 7065 6369 6669 6320 6c61 7965 7228 7329  pecific layer(s)
+00024a40: 2074 6f20 7075 7420 7468 6520 7769 7265   to put the wire
+00024a50: 7320 6f6e 2e0a 2020 2020 7061 645f 6c61  s on..    pad_la
+00024a60: 7965 7220 3a20 696e 740a 2020 2020 2020  yer : int.      
+00024a70: 2020 5370 6563 6966 6963 206c 6179 6572    Specific layer
+00024a80: 2873 2920 746f 2070 7574 2074 6865 2070  (s) to put the p
+00024a90: 6164 7320 6f6e 2e0a 2020 2020 676e 645f  ads on..    gnd_
+00024aa0: 6c61 7965 7220 3a20 696e 7420 6f72 204e  layer : int or N
+00024ab0: 6f6e 650a 2020 2020 2020 2020 5370 6563  one.        Spec
+00024ac0: 6966 6963 206c 6179 6572 2873 2920 746f  ific layer(s) to
+00024ad0: 2070 7574 2074 6865 2067 726f 756e 6420   put the ground 
+00024ae0: 706c 616e 6520 6f6e 2e0a 0a20 2020 2052  plane on...    R
+00024af0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00024b00: 2d2d 0a20 2020 2044 6576 6963 650a 2020  --.    Device.  
+00024b10: 2020 2020 2020 4120 4465 7669 6365 2063        A Device c
+00024b20: 6f6e 7461 696e 696e 6720 7468 6520 6372  ontaining the cr
+00024b30: 6974 6963 616c 2d63 7572 7265 6e74 2074  itical-current t
+00024b40: 6573 7420 7374 7275 6374 7572 652e 0a20  est structure.. 
+00024b50: 2020 2022 2222 0a20 2020 2049 4353 203d     """.    ICS =
+00024b60: 2044 6576 6963 6528 2274 6573 745f 6963   Device("test_ic
+00024b70: 2229 0a0a 2020 2020 2320 6966 2067 6e64  ")..    # if gnd
+00024b80: 5f6c 6179 6572 2069 7320 4e6f 6e65 3a20  _layer is None: 
+00024b90: 676e 645f 6c61 7965 7220 3d20 7061 645f  gnd_layer = pad_
+00024ba0: 6c61 7965 720a 2020 2020 7472 616e 736c  layer.    transl
+00024bb0: 6174 696f 6e20 3d20 300a 2020 2020 7061  ation = 0.    pa
+00024bc0: 6462 203d 2049 4353 2e61 6464 5f72 6566  db = ICS.add_ref
+00024bd0: 280a 2020 2020 2020 2020 7265 6374 616e  (.        rectan
+00024be0: 676c 6528 0a20 2020 2020 2020 2020 2020  gle(.           
+00024bf0: 2073 697a 653d 286e 702e 7369 7a65 2877   size=(np.size(w
+00024c00: 6972 655f 7769 6474 6873 2920 2a20 2870  ire_widths) * (p
+00024c10: 6164 5f73 697a 655b 305d 202a 2036 202f  ad_size[0] * 6 /
+00024c20: 2035 292c 2070 6164 5f73 697a 655b 315d   5), pad_size[1]
+00024c30: 292c 0a20 2020 2020 2020 2020 2020 206c  ),.            l
+00024c40: 6179 6572 3d77 6972 655f 6c61 7965 722c  ayer=wire_layer,
+00024c50: 0a20 2020 2020 2020 2029 0a20 2020 2029  .        ).    )
+00024c60: 0a0a 2020 2020 7061 6462 5f6f 7665 726c  ..    padb_overl
+00024c70: 6179 203d 2049 4353 2e61 6464 5f72 6566  ay = ICS.add_ref
+00024c80: 280a 2020 2020 2020 2020 7265 6374 616e  (.        rectan
+00024c90: 676c 6528 0a20 2020 2020 2020 2020 2020  gle(.           
+00024ca0: 2073 697a 653d 280a 2020 2020 2020 2020   size=(.        
+00024cb0: 2020 2020 2020 2020 286e 702e 7369 7a65          (np.size
+00024cc0: 2877 6972 655f 7769 6474 6873 2920 2a20  (wire_widths) * 
+00024cd0: 2870 6164 5f73 697a 655b 305d 202a 2036  (pad_size[0] * 6
+00024ce0: 202f 2035 2929 202a 2039 202f 2031 302c   / 5)) * 9 / 10,
+00024cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024d00: 2070 6164 5f73 697a 655b 315d 202a 2039   pad_size[1] * 9
+00024d10: 202f 2031 302c 0a20 2020 2020 2020 2020   / 10,.         
+00024d20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00024d30: 2020 6c61 7965 723d 676e 645f 6c61 7965    layer=gnd_laye
+00024d40: 722c 0a20 2020 2020 2020 2029 0a20 2020  r,.        ).   
+00024d50: 2029 0a20 2020 2070 6164 625f 6f76 6572   ).    padb_over
+00024d60: 6c61 792e 6365 6e74 6572 203d 2070 6164  lay.center = pad
+00024d70: 622e 6365 6e74 6572 0a20 2020 2070 6164  b.center.    pad
+00024d80: 625f 6f76 6572 6c61 792e 796d 696e 203d  b_overlay.ymin =
+00024d90: 2070 6164 622e 796d 696e 0a20 2020 2066   padb.ymin.    f
+00024da0: 6f72 2069 2c20 7820 696e 2065 6e75 6d65  or i, x in enume
+00024db0: 7261 7465 2877 6972 655f 7769 6474 6873  rate(wire_widths
+00024dc0: 5f77 6964 6529 3a0a 2020 2020 2020 2020  _wide):.        
+00024dd0: 7061 6474 203d 2049 4353 2e61 6464 5f72  padt = ICS.add_r
+00024de0: 6566 2872 6563 7461 6e67 6c65 2870 6164  ef(rectangle(pad
+00024df0: 5f73 697a 652c 2077 6972 655f 6c61 7965  _size, wire_laye
+00024e00: 7229 290a 2020 2020 2020 2020 7061 6474  r)).        padt
+00024e10: 2e78 6d69 6e20 3d20 7061 6462 2e78 6d69  .xmin = padb.xmi
+00024e20: 6e20 2b20 7472 616e 736c 6174 696f 6e0a  n + translation.
+00024e30: 2020 2020 2020 2020 7061 6474 2e79 6d69          padt.ymi
+00024e40: 6e20 3d20 7061 6462 2e79 6d61 7820 2b20  n = padb.ymax + 
+00024e50: 7061 645f 6761 700a 2020 2020 2020 2020  pad_gap.        
+00024e60: 7061 6474 5f6f 7665 726c 6179 203d 2049  padt_overlay = I
+00024e70: 4353 2e61 6464 5f72 6566 280a 2020 2020  CS.add_ref(.    
+00024e80: 2020 2020 2020 2020 7265 6374 616e 676c          rectangl
+00024e90: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00024ea0: 2020 2073 697a 653d 2870 6164 5f73 697a     size=(pad_siz
+00024eb0: 655b 305d 202a 2039 202f 2031 302c 2070  e[0] * 9 / 10, p
+00024ec0: 6164 5f73 697a 655b 315d 202a 2039 202f  ad_size[1] * 9 /
+00024ed0: 2031 3029 2c20 6c61 7965 723d 7061 645f   10), layer=pad_
+00024ee0: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
+00024ef0: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
+00024f00: 2020 2020 2020 7061 6474 5f6f 7665 726c        padt_overl
+00024f10: 6179 2e63 656e 7465 7220 3d20 7061 6474  ay.center = padt
+00024f20: 2e63 656e 7465 720a 2020 2020 2020 2020  .center.        
+00024f30: 7061 6474 5f6f 7665 726c 6179 2e79 6d61  padt_overlay.yma
+00024f40: 7820 3d20 7061 6474 2e79 6d61 780a 2020  x = padt.ymax.  
+00024f50: 2020 2020 2020 6469 6666 6572 656e 6365        difference
+00024f60: 203d 2070 6164 742e 796d 696e 202d 2070   = padt.ymin - p
+00024f70: 6164 622e 796d 6178 0a20 2020 2020 2020  adb.ymax.       
+00024f80: 2077 6972 655f 7374 6570 203d 2049 4353   wire_step = ICS
+00024f90: 2e61 6464 5f72 6566 280a 2020 2020 2020  .add_ref(.      
+00024fa0: 2020 2020 2020 5f74 6573 745f 6963 5f77        _test_ic_w
+00024fb0: 6972 655f 7374 6570 280a 2020 2020 2020  ire_step(.      
+00024fc0: 2020 2020 2020 2020 2020 7769 7265 5f77            wire_w
+00024fd0: 6964 7468 735f 7769 6465 5b69 5d2c 2077  idths_wide[i], w
+00024fe0: 6972 655f 7769 6474 6873 5b69 5d2c 2077  ire_widths[i], w
+00024ff0: 6972 655f 6c61 7965 723d 7769 7265 5f6c  ire_layer=wire_l
+00025000: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
+00025010: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
+00025020: 2020 2020 2077 6972 655f 7374 6570 2e72       wire_step.r
+00025030: 6f74 6174 6528 3930 290a 2020 2020 2020  otate(90).      
+00025040: 2020 7769 7265 5f73 7465 702e 6365 6e74    wire_step.cent
+00025050: 6572 203d 2028 7061 6474 2e63 656e 7465  er = (padt.cente
+00025060: 725b 305d 2c20 7061 6462 2e79 6d61 7820  r[0], padb.ymax 
+00025070: 2b20 6469 6666 6572 656e 6365 202f 2032  + difference / 2
+00025080: 290a 2020 2020 2020 2020 7472 616e 736c  ).        transl
+00025090: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+000250a0: 696f 6e20 2b20 7061 645f 7369 7a65 5b30  ion + pad_size[0
+000250b0: 5d20 2a20 3132 202f 2031 300a 2020 2020  ] * 12 / 10.    
+000250c0: 2020 2020 636f 6e6e 5f77 6972 655f 746f      conn_wire_to
+000250d0: 7020 3d20 4943 532e 6164 645f 7265 6628  p = ICS.add_ref(
+000250e0: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+000250f0: 7461 6e67 6c65 280a 2020 2020 2020 2020  tangle(.        
+00025100: 2020 2020 2020 2020 7369 7a65 3d28 7769          size=(wi
+00025110: 7265 5f77 6964 7468 735f 7769 6465 5b69  re_widths_wide[i
+00025120: 5d2c 2070 6164 742e 796d 696e 202d 2077  ], padt.ymin - w
+00025130: 6972 655f 7374 6570 2e79 6d61 7829 2c20  ire_step.ymax), 
+00025140: 6c61 7965 723d 7769 7265 5f6c 6179 6572  layer=wire_layer
+00025150: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00025160: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00025170: 2063 6f6e 6e5f 7769 7265 5f62 6f74 746f   conn_wire_botto
+00025180: 6d20 3d20 4943 532e 6164 645f 7265 6628  m = ICS.add_ref(
+00025190: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+000251a0: 7461 6e67 6c65 280a 2020 2020 2020 2020  tangle(.        
+000251b0: 2020 2020 2020 2020 7369 7a65 3d28 7769          size=(wi
+000251c0: 7265 5f77 6964 7468 735f 7769 6465 5b69  re_widths_wide[i
+000251d0: 5d2c 2077 6972 655f 7374 6570 2e79 6d69  ], wire_step.ymi
+000251e0: 6e20 2d20 7061 6462 2e79 6d61 7829 2c20  n - padb.ymax), 
+000251f0: 6c61 7965 723d 7769 7265 5f6c 6179 6572  layer=wire_layer
+00025200: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00025210: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00025220: 2063 6f6e 6e5f 7769 7265 5f74 6f70 2e79   conn_wire_top.y
+00025230: 6d61 7820 3d20 7061 6474 2e79 6d69 6e0a  max = padt.ymin.
+00025240: 2020 2020 2020 2020 636f 6e6e 5f77 6972          conn_wir
+00025250: 655f 746f 702e 786d 696e 203d 2077 6972  e_top.xmin = wir
+00025260: 655f 7374 6570 2e78 6d69 6e0a 2020 2020  e_step.xmin.    
+00025270: 2020 2020 636f 6e6e 5f77 6972 655f 626f      conn_wire_bo
+00025280: 7474 6f6d 2e79 6d69 6e20 3d20 7061 6462  ttom.ymin = padb
+00025290: 2e79 6d61 780a 2020 2020 2020 2020 636f  .ymax.        co
+000252a0: 6e6e 5f77 6972 655f 626f 7474 6f6d 2e78  nn_wire_bottom.x
+000252b0: 6d69 6e20 3d20 7769 7265 5f73 7465 702e  min = wire_step.
+000252c0: 786d 696e 0a0a 2020 2020 7265 7475 726e  xmin..    return
+000252d0: 2049 4353 0a0a 0a64 6566 2074 6573 745f   ICS...def test_
+000252e0: 7265 7328 0a20 2020 2070 6164 5f73 697a  res(.    pad_siz
+000252f0: 653d 5b35 302c 2035 305d 2c20 6e75 6d5f  e=[50, 50], num_
+00025300: 7371 7561 7265 733d 3130 3030 2c20 7769  squares=1000, wi
+00025310: 6474 683d 312c 2072 6573 5f6c 6179 6572  dth=1, res_layer
+00025320: 3d30 2c20 7061 645f 6c61 7965 723d 312c  =0, pad_layer=1,
+00025330: 2067 6e64 5f6c 6179 6572 3d32 0a29 3a0a   gnd_layer=2.):.
+00025340: 2020 2020 2222 2243 7265 6174 6573 2061      """Creates a
+00025350: 6e20 6566 6669 6369 656e 7420 7265 736f  n efficient reso
+00025360: 6e61 746f 7220 7374 7275 6374 7572 6520  nator structure 
+00025370: 666f 7220 6120 7761 6665 7220 6c61 796f  for a wafer layo
+00025380: 7574 2e0a 0a20 2020 2050 6172 616d 6574  ut...    Paramet
+00025390: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000253a0: 2d2d 0a20 2020 2070 6164 5f73 697a 6520  --.    pad_size 
+000253b0: 3a20 6172 7261 792d 6c69 6b65 5b32 5d20  : array-like[2] 
+000253c0: 6f66 2069 6e74 206f 7220 666c 6f61 740a  of int or float.
+000253d0: 2020 2020 2020 2020 2877 6964 7468 2c20          (width, 
+000253e0: 6865 6967 6874 2920 6f66 2074 6865 2074  height) of the t
+000253f0: 776f 206d 6174 6368 6564 2069 6d70 6564  wo matched imped
+00025400: 616e 6365 2070 6164 7320 696e 206d 6963  ance pads in mic
+00025410: 726f 6e73 2e0a 2020 2020 6e75 6d5f 7371  rons..    num_sq
+00025420: 7561 7265 7320 3a20 696e 7420 6f72 2066  uares : int or f
+00025430: 6c6f 6174 0a20 2020 2020 2020 204e 756d  loat.        Num
+00025440: 6265 7220 6f66 2073 7175 6172 6573 2063  ber of squares c
+00025450: 6f6d 7072 6973 696e 6720 7468 6520 7265  omprising the re
+00025460: 736f 6e61 746f 7220 7769 7265 2e0a 2020  sonator wire..  
+00025470: 2020 7769 6474 6820 3a20 696e 7420 6f72    width : int or
+00025480: 2066 6c6f 6174 0a20 2020 2020 2020 2054   float.        T
+00025490: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
+000254a0: 7371 7561 7265 7320 696e 206d 6963 726f  squares in micro
+000254b0: 6e73 2e0a 2020 2020 7265 735f 6c61 7965  ns..    res_laye
+000254c0: 7220 3a20 696e 740a 2020 2020 2020 2020  r : int.        
+000254d0: 5370 6563 6966 6963 206c 6179 6572 2873  Specific layer(s
+000254e0: 2920 746f 2070 7574 2074 6865 2072 6573  ) to put the res
+000254f0: 6f6e 6174 6f72 2073 7472 7563 7475 7265  onator structure
+00025500: 206f 6e2e 0a20 2020 2070 6164 5f6c 6179   on..    pad_lay
+00025510: 6572 203a 2069 6e74 206f 7220 4e6f 6e65  er : int or None
+00025520: 0a20 2020 2020 2020 2053 7065 6369 6669  .        Specifi
+00025530: 6320 6c61 7965 7228 7329 2074 6f20 7075  c layer(s) to pu
+00025540: 7420 7468 6520 7061 6473 206f 6e2e 0a20  t the pads on.. 
+00025550: 2020 2067 6e64 5f6c 6179 6572 203a 2020     gnd_layer :  
+00025560: 696e 7420 6f72 204e 6f6e 650a 2020 2020  int or None.    
+00025570: 2020 2020 5370 6563 6966 6963 206c 6179      Specific lay
+00025580: 6572 2873 2920 746f 2070 7574 2074 6865  er(s) to put the
+00025590: 2067 726f 756e 6420 706c 616e 6520 6f6e   ground plane on
+000255a0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+000255b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2050     -------.    P
+000255c0: 203a 2044 6576 6963 650a 2020 2020 2020   : Device.      
+000255d0: 2020 4120 4465 7669 6365 2063 6f6e 7461    A Device conta
+000255e0: 696e 696e 6720 616e 2065 6666 6963 6965  ining an efficie
+000255f0: 6e74 2072 6573 6f6e 6174 6f72 2073 7472  nt resonator str
+00025600: 7563 7475 7265 2e0a 2020 2020 2222 220a  ucture..    """.
+00025610: 2020 2020 7820 3d20 7061 645f 7369 7a65      x = pad_size
+00025620: 5b30 5d0a 2020 2020 7a20 3d20 7061 645f  [0].    z = pad_
+00025630: 7369 7a65 5b31 5d0a 0a20 2020 2023 2043  size[1]..    # C
+00025640: 6865 636b 696e 6720 7661 6c69 6469 7479  hecking validity
+00025650: 206f 6620 696e 7075 740a 2020 2020 6966   of input.    if
+00025660: 2078 203c 3d20 3020 6f72 207a 203c 3d20   x <= 0 or z <= 
+00025670: 303a 0a20 2020 2020 2020 2072 6169 7365  0:.        raise
+00025680: 2056 616c 7565 4572 726f 7228 2250 6164   ValueError("Pad
+00025690: 206d 7573 7420 6861 7665 2070 6f73 6974   must have posit
+000256a0: 6976 652c 2072 6561 6c20 6469 6d65 6e73  ive, real dimens
+000256b0: 696f 6e73 2229 0a20 2020 2065 6c69 6620  ions").    elif 
+000256c0: 7769 6474 6820 3e20 7a3a 0a20 2020 2020  width > z:.     
+000256d0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000256e0: 726f 7228 2257 6964 7468 206f 6620 6365  ror("Width of ce
+000256f0: 6c6c 2063 616e 6e6f 7420 6265 2067 7265  ll cannot be gre
+00025700: 6174 6572 2074 6861 6e20 6865 6967 6874  ater than height
+00025710: 206f 6620 7061 6422 290a 2020 2020 656c   of pad").    el
+00025720: 6966 206e 756d 5f73 7175 6172 6573 203c  if num_squares <
+00025730: 3d20 303a 0a20 2020 2020 2020 2072 6169  = 0:.        rai
+00025740: 7365 2056 616c 7565 4572 726f 7228 224e  se ValueError("N
+00025750: 756d 6265 7220 6f66 2073 7175 6172 6573  umber of squares
+00025760: 206d 7573 7420 6265 2061 2070 6f73 6974   must be a posit
+00025770: 6976 6520 7265 616c 206e 756d 6265 7222  ive real number"
+00025780: 290a 2020 2020 656c 6966 2077 6964 7468  ).    elif width
+00025790: 203c 3d20 303a 0a20 2020 2020 2020 2072   <= 0:.        r
+000257a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000257b0: 2257 6964 7468 206f 6620 6365 6c6c 206d  "Width of cell m
+000257c0: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
+000257d0: 6520 7265 616c 206e 756d 6265 7222 290a  e real number").
+000257e0: 0a20 2020 2023 2050 6572 666f 726d 696e  .    # Performin
+000257f0: 6720 7072 656c 696d 696e 6172 7920 6361  g preliminary ca
+00025800: 6c63 756c 6174 696f 6e73 0a20 2020 206e  lculations.    n
+00025810: 756d 5f72 6f77 7320 3d20 696e 7428 6e70  um_rows = int(np
+00025820: 2e66 6c6f 6f72 287a 202f 2028 3220 2a20  .floor(z / (2 * 
+00025830: 7769 6474 6829 2929 0a20 2020 2069 6620  width))).    if 
+00025840: 6e75 6d5f 726f 7773 2025 2032 203d 3d20  num_rows % 2 == 
+00025850: 303a 0a20 2020 2020 2020 206e 756d 5f72  0:.        num_r
+00025860: 6f77 7320 2d3d 2031 0a20 2020 206e 756d  ows -= 1.    num
+00025870: 5f63 6f6c 756d 6e73 203d 206e 756d 5f72  _columns = num_r
+00025880: 6f77 7320 2d20 310a 2020 2020 7371 7561  ows - 1.    squa
+00025890: 7265 735f 696e 5f72 6f77 203d 2028 6e75  res_in_row = (nu
+000258a0: 6d5f 7371 7561 7265 7320 2d20 6e75 6d5f  m_squares - num_
+000258b0: 636f 6c75 6d6e 7320 2d20 3229 202f 206e  columns - 2) / n
+000258c0: 756d 5f72 6f77 730a 0a20 2020 2023 2043  um_rows..    # C
+000258d0: 6f6d 7065 6e73 6174 696e 6720 666f 7220  ompensating for 
+000258e0: 7765 6972 6420 6564 6765 2063 6173 6573  weird edge cases
+000258f0: 0a20 2020 2069 6620 7371 7561 7265 735f  .    if squares_
+00025900: 696e 5f72 6f77 203c 2031 3a0a 2020 2020  in_row < 1:.    
+00025910: 2020 2020 6e75 6d5f 726f 7773 203d 2069      num_rows = i
+00025920: 6e74 2872 6f75 6e64 286e 756d 5f72 6f77  nt(round(num_row
+00025930: 7320 2f20 3229 202d 2032 290a 2020 2020  s / 2) - 2).    
+00025940: 2020 2020 7371 7561 7265 735f 696e 5f72      squares_in_r
+00025950: 6f77 203d 2031 0a20 2020 2069 6620 7769  ow = 1.    if wi
+00025960: 6474 6820 2a20 3220 3e20 7a3a 0a20 2020  dth * 2 > z:.   
+00025970: 2020 2020 206e 756d 5f72 6f77 7320 3d20       num_rows = 
+00025980: 310a 2020 2020 2020 2020 7371 7561 7265  1.        square
+00025990: 735f 696e 5f72 6f77 203d 206e 756d 5f73  s_in_row = num_s
+000259a0: 7175 6172 6573 202d 2032 0a0a 2020 2020  quares - 2..    
+000259b0: 6c65 6e67 7468 5f72 6f77 203d 2073 7175  length_row = squ
+000259c0: 6172 6573 5f69 6e5f 726f 7720 2a20 7769  ares_in_row * wi
+000259d0: 6474 680a 0a20 2020 2023 2043 7265 6174  dth..    # Creat
+000259e0: 696e 6720 726f 772f 636f 6c75 6d6e 2063  ing row/column c
+000259f0: 6f72 6e65 7220 636f 6d62 696e 6174 696f  orner combinatio
+00025a00: 6e20 7374 7275 6374 7572 650a 2020 2020  n structure.    
+00025a10: 5420 3d20 4465 7669 6365 2829 0a20 2020  T = Device().   
+00025a20: 2052 6f77 203d 2072 6563 7461 6e67 6c65   Row = rectangle
+00025a30: 2873 697a 653d 286c 656e 6774 685f 726f  (size=(length_ro
+00025a40: 772c 2077 6964 7468 292c 206c 6179 6572  w, width), layer
+00025a50: 3d72 6573 5f6c 6179 6572 290a 2020 2020  =res_layer).    
+00025a60: 436f 6c20 3d20 7265 6374 616e 676c 6528  Col = rectangle(
+00025a70: 7369 7a65 3d28 7769 6474 682c 2077 6964  size=(width, wid
+00025a80: 7468 292c 206c 6179 6572 3d72 6573 5f6c  th), layer=res_l
+00025a90: 6179 6572 290a 0a20 2020 2054 2e61 6464  ayer)..    T.add
+00025aa0: 5f72 6566 2852 6f77 290a 2020 2020 636f  _ref(Row).    co
+00025ab0: 6c20 3d20 542e 6164 645f 7265 6628 436f  l = T.add_ref(Co
+00025ac0: 6c29 0a20 2020 2063 6f6c 2e6d 6f76 6528  l).    col.move(
+00025ad0: 5b6c 656e 6774 685f 726f 7720 2d20 7769  [length_row - wi
+00025ae0: 6474 682c 202d 7769 6474 685d 290a 0a20  dth, -width]).. 
+00025af0: 2020 2023 2043 7265 6174 696e 6720 656e     # Creating en
+00025b00: 7469 7265 2077 6176 6567 7569 6465 206e  tire waveguide n
+00025b10: 6574 0a20 2020 204e 203d 2044 6576 6963  et.    N = Devic
+00025b20: 6528 226e 6574 2229 0a20 2020 206e 203d  e("net").    n =
+00025b30: 2031 0a20 2020 2066 6f72 2069 2069 6e20   1.    for i in 
+00025b40: 7261 6e67 6528 6e75 6d5f 726f 7773 293a  range(num_rows):
+00025b50: 0a20 2020 2020 2020 2069 6620 6920 213d  .        if i !=
+00025b60: 206e 756d 5f72 6f77 7320 2d20 313a 0a20   num_rows - 1:. 
+00025b70: 2020 2020 2020 2020 2020 2064 203d 204e             d = N
+00025b80: 2e61 6464 5f72 6566 2854 290a 2020 2020  .add_ref(T).    
+00025b90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00025ba0: 2020 2020 2020 6420 3d20 4e2e 6164 645f        d = N.add_
+00025bb0: 7265 6628 526f 7729 0a20 2020 2020 2020  ref(Row).       
+00025bc0: 2069 6620 6e20 2520 3220 3d3d 2030 3a0a   if n % 2 == 0:.
+00025bd0: 2020 2020 2020 2020 2020 2020 642e 6d69              d.mi
+00025be0: 7272 6f72 2870 313d 2864 2e78 2c20 642e  rror(p1=(d.x, d.
+00025bf0: 796d 6178 292c 2070 323d 2864 2e78 2c20  ymax), p2=(d.x, 
+00025c00: 642e 796d 696e 2929 0a20 2020 2020 2020  d.ymin)).       
+00025c10: 2064 2e6d 6f76 6579 282d 286e 202d 2031   d.movey(-(n - 1
+00025c20: 2920 2a20 542e 7973 697a 6529 0a20 2020  ) * T.ysize).   
+00025c30: 2020 2020 206e 202b 3d20 310a 2020 2020       n += 1.    
+00025c40: 6420 3d20 4e2e 6164 645f 7265 6628 436f  d = N.add_ref(Co
+00025c50: 6c29 2e6d 6f76 6578 282d 7769 6474 6829  l).movex(-width)
+00025c60: 0a20 2020 2064 203d 204e 2e61 6464 5f72  .    d = N.add_r
+00025c70: 6566 2843 6f6c 292e 6d6f 7665 285b 6c65  ef(Col).move([le
+00025c80: 6e67 7468 5f72 6f77 2c20 2d28 6e20 2d20  ngth_row, -(n - 
+00025c90: 3229 202a 2054 2e79 7369 7a65 5d29 0a0a  2) * T.ysize])..
+00025ca0: 2020 2020 2320 4372 6561 7469 6e67 2070      # Creating p
+00025cb0: 6164 730a 2020 2020 5020 3d20 4465 7669  ads.    P = Devi
+00025cc0: 6365 2822 7465 7374 5f72 6573 2229 0a20  ce("test_res"). 
+00025cd0: 2020 2050 6164 3120 3d20 7265 6374 616e     Pad1 = rectan
+00025ce0: 676c 6528 7369 7a65 3d28 782c 207a 292c  gle(size=(x, z),
+00025cf0: 206c 6179 6572 3d70 6164 5f6c 6179 6572   layer=pad_layer
+00025d00: 290a 2020 2020 5061 6432 203d 2072 6563  ).    Pad2 = rec
+00025d10: 7461 6e67 6c65 2873 697a 653d 2878 202b  tangle(size=(x +
+00025d20: 2035 2c20 7a29 2c20 6c61 7965 723d 7061   5, z), layer=pa
+00025d30: 645f 6c61 7965 7229 0a20 2020 2047 6e64  d_layer).    Gnd
+00025d40: 3120 3d20 6f66 6673 6574 2850 6164 312c  1 = offset(Pad1,
+00025d50: 2064 6973 7461 6e63 653d 2d35 2c20 6c61   distance=-5, la
+00025d60: 7965 723d 676e 645f 6c61 7965 7229 0a20  yer=gnd_layer). 
+00025d70: 2020 2047 6e64 3220 3d20 6f66 6673 6574     Gnd2 = offset
+00025d80: 2850 6164 322c 2064 6973 7461 6e63 653d  (Pad2, distance=
+00025d90: 2d35 2c20 6c61 7965 723d 676e 645f 6c61  -5, layer=gnd_la
+00025da0: 7965 7229 0a20 2020 2070 6164 3120 3d20  yer).    pad1 = 
+00025db0: 502e 6164 645f 7265 6628 5061 6431 292e  P.add_ref(Pad1).
+00025dc0: 6d6f 7665 7828 2d78 202d 2077 6964 7468  movex(-x - width
+00025dd0: 290a 2020 2020 7061 6432 203d 2050 2e61  ).    pad2 = P.a
+00025de0: 6464 5f72 6566 2850 6164 3129 2e6d 6f76  dd_ref(Pad1).mov
+00025df0: 6578 286c 656e 6774 685f 726f 7720 2b20  ex(length_row + 
+00025e00: 7769 6474 6829 0a20 2020 2050 2e61 6464  width).    P.add
+00025e10: 5f72 6566 2847 6e64 3129 2e63 656e 7465  _ref(Gnd1).cente
+00025e20: 7220 3d20 7061 6431 2e63 656e 7465 7220  r = pad1.center 
+00025e30: 2023 2067 6e64 310a 2020 2020 676e 6432   # gnd1.    gnd2
+00025e40: 203d 2050 2e61 6464 5f72 6566 2847 6e64   = P.add_ref(Gnd
+00025e50: 3229 0a20 2020 2050 2e61 6464 5f72 6566  2).    P.add_ref
+00025e60: 284e 292e 7920 3d20 7061 6431 2e79 2020  (N).y = pad1.y  
+00025e70: 2320 6e65 7473 0a20 2020 2067 6e64 322e  # nets.    gnd2.
+00025e80: 6365 6e74 6572 203d 2070 6164 322e 6365  center = pad2.ce
+00025e90: 6e74 6572 0a20 2020 2067 6e64 322e 6d6f  nter.    gnd2.mo
+00025ea0: 7665 7828 322e 3529 0a0a 2020 2020 7265  vex(2.5)..    re
+00025eb0: 7475 726e 2050 0a0a 0a23 203d 3d3d 3d3d  turn P...# =====
+00025ec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00025ed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00025ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00025ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025f00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00025f10: 3d3d 3d3d 3d0a 0a0a 4064 6576 6963 655f  =====...@device_
-00025f20: 6c72 755f 6361 6368 650a 6465 6620 6f70  lru_cache.def op
-00025f30: 7469 6d61 6c5f 6861 6972 7069 6e28 7769  timal_hairpin(wi
-00025f40: 6474 683d 302e 322c 2070 6974 6368 3d30  dth=0.2, pitch=0
-00025f50: 2e36 2c20 6c65 6e67 7468 3d31 302c 2074  .6, length=10, t
-00025f60: 7572 6e5f 7261 7469 6f3d 342c 206e 756d  urn_ratio=4, num
-00025f70: 5f70 7473 3d35 302c 206c 6179 6572 3d30  _pts=50, layer=0
-00025f80: 293a 0a20 2020 2022 2222 4372 6561 7465  ):.    """Create
-00025f90: 7320 616e 206f 7074 696d 616c 6c79 2d72  s an optimally-r
-00025fa0: 6f75 6e64 6564 2068 6169 7270 696e 2067  ounded hairpin g
-00025fb0: 656f 6d65 7472 792c 2077 6974 6820 6120  eometry, with a 
-00025fc0: 3138 3020 6465 6772 6565 2074 7572 6e0a  180 degree turn.
-00025fd0: 2020 2020 6f6e 2074 6865 2072 6967 6874      on the right
-00025fe0: 2065 6e64 206f 6620 7468 6520 706f 6c79   end of the poly
-00025ff0: 676f 6e20 636f 6e6e 6563 7465 6420 746f  gon connected to
-00026000: 2074 776f 2070 726f 6e67 7320 6578 7465   two prongs exte
-00026010: 6e64 696e 6720 746f 7761 7264 730a 2020  nding towards.  
-00026020: 2020 706f 7274 7320 6f6e 2074 6865 206c    ports on the l
-00026030: 6566 7420 656e 642e 0a0a 2020 2020 5061  eft end...    Pa
-00026040: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00026050: 2d2d 2d2d 2d2d 2d0a 2020 2020 7769 6474  -------.    widt
-00026060: 6820 3a20 696e 7420 6f72 2066 6c6f 6174  h : int or float
-00026070: 0a20 2020 2020 2020 2057 6964 7468 206f  .        Width o
-00026080: 6620 7468 6520 6861 6972 7069 6e20 6c65  f the hairpin le
-00026090: 6164 732e 0a20 2020 2070 6974 6368 203a  ads..    pitch :
-000260a0: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
-000260b0: 2020 2020 2020 4469 7374 616e 6365 2062        Distance b
-000260c0: 6574 7765 656e 2074 6865 2074 776f 2068  etween the two h
-000260d0: 6169 7270 696e 206c 6561 6473 2e20 4d75  airpin leads. Mu
-000260e0: 7374 2062 6520 6772 6561 7465 7220 7468  st be greater th
-000260f0: 616e 2077 6964 7468 2e0a 2020 2020 6c65  an width..    le
-00026100: 6e67 7468 203a 2069 6e74 206f 7220 666c  ngth : int or fl
-00026110: 6f61 740a 2020 2020 2020 2020 4c65 6e67  oat.        Leng
-00026120: 7468 206f 6620 7468 6520 6861 6972 7069  th of the hairpi
-00026130: 6e20 6672 6f6d 2074 6865 2063 6f6e 6e65  n from the conne
-00026140: 6374 6f72 7320 746f 2074 6865 206f 7070  ctors to the opp
-00026150: 6f73 6974 6520 656e 6420 6f66 2074 6865  osite end of the
-00026160: 0a20 2020 2020 2020 2063 7572 7665 2e0a  .        curve..
-00026170: 2020 2020 7475 726e 5f72 6174 696f 203a      turn_ratio :
-00026180: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
-00026190: 2020 2020 2020 5370 6563 6966 6965 7320        Specifies 
-000261a0: 686f 7720 6d75 6368 206f 6620 7468 6520  how much of the 
-000261b0: 6861 6972 7069 6e20 6973 2064 6564 6963  hairpin is dedic
-000261c0: 6174 6564 2074 6f20 7468 6520 3138 3020  ated to the 180 
-000261d0: 6465 6772 6565 2074 7572 6e2e 0a20 2020  degree turn..   
-000261e0: 2020 2020 2041 2074 7572 6e5f 7261 7469       A turn_rati
-000261f0: 6f20 6f66 2031 3020 7769 6c6c 2072 6573  o of 10 will res
-00026200: 756c 7420 696e 2032 3025 206f 6620 7468  ult in 20% of th
-00026210: 6520 6861 6972 7069 6e20 6265 696e 6720  e hairpin being 
-00026220: 636f 6d70 7269 7365 6420 6f66 2074 6865  comprised of the
-00026230: 2074 7572 6e2e 0a20 2020 206e 756d 5f70   turn..    num_p
-00026240: 7473 203a 2069 6e74 0a20 2020 2020 2020  ts : int.       
-00026250: 204e 756d 6265 7220 6f66 2070 6f69 6e74   Number of point
-00026260: 7320 636f 6e73 7469 7475 7469 6e67 2074  s constituting t
-00026270: 6865 2031 3830 2064 6567 7265 6520 7475  he 180 degree tu
-00026280: 726e 2e0a 2020 2020 6c61 7965 7220 3a20  rn..    layer : 
-00026290: 696e 742c 2061 7272 6179 2d6c 696b 655b  int, array-like[
-000262a0: 325d 2c20 6f72 2073 6574 0a20 2020 2020  2], or set.     
-000262b0: 2020 2053 7065 6369 6669 6320 6c61 7965     Specific laye
-000262c0: 7228 7329 2074 6f20 7075 7420 706f 6c79  r(s) to put poly
-000262d0: 676f 6e20 6765 6f6d 6574 7279 206f 6e2e  gon geometry on.
-000262e0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-000262f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4420    -------.    D 
-00026300: 3a20 4465 7669 6365 0a20 2020 2020 2020  : Device.       
-00026310: 2041 2044 6576 6963 6520 636f 6e74 6169   A Device contai
-00026320: 6e69 6e67 2061 6e20 6f70 7469 6d61 6c6c  ning an optimall
-00026330: 792d 726f 756e 6465 6420 6861 6972 7069  y-rounded hairpi
-00026340: 6e20 6765 6f6d 6574 7279 2e0a 0a20 2020  n geometry...   
-00026350: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-00026360: 0a20 2020 2048 6169 7270 696e 2070 6974  .    Hairpin pit
-00026370: 6368 206d 7573 7420 6265 2067 7265 6174  ch must be great
-00026380: 6572 2074 6861 6e20 7769 6474 682e 0a0a  er than width...
-00026390: 2020 2020 4f70 7469 6d61 6c20 7374 7275      Optimal stru
-000263a0: 6374 7572 6520 6672 6f6d 2068 7474 7073  cture from https
-000263b0: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3131  ://doi.org/10.11
-000263c0: 3033 2f50 6879 7352 6576 422e 3834 2e31  03/PhysRevB.84.1
-000263d0: 3734 3531 300a 2020 2020 436c 656d 2c20  74510.    Clem, 
-000263e0: 4a2e 2c20 2620 4265 7267 6772 656e 2c20  J., & Berggren, 
-000263f0: 4b2e 2028 3230 3131 292e 2047 656f 6d65  K. (2011). Geome
-00026400: 7472 792d 6465 7065 6e64 656e 7420 6372  try-dependent cr
-00026410: 6974 6963 616c 2063 7572 7265 6e74 7320  itical currents 
-00026420: 696e 0a20 2020 2073 7570 6572 636f 6e64  in.    supercond
-00026430: 7563 7469 6e67 206e 616e 6f63 6972 6375  ucting nanocircu
-00026440: 6974 732e 2050 6879 7369 6361 6c20 5265  its. Physical Re
-00026450: 7669 6577 2042 2c20 3834 2831 3729 2c20  view B, 84(17), 
-00026460: 31e2 8093 3237 2e0a 2020 2020 2222 220a  1...27..    """.
-00026470: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
-00026480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000264a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000264b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000264c0: 0a20 2020 2023 2020 4372 6561 7465 2074  .    #  Create t
-000264d0: 6865 2062 6173 6963 2067 656f 6d65 7472  he basic geometr
-000264e0: 790a 2020 2020 2320 3d3d 3d3d 3d3d 3d3d  y.    # ========
-000264f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00025f00: 3d3d 3d3d 3d3d 3d3d 3d0a 230a 2320 4f70  =========.#.# Op
+00025f10: 7469 6d61 6c20 6375 7272 656e 742d 6372  timal current-cr
+00025f20: 6f77 6469 6e67 2073 7570 6572 636f 6e64  owding supercond
+00025f30: 7563 7469 6e67 2073 7472 7563 7475 7265  ucting structure
+00025f40: 730a 230a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  s.#.# ==========
+00025f50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00025f60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00025f70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00025f80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00025f90: 3d3d 3d3d 0a0a 0a40 6465 7669 6365 5f6c  ====...@device_l
+00025fa0: 7275 5f63 6163 6865 0a64 6566 206f 7074  ru_cache.def opt
+00025fb0: 696d 616c 5f68 6169 7270 696e 2877 6964  imal_hairpin(wid
+00025fc0: 7468 3d30 2e32 2c20 7069 7463 683d 302e  th=0.2, pitch=0.
+00025fd0: 362c 206c 656e 6774 683d 3130 2c20 7475  6, length=10, tu
+00025fe0: 726e 5f72 6174 696f 3d34 2c20 6e75 6d5f  rn_ratio=4, num_
+00025ff0: 7074 733d 3530 2c20 6c61 7965 723d 3029  pts=50, layer=0)
+00026000: 3a0a 2020 2020 2222 2243 7265 6174 6573  :.    """Creates
+00026010: 2061 6e20 6f70 7469 6d61 6c6c 792d 726f   an optimally-ro
+00026020: 756e 6465 6420 6861 6972 7069 6e20 6765  unded hairpin ge
+00026030: 6f6d 6574 7279 2c20 7769 7468 2061 2031  ometry, with a 1
+00026040: 3830 2064 6567 7265 6520 7475 726e 0a20  80 degree turn. 
+00026050: 2020 206f 6e20 7468 6520 7269 6768 7420     on the right 
+00026060: 656e 6420 6f66 2074 6865 2070 6f6c 7967  end of the polyg
+00026070: 6f6e 2063 6f6e 6e65 6374 6564 2074 6f20  on connected to 
+00026080: 7477 6f20 7072 6f6e 6773 2065 7874 656e  two prongs exten
+00026090: 6469 6e67 2074 6f77 6172 6473 0a20 2020  ding towards.   
+000260a0: 2070 6f72 7473 206f 6e20 7468 6520 6c65   ports on the le
+000260b0: 6674 2065 6e64 2e0a 0a20 2020 2050 6172  ft end...    Par
+000260c0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000260d0: 2d2d 2d2d 2d2d 0a20 2020 2077 6964 7468  ------.    width
+000260e0: 203a 2069 6e74 206f 7220 666c 6f61 740a   : int or float.
+000260f0: 2020 2020 2020 2020 5769 6474 6820 6f66          Width of
+00026100: 2074 6865 2068 6169 7270 696e 206c 6561   the hairpin lea
+00026110: 6473 2e0a 2020 2020 7069 7463 6820 3a20  ds..    pitch : 
+00026120: 696e 7420 6f72 2066 6c6f 6174 0a20 2020  int or float.   
+00026130: 2020 2020 2044 6973 7461 6e63 6520 6265       Distance be
+00026140: 7477 6565 6e20 7468 6520 7477 6f20 6861  tween the two ha
+00026150: 6972 7069 6e20 6c65 6164 732e 204d 7573  irpin leads. Mus
+00026160: 7420 6265 2067 7265 6174 6572 2074 6861  t be greater tha
+00026170: 6e20 7769 6474 682e 0a20 2020 206c 656e  n width..    len
+00026180: 6774 6820 3a20 696e 7420 6f72 2066 6c6f  gth : int or flo
+00026190: 6174 0a20 2020 2020 2020 204c 656e 6774  at.        Lengt
+000261a0: 6820 6f66 2074 6865 2068 6169 7270 696e  h of the hairpin
+000261b0: 2066 726f 6d20 7468 6520 636f 6e6e 6563   from the connec
+000261c0: 746f 7273 2074 6f20 7468 6520 6f70 706f  tors to the oppo
+000261d0: 7369 7465 2065 6e64 206f 6620 7468 650a  site end of the.
+000261e0: 2020 2020 2020 2020 6375 7276 652e 0a20          curve.. 
+000261f0: 2020 2074 7572 6e5f 7261 7469 6f20 3a20     turn_ratio : 
+00026200: 696e 7420 6f72 2066 6c6f 6174 0a20 2020  int or float.   
+00026210: 2020 2020 2053 7065 6369 6669 6573 2068       Specifies h
+00026220: 6f77 206d 7563 6820 6f66 2074 6865 2068  ow much of the h
+00026230: 6169 7270 696e 2069 7320 6465 6469 6361  airpin is dedica
+00026240: 7465 6420 746f 2074 6865 2031 3830 2064  ted to the 180 d
+00026250: 6567 7265 6520 7475 726e 2e0a 2020 2020  egree turn..    
+00026260: 2020 2020 4120 7475 726e 5f72 6174 696f      A turn_ratio
+00026270: 206f 6620 3130 2077 696c 6c20 7265 7375   of 10 will resu
+00026280: 6c74 2069 6e20 3230 2520 6f66 2074 6865  lt in 20% of the
+00026290: 2068 6169 7270 696e 2062 6569 6e67 2063   hairpin being c
+000262a0: 6f6d 7072 6973 6564 206f 6620 7468 6520  omprised of the 
+000262b0: 7475 726e 2e0a 2020 2020 6e75 6d5f 7074  turn..    num_pt
+000262c0: 7320 3a20 696e 740a 2020 2020 2020 2020  s : int.        
+000262d0: 4e75 6d62 6572 206f 6620 706f 696e 7473  Number of points
+000262e0: 2063 6f6e 7374 6974 7574 696e 6720 7468   constituting th
+000262f0: 6520 3138 3020 6465 6772 6565 2074 7572  e 180 degree tur
+00026300: 6e2e 0a20 2020 206c 6179 6572 203a 2069  n..    layer : i
+00026310: 6e74 2c20 6172 7261 792d 6c69 6b65 5b32  nt, array-like[2
+00026320: 5d2c 206f 7220 7365 740a 2020 2020 2020  ], or set.      
+00026330: 2020 5370 6563 6966 6963 206c 6179 6572    Specific layer
+00026340: 2873 2920 746f 2070 7574 2070 6f6c 7967  (s) to put polyg
+00026350: 6f6e 2067 656f 6d65 7472 7920 6f6e 2e0a  on geometry on..
+00026360: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00026370: 202d 2d2d 2d2d 2d2d 0a20 2020 2044 203a   -------.    D :
+00026380: 2044 6576 6963 650a 2020 2020 2020 2020   Device.        
+00026390: 4120 4465 7669 6365 2063 6f6e 7461 696e  A Device contain
+000263a0: 696e 6720 616e 206f 7074 696d 616c 6c79  ing an optimally
+000263b0: 2d72 6f75 6e64 6564 2068 6169 7270 696e  -rounded hairpin
+000263c0: 2067 656f 6d65 7472 792e 0a0a 2020 2020   geometry...    
+000263d0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+000263e0: 2020 2020 4861 6972 7069 6e20 7069 7463      Hairpin pitc
+000263f0: 6820 6d75 7374 2062 6520 6772 6561 7465  h must be greate
+00026400: 7220 7468 616e 2077 6964 7468 2e0a 0a20  r than width... 
+00026410: 2020 204f 7074 696d 616c 2073 7472 7563     Optimal struc
+00026420: 7475 7265 2066 726f 6d20 6874 7470 733a  ture from https:
+00026430: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
+00026440: 332f 5068 7973 5265 7642 2e38 342e 3137  3/PhysRevB.84.17
+00026450: 3435 3130 0a20 2020 2043 6c65 6d2c 204a  4510.    Clem, J
+00026460: 2e2c 2026 2042 6572 6767 7265 6e2c 204b  ., & Berggren, K
+00026470: 2e20 2832 3031 3129 2e20 4765 6f6d 6574  . (2011). Geomet
+00026480: 7279 2d64 6570 656e 6465 6e74 2063 7269  ry-dependent cri
+00026490: 7469 6361 6c20 6375 7272 656e 7473 2069  tical currents i
+000264a0: 6e0a 2020 2020 7375 7065 7263 6f6e 6475  n.    supercondu
+000264b0: 6374 696e 6720 6e61 6e6f 6369 7263 7569  cting nanocircui
+000264c0: 7473 2e20 5068 7973 6963 616c 2052 6576  ts. Physical Rev
+000264d0: 6965 7720 422c 2038 3428 3137 292c 2031  iew B, 84(17), 1
+000264e0: e280 9332 372e 0a20 2020 2022 2222 0a20  ...27..    """. 
+000264f0: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
 00026500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00026510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00026520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026530: 3d3d 0a20 2020 2061 203d 2028 7069 7463  ==.    a = (pitc
-00026540: 6820 2b20 7769 6474 6829 202f 2032 0a20  h + width) / 2. 
-00026550: 2020 2079 203d 202d 2870 6974 6368 202d     y = -(pitch -
-00026560: 2077 6964 7468 2920 2f20 320a 2020 2020   width) / 2.    
-00026570: 7820 3d20 2d70 6974 6368 0a20 2020 2064  x = -pitch.    d
-00026580: 6c20 3d20 7769 6474 6820 2f20 286e 756d  l = width / (num
-00026590: 5f70 7473 202a 2032 290a 2020 2020 6e20  _pts * 2).    n 
-000265a0: 3d20 300a 0a20 2020 2023 2047 6574 2070  = 0..    # Get p
-000265b0: 6f69 6e74 7320 6f66 2069 6465 616c 2063  oints of ideal c
-000265c0: 7572 7665 2066 726f 6d20 636f 6e66 6f72  urve from confor
-000265d0: 6d61 6c20 6d61 7070 696e 670a 2020 2020  mal mapping.    
-000265e0: 2320 544f 444f 2054 6869 7320 6973 2061  # TODO This is a
-000265f0: 6e20 696e 6566 6669 6369 656e 7420 7761  n inefficient wa
-00026600: 7920 6f66 2066 696e 6469 6e67 2070 6f69  y of finding poi
-00026610: 6e74 7320 7468 6174 2079 6f75 206e 6565  nts that you nee
-00026620: 640a 2020 2020 7870 7473 203d 205b 785d  d.    xpts = [x]
-00026630: 0a20 2020 2079 7074 7320 3d20 5b79 5d0a  .    ypts = [y].
-00026640: 2020 2020 7768 696c 6520 2879 203c 2030      while (y < 0
-00026650: 2920 2620 286e 203c 2031 6536 293a 0a20  ) & (n < 1e6):. 
-00026660: 2020 2020 2020 2073 203d 2078 202b 2031         s = x + 1
-00026670: 6a20 2a20 790a 2020 2020 2020 2020 7720  j * y.        w 
-00026680: 3d20 7371 7274 2831 202d 206e 702e 6578  = sqrt(1 - np.ex
-00026690: 7028 7069 202a 2073 202f 2061 2929 0a20  p(pi * s / a)). 
-000266a0: 2020 2020 2020 2077 7820 3d20 6e70 2e72         wx = np.r
-000266b0: 6561 6c28 7729 0a20 2020 2020 2020 2077  eal(w).        w
-000266c0: 7920 3d20 6e70 2e69 6d61 6728 7729 0a20  y = np.imag(w). 
-000266d0: 2020 2020 2020 2077 7820 3d20 7778 202f         wx = wx /
-000266e0: 2073 7172 7428 7778 2a2a 3220 2b20 7779   sqrt(wx**2 + wy
-000266f0: 2a2a 3229 0a20 2020 2020 2020 2077 7920  **2).        wy 
-00026700: 3d20 7779 202f 2073 7172 7428 7778 2a2a  = wy / sqrt(wx**
-00026710: 3220 2b20 7779 2a2a 3229 0a20 2020 2020  2 + wy**2).     
-00026720: 2020 2078 203d 2078 202b 2077 7820 2a20     x = x + wx * 
-00026730: 646c 0a20 2020 2020 2020 2079 203d 2079  dl.        y = y
-00026740: 202b 2077 7920 2a20 646c 0a20 2020 2020   + wy * dl.     
-00026750: 2020 2078 7074 732e 6170 7065 6e64 2878     xpts.append(x
-00026760: 290a 2020 2020 2020 2020 7970 7473 2e61  ).        ypts.a
-00026770: 7070 656e 6428 7929 0a20 2020 2020 2020  ppend(y).       
-00026780: 206e 203d 206e 202b 2031 0a20 2020 2079   n = n + 1.    y
-00026790: 7074 735b 2d31 5d20 3d20 3020 2023 2053  pts[-1] = 0  # S
-000267a0: 6574 206c 6173 7420 706f 696e 7420 6265  et last point be
-000267b0: 206f 6e20 7468 6520 783d 3020 6178 6973   on the x=0 axis
-000267c0: 2066 6f72 2073 616b 6520 6f66 2063 6c65   for sake of cle
-000267d0: 616e 6c69 6e65 7373 0a20 2020 2064 735f  anliness.    ds_
-000267e0: 6661 6374 6f72 203d 2069 6e74 286c 656e  factor = int(len
-000267f0: 2878 7074 7329 202f 206e 756d 5f70 7473  (xpts) / num_pts
-00026800: 2920 2023 2044 6f77 6e73 616d 706c 6520  )  # Downsample 
-00026810: 7468 6520 746f 7461 6c20 6e75 6d62 6572  the total number
-00026820: 206f 6620 706f 696e 7473 0a20 2020 2078   of points.    x
-00026830: 7074 7320 3d20 7870 7473 5b3a 3a2d 6473  pts = xpts[::-ds
-00026840: 5f66 6163 746f 725d 0a20 2020 2078 7074  _factor].    xpt
-00026850: 7320 3d20 7870 7473 5b3a 3a2d 315d 2020  s = xpts[::-1]  
-00026860: 2320 5468 6973 206c 6f6f 6b73 2063 6f6e  # This looks con
-00026870: 6675 7369 6e67 2c20 6275 7420 6974 2773  fusing, but it's
-00026880: 206a 7573 7420 666c 6970 7069 6e67 2074   just flipping t
-00026890: 6865 2061 7272 6179 7320 6172 6f75 6e64  he arrays around
-000268a0: 0a20 2020 2079 7074 7320 3d20 7970 7473  .    ypts = ypts
-000268b0: 5b3a 3a2d 6473 5f66 6163 746f 725d 0a20  [::-ds_factor]. 
-000268c0: 2020 2079 7074 7320 3d20 7970 7473 5b3a     ypts = ypts[:
-000268d0: 3a2d 315d 2020 2320 736f 2074 6865 206c  :-1]  # so the l
-000268e0: 6173 7420 706f 696e 7420 6973 2067 7561  ast point is gua
-000268f0: 7261 6e74 6565 6420 746f 2062 6520 696e  ranteed to be in
-00026900: 636c 7564 6564 2077 6865 6e20 646f 776e  cluded when down
-00026910: 7361 6d70 6c65 640a 0a20 2020 2023 2041  sampled..    # A
-00026920: 6464 2070 6f69 6e74 7320 666f 7220 7468  dd points for th
-00026930: 6520 7265 7374 206f 6620 6d65 616e 6465  e rest of meande
-00026940: 720a 2020 2020 7870 7473 2e61 7070 656e  r.    xpts.appen
-00026950: 6428 7870 7473 5b2d 315d 202b 2074 7572  d(xpts[-1] + tur
-00026960: 6e5f 7261 7469 6f20 2a20 7769 6474 6829  n_ratio * width)
-00026970: 0a20 2020 2079 7074 732e 6170 7065 6e64  .    ypts.append
-00026980: 2830 290a 2020 2020 7870 7473 2e61 7070  (0).    xpts.app
-00026990: 656e 6428 7870 7473 5b2d 315d 290a 2020  end(xpts[-1]).  
-000269a0: 2020 7970 7473 2e61 7070 656e 6428 2d61    ypts.append(-a
-000269b0: 290a 2020 2020 7870 7473 2e61 7070 656e  ).    xpts.appen
-000269c0: 6428 7870 7473 5b30 5d29 0a20 2020 2079  d(xpts[0]).    y
-000269d0: 7074 732e 6170 7065 6e64 282d 6129 0a20  pts.append(-a). 
-000269e0: 2020 2078 7074 732e 6170 7065 6e64 286d     xpts.append(m
-000269f0: 6178 2878 7074 7329 202d 206c 656e 6774  ax(xpts) - lengt
-00026a00: 6829 0a20 2020 2079 7074 732e 6170 7065  h).    ypts.appe
-00026a10: 6e64 282d 6129 0a20 2020 2078 7074 732e  nd(-a).    xpts.
-00026a20: 6170 7065 6e64 2878 7074 735b 2d31 5d29  append(xpts[-1])
-00026a30: 0a20 2020 2079 7074 732e 6170 7065 6e64  .    ypts.append
-00026a40: 282d 6120 2b20 7769 6474 6829 0a20 2020  (-a + width).   
-00026a50: 2078 7074 732e 6170 7065 6e64 2878 7074   xpts.append(xpt
-00026a60: 735b 305d 290a 2020 2020 7970 7473 2e61  s[0]).    ypts.a
-00026a70: 7070 656e 6428 7970 7473 5b30 5d29 0a0a  ppend(ypts[0])..
-00026a80: 2020 2020 7870 7473 203d 206e 702e 6172      xpts = np.ar
-00026a90: 7261 7928 7870 7473 290a 2020 2020 7970  ray(xpts).    yp
-00026aa0: 7473 203d 206e 702e 6172 7261 7928 7970  ts = np.array(yp
-00026ab0: 7473 290a 0a20 2020 2023 203d 3d3d 3d3d  ts)..    # =====
-00026ac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026ad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026ae0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026af0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026b00: 3d3d 3d3d 3d0a 2020 2020 2320 2043 7265  =====.    #  Cre
-00026b10: 6174 6520 6120 626c 616e 6b20 6465 7669  ate a blank devi
-00026b20: 6365 2c20 6164 6420 7468 6520 6765 6f6d  ce, add the geom
-00026b30: 6574 7279 2c20 616e 6420 6465 6669 6e65  etry, and define
-00026b40: 2074 6865 2070 6f72 7473 0a20 2020 2023   the ports.    #
-00026b50: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00026530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00026540: 2020 2020 2320 2043 7265 6174 6520 7468      #  Create th
+00026550: 6520 6261 7369 6320 6765 6f6d 6574 7279  e basic geometry
+00026560: 0a20 2020 2023 203d 3d3d 3d3d 3d3d 3d3d  .    # =========
+00026570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000265a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000265b0: 3d0a 2020 2020 6120 3d20 2870 6974 6368  =.    a = (pitch
+000265c0: 202b 2077 6964 7468 2920 2f20 320a 2020   + width) / 2.  
+000265d0: 2020 7920 3d20 2d28 7069 7463 6820 2d20    y = -(pitch - 
+000265e0: 7769 6474 6829 202f 2032 0a20 2020 2078  width) / 2.    x
+000265f0: 203d 202d 7069 7463 680a 2020 2020 646c   = -pitch.    dl
+00026600: 203d 2077 6964 7468 202f 2028 6e75 6d5f   = width / (num_
+00026610: 7074 7320 2a20 3229 0a20 2020 206e 203d  pts * 2).    n =
+00026620: 2030 0a0a 2020 2020 2320 4765 7420 706f   0..    # Get po
+00026630: 696e 7473 206f 6620 6964 6561 6c20 6375  ints of ideal cu
+00026640: 7276 6520 6672 6f6d 2063 6f6e 666f 726d  rve from conform
+00026650: 616c 206d 6170 7069 6e67 0a20 2020 2023  al mapping.    #
+00026660: 2054 4f44 4f20 5468 6973 2069 7320 616e   TODO This is an
+00026670: 2069 6e65 6666 6963 6965 6e74 2077 6179   inefficient way
+00026680: 206f 6620 6669 6e64 696e 6720 706f 696e   of finding poin
+00026690: 7473 2074 6861 7420 796f 7520 6e65 6564  ts that you need
+000266a0: 0a20 2020 2078 7074 7320 3d20 5b78 5d0a  .    xpts = [x].
+000266b0: 2020 2020 7970 7473 203d 205b 795d 0a20      ypts = [y]. 
+000266c0: 2020 2077 6869 6c65 2028 7920 3c20 3029     while (y < 0)
+000266d0: 2026 2028 6e20 3c20 3165 3629 3a0a 2020   & (n < 1e6):.  
+000266e0: 2020 2020 2020 7320 3d20 7820 2b20 316a        s = x + 1j
+000266f0: 202a 2079 0a20 2020 2020 2020 2077 203d   * y.        w =
+00026700: 2073 7172 7428 3120 2d20 6e70 2e65 7870   sqrt(1 - np.exp
+00026710: 2870 6920 2a20 7320 2f20 6129 290a 2020  (pi * s / a)).  
+00026720: 2020 2020 2020 7778 203d 206e 702e 7265        wx = np.re
+00026730: 616c 2877 290a 2020 2020 2020 2020 7779  al(w).        wy
+00026740: 203d 206e 702e 696d 6167 2877 290a 2020   = np.imag(w).  
+00026750: 2020 2020 2020 7778 203d 2077 7820 2f20        wx = wx / 
+00026760: 7371 7274 2877 782a 2a32 202b 2077 792a  sqrt(wx**2 + wy*
+00026770: 2a32 290a 2020 2020 2020 2020 7779 203d  *2).        wy =
+00026780: 2077 7920 2f20 7371 7274 2877 782a 2a32   wy / sqrt(wx**2
+00026790: 202b 2077 792a 2a32 290a 2020 2020 2020   + wy**2).      
+000267a0: 2020 7820 3d20 7820 2b20 7778 202a 2064    x = x + wx * d
+000267b0: 6c0a 2020 2020 2020 2020 7920 3d20 7920  l.        y = y 
+000267c0: 2b20 7779 202a 2064 6c0a 2020 2020 2020  + wy * dl.      
+000267d0: 2020 7870 7473 2e61 7070 656e 6428 7829    xpts.append(x)
+000267e0: 0a20 2020 2020 2020 2079 7074 732e 6170  .        ypts.ap
+000267f0: 7065 6e64 2879 290a 2020 2020 2020 2020  pend(y).        
+00026800: 6e20 3d20 6e20 2b20 310a 2020 2020 7970  n = n + 1.    yp
+00026810: 7473 5b2d 315d 203d 2030 2020 2320 5365  ts[-1] = 0  # Se
+00026820: 7420 6c61 7374 2070 6f69 6e74 2062 6520  t last point be 
+00026830: 6f6e 2074 6865 2078 3d30 2061 7869 7320  on the x=0 axis 
+00026840: 666f 7220 7361 6b65 206f 6620 636c 6561  for sake of clea
+00026850: 6e6c 696e 6573 730a 2020 2020 6473 5f66  nliness.    ds_f
+00026860: 6163 746f 7220 3d20 696e 7428 6c65 6e28  actor = int(len(
+00026870: 7870 7473 2920 2f20 6e75 6d5f 7074 7329  xpts) / num_pts)
+00026880: 2020 2320 446f 776e 7361 6d70 6c65 2074    # Downsample t
+00026890: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
+000268a0: 6f66 2070 6f69 6e74 730a 2020 2020 7870  of points.    xp
+000268b0: 7473 203d 2078 7074 735b 3a3a 2d64 735f  ts = xpts[::-ds_
+000268c0: 6661 6374 6f72 5d0a 2020 2020 7870 7473  factor].    xpts
+000268d0: 203d 2078 7074 735b 3a3a 2d31 5d20 2023   = xpts[::-1]  #
+000268e0: 2054 6869 7320 6c6f 6f6b 7320 636f 6e66   This looks conf
+000268f0: 7573 696e 672c 2062 7574 2069 7427 7320  using, but it's 
+00026900: 6a75 7374 2066 6c69 7070 696e 6720 7468  just flipping th
+00026910: 6520 6172 7261 7973 2061 726f 756e 640a  e arrays around.
+00026920: 2020 2020 7970 7473 203d 2079 7074 735b      ypts = ypts[
+00026930: 3a3a 2d64 735f 6661 6374 6f72 5d0a 2020  ::-ds_factor].  
+00026940: 2020 7970 7473 203d 2079 7074 735b 3a3a    ypts = ypts[::
+00026950: 2d31 5d20 2023 2073 6f20 7468 6520 6c61  -1]  # so the la
+00026960: 7374 2070 6f69 6e74 2069 7320 6775 6172  st point is guar
+00026970: 616e 7465 6564 2074 6f20 6265 2069 6e63  anteed to be inc
+00026980: 6c75 6465 6420 7768 656e 2064 6f77 6e73  luded when downs
+00026990: 616d 706c 6564 0a0a 2020 2020 2320 4164  ampled..    # Ad
+000269a0: 6420 706f 696e 7473 2066 6f72 2074 6865  d points for the
+000269b0: 2072 6573 7420 6f66 206d 6561 6e64 6572   rest of meander
+000269c0: 0a20 2020 2078 7074 732e 6170 7065 6e64  .    xpts.append
+000269d0: 2878 7074 735b 2d31 5d20 2b20 7475 726e  (xpts[-1] + turn
+000269e0: 5f72 6174 696f 202a 2077 6964 7468 290a  _ratio * width).
+000269f0: 2020 2020 7970 7473 2e61 7070 656e 6428      ypts.append(
+00026a00: 3029 0a20 2020 2078 7074 732e 6170 7065  0).    xpts.appe
+00026a10: 6e64 2878 7074 735b 2d31 5d29 0a20 2020  nd(xpts[-1]).   
+00026a20: 2079 7074 732e 6170 7065 6e64 282d 6129   ypts.append(-a)
+00026a30: 0a20 2020 2078 7074 732e 6170 7065 6e64  .    xpts.append
+00026a40: 2878 7074 735b 305d 290a 2020 2020 7970  (xpts[0]).    yp
+00026a50: 7473 2e61 7070 656e 6428 2d61 290a 2020  ts.append(-a).  
+00026a60: 2020 7870 7473 2e61 7070 656e 6428 6d61    xpts.append(ma
+00026a70: 7828 7870 7473 2920 2d20 6c65 6e67 7468  x(xpts) - length
+00026a80: 290a 2020 2020 7970 7473 2e61 7070 656e  ).    ypts.appen
+00026a90: 6428 2d61 290a 2020 2020 7870 7473 2e61  d(-a).    xpts.a
+00026aa0: 7070 656e 6428 7870 7473 5b2d 315d 290a  ppend(xpts[-1]).
+00026ab0: 2020 2020 7970 7473 2e61 7070 656e 6428      ypts.append(
+00026ac0: 2d61 202b 2077 6964 7468 290a 2020 2020  -a + width).    
+00026ad0: 7870 7473 2e61 7070 656e 6428 7870 7473  xpts.append(xpts
+00026ae0: 5b30 5d29 0a20 2020 2079 7074 732e 6170  [0]).    ypts.ap
+00026af0: 7065 6e64 2879 7074 735b 305d 290a 0a20  pend(ypts[0]).. 
+00026b00: 2020 2078 7074 7320 3d20 6e70 2e61 7272     xpts = np.arr
+00026b10: 6179 2878 7074 7329 0a20 2020 2079 7074  ay(xpts).    ypt
+00026b20: 7320 3d20 6e70 2e61 7272 6179 2879 7074  s = np.array(ypt
+00026b30: 7329 0a0a 2020 2020 2320 3d3d 3d3d 3d3d  s)..    # ======
+00026b40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026b50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00026b60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00026b70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026b80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00026b90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-00026ba0: 4420 3d20 4465 7669 6365 286e 616d 653d  D = Device(name=
-00026bb0: 2268 6169 7270 696e 2229 0a20 2020 2044  "hairpin").    D
-00026bc0: 2e61 6464 5f70 6f6c 7967 6f6e 285b 7870  .add_polygon([xp
-00026bd0: 7473 2c20 7970 7473 5d2c 206c 6179 6572  ts, ypts], layer
-00026be0: 3d6c 6179 6572 290a 2020 2020 442e 6164  =layer).    D.ad
-00026bf0: 645f 706f 6c79 676f 6e28 5b78 7074 732c  d_polygon([xpts,
-00026c00: 202d 7970 7473 5d2c 206c 6179 6572 3d6c   -ypts], layer=l
-00026c10: 6179 6572 290a 0a20 2020 2078 706f 7274  ayer)..    xport
-00026c20: 7320 3d20 6d69 6e28 7870 7473 290a 2020  s = min(xpts).  
-00026c30: 2020 7970 6f72 7473 203d 202d 6120 2b20    yports = -a + 
-00026c40: 7769 6474 6820 2f20 320a 2020 2020 442e  width / 2.    D.
-00026c50: 6164 645f 706f 7274 286e 616d 653d 312c  add_port(name=1,
-00026c60: 206d 6964 706f 696e 743d 5b78 706f 7274   midpoint=[xport
-00026c70: 732c 202d 7970 6f72 7473 5d2c 2077 6964  s, -yports], wid
-00026c80: 7468 3d77 6964 7468 2c20 6f72 6965 6e74  th=width, orient
-00026c90: 6174 696f 6e3d 3138 3029 0a20 2020 2044  ation=180).    D
-00026ca0: 2e61 6464 5f70 6f72 7428 6e61 6d65 3d32  .add_port(name=2
-00026cb0: 2c20 6d69 6470 6f69 6e74 3d5b 7870 6f72  , midpoint=[xpor
-00026cc0: 7473 2c20 7970 6f72 7473 5d2c 2077 6964  ts, yports], wid
-00026cd0: 7468 3d77 6964 7468 2c20 6f72 6965 6e74  th=width, orient
-00026ce0: 6174 696f 6e3d 3138 3029 0a0a 2020 2020  ation=180)..    
-00026cf0: 7265 7475 726e 2044 0a0a 0a40 6465 7669  return D...@devi
-00026d00: 6365 5f6c 7275 5f63 6163 6865 0a64 6566  ce_lru_cache.def
-00026d10: 206f 7074 696d 616c 5f73 7465 7028 0a20   optimal_step(. 
-00026d20: 2020 2073 7461 7274 5f77 6964 7468 3d31     start_width=1
-00026d30: 302c 0a20 2020 2065 6e64 5f77 6964 7468  0,.    end_width
-00026d40: 3d32 322c 0a20 2020 206e 756d 5f70 7473  =22,.    num_pts
-00026d50: 3d35 302c 0a20 2020 2077 6964 7468 5f74  =50,.    width_t
-00026d60: 6f6c 3d31 652d 332c 0a20 2020 2061 6e74  ol=1e-3,.    ant
-00026d70: 6963 726f 7764 696e 675f 6661 6374 6f72  icrowding_factor
-00026d80: 3d31 2e32 2c0a 2020 2020 7379 6d6d 6574  =1.2,.    symmet
-00026d90: 7269 633d 4661 6c73 652c 0a20 2020 206c  ric=False,.    l
-00026da0: 6179 6572 3d30 2c0a 293a 0a20 2020 2022  ayer=0,.):.    "
-00026db0: 2222 4372 6561 7465 7320 616e 206f 7074  ""Creates an opt
-00026dc0: 696d 616c 6c79 2d72 6f75 6e64 6564 2073  imally-rounded s
-00026dd0: 7465 7020 6765 6f6d 6574 7279 2e0a 0a20  tep geometry... 
-00026de0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00026df0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00026e00: 2073 7461 7274 5f77 6964 7468 203a 2069   start_width : i
-00026e10: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
-00026e20: 2020 2020 5769 6474 6820 6f66 2074 6865      Width of the
-00026e30: 2063 6f6e 6e65 6374 6f72 206f 6e20 7468   connector on th
-00026e40: 6520 6c65 6674 2065 6e64 206f 6620 7468  e left end of th
-00026e50: 6520 7374 6570 2e0a 2020 2020 656e 645f  e step..    end_
-00026e60: 7769 6474 6820 3a20 696e 7420 6f72 2066  width : int or f
-00026e70: 6c6f 6174 0a20 2020 2020 2020 2057 6964  loat.        Wid
-00026e80: 7468 206f 6620 7468 6520 636f 6e6e 6563  th of the connec
-00026e90: 746f 7220 6f6e 2074 6865 2072 6967 6874  tor on the right
-00026ea0: 2065 6e64 206f 6620 7468 6520 7374 6570   end of the step
-00026eb0: 2e0a 2020 2020 6e75 6d5f 7074 7320 3a20  ..    num_pts : 
-00026ec0: 696e 740a 2020 2020 2020 2020 5468 6520  int.        The 
-00026ed0: 6e75 6d62 6572 206f 6620 706f 696e 7473  number of points
-00026ee0: 2063 6f6d 7072 6973 696e 6720 7468 6520   comprising the 
-00026ef0: 656e 7469 7265 2073 7465 7020 6765 6f6d  entire step geom
-00026f00: 6574 7279 2e0a 2020 2020 7769 6474 685f  etry..    width_
-00026f10: 746f 6c20 3a20 666c 6f61 740a 2020 2020  tol : float.    
-00026f20: 2020 2020 506f 696e 7420 6174 2077 6869      Point at whi
-00026f30: 6368 2074 6f20 7465 726d 696e 6174 6520  ch to terminate 
-00026f40: 7468 6520 6361 6c63 756c 6174 696f 6e20  the calculation 
-00026f50: 6f66 2074 6865 206f 7074 696d 616c 2073  of the optimal s
-00026f60: 7465 700a 2020 2020 616e 7469 6372 6f77  tep.    anticrow
-00026f70: 6469 6e67 5f66 6163 746f 7220 3a20 696e  ding_factor : in
-00026f80: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-00026f90: 2020 2046 6163 746f 7220 746f 2072 6564     Factor to red
-00026fa0: 7563 6520 6375 7272 656e 7420 6372 6f77  uce current crow
-00026fb0: 6469 6e67 2062 7920 656c 6f6e 6761 7469  ding by elongati
-00026fc0: 6e67 0a20 2020 2020 2020 2074 6865 2073  ng.        the s
-00026fd0: 7472 7563 7475 7265 2061 6e64 2072 6564  tructure and red
-00026fe0: 7563 696e 6720 7468 6520 6375 7276 6174  ucing the curvat
-00026ff0: 7572 650a 2020 2020 7379 6d6d 6574 7269  ure.    symmetri
-00027000: 6320 3a20 626f 6f6c 0a20 2020 2020 2020  c : bool.       
-00027010: 2049 6620 5472 7565 2c20 6164 6473 2061   If True, adds a
-00027020: 206d 6972 726f 7265 6420 636f 7079 206f   mirrored copy o
-00027030: 6620 7468 6520 7374 6570 2061 6372 6f73  f the step acros
-00027040: 7320 7468 6520 782d 6178 6973 2074 6f20  s the x-axis to 
-00027050: 7468 650a 2020 2020 2020 2020 6765 6f6d  the.        geom
-00027060: 6574 7279 2061 6e64 2061 646a 7573 7473  etry and adjusts
-00027070: 2074 6865 2077 6964 7468 206f 6620 7468   the width of th
-00027080: 6520 706f 7274 732e 0a20 2020 206c 6179  e ports..    lay
-00027090: 6572 203a 2069 6e74 2c20 6172 7261 792d  er : int, array-
-000270a0: 6c69 6b65 5b32 5d2c 206f 7220 7365 740a  like[2], or set.
-000270b0: 2020 2020 2020 2020 5370 6563 6966 6963          Specific
-000270c0: 206c 6179 6572 2873 2920 746f 2070 7574   layer(s) to put
-000270d0: 2070 6f6c 7967 6f6e 2067 656f 6d65 7472   polygon geometr
-000270e0: 7920 6f6e 2e0a 0a20 2020 2052 6574 7572  y on...    Retur
-000270f0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00027100: 2020 2044 203a 2044 6576 6963 650a 2020     D : Device.  
-00027110: 2020 2020 2020 4120 4465 7669 6365 2063        A Device c
-00027120: 6f6e 7461 696e 696e 6720 616e 206f 7074  ontaining an opt
-00027130: 696d 616c 6c79 2d72 6f75 6e64 6564 2073  imally-rounded s
-00027140: 7465 702e 0a0a 2020 2020 4e6f 7465 730a  tep...    Notes.
-00027150: 2020 2020 2d2d 2d2d 2d0a 2020 2020 4f70      -----.    Op
-00027160: 7469 6d61 6c20 7374 7275 6374 7572 6520  timal structure 
-00027170: 6672 6f6d 2068 7474 7073 3a2f 2f64 6f69  from https://doi
-00027180: 2e6f 7267 2f31 302e 3131 3033 2f50 6879  .org/10.1103/Phy
-00027190: 7352 6576 422e 3834 2e31 3734 3531 300a  sRevB.84.174510.
-000271a0: 2020 2020 436c 656d 2c20 4a2e 2c20 2620      Clem, J., & 
-000271b0: 4265 7267 6772 656e 2c20 4b2e 2028 3230  Berggren, K. (20
-000271c0: 3131 292e 2047 656f 6d65 7472 792d 6465  11). Geometry-de
-000271d0: 7065 6e64 656e 7420 6372 6974 6963 616c  pendent critical
-000271e0: 2063 7572 7265 6e74 7320 696e 0a20 2020   currents in.   
-000271f0: 2073 7570 6572 636f 6e64 7563 7469 6e67   superconducting
-00027200: 206e 616e 6f63 6972 6375 6974 732e 2050   nanocircuits. P
-00027210: 6879 7369 6361 6c20 5265 7669 6577 2042  hysical Review B
-00027220: 2c20 3834 2831 3729 2c20 31e2 8093 3237  , 84(17), 1...27
-00027230: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
-00027240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00027250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00027260: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00027270: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00027280: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2023  ==========.    #
-00027290: 2020 4372 6561 7465 2074 6865 2062 6173    Create the bas
-000272a0: 6963 2067 656f 6d65 7472 790a 2020 2020  ic geometry.    
-000272b0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+00026b80: 3d3d 3d3d 0a20 2020 2023 2020 4372 6561  ====.    #  Crea
+00026b90: 7465 2061 2062 6c61 6e6b 2064 6576 6963  te a blank devic
+00026ba0: 652c 2061 6464 2074 6865 2067 656f 6d65  e, add the geome
+00026bb0: 7472 792c 2061 6e64 2064 6566 696e 6520  try, and define 
+00026bc0: 7468 6520 706f 7274 730a 2020 2020 2320  the ports.    # 
+00026bd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026bf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026c00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00026c10: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2044  ==========.    D
+00026c20: 203d 2044 6576 6963 6528 6e61 6d65 3d22   = Device(name="
+00026c30: 6861 6972 7069 6e22 290a 2020 2020 442e  hairpin").    D.
+00026c40: 6164 645f 706f 6c79 676f 6e28 5b78 7074  add_polygon([xpt
+00026c50: 732c 2079 7074 735d 2c20 6c61 7965 723d  s, ypts], layer=
+00026c60: 6c61 7965 7229 0a20 2020 2044 2e61 6464  layer).    D.add
+00026c70: 5f70 6f6c 7967 6f6e 285b 7870 7473 2c20  _polygon([xpts, 
+00026c80: 2d79 7074 735d 2c20 6c61 7965 723d 6c61  -ypts], layer=la
+00026c90: 7965 7229 0a0a 2020 2020 7870 6f72 7473  yer)..    xports
+00026ca0: 203d 206d 696e 2878 7074 7329 0a20 2020   = min(xpts).   
+00026cb0: 2079 706f 7274 7320 3d20 2d61 202b 2077   yports = -a + w
+00026cc0: 6964 7468 202f 2032 0a20 2020 2044 2e61  idth / 2.    D.a
+00026cd0: 6464 5f70 6f72 7428 6e61 6d65 3d31 2c20  dd_port(name=1, 
+00026ce0: 6d69 6470 6f69 6e74 3d5b 7870 6f72 7473  midpoint=[xports
+00026cf0: 2c20 2d79 706f 7274 735d 2c20 7769 6474  , -yports], widt
+00026d00: 683d 7769 6474 682c 206f 7269 656e 7461  h=width, orienta
+00026d10: 7469 6f6e 3d31 3830 290a 2020 2020 442e  tion=180).    D.
+00026d20: 6164 645f 706f 7274 286e 616d 653d 322c  add_port(name=2,
+00026d30: 206d 6964 706f 696e 743d 5b78 706f 7274   midpoint=[xport
+00026d40: 732c 2079 706f 7274 735d 2c20 7769 6474  s, yports], widt
+00026d50: 683d 7769 6474 682c 206f 7269 656e 7461  h=width, orienta
+00026d60: 7469 6f6e 3d31 3830 290a 0a20 2020 2072  tion=180)..    r
+00026d70: 6574 7572 6e20 440a 0a0a 4064 6576 6963  eturn D...@devic
+00026d80: 655f 6c72 755f 6361 6368 650a 6465 6620  e_lru_cache.def 
+00026d90: 6f70 7469 6d61 6c5f 7374 6570 280a 2020  optimal_step(.  
+00026da0: 2020 7374 6172 745f 7769 6474 683d 3130    start_width=10
+00026db0: 2c0a 2020 2020 656e 645f 7769 6474 683d  ,.    end_width=
+00026dc0: 3232 2c0a 2020 2020 6e75 6d5f 7074 733d  22,.    num_pts=
+00026dd0: 3530 2c0a 2020 2020 7769 6474 685f 746f  50,.    width_to
+00026de0: 6c3d 3165 2d33 2c0a 2020 2020 616e 7469  l=1e-3,.    anti
+00026df0: 6372 6f77 6469 6e67 5f66 6163 746f 723d  crowding_factor=
+00026e00: 312e 322c 0a20 2020 2073 796d 6d65 7472  1.2,.    symmetr
+00026e10: 6963 3d46 616c 7365 2c0a 2020 2020 6c61  ic=False,.    la
+00026e20: 7965 723d 302c 0a29 3a0a 2020 2020 2222  yer=0,.):.    ""
+00026e30: 2243 7265 6174 6573 2061 6e20 6f70 7469  "Creates an opti
+00026e40: 6d61 6c6c 792d 726f 756e 6465 6420 7374  mally-rounded st
+00026e50: 6570 2067 656f 6d65 7472 792e 0a0a 2020  ep geometry...  
+00026e60: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00026e70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00026e80: 7374 6172 745f 7769 6474 6820 3a20 696e  start_width : in
+00026e90: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
+00026ea0: 2020 2057 6964 7468 206f 6620 7468 6520     Width of the 
+00026eb0: 636f 6e6e 6563 746f 7220 6f6e 2074 6865  connector on the
+00026ec0: 206c 6566 7420 656e 6420 6f66 2074 6865   left end of the
+00026ed0: 2073 7465 702e 0a20 2020 2065 6e64 5f77   step..    end_w
+00026ee0: 6964 7468 203a 2069 6e74 206f 7220 666c  idth : int or fl
+00026ef0: 6f61 740a 2020 2020 2020 2020 5769 6474  oat.        Widt
+00026f00: 6820 6f66 2074 6865 2063 6f6e 6e65 6374  h of the connect
+00026f10: 6f72 206f 6e20 7468 6520 7269 6768 7420  or on the right 
+00026f20: 656e 6420 6f66 2074 6865 2073 7465 702e  end of the step.
+00026f30: 0a20 2020 206e 756d 5f70 7473 203a 2069  .    num_pts : i
+00026f40: 6e74 0a20 2020 2020 2020 2054 6865 206e  nt.        The n
+00026f50: 756d 6265 7220 6f66 2070 6f69 6e74 7320  umber of points 
+00026f60: 636f 6d70 7269 7369 6e67 2074 6865 2065  comprising the e
+00026f70: 6e74 6972 6520 7374 6570 2067 656f 6d65  ntire step geome
+00026f80: 7472 792e 0a20 2020 2077 6964 7468 5f74  try..    width_t
+00026f90: 6f6c 203a 2066 6c6f 6174 0a20 2020 2020  ol : float.     
+00026fa0: 2020 2050 6f69 6e74 2061 7420 7768 6963     Point at whic
+00026fb0: 6820 746f 2074 6572 6d69 6e61 7465 2074  h to terminate t
+00026fc0: 6865 2063 616c 6375 6c61 7469 6f6e 206f  he calculation o
+00026fd0: 6620 7468 6520 6f70 7469 6d61 6c20 7374  f the optimal st
+00026fe0: 6570 0a20 2020 2061 6e74 6963 726f 7764  ep.    anticrowd
+00026ff0: 696e 675f 6661 6374 6f72 203a 2069 6e74  ing_factor : int
+00027000: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
+00027010: 2020 4661 6374 6f72 2074 6f20 7265 6475    Factor to redu
+00027020: 6365 2063 7572 7265 6e74 2063 726f 7764  ce current crowd
+00027030: 696e 6720 6279 2065 6c6f 6e67 6174 696e  ing by elongatin
+00027040: 670a 2020 2020 2020 2020 7468 6520 7374  g.        the st
+00027050: 7275 6374 7572 6520 616e 6420 7265 6475  ructure and redu
+00027060: 6369 6e67 2074 6865 2063 7572 7661 7475  cing the curvatu
+00027070: 7265 0a20 2020 2073 796d 6d65 7472 6963  re.    symmetric
+00027080: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
+00027090: 4966 2054 7275 652c 2061 6464 7320 6120  If True, adds a 
+000270a0: 6d69 7272 6f72 6564 2063 6f70 7920 6f66  mirrored copy of
+000270b0: 2074 6865 2073 7465 7020 6163 726f 7373   the step across
+000270c0: 2074 6865 2078 2d61 7869 7320 746f 2074   the x-axis to t
+000270d0: 6865 0a20 2020 2020 2020 2067 656f 6d65  he.        geome
+000270e0: 7472 7920 616e 6420 6164 6a75 7374 7320  try and adjusts 
+000270f0: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+00027100: 2070 6f72 7473 2e0a 2020 2020 6c61 7965   ports..    laye
+00027110: 7220 3a20 696e 742c 2061 7272 6179 2d6c  r : int, array-l
+00027120: 696b 655b 325d 2c20 6f72 2073 6574 0a20  ike[2], or set. 
+00027130: 2020 2020 2020 2053 7065 6369 6669 6320         Specific 
+00027140: 6c61 7965 7228 7329 2074 6f20 7075 7420  layer(s) to put 
+00027150: 706f 6c79 676f 6e20 6765 6f6d 6574 7279  polygon geometry
+00027160: 206f 6e2e 0a0a 2020 2020 5265 7475 726e   on...    Return
+00027170: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00027180: 2020 4420 3a20 4465 7669 6365 0a20 2020    D : Device.   
+00027190: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
+000271a0: 6e74 6169 6e69 6e67 2061 6e20 6f70 7469  ntaining an opti
+000271b0: 6d61 6c6c 792d 726f 756e 6465 6420 7374  mally-rounded st
+000271c0: 6570 2e0a 0a20 2020 204e 6f74 6573 0a20  ep...    Notes. 
+000271d0: 2020 202d 2d2d 2d2d 0a20 2020 204f 7074     -----.    Opt
+000271e0: 696d 616c 2073 7472 7563 7475 7265 2066  imal structure f
+000271f0: 726f 6d20 6874 7470 733a 2f2f 646f 692e  rom https://doi.
+00027200: 6f72 672f 3130 2e31 3130 332f 5068 7973  org/10.1103/Phys
+00027210: 5265 7642 2e38 342e 3137 3435 3130 0a20  RevB.84.174510. 
+00027220: 2020 2043 6c65 6d2c 204a 2e2c 2026 2042     Clem, J., & B
+00027230: 6572 6767 7265 6e2c 204b 2e20 2832 3031  erggren, K. (201
+00027240: 3129 2e20 4765 6f6d 6574 7279 2d64 6570  1). Geometry-dep
+00027250: 656e 6465 6e74 2063 7269 7469 6361 6c20  endent critical 
+00027260: 6375 7272 656e 7473 2069 6e0a 2020 2020  currents in.    
+00027270: 7375 7065 7263 6f6e 6475 6374 696e 6720  superconducting 
+00027280: 6e61 6e6f 6369 7263 7569 7473 2e20 5068  nanocircuits. Ph
+00027290: 7973 6963 616c 2052 6576 6965 7720 422c  ysical Review B,
+000272a0: 2038 3428 3137 292c 2031 e280 9332 372e   84(17), 1...27.
+000272b0: 0a20 2020 2022 2222 0a20 2020 2023 203d  .    """.    # =
 000272c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000272d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000272e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000272f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
-00027300: 2064 6566 2073 7465 705f 706f 696e 7473   def step_points
-00027310: 2865 7461 2c20 572c 2061 293a 0a20 2020  (eta, W, a):.   
-00027320: 2020 2020 2023 2052 6574 7572 6e73 2070       # Returns p
-00027330: 6f69 6e74 7320 6672 6f6d 2061 2075 6e69  oints from a uni
-00027340: 7420 7365 6d69 6369 7263 6c65 2069 6e20  t semicircle in 
-00027350: 7468 6520 7720 283d 2075 202b 2069 7629  the w (= u + iv)
-00027360: 2070 6c61 6e65 2074 6f0a 2020 2020 2020   plane to.      
-00027370: 2020 2320 7468 6520 6f70 7469 6d61 6c20    # the optimal 
-00027380: 6375 7276 6520 696e 2074 6865 207a 6574  curve in the zet
-00027390: 6120 283d 2078 202b 2069 7929 2070 6c61  a (= x + iy) pla
-000273a0: 6e65 2077 6869 6368 2074 7261 6e73 6974  ne which transit
-000273b0: 696f 6e73 0a20 2020 2020 2020 2023 2061  ions.        # a
-000273c0: 2077 6972 6520 6672 6f6d 2061 2077 6964   wire from a wid
-000273d0: 7468 206f 6620 2757 2720 746f 2061 2077  th of 'W' to a w
-000273e0: 6964 7468 206f 6620 2761 270a 2020 2020  idth of 'a'.    
-000273f0: 2020 2020 2320 6574 6120 7461 6b65 7320      # eta takes 
-00027400: 7661 6c75 6520 3020 746f 2070 690a 0a20  value 0 to pi.. 
-00027410: 2020 2020 2020 2057 203d 206e 702e 6172         W = np.ar
-00027420: 7261 7928 572c 2064 7479 7065 3d63 6f6d  ray(W, dtype=com
-00027430: 706c 6578 290a 2020 2020 2020 2020 6120  plex).        a 
-00027440: 3d20 6e70 2e61 7272 6179 2861 2c20 6474  = np.array(a, dt
-00027450: 7970 653d 636f 6d70 6c65 7829 0a0a 2020  ype=complex)..  
-00027460: 2020 2020 2020 6761 6d6d 6120 3d20 2861        gamma = (a
-00027470: 202a 2061 202b 2057 202a 2057 2920 2f20   * a + W * W) / 
-00027480: 2861 202a 2061 202d 2057 202a 2057 290a  (a * a - W * W).
-00027490: 0a20 2020 2020 2020 2077 203d 206e 702e  .        w = np.
-000274a0: 6578 7028 316a 202a 2065 7461 290a 0a20  exp(1j * eta).. 
-000274b0: 2020 2020 2020 207a 6574 6120 3d20 280a         zeta = (.
-000274c0: 2020 2020 2020 2020 2020 2020 340a 2020              4.  
-000274d0: 2020 2020 2020 2020 2020 2a20 316a 0a20            * 1j. 
-000274e0: 2020 2020 2020 2020 2020 202f 2070 690a             / pi.
-000274f0: 2020 2020 2020 2020 2020 2020 2a20 280a              * (.
-00027500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027510: 5720 2a20 6e70 2e61 7263 7461 6e28 7371  W * np.arctan(sq
-00027520: 7274 2828 7720 2d20 6761 6d6d 6129 202f  rt((w - gamma) /
-00027530: 2028 6761 6d6d 6120 2b20 3129 2929 0a20   (gamma + 1))). 
-00027540: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00027550: 2061 202a 206e 702e 6172 6374 616e 2873   a * np.arctan(s
-00027560: 7172 7428 2867 616d 6d61 202d 2031 2920  qrt((gamma - 1) 
-00027570: 2f20 2877 202d 2067 616d 6d61 2929 290a  / (w - gamma))).
-00027580: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00027590: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000275a0: 2078 203d 206e 702e 7265 616c 287a 6574   x = np.real(zet
-000275b0: 6129 0a20 2020 2020 2020 2079 203d 206e  a).        y = n
-000275c0: 702e 696d 6167 287a 6574 6129 0a20 2020  p.imag(zeta).   
-000275d0: 2020 2020 2072 6574 7572 6e20 782c 2079       return x, y
-000275e0: 0a0a 2020 2020 6465 6620 696e 7665 7274  ..    def invert
-000275f0: 5f73 7465 705f 706f 696e 7428 785f 6465  _step_point(x_de
-00027600: 7369 7265 643d 2d31 302c 2079 5f64 6573  sired=-10, y_des
-00027610: 6972 6564 3d4e 6f6e 652c 2057 3d31 2c20  ired=None, W=1, 
-00027620: 613d 3229 3a0a 2020 2020 2020 2020 2320  a=2):.        # 
-00027630: 4669 6e64 7320 7468 6520 6574 6120 6173  Finds the eta as
-00027640: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
-00027650: 6520 7661 6c75 6520 785f 6465 7369 7265  e value x_desire
-00027660: 6420 616c 6f6e 6720 7468 650a 2020 2020  d along the.    
-00027670: 2020 2020 2320 6f70 7469 6d61 6c20 6375      # optimal cu
-00027680: 7276 650a 2020 2020 2020 2020 6465 6620  rve.        def 
-00027690: 6668 2865 7461 293a 0a20 2020 2020 2020  fh(eta):.       
-000276a0: 2020 2020 2067 7565 7373 6564 5f78 2c20       guessed_x, 
-000276b0: 6775 6573 7365 645f 7920 3d20 7374 6570  guessed_y = step
-000276c0: 5f70 6f69 6e74 7328 6574 612c 2057 3d57  _points(eta, W=W
-000276d0: 2c20 613d 6129 0a20 2020 2020 2020 2020  , a=a).         
-000276e0: 2020 2069 6620 795f 6465 7369 7265 6420     if y_desired 
-000276f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00027700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00027710: 2867 7565 7373 6564 5f78 202d 2078 5f64  (guessed_x - x_d
-00027720: 6573 6972 6564 2920 2a2a 2032 2020 2320  esired) ** 2  # 
-00027730: 5468 6520 6572 726f 720a 2020 2020 2020  The error.      
-00027740: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00027750: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00027760: 726e 2028 6775 6573 7365 645f 7920 2d20  rn (guessed_y - 
-00027770: 795f 6465 7369 7265 6429 202a 2a20 320a  y_desired) ** 2.
-00027780: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00027790: 2020 2020 2020 2020 2020 6672 6f6d 2073            from s
-000277a0: 6369 7079 2e6f 7074 696d 697a 6520 696d  cipy.optimize im
-000277b0: 706f 7274 2066 6d69 6e62 6f75 6e64 0a20  port fminbound. 
-000277c0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000277d0: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
-000277e0: 2020 2020 2072 6169 7365 2049 6d70 6f72       raise Impor
-000277f0: 7445 7272 6f72 280a 2020 2020 2020 2020  tError(.        
-00027800: 2020 2020 2020 2020 2220 5b50 4849 444c          " [PHIDL
-00027810: 5d20 546f 2072 756e 2074 6865 206f 7074  ] To run the opt
-00027820: 696d 616c 2d63 7572 7665 2067 656f 6d65  imal-curve geome
-00027830: 7472 7920 220a 2020 2020 2020 2020 2020  try ".          
-00027840: 2020 2020 2020 2266 756e 6374 696f 6e73        "functions
-00027850: 2079 6f75 206e 6565 6420 7363 6970 792c   you need scipy,
-00027860: 2070 6c65 6173 6520 696e 7374 616c 6c20   please install 
-00027870: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00027880: 2020 2269 7420 7769 7468 2060 7069 7020    "it with `pip 
-00027890: 696e 7374 616c 6c20 7363 6970 7960 220a  install scipy`".
-000278a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000278b0: 2020 2020 2020 666f 756e 645f 6574 6120        found_eta 
-000278c0: 3d20 666d 696e 626f 756e 6428 6668 2c20  = fminbound(fh, 
-000278d0: 7831 3d30 2c20 7832 3d70 692c 2061 7267  x1=0, x2=pi, arg
-000278e0: 733d 2829 290a 2020 2020 2020 2020 7265  s=()).        re
-000278f0: 7475 726e 2073 7465 705f 706f 696e 7473  turn step_points
-00027900: 2866 6f75 6e64 5f65 7461 2c20 573d 572c  (found_eta, W=W,
-00027910: 2061 3d61 290a 0a20 2020 2069 6620 7374   a=a)..    if st
-00027920: 6172 745f 7769 6474 6820 3e20 656e 645f  art_width > end_
-00027930: 7769 6474 683a 0a20 2020 2020 2020 2072  width:.        r
-00027940: 6576 6572 7365 203d 2054 7275 650a 2020  everse = True.  
-00027950: 2020 2020 2020 7374 6172 745f 7769 6474        start_widt
-00027960: 682c 2065 6e64 5f77 6964 7468 203d 2065  h, end_width = e
-00027970: 6e64 5f77 6964 7468 2c20 7374 6172 745f  nd_width, start_
-00027980: 7769 6474 680a 2020 2020 656c 7365 3a0a  width.    else:.
-00027990: 2020 2020 2020 2020 7265 7665 7273 6520          reverse 
-000279a0: 3d20 4661 6c73 650a 0a20 2020 2044 203d  = False..    D =
-000279b0: 2044 6576 6963 6528 6e61 6d65 3d22 7374   Device(name="st
-000279c0: 6570 2229 0a20 2020 2069 6620 7374 6172  ep").    if star
-000279d0: 745f 7769 6474 6820 3d3d 2065 6e64 5f77  t_width == end_w
-000279e0: 6964 7468 3a20 2023 204a 7573 7420 7265  idth:  # Just re
-000279f0: 7475 726e 2061 2073 7175 6172 650a 2020  turn a square.  
-00027a00: 2020 2020 2020 6966 2073 796d 6d65 7472        if symmetr
-00027a10: 6963 3a0a 2020 2020 2020 2020 2020 2020  ic:.            
-00027a20: 7970 7473 203d 205b 0a20 2020 2020 2020  ypts = [.       
-00027a30: 2020 2020 2020 2020 202d 7374 6172 745f           -start_
-00027a40: 7769 6474 6820 2f20 322c 0a20 2020 2020  width / 2,.     
-00027a50: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00027a60: 5f77 6964 7468 202f 2032 2c0a 2020 2020  _width / 2,.    
-00027a70: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00027a80: 745f 7769 6474 6820 2f20 322c 0a20 2020  t_width / 2,.   
-00027a90: 2020 2020 2020 2020 2020 2020 202d 7374               -st
-00027aa0: 6172 745f 7769 6474 6820 2f20 322c 0a20  art_width / 2,. 
-00027ab0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00027ac0: 2020 2020 2020 2020 2078 7074 7320 3d20           xpts = 
-00027ad0: 5b30 2c20 302c 2073 7461 7274 5f77 6964  [0, 0, start_wid
-00027ae0: 7468 2c20 7374 6172 745f 7769 6474 685d  th, start_width]
-00027af0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00027b00: 7379 6d6d 6574 7269 633a 0a20 2020 2020  symmetric:.     
-00027b10: 2020 2020 2020 2079 7074 7320 3d20 5b30         ypts = [0
-00027b20: 2c20 7374 6172 745f 7769 6474 682c 2073  , start_width, s
-00027b30: 7461 7274 5f77 6964 7468 2c20 305d 0a20  tart_width, 0]. 
-00027b40: 2020 2020 2020 2020 2020 2078 7074 7320             xpts 
-00027b50: 3d20 5b30 2c20 302c 2073 7461 7274 5f77  = [0, 0, start_w
-00027b60: 6964 7468 2c20 7374 6172 745f 7769 6474  idth, start_widt
-00027b70: 685d 0a20 2020 2020 2020 2044 2e69 6e66  h].        D.inf
-00027b80: 6f5b 226e 756d 5f73 7175 6172 6573 225d  o["num_squares"]
-00027b90: 203d 2031 0a20 2020 2065 6c73 653a 0a20   = 1.    else:. 
-00027ba0: 2020 2020 2020 2078 6d69 6e2c 2079 6d69         xmin, ymi
-00027bb0: 6e20 3d20 696e 7665 7274 5f73 7465 705f  n = invert_step_
-00027bc0: 706f 696e 7428 0a20 2020 2020 2020 2020  point(.         
-00027bd0: 2020 2079 5f64 6573 6972 6564 3d73 7461     y_desired=sta
-00027be0: 7274 5f77 6964 7468 202a 2028 3120 2b20  rt_width * (1 + 
-00027bf0: 7769 6474 685f 746f 6c29 2c20 573d 7374  width_tol), W=st
-00027c00: 6172 745f 7769 6474 682c 2061 3d65 6e64  art_width, a=end
-00027c10: 5f77 6964 7468 0a20 2020 2020 2020 2029  _width.        )
-00027c20: 0a20 2020 2020 2020 2078 6d61 782c 2079  .        xmax, y
-00027c30: 6d61 7820 3d20 696e 7665 7274 5f73 7465  max = invert_ste
-00027c40: 705f 706f 696e 7428 0a20 2020 2020 2020  p_point(.       
-00027c50: 2020 2020 2079 5f64 6573 6972 6564 3d65       y_desired=e
-00027c60: 6e64 5f77 6964 7468 202a 2028 3120 2d20  nd_width * (1 - 
-00027c70: 7769 6474 685f 746f 6c29 2c20 573d 7374  width_tol), W=st
-00027c80: 6172 745f 7769 6474 682c 2061 3d65 6e64  art_width, a=end
-00027c90: 5f77 6964 7468 0a20 2020 2020 2020 2029  _width.        )
-00027ca0: 0a0a 2020 2020 2020 2020 7870 7473 203d  ..        xpts =
-00027cb0: 206e 702e 6c69 6e73 7061 6365 2878 6d69   np.linspace(xmi
-00027cc0: 6e2c 2078 6d61 782c 206e 756d 5f70 7473  n, xmax, num_pts
-00027cd0: 292e 746f 6c69 7374 2829 0a20 2020 2020  ).tolist().     
-00027ce0: 2020 2079 7074 7320 3d20 5b5d 0a20 2020     ypts = [].   
-00027cf0: 2020 2020 2066 6f72 2078 2069 6e20 7870       for x in xp
-00027d00: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00027d10: 782c 2079 203d 2069 6e76 6572 745f 7374  x, y = invert_st
-00027d20: 6570 5f70 6f69 6e74 2878 5f64 6573 6972  ep_point(x_desir
-00027d30: 6564 3d78 2c20 573d 7374 6172 745f 7769  ed=x, W=start_wi
-00027d40: 6474 682c 2061 3d65 6e64 5f77 6964 7468  dth, a=end_width
-00027d50: 290a 2020 2020 2020 2020 2020 2020 7970  ).            yp
-00027d60: 7473 2e61 7070 656e 6428 7929 0a0a 2020  ts.append(y)..  
-00027d70: 2020 2020 2020 7970 7473 5b2d 315d 203d        ypts[-1] =
-00027d80: 2065 6e64 5f77 6964 7468 0a20 2020 2020   end_width.     
-00027d90: 2020 2079 7074 735b 305d 203d 2073 7461     ypts[0] = sta
-00027da0: 7274 5f77 6964 7468 0a20 2020 2020 2020  rt_width.       
-00027db0: 2079 5f6e 756d 5f73 7120 3d20 6e70 2e61   y_num_sq = np.a
-00027dc0: 7272 6179 2879 7074 7329 0a20 2020 2020  rray(ypts).     
-00027dd0: 2020 2078 5f6e 756d 5f73 7120 3d20 6e70     x_num_sq = np
-00027de0: 2e61 7272 6179 2878 7074 7329 0a0a 2020  .array(xpts)..  
-00027df0: 2020 2020 2020 6966 206e 6f74 2073 796d        if not sym
-00027e00: 6d65 7472 6963 3a0a 2020 2020 2020 2020  metric:.        
-00027e10: 2020 2020 7870 7473 2e61 7070 656e 6428      xpts.append(
-00027e20: 7870 7473 5b2d 315d 290a 2020 2020 2020  xpts[-1]).      
-00027e30: 2020 2020 2020 7970 7473 2e61 7070 656e        ypts.appen
-00027e40: 6428 3029 0a20 2020 2020 2020 2020 2020  d(0).           
-00027e50: 2078 7074 732e 6170 7065 6e64 2878 7074   xpts.append(xpt
-00027e60: 735b 305d 290a 2020 2020 2020 2020 2020  s[0]).          
-00027e70: 2020 7970 7473 2e61 7070 656e 6428 3029    ypts.append(0)
-00027e80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00027e90: 2020 2020 2020 2020 2020 2078 7074 7320             xpts 
-00027ea0: 2b3d 205b 7820 666f 7220 7820 696e 2078  += [x for x in x
-00027eb0: 7074 735b 3a3a 2d31 5d5d 0a20 2020 2020  pts[::-1]].     
-00027ec0: 2020 2020 2020 2079 7074 7320 2b3d 205b         ypts += [
-00027ed0: 2d79 2066 6f72 2079 2069 6e20 7970 7473  -y for y in ypts
-00027ee0: 5b3a 3a2d 315d 5d0a 2020 2020 2020 2020  [::-1]].        
-00027ef0: 2020 2020 7870 7473 203d 205b 7820 2f20      xpts = [x / 
-00027f00: 3220 666f 7220 7820 696e 2078 7074 735d  2 for x in xpts]
-00027f10: 0a20 2020 2020 2020 2020 2020 2079 7074  .            ypt
-00027f20: 7320 3d20 5b79 202f 2032 2066 6f72 2079  s = [y / 2 for y
-00027f30: 2069 6e20 7970 7473 5d0a 0a20 2020 2020   in ypts]..     
-00027f40: 2020 2023 2061 6e74 6963 726f 7764 696e     # anticrowdin
-00027f50: 675f 6661 6374 6f72 2073 7472 6574 6368  g_factor stretch
-00027f60: 6573 2074 6865 2077 6972 6520 6f75 743b  es the wire out;
-00027f70: 2061 2073 7472 6574 6368 6564 2077 6972   a stretched wir
-00027f80: 6520 6973 2061 0a20 2020 2020 2020 2023  e is a.        #
-00027f90: 2067 656e 746c 6572 2074 7261 6e73 6974   gentler transit
-00027fa0: 696f 6e2c 2073 6f20 7468 6572 6527 7320  ion, so there's 
-00027fb0: 6c65 7373 2063 6861 6e63 6520 6f66 2063  less chance of c
-00027fc0: 7572 7265 6e74 2063 726f 7764 696e 6720  urrent crowding 
-00027fd0: 6966 0a20 2020 2020 2020 2023 2074 6865  if.        # the
-00027fe0: 2066 6162 7269 6361 7469 6f6e 2069 736e   fabrication isn
-00027ff0: 2774 2070 6572 6665 6374 2062 7574 2061  't perfect but a
-00028000: 7320 6120 7265 7375 6c74 2c20 7468 6520  s a result, the 
-00028010: 7769 7265 2069 736e 2774 2061 730a 2020  wire isn't as.  
-00028020: 2020 2020 2020 2320 7368 6f72 7420 6173        # short as
-00028030: 2069 7420 636f 756c 6420 6265 0a20 2020   it could be.   
-00028040: 2020 2020 2078 7074 7320 3d20 286e 702e       xpts = (np.
-00028050: 6172 7261 7928 7870 7473 2920 2a20 616e  array(xpts) * an
-00028060: 7469 6372 6f77 6469 6e67 5f66 6163 746f  ticrowding_facto
-00028070: 7229 2e74 6f6c 6973 7428 290a 0a20 2020  r).tolist()..   
-00028080: 2020 2020 2069 6620 7265 7665 7273 6520       if reverse 
-00028090: 6973 2054 7275 653a 0a20 2020 2020 2020  is True:.       
-000280a0: 2020 2020 2078 7074 7320 3d20 282d 6e70       xpts = (-np
-000280b0: 2e61 7272 6179 2878 7074 7329 292e 746f  .array(xpts)).to
-000280c0: 6c69 7374 2829 0a20 2020 2020 2020 2020  list().         
-000280d0: 2020 2073 7461 7274 5f77 6964 7468 2c20     start_width, 
-000280e0: 656e 645f 7769 6474 6820 3d20 656e 645f  end_width = end_
-000280f0: 7769 6474 682c 2073 7461 7274 5f77 6964  width, start_wid
-00028100: 7468 0a0a 2020 2020 2020 2020 442e 696e  th..        D.in
-00028110: 666f 5b22 6e75 6d5f 7371 7561 7265 7322  fo["num_squares"
-00028120: 5d20 3d20 6e70 2e73 756d 280a 2020 2020  ] = np.sum(.    
-00028130: 2020 2020 2020 2020 6e70 2e64 6966 6628          np.diff(
-00028140: 785f 6e75 6d5f 7371 2920 2f20 2828 795f  x_num_sq) / ((y_
-00028150: 6e75 6d5f 7371 5b3a 2d31 5d20 2b20 795f  num_sq[:-1] + y_
-00028160: 6e75 6d5f 7371 5b31 3a5d 2920 2f20 3229  num_sq[1:]) / 2)
-00028170: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00028180: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
-00028190: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000281a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000281b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000281c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
-000281d0: 2023 2020 4372 6561 7465 2061 2062 6c61   #  Create a bla
-000281e0: 6e6b 2064 6576 6963 652c 2061 6464 2074  nk device, add t
-000281f0: 6865 2067 656f 6d65 7472 792c 2061 6e64  he geometry, and
-00028200: 2064 6566 696e 6520 7468 6520 706f 7274   define the port
-00028210: 730a 2020 2020 2320 3d3d 3d3d 3d3d 3d3d  s.    # ========
+000272f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00027300: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2320  =========.    # 
+00027310: 2043 7265 6174 6520 7468 6520 6261 7369   Create the basi
+00027320: 6320 6765 6f6d 6574 7279 0a20 2020 2023  c geometry.    #
+00027330: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00027340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00027350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00027360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00027370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00027380: 6465 6620 7374 6570 5f70 6f69 6e74 7328  def step_points(
+00027390: 6574 612c 2057 2c20 6129 3a0a 2020 2020  eta, W, a):.    
+000273a0: 2020 2020 2320 5265 7475 726e 7320 706f      # Returns po
+000273b0: 696e 7473 2066 726f 6d20 6120 756e 6974  ints from a unit
+000273c0: 2073 656d 6963 6972 636c 6520 696e 2074   semicircle in t
+000273d0: 6865 2077 2028 3d20 7520 2b20 6976 2920  he w (= u + iv) 
+000273e0: 706c 616e 6520 746f 0a20 2020 2020 2020  plane to.       
+000273f0: 2023 2074 6865 206f 7074 696d 616c 2063   # the optimal c
+00027400: 7572 7665 2069 6e20 7468 6520 7a65 7461  urve in the zeta
+00027410: 2028 3d20 7820 2b20 6979 2920 706c 616e   (= x + iy) plan
+00027420: 6520 7768 6963 6820 7472 616e 7369 7469  e which transiti
+00027430: 6f6e 730a 2020 2020 2020 2020 2320 6120  ons.        # a 
+00027440: 7769 7265 2066 726f 6d20 6120 7769 6474  wire from a widt
+00027450: 6820 6f66 2027 5727 2074 6f20 6120 7769  h of 'W' to a wi
+00027460: 6474 6820 6f66 2027 6127 0a20 2020 2020  dth of 'a'.     
+00027470: 2020 2023 2065 7461 2074 616b 6573 2076     # eta takes v
+00027480: 616c 7565 2030 2074 6f20 7069 0a0a 2020  alue 0 to pi..  
+00027490: 2020 2020 2020 5720 3d20 6e70 2e61 7272        W = np.arr
+000274a0: 6179 2857 2c20 6474 7970 653d 636f 6d70  ay(W, dtype=comp
+000274b0: 6c65 7829 0a20 2020 2020 2020 2061 203d  lex).        a =
+000274c0: 206e 702e 6172 7261 7928 612c 2064 7479   np.array(a, dty
+000274d0: 7065 3d63 6f6d 706c 6578 290a 0a20 2020  pe=complex)..   
+000274e0: 2020 2020 2067 616d 6d61 203d 2028 6120       gamma = (a 
+000274f0: 2a20 6120 2b20 5720 2a20 5729 202f 2028  * a + W * W) / (
+00027500: 6120 2a20 6120 2d20 5720 2a20 5729 0a0a  a * a - W * W)..
+00027510: 2020 2020 2020 2020 7720 3d20 6e70 2e65          w = np.e
+00027520: 7870 2831 6a20 2a20 6574 6129 0a0a 2020  xp(1j * eta)..  
+00027530: 2020 2020 2020 7a65 7461 203d 2028 0a20        zeta = (. 
+00027540: 2020 2020 2020 2020 2020 2034 0a20 2020             4.   
+00027550: 2020 2020 2020 2020 202a 2031 6a0a 2020           * 1j.  
+00027560: 2020 2020 2020 2020 2020 2f20 7069 0a20            / pi. 
+00027570: 2020 2020 2020 2020 2020 202a 2028 0a20             * (. 
+00027580: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+00027590: 202a 206e 702e 6172 6374 616e 2873 7172   * np.arctan(sqr
+000275a0: 7428 2877 202d 2067 616d 6d61 2920 2f20  t((w - gamma) / 
+000275b0: 2867 616d 6d61 202b 2031 2929 290a 2020  (gamma + 1))).  
+000275c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000275d0: 6120 2a20 6e70 2e61 7263 7461 6e28 7371  a * np.arctan(sq
+000275e0: 7274 2828 6761 6d6d 6120 2d20 3129 202f  rt((gamma - 1) /
+000275f0: 2028 7720 2d20 6761 6d6d 6129 2929 0a20   (w - gamma))). 
+00027600: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00027610: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00027620: 7820 3d20 6e70 2e72 6561 6c28 7a65 7461  x = np.real(zeta
+00027630: 290a 2020 2020 2020 2020 7920 3d20 6e70  ).        y = np
+00027640: 2e69 6d61 6728 7a65 7461 290a 2020 2020  .imag(zeta).    
+00027650: 2020 2020 7265 7475 726e 2078 2c20 790a      return x, y.
+00027660: 0a20 2020 2064 6566 2069 6e76 6572 745f  .    def invert_
+00027670: 7374 6570 5f70 6f69 6e74 2878 5f64 6573  step_point(x_des
+00027680: 6972 6564 3d2d 3130 2c20 795f 6465 7369  ired=-10, y_desi
+00027690: 7265 643d 4e6f 6e65 2c20 573d 312c 2061  red=None, W=1, a
+000276a0: 3d32 293a 0a20 2020 2020 2020 2023 2046  =2):.        # F
+000276b0: 696e 6473 2074 6865 2065 7461 2061 7373  inds the eta ass
+000276c0: 6f63 6961 7465 6420 7769 7468 2074 6865  ociated with the
+000276d0: 2076 616c 7565 2078 5f64 6573 6972 6564   value x_desired
+000276e0: 2061 6c6f 6e67 2074 6865 0a20 2020 2020   along the.     
+000276f0: 2020 2023 206f 7074 696d 616c 2063 7572     # optimal cur
+00027700: 7665 0a20 2020 2020 2020 2064 6566 2066  ve.        def f
+00027710: 6828 6574 6129 3a0a 2020 2020 2020 2020  h(eta):.        
+00027720: 2020 2020 6775 6573 7365 645f 782c 2067      guessed_x, g
+00027730: 7565 7373 6564 5f79 203d 2073 7465 705f  uessed_y = step_
+00027740: 706f 696e 7473 2865 7461 2c20 573d 572c  points(eta, W=W,
+00027750: 2061 3d61 290a 2020 2020 2020 2020 2020   a=a).          
+00027760: 2020 6966 2079 5f64 6573 6972 6564 2069    if y_desired i
+00027770: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00027780: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00027790: 6775 6573 7365 645f 7820 2d20 785f 6465  guessed_x - x_de
+000277a0: 7369 7265 6429 202a 2a20 3220 2023 2054  sired) ** 2  # T
+000277b0: 6865 2065 7272 6f72 0a20 2020 2020 2020  he error.       
+000277c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000277d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000277e0: 6e20 2867 7565 7373 6564 5f79 202d 2079  n (guessed_y - y
+000277f0: 5f64 6573 6972 6564 2920 2a2a 2032 0a0a  _desired) ** 2..
+00027800: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00027810: 2020 2020 2020 2020 2066 726f 6d20 7363           from sc
+00027820: 6970 792e 6f70 7469 6d69 7a65 2069 6d70  ipy.optimize imp
+00027830: 6f72 7420 666d 696e 626f 756e 640a 2020  ort fminbound.  
+00027840: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00027850: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+00027860: 2020 2020 7261 6973 6520 496d 706f 7274      raise Import
+00027870: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00027880: 2020 2020 2020 2022 205b 5048 4944 4c5d         " [PHIDL]
+00027890: 2054 6f20 7275 6e20 7468 6520 6f70 7469   To run the opti
+000278a0: 6d61 6c2d 6375 7276 6520 6765 6f6d 6574  mal-curve geomet
+000278b0: 7279 2022 0a20 2020 2020 2020 2020 2020  ry ".           
+000278c0: 2020 2020 2022 6675 6e63 7469 6f6e 7320       "functions 
+000278d0: 796f 7520 6e65 6564 2073 6369 7079 2c20  you need scipy, 
+000278e0: 706c 6561 7365 2069 6e73 7461 6c6c 2022  please install "
+000278f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027900: 2022 6974 2077 6974 6820 6070 6970 2069   "it with `pip i
+00027910: 6e73 7461 6c6c 2073 6369 7079 6022 0a20  nstall scipy`". 
+00027920: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00027930: 2020 2020 2066 6f75 6e64 5f65 7461 203d       found_eta =
+00027940: 2066 6d69 6e62 6f75 6e64 2866 682c 2078   fminbound(fh, x
+00027950: 313d 302c 2078 323d 7069 2c20 6172 6773  1=0, x2=pi, args
+00027960: 3d28 2929 0a20 2020 2020 2020 2072 6574  =()).        ret
+00027970: 7572 6e20 7374 6570 5f70 6f69 6e74 7328  urn step_points(
+00027980: 666f 756e 645f 6574 612c 2057 3d57 2c20  found_eta, W=W, 
+00027990: 613d 6129 0a0a 2020 2020 6966 2073 7461  a=a)..    if sta
+000279a0: 7274 5f77 6964 7468 203e 2065 6e64 5f77  rt_width > end_w
+000279b0: 6964 7468 3a0a 2020 2020 2020 2020 7265  idth:.        re
+000279c0: 7665 7273 6520 3d20 5472 7565 0a20 2020  verse = True.   
+000279d0: 2020 2020 2073 7461 7274 5f77 6964 7468       start_width
+000279e0: 2c20 656e 645f 7769 6474 6820 3d20 656e  , end_width = en
+000279f0: 645f 7769 6474 682c 2073 7461 7274 5f77  d_width, start_w
+00027a00: 6964 7468 0a20 2020 2065 6c73 653a 0a20  idth.    else:. 
+00027a10: 2020 2020 2020 2072 6576 6572 7365 203d         reverse =
+00027a20: 2046 616c 7365 0a0a 2020 2020 4420 3d20   False..    D = 
+00027a30: 4465 7669 6365 286e 616d 653d 2273 7465  Device(name="ste
+00027a40: 7022 290a 2020 2020 6966 2073 7461 7274  p").    if start
+00027a50: 5f77 6964 7468 203d 3d20 656e 645f 7769  _width == end_wi
+00027a60: 6474 683a 2020 2320 4a75 7374 2072 6574  dth:  # Just ret
+00027a70: 7572 6e20 6120 7371 7561 7265 0a20 2020  urn a square.   
+00027a80: 2020 2020 2069 6620 7379 6d6d 6574 7269       if symmetri
+00027a90: 633a 0a20 2020 2020 2020 2020 2020 2079  c:.            y
+00027aa0: 7074 7320 3d20 5b0a 2020 2020 2020 2020  pts = [.        
+00027ab0: 2020 2020 2020 2020 2d73 7461 7274 5f77          -start_w
+00027ac0: 6964 7468 202f 2032 2c0a 2020 2020 2020  idth / 2,.      
+00027ad0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+00027ae0: 7769 6474 6820 2f20 322c 0a20 2020 2020  width / 2,.     
+00027af0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00027b00: 5f77 6964 7468 202f 2032 2c0a 2020 2020  _width / 2,.    
+00027b10: 2020 2020 2020 2020 2020 2020 2d73 7461              -sta
+00027b20: 7274 5f77 6964 7468 202f 2032 2c0a 2020  rt_width / 2,.  
+00027b30: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00027b40: 2020 2020 2020 2020 7870 7473 203d 205b          xpts = [
+00027b50: 302c 2030 2c20 7374 6172 745f 7769 6474  0, 0, start_widt
+00027b60: 682c 2073 7461 7274 5f77 6964 7468 5d0a  h, start_width].
+00027b70: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00027b80: 796d 6d65 7472 6963 3a0a 2020 2020 2020  ymmetric:.      
+00027b90: 2020 2020 2020 7970 7473 203d 205b 302c        ypts = [0,
+00027ba0: 2073 7461 7274 5f77 6964 7468 2c20 7374   start_width, st
+00027bb0: 6172 745f 7769 6474 682c 2030 5d0a 2020  art_width, 0].  
+00027bc0: 2020 2020 2020 2020 2020 7870 7473 203d            xpts =
+00027bd0: 205b 302c 2030 2c20 7374 6172 745f 7769   [0, 0, start_wi
+00027be0: 6474 682c 2073 7461 7274 5f77 6964 7468  dth, start_width
+00027bf0: 5d0a 2020 2020 2020 2020 442e 696e 666f  ].        D.info
+00027c00: 5b22 6e75 6d5f 7371 7561 7265 7322 5d20  ["num_squares"] 
+00027c10: 3d20 310a 2020 2020 656c 7365 3a0a 2020  = 1.    else:.  
+00027c20: 2020 2020 2020 786d 696e 2c20 796d 696e        xmin, ymin
+00027c30: 203d 2069 6e76 6572 745f 7374 6570 5f70   = invert_step_p
+00027c40: 6f69 6e74 280a 2020 2020 2020 2020 2020  oint(.          
+00027c50: 2020 795f 6465 7369 7265 643d 7374 6172    y_desired=star
+00027c60: 745f 7769 6474 6820 2a20 2831 202b 2077  t_width * (1 + w
+00027c70: 6964 7468 5f74 6f6c 292c 2057 3d73 7461  idth_tol), W=sta
+00027c80: 7274 5f77 6964 7468 2c20 613d 656e 645f  rt_width, a=end_
+00027c90: 7769 6474 680a 2020 2020 2020 2020 290a  width.        ).
+00027ca0: 2020 2020 2020 2020 786d 6178 2c20 796d          xmax, ym
+00027cb0: 6178 203d 2069 6e76 6572 745f 7374 6570  ax = invert_step
+00027cc0: 5f70 6f69 6e74 280a 2020 2020 2020 2020  _point(.        
+00027cd0: 2020 2020 795f 6465 7369 7265 643d 656e      y_desired=en
+00027ce0: 645f 7769 6474 6820 2a20 2831 202d 2077  d_width * (1 - w
+00027cf0: 6964 7468 5f74 6f6c 292c 2057 3d73 7461  idth_tol), W=sta
+00027d00: 7274 5f77 6964 7468 2c20 613d 656e 645f  rt_width, a=end_
+00027d10: 7769 6474 680a 2020 2020 2020 2020 290a  width.        ).
+00027d20: 0a20 2020 2020 2020 2078 7074 7320 3d20  .        xpts = 
+00027d30: 6e70 2e6c 696e 7370 6163 6528 786d 696e  np.linspace(xmin
+00027d40: 2c20 786d 6178 2c20 6e75 6d5f 7074 7329  , xmax, num_pts)
+00027d50: 2e74 6f6c 6973 7428 290a 2020 2020 2020  .tolist().      
+00027d60: 2020 7970 7473 203d 205b 5d0a 2020 2020    ypts = [].    
+00027d70: 2020 2020 666f 7220 7820 696e 2078 7074      for x in xpt
+00027d80: 733a 0a20 2020 2020 2020 2020 2020 2078  s:.            x
+00027d90: 2c20 7920 3d20 696e 7665 7274 5f73 7465  , y = invert_ste
+00027da0: 705f 706f 696e 7428 785f 6465 7369 7265  p_point(x_desire
+00027db0: 643d 782c 2057 3d73 7461 7274 5f77 6964  d=x, W=start_wid
+00027dc0: 7468 2c20 613d 656e 645f 7769 6474 6829  th, a=end_width)
+00027dd0: 0a20 2020 2020 2020 2020 2020 2079 7074  .            ypt
+00027de0: 732e 6170 7065 6e64 2879 290a 0a20 2020  s.append(y)..   
+00027df0: 2020 2020 2079 7074 735b 2d31 5d20 3d20       ypts[-1] = 
+00027e00: 656e 645f 7769 6474 680a 2020 2020 2020  end_width.      
+00027e10: 2020 7970 7473 5b30 5d20 3d20 7374 6172    ypts[0] = star
+00027e20: 745f 7769 6474 680a 2020 2020 2020 2020  t_width.        
+00027e30: 795f 6e75 6d5f 7371 203d 206e 702e 6172  y_num_sq = np.ar
+00027e40: 7261 7928 7970 7473 290a 2020 2020 2020  ray(ypts).      
+00027e50: 2020 785f 6e75 6d5f 7371 203d 206e 702e    x_num_sq = np.
+00027e60: 6172 7261 7928 7870 7473 290a 0a20 2020  array(xpts)..   
+00027e70: 2020 2020 2069 6620 6e6f 7420 7379 6d6d       if not symm
+00027e80: 6574 7269 633a 0a20 2020 2020 2020 2020  etric:.         
+00027e90: 2020 2078 7074 732e 6170 7065 6e64 2878     xpts.append(x
+00027ea0: 7074 735b 2d31 5d29 0a20 2020 2020 2020  pts[-1]).       
+00027eb0: 2020 2020 2079 7074 732e 6170 7065 6e64       ypts.append
+00027ec0: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+00027ed0: 7870 7473 2e61 7070 656e 6428 7870 7473  xpts.append(xpts
+00027ee0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+00027ef0: 2079 7074 732e 6170 7065 6e64 2830 290a   ypts.append(0).
+00027f00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00027f10: 2020 2020 2020 2020 2020 7870 7473 202b            xpts +
+00027f20: 3d20 5b78 2066 6f72 2078 2069 6e20 7870  = [x for x in xp
+00027f30: 7473 5b3a 3a2d 315d 5d0a 2020 2020 2020  ts[::-1]].      
+00027f40: 2020 2020 2020 7970 7473 202b 3d20 5b2d        ypts += [-
+00027f50: 7920 666f 7220 7920 696e 2079 7074 735b  y for y in ypts[
+00027f60: 3a3a 2d31 5d5d 0a20 2020 2020 2020 2020  ::-1]].         
+00027f70: 2020 2078 7074 7320 3d20 5b78 202f 2032     xpts = [x / 2
+00027f80: 2066 6f72 2078 2069 6e20 7870 7473 5d0a   for x in xpts].
+00027f90: 2020 2020 2020 2020 2020 2020 7970 7473              ypts
+00027fa0: 203d 205b 7920 2f20 3220 666f 7220 7920   = [y / 2 for y 
+00027fb0: 696e 2079 7074 735d 0a0a 2020 2020 2020  in ypts]..      
+00027fc0: 2020 2320 616e 7469 6372 6f77 6469 6e67    # anticrowding
+00027fd0: 5f66 6163 746f 7220 7374 7265 7463 6865  _factor stretche
+00027fe0: 7320 7468 6520 7769 7265 206f 7574 3b20  s the wire out; 
+00027ff0: 6120 7374 7265 7463 6865 6420 7769 7265  a stretched wire
+00028000: 2069 7320 610a 2020 2020 2020 2020 2320   is a.        # 
+00028010: 6765 6e74 6c65 7220 7472 616e 7369 7469  gentler transiti
+00028020: 6f6e 2c20 736f 2074 6865 7265 2773 206c  on, so there's l
+00028030: 6573 7320 6368 616e 6365 206f 6620 6375  ess chance of cu
+00028040: 7272 656e 7420 6372 6f77 6469 6e67 2069  rrent crowding i
+00028050: 660a 2020 2020 2020 2020 2320 7468 6520  f.        # the 
+00028060: 6661 6272 6963 6174 696f 6e20 6973 6e27  fabrication isn'
+00028070: 7420 7065 7266 6563 7420 6275 7420 6173  t perfect but as
+00028080: 2061 2072 6573 756c 742c 2074 6865 2077   a result, the w
+00028090: 6972 6520 6973 6e27 7420 6173 0a20 2020  ire isn't as.   
+000280a0: 2020 2020 2023 2073 686f 7274 2061 7320       # short as 
+000280b0: 6974 2063 6f75 6c64 2062 650a 2020 2020  it could be.    
+000280c0: 2020 2020 7870 7473 203d 2028 6e70 2e61      xpts = (np.a
+000280d0: 7272 6179 2878 7074 7329 202a 2061 6e74  rray(xpts) * ant
+000280e0: 6963 726f 7764 696e 675f 6661 6374 6f72  icrowding_factor
+000280f0: 292e 746f 6c69 7374 2829 0a0a 2020 2020  ).tolist()..    
+00028100: 2020 2020 6966 2072 6576 6572 7365 2069      if reverse i
+00028110: 7320 5472 7565 3a0a 2020 2020 2020 2020  s True:.        
+00028120: 2020 2020 7870 7473 203d 2028 2d6e 702e      xpts = (-np.
+00028130: 6172 7261 7928 7870 7473 2929 2e74 6f6c  array(xpts)).tol
+00028140: 6973 7428 290a 2020 2020 2020 2020 2020  ist().          
+00028150: 2020 7374 6172 745f 7769 6474 682c 2065    start_width, e
+00028160: 6e64 5f77 6964 7468 203d 2065 6e64 5f77  nd_width = end_w
+00028170: 6964 7468 2c20 7374 6172 745f 7769 6474  idth, start_widt
+00028180: 680a 0a20 2020 2020 2020 2044 2e69 6e66  h..        D.inf
+00028190: 6f5b 226e 756d 5f73 7175 6172 6573 225d  o["num_squares"]
+000281a0: 203d 206e 702e 7375 6d28 0a20 2020 2020   = np.sum(.     
+000281b0: 2020 2020 2020 206e 702e 6469 6666 2878         np.diff(x
+000281c0: 5f6e 756d 5f73 7129 202f 2028 2879 5f6e  _num_sq) / ((y_n
+000281d0: 756d 5f73 715b 3a2d 315d 202b 2079 5f6e  um_sq[:-1] + y_n
+000281e0: 756d 5f73 715b 313a 5d29 202f 2032 290a  um_sq[1:]) / 2).
+000281f0: 2020 2020 2020 2020 290a 0a20 2020 2023          )..    #
+00028200: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00028210: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00028220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00028230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028260: 3d3d 0a20 2020 2044 2e61 6464 5f70 6f6c  ==.    D.add_pol
-00028270: 7967 6f6e 285b 7870 7473 2c20 7970 7473  ygon([xpts, ypts
-00028280: 5d2c 206c 6179 6572 3d6c 6179 6572 290a  ], layer=layer).
-00028290: 0a20 2020 2069 6620 6e6f 7420 7379 6d6d  .    if not symm
-000282a0: 6574 7269 633a 0a20 2020 2020 2020 2044  etric:.        D
-000282b0: 2e61 6464 5f70 6f72 7428 0a20 2020 2020  .add_port(.     
-000282c0: 2020 2020 2020 206e 616d 653d 312c 0a20         name=1,. 
-000282d0: 2020 2020 2020 2020 2020 206d 6964 706f             midpo
-000282e0: 696e 743d 5b6d 696e 2878 7074 7329 2c20  int=[min(xpts), 
-000282f0: 7374 6172 745f 7769 6474 6820 2f20 325d  start_width / 2]
-00028300: 2c0a 2020 2020 2020 2020 2020 2020 7769  ,.            wi
-00028310: 6474 683d 7374 6172 745f 7769 6474 682c  dth=start_width,
-00028320: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
-00028330: 656e 7461 7469 6f6e 3d31 3830 2c0a 2020  entation=180,.  
-00028340: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00028350: 442e 6164 645f 706f 7274 280a 2020 2020  D.add_port(.    
-00028360: 2020 2020 2020 2020 6e61 6d65 3d32 2c20          name=2, 
-00028370: 6d69 6470 6f69 6e74 3d5b 6d61 7828 7870  midpoint=[max(xp
-00028380: 7473 292c 2065 6e64 5f77 6964 7468 202f  ts), end_width /
-00028390: 2032 5d2c 2077 6964 7468 3d65 6e64 5f77   2], width=end_w
-000283a0: 6964 7468 2c20 6f72 6965 6e74 6174 696f  idth, orientatio
-000283b0: 6e3d 300a 2020 2020 2020 2020 290a 2020  n=0.        ).  
-000283c0: 2020 6966 2073 796d 6d65 7472 6963 3a0a    if symmetric:.
-000283d0: 2020 2020 2020 2020 442e 6164 645f 706f          D.add_po
-000283e0: 7274 286e 616d 653d 312c 206d 6964 706f  rt(name=1, midpo
-000283f0: 696e 743d 5b6d 696e 2878 7074 7329 2c20  int=[min(xpts), 
-00028400: 305d 2c20 7769 6474 683d 7374 6172 745f  0], width=start_
-00028410: 7769 6474 682c 206f 7269 656e 7461 7469  width, orientati
-00028420: 6f6e 3d31 3830 290a 2020 2020 2020 2020  on=180).        
-00028430: 442e 6164 645f 706f 7274 286e 616d 653d  D.add_port(name=
-00028440: 322c 206d 6964 706f 696e 743d 5b6d 6178  2, midpoint=[max
-00028450: 2878 7074 7329 2c20 305d 2c20 7769 6474  (xpts), 0], widt
-00028460: 683d 656e 645f 7769 6474 682c 206f 7269  h=end_width, ori
-00028470: 656e 7461 7469 6f6e 3d30 290a 0a20 2020  entation=0)..   
-00028480: 2072 6574 7572 6e20 440a 0a0a 6465 6620   return D...def 
-00028490: 6f70 7469 6d61 6c5f 3930 6465 6728 7769  optimal_90deg(wi
-000284a0: 6474 683d 3130 302e 302c 206e 756d 5f70  dth=100.0, num_p
-000284b0: 7473 3d31 352c 206c 656e 6774 685f 6164  ts=15, length_ad
-000284c0: 6a75 7374 3d31 2c20 6c61 7965 723d 3029  just=1, layer=0)
-000284d0: 3a0a 2020 2020 2222 2243 7265 6174 6573  :.    """Creates
-000284e0: 2061 6e20 6f70 7469 6d61 6c6c 792d 726f   an optimally-ro
-000284f0: 756e 6465 6420 3930 2064 6567 7265 6520  unded 90 degree 
-00028500: 6265 6e64 2074 6861 7420 6973 2073 6861  bend that is sha
-00028510: 7270 206f 6e20 7468 6520 6f75 7465 720a  rp on the outer.
-00028520: 2020 2020 636f 726e 6572 2e0a 0a20 2020      corner...   
-00028530: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00028540: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2077  ----------.    w
-00028550: 6964 7468 203a 2069 6e74 206f 7220 666c  idth : int or fl
-00028560: 6f61 740a 2020 2020 2020 2020 5769 6474  oat.        Widt
-00028570: 6820 6f66 2074 6865 2070 6f72 7473 206f  h of the ports o
-00028580: 6e20 6569 7468 6572 2073 6964 6520 6f66  n either side of
-00028590: 2074 6865 2062 656e 642e 0a20 2020 206e   the bend..    n
-000285a0: 756d 5f70 7473 203a 2069 6e74 0a20 2020  um_pts : int.   
-000285b0: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
-000285c0: 6f66 2070 6f69 6e74 7320 636f 6d70 7269  of points compri
-000285d0: 7369 6e67 2074 6865 2063 7572 7665 6420  sing the curved 
-000285e0: 7365 6374 696f 6e20 6f66 2074 6865 2062  section of the b
-000285f0: 656e 642e 0a20 2020 206c 656e 6774 685f  end..    length_
-00028600: 6164 6a75 7374 203a 2069 6e74 206f 7220  adjust : int or 
-00028610: 666c 6f61 740a 2020 2020 2020 2020 4164  float.        Ad
-00028620: 6a75 7374 7320 7468 6520 6c65 6e67 7468  justs the length
-00028630: 206f 6620 7468 6520 6e6f 6e2d 6375 7276   of the non-curv
-00028640: 6564 2070 6f72 7469 6f6e 206f 6620 7468  ed portion of th
-00028650: 6520 6265 6e64 2e0a 2020 2020 6c61 7965  e bend..    laye
-00028660: 7220 3a20 696e 742c 2061 7272 6179 2d6c  r : int, array-l
-00028670: 696b 655b 325d 2c20 6f72 2073 6574 0a20  ike[2], or set. 
-00028680: 2020 2020 2020 2053 7065 6369 6669 6320         Specific 
-00028690: 6c61 7965 7228 7329 2074 6f20 7075 7420  layer(s) to put 
-000286a0: 706f 6c79 676f 6e20 6765 6f6d 6574 7279  polygon geometry
-000286b0: 206f 6e2e 0a0a 2020 2020 5265 7475 726e   on...    Return
-000286c0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-000286d0: 2020 4420 3a20 4465 7669 6365 0a20 2020    D : Device.   
-000286e0: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
-000286f0: 6e74 6169 6e69 6e67 2061 6e20 6f70 7469  ntaining an opti
-00028700: 6d61 6c6c 792d 726f 756e 6465 6420 3930  mally-rounded 90
-00028710: 2064 6567 7265 6520 6265 6e64 2e0a 0a20   degree bend... 
-00028720: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-00028730: 2d2d 0a20 2020 204f 7074 696d 616c 2073  --.    Optimal s
-00028740: 7472 7563 7475 7265 2066 726f 6d20 6874  tructure from ht
-00028750: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
-00028760: 2e31 3130 332f 5068 7973 5265 7642 2e38  .1103/PhysRevB.8
-00028770: 342e 3137 3435 3130 0a20 2020 2043 6c65  4.174510.    Cle
-00028780: 6d2c 204a 2e2c 2026 2042 6572 6767 7265  m, J., & Berggre
-00028790: 6e2c 204b 2e20 2832 3031 3129 2e20 4765  n, K. (2011). Ge
-000287a0: 6f6d 6574 7279 2d64 6570 656e 6465 6e74  ometry-dependent
-000287b0: 2063 7269 7469 6361 6c20 6375 7272 656e   critical curren
-000287c0: 7473 2069 6e0a 2020 2020 7375 7065 7263  ts in.    superc
-000287d0: 6f6e 6475 6374 696e 6720 6e61 6e6f 6369  onducting nanoci
-000287e0: 7263 7569 7473 2e20 5068 7973 6963 616c  rcuits. Physical
-000287f0: 2052 6576 6965 7720 422c 2038 3428 3137   Review B, 84(17
-00028800: 292c 2031 e280 9332 372e 0a20 2020 2022  ), 1...27..    "
-00028810: 2222 0a20 2020 2044 203d 2044 6576 6963  "".    D = Devic
-00028820: 6528 2239 3064 6567 2229 0a0a 2020 2020  e("90deg")..    
-00028830: 2320 4765 7420 706f 696e 7473 206f 6620  # Get points of 
-00028840: 6964 6561 6c20 6375 7276 650a 2020 2020  ideal curve.    
-00028850: 6120 3d20 3220 2a20 7769 6474 680a 2020  a = 2 * width.  
-00028860: 2020 7620 3d20 6e70 2e6c 6f67 7370 6163    v = np.logspac
-00028870: 6528 2d6c 656e 6774 685f 6164 6a75 7374  e(-length_adjust
-00028880: 2c20 6c65 6e67 7468 5f61 646a 7573 742c  , length_adjust,
-00028890: 206e 756d 5f70 7473 290a 2020 2020 7869   num_pts).    xi
-000288a0: 203d 2028 0a20 2020 2020 2020 2061 202f   = (.        a /
-000288b0: 2032 2e30 202a 2028 2831 202b 2032 202f   2.0 * ((1 + 2 /
-000288c0: 2070 6920 2a20 6e70 2e61 7263 7369 6e68   pi * np.arcsinh
-000288d0: 2831 202f 2076 2929 202b 2031 6a20 2a20  (1 / v)) + 1j * 
-000288e0: 2831 202b 2032 202f 2070 6920 2a20 6e70  (1 + 2 / pi * np
-000288f0: 2e61 7263 7369 6e68 2876 2929 290a 2020  .arcsinh(v))).  
-00028900: 2020 290a 2020 2020 7870 7473 203d 206c    ).    xpts = l
-00028910: 6973 7428 6e70 2e72 6561 6c28 7869 2929  ist(np.real(xi))
-00028920: 0a20 2020 2079 7074 7320 3d20 6c69 7374  .    ypts = list
-00028930: 286e 702e 696d 6167 2878 6929 290a 0a20  (np.imag(xi)).. 
-00028940: 2020 2023 2041 6464 2070 6f69 6e74 7320     # Add points 
-00028950: 666f 7220 7468 6520 7265 7374 206f 6620  for the rest of 
-00028960: 6375 7276 650a 2020 2020 6420 3d20 3220  curve.    d = 2 
-00028970: 2a20 7870 7473 5b30 5d20 2023 2046 6172  * xpts[0]  # Far
-00028980: 7468 6573 7420 706f 696e 7420 6f75 7420  thest point out 
-00028990: 2a20 322c 2072 6f75 6e64 6564 2074 6f20  * 2, rounded to 
-000289a0: 6e65 6172 6573 7420 3130 300a 2020 2020  nearest 100.    
-000289b0: 7870 7473 2e61 7070 656e 6428 7769 6474  xpts.append(widt
-000289c0: 6829 0a20 2020 2079 7074 732e 6170 7065  h).    ypts.appe
-000289d0: 6e64 2864 290a 2020 2020 7870 7473 2e61  nd(d).    xpts.a
-000289e0: 7070 656e 6428 3029 0a20 2020 2079 7074  ppend(0).    ypt
-000289f0: 732e 6170 7065 6e64 2864 290a 2020 2020  s.append(d).    
-00028a00: 7870 7473 2e61 7070 656e 6428 3029 0a20  xpts.append(0). 
-00028a10: 2020 2079 7074 732e 6170 7065 6e64 2830     ypts.append(0
-00028a20: 290a 2020 2020 7870 7473 2e61 7070 656e  ).    xpts.appen
-00028a30: 6428 6429 0a20 2020 2079 7074 732e 6170  d(d).    ypts.ap
-00028a40: 7065 6e64 2830 290a 2020 2020 7870 7473  pend(0).    xpts
-00028a50: 2e61 7070 656e 6428 6429 0a20 2020 2079  .append(d).    y
-00028a60: 7074 732e 6170 7065 6e64 2877 6964 7468  pts.append(width
-00028a70: 290a 2020 2020 7870 7473 2e61 7070 656e  ).    xpts.appen
-00028a80: 6428 7870 7473 5b30 5d29 0a20 2020 2079  d(xpts[0]).    y
-00028a90: 7074 732e 6170 7065 6e64 2879 7074 735b  pts.append(ypts[
-00028aa0: 305d 290a 0a20 2020 2044 2e61 6464 5f70  0])..    D.add_p
-00028ab0: 6f6c 7967 6f6e 285b 7870 7473 2c20 7970  olygon([xpts, yp
-00028ac0: 7473 5d2c 206c 6179 6572 3d6c 6179 6572  ts], layer=layer
-00028ad0: 290a 0a20 2020 2044 2e61 6464 5f70 6f72  )..    D.add_por
-00028ae0: 7428 6e61 6d65 3d31 2c20 6d69 6470 6f69  t(name=1, midpoi
-00028af0: 6e74 3d5b 6120 2f20 342c 2064 5d2c 2077  nt=[a / 4, d], w
-00028b00: 6964 7468 3d61 202f 2032 2c20 6f72 6965  idth=a / 2, orie
-00028b10: 6e74 6174 696f 6e3d 3930 290a 2020 2020  ntation=90).    
-00028b20: 442e 6164 645f 706f 7274 286e 616d 653d  D.add_port(name=
-00028b30: 322c 206d 6964 706f 696e 743d 5b64 2c20  2, midpoint=[d, 
-00028b40: 6120 2f20 345d 2c20 7769 6474 683d 6120  a / 4], width=a 
-00028b50: 2f20 322c 206f 7269 656e 7461 7469 6f6e  / 2, orientation
-00028b60: 3d30 290a 2020 2020 7265 7475 726e 2044  =0).    return D
-00028b70: 0a0a 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ...# ===========
-00028b80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028b90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028bb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028bc0: 3d3d 3d0a 2320 4578 616d 706c 6520 636f  ===.# Example co
-00028bd0: 6465 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d  de.# ===========
-00028be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028bf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00028250: 2320 2043 7265 6174 6520 6120 626c 616e  #  Create a blan
+00028260: 6b20 6465 7669 6365 2c20 6164 6420 7468  k device, add th
+00028270: 6520 6765 6f6d 6574 7279 2c20 616e 6420  e geometry, and 
+00028280: 6465 6669 6e65 2074 6865 2070 6f72 7473  define the ports
+00028290: 0a20 2020 2023 203d 3d3d 3d3d 3d3d 3d3d  .    # =========
+000282a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000282b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000282c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000282d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000282e0: 3d0a 2020 2020 442e 6164 645f 706f 6c79  =.    D.add_poly
+000282f0: 676f 6e28 5b78 7074 732c 2079 7074 735d  gon([xpts, ypts]
+00028300: 2c20 6c61 7965 723d 6c61 7965 7229 0a0a  , layer=layer)..
+00028310: 2020 2020 6966 206e 6f74 2073 796d 6d65      if not symme
+00028320: 7472 6963 3a0a 2020 2020 2020 2020 442e  tric:.        D.
+00028330: 6164 645f 706f 7274 280a 2020 2020 2020  add_port(.      
+00028340: 2020 2020 2020 6e61 6d65 3d31 2c0a 2020        name=1,.  
+00028350: 2020 2020 2020 2020 2020 6d69 6470 6f69            midpoi
+00028360: 6e74 3d5b 6d69 6e28 7870 7473 292c 2073  nt=[min(xpts), s
+00028370: 7461 7274 5f77 6964 7468 202f 2032 5d2c  tart_width / 2],
+00028380: 0a20 2020 2020 2020 2020 2020 2077 6964  .            wid
+00028390: 7468 3d73 7461 7274 5f77 6964 7468 2c0a  th=start_width,.
+000283a0: 2020 2020 2020 2020 2020 2020 6f72 6965              orie
+000283b0: 6e74 6174 696f 6e3d 3138 302c 0a20 2020  ntation=180,.   
+000283c0: 2020 2020 2029 0a20 2020 2020 2020 2044       ).        D
+000283d0: 2e61 6464 5f70 6f72 7428 0a20 2020 2020  .add_port(.     
+000283e0: 2020 2020 2020 206e 616d 653d 322c 206d         name=2, m
+000283f0: 6964 706f 696e 743d 5b6d 6178 2878 7074  idpoint=[max(xpt
+00028400: 7329 2c20 656e 645f 7769 6474 6820 2f20  s), end_width / 
+00028410: 325d 2c20 7769 6474 683d 656e 645f 7769  2], width=end_wi
+00028420: 6474 682c 206f 7269 656e 7461 7469 6f6e  dth, orientation
+00028430: 3d30 0a20 2020 2020 2020 2029 0a20 2020  =0.        ).   
+00028440: 2069 6620 7379 6d6d 6574 7269 633a 0a20   if symmetric:. 
+00028450: 2020 2020 2020 2044 2e61 6464 5f70 6f72         D.add_por
+00028460: 7428 6e61 6d65 3d31 2c20 6d69 6470 6f69  t(name=1, midpoi
+00028470: 6e74 3d5b 6d69 6e28 7870 7473 292c 2030  nt=[min(xpts), 0
+00028480: 5d2c 2077 6964 7468 3d73 7461 7274 5f77  ], width=start_w
+00028490: 6964 7468 2c20 6f72 6965 6e74 6174 696f  idth, orientatio
+000284a0: 6e3d 3138 3029 0a20 2020 2020 2020 2044  n=180).        D
+000284b0: 2e61 6464 5f70 6f72 7428 6e61 6d65 3d32  .add_port(name=2
+000284c0: 2c20 6d69 6470 6f69 6e74 3d5b 6d61 7828  , midpoint=[max(
+000284d0: 7870 7473 292c 2030 5d2c 2077 6964 7468  xpts), 0], width
+000284e0: 3d65 6e64 5f77 6964 7468 2c20 6f72 6965  =end_width, orie
+000284f0: 6e74 6174 696f 6e3d 3029 0a0a 2020 2020  ntation=0)..    
+00028500: 7265 7475 726e 2044 0a0a 0a64 6566 206f  return D...def o
+00028510: 7074 696d 616c 5f39 3064 6567 2877 6964  ptimal_90deg(wid
+00028520: 7468 3d31 3030 2e30 2c20 6e75 6d5f 7074  th=100.0, num_pt
+00028530: 733d 3135 2c20 6c65 6e67 7468 5f61 646a  s=15, length_adj
+00028540: 7573 743d 312c 206c 6179 6572 3d30 293a  ust=1, layer=0):
+00028550: 0a20 2020 2022 2222 4372 6561 7465 7320  .    """Creates 
+00028560: 616e 206f 7074 696d 616c 6c79 2d72 6f75  an optimally-rou
+00028570: 6e64 6564 2039 3020 6465 6772 6565 2062  nded 90 degree b
+00028580: 656e 6420 7468 6174 2069 7320 7368 6172  end that is shar
+00028590: 7020 6f6e 2074 6865 206f 7574 6572 0a20  p on the outer. 
+000285a0: 2020 2063 6f72 6e65 722e 0a0a 2020 2020     corner...    
+000285b0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000285c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7769  ---------.    wi
+000285d0: 6474 6820 3a20 696e 7420 6f72 2066 6c6f  dth : int or flo
+000285e0: 6174 0a20 2020 2020 2020 2057 6964 7468  at.        Width
+000285f0: 206f 6620 7468 6520 706f 7274 7320 6f6e   of the ports on
+00028600: 2065 6974 6865 7220 7369 6465 206f 6620   either side of 
+00028610: 7468 6520 6265 6e64 2e0a 2020 2020 6e75  the bend..    nu
+00028620: 6d5f 7074 7320 3a20 696e 740a 2020 2020  m_pts : int.    
+00028630: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
+00028640: 6620 706f 696e 7473 2063 6f6d 7072 6973  f points compris
+00028650: 696e 6720 7468 6520 6375 7276 6564 2073  ing the curved s
+00028660: 6563 7469 6f6e 206f 6620 7468 6520 6265  ection of the be
+00028670: 6e64 2e0a 2020 2020 6c65 6e67 7468 5f61  nd..    length_a
+00028680: 646a 7573 7420 3a20 696e 7420 6f72 2066  djust : int or f
+00028690: 6c6f 6174 0a20 2020 2020 2020 2041 646a  loat.        Adj
+000286a0: 7573 7473 2074 6865 206c 656e 6774 6820  usts the length 
+000286b0: 6f66 2074 6865 206e 6f6e 2d63 7572 7665  of the non-curve
+000286c0: 6420 706f 7274 696f 6e20 6f66 2074 6865  d portion of the
+000286d0: 2062 656e 642e 0a20 2020 206c 6179 6572   bend..    layer
+000286e0: 203a 2069 6e74 2c20 6172 7261 792d 6c69   : int, array-li
+000286f0: 6b65 5b32 5d2c 206f 7220 7365 740a 2020  ke[2], or set.  
+00028700: 2020 2020 2020 5370 6563 6966 6963 206c        Specific l
+00028710: 6179 6572 2873 2920 746f 2070 7574 2070  ayer(s) to put p
+00028720: 6f6c 7967 6f6e 2067 656f 6d65 7472 7920  olygon geometry 
+00028730: 6f6e 2e0a 0a20 2020 2052 6574 7572 6e73  on...    Returns
+00028740: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00028750: 2044 203a 2044 6576 6963 650a 2020 2020   D : Device.    
+00028760: 2020 2020 4120 4465 7669 6365 2063 6f6e      A Device con
+00028770: 7461 696e 696e 6720 616e 206f 7074 696d  taining an optim
+00028780: 616c 6c79 2d72 6f75 6e64 6564 2039 3020  ally-rounded 90 
+00028790: 6465 6772 6565 2062 656e 642e 0a0a 2020  degree bend...  
+000287a0: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
+000287b0: 2d0a 2020 2020 4f70 7469 6d61 6c20 7374  -.    Optimal st
+000287c0: 7275 6374 7572 6520 6672 6f6d 2068 7474  ructure from htt
+000287d0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+000287e0: 3131 3033 2f50 6879 7352 6576 422e 3834  1103/PhysRevB.84
+000287f0: 2e31 3734 3531 300a 2020 2020 436c 656d  .174510.    Clem
+00028800: 2c20 4a2e 2c20 2620 4265 7267 6772 656e  , J., & Berggren
+00028810: 2c20 4b2e 2028 3230 3131 292e 2047 656f  , K. (2011). Geo
+00028820: 6d65 7472 792d 6465 7065 6e64 656e 7420  metry-dependent 
+00028830: 6372 6974 6963 616c 2063 7572 7265 6e74  critical current
+00028840: 7320 696e 0a20 2020 2073 7570 6572 636f  s in.    superco
+00028850: 6e64 7563 7469 6e67 206e 616e 6f63 6972  nducting nanocir
+00028860: 6375 6974 732e 2050 6879 7369 6361 6c20  cuits. Physical 
+00028870: 5265 7669 6577 2042 2c20 3834 2831 3729  Review B, 84(17)
+00028880: 2c20 31e2 8093 3237 2e0a 2020 2020 2222  , 1...27..    ""
+00028890: 220a 2020 2020 4420 3d20 4465 7669 6365  ".    D = Device
+000288a0: 2822 3930 6465 6722 290a 0a20 2020 2023  ("90deg")..    #
+000288b0: 2047 6574 2070 6f69 6e74 7320 6f66 2069   Get points of i
+000288c0: 6465 616c 2063 7572 7665 0a20 2020 2061  deal curve.    a
+000288d0: 203d 2032 202a 2077 6964 7468 0a20 2020   = 2 * width.   
+000288e0: 2076 203d 206e 702e 6c6f 6773 7061 6365   v = np.logspace
+000288f0: 282d 6c65 6e67 7468 5f61 646a 7573 742c  (-length_adjust,
+00028900: 206c 656e 6774 685f 6164 6a75 7374 2c20   length_adjust, 
+00028910: 6e75 6d5f 7074 7329 0a20 2020 2078 6920  num_pts).    xi 
+00028920: 3d20 280a 2020 2020 2020 2020 6120 2f20  = (.        a / 
+00028930: 322e 3020 2a20 2828 3120 2b20 3220 2f20  2.0 * ((1 + 2 / 
+00028940: 7069 202a 206e 702e 6172 6373 696e 6828  pi * np.arcsinh(
+00028950: 3120 2f20 7629 2920 2b20 316a 202a 2028  1 / v)) + 1j * (
+00028960: 3120 2b20 3220 2f20 7069 202a 206e 702e  1 + 2 / pi * np.
+00028970: 6172 6373 696e 6828 7629 2929 0a20 2020  arcsinh(v))).   
+00028980: 2029 0a20 2020 2078 7074 7320 3d20 6c69   ).    xpts = li
+00028990: 7374 286e 702e 7265 616c 2878 6929 290a  st(np.real(xi)).
+000289a0: 2020 2020 7970 7473 203d 206c 6973 7428      ypts = list(
+000289b0: 6e70 2e69 6d61 6728 7869 2929 0a0a 2020  np.imag(xi))..  
+000289c0: 2020 2320 4164 6420 706f 696e 7473 2066    # Add points f
+000289d0: 6f72 2074 6865 2072 6573 7420 6f66 2063  or the rest of c
+000289e0: 7572 7665 0a20 2020 2064 203d 2032 202a  urve.    d = 2 *
+000289f0: 2078 7074 735b 305d 2020 2320 4661 7274   xpts[0]  # Fart
+00028a00: 6865 7374 2070 6f69 6e74 206f 7574 202a  hest point out *
+00028a10: 2032 2c20 726f 756e 6465 6420 746f 206e   2, rounded to n
+00028a20: 6561 7265 7374 2031 3030 0a20 2020 2078  earest 100.    x
+00028a30: 7074 732e 6170 7065 6e64 2877 6964 7468  pts.append(width
+00028a40: 290a 2020 2020 7970 7473 2e61 7070 656e  ).    ypts.appen
+00028a50: 6428 6429 0a20 2020 2078 7074 732e 6170  d(d).    xpts.ap
+00028a60: 7065 6e64 2830 290a 2020 2020 7970 7473  pend(0).    ypts
+00028a70: 2e61 7070 656e 6428 6429 0a20 2020 2078  .append(d).    x
+00028a80: 7074 732e 6170 7065 6e64 2830 290a 2020  pts.append(0).  
+00028a90: 2020 7970 7473 2e61 7070 656e 6428 3029    ypts.append(0)
+00028aa0: 0a20 2020 2078 7074 732e 6170 7065 6e64  .    xpts.append
+00028ab0: 2864 290a 2020 2020 7970 7473 2e61 7070  (d).    ypts.app
+00028ac0: 656e 6428 3029 0a20 2020 2078 7074 732e  end(0).    xpts.
+00028ad0: 6170 7065 6e64 2864 290a 2020 2020 7970  append(d).    yp
+00028ae0: 7473 2e61 7070 656e 6428 7769 6474 6829  ts.append(width)
+00028af0: 0a20 2020 2078 7074 732e 6170 7065 6e64  .    xpts.append
+00028b00: 2878 7074 735b 305d 290a 2020 2020 7970  (xpts[0]).    yp
+00028b10: 7473 2e61 7070 656e 6428 7970 7473 5b30  ts.append(ypts[0
+00028b20: 5d29 0a0a 2020 2020 442e 6164 645f 706f  ])..    D.add_po
+00028b30: 6c79 676f 6e28 5b78 7074 732c 2079 7074  lygon([xpts, ypt
+00028b40: 735d 2c20 6c61 7965 723d 6c61 7965 7229  s], layer=layer)
+00028b50: 0a0a 2020 2020 442e 6164 645f 706f 7274  ..    D.add_port
+00028b60: 286e 616d 653d 312c 206d 6964 706f 696e  (name=1, midpoin
+00028b70: 743d 5b61 202f 2034 2c20 645d 2c20 7769  t=[a / 4, d], wi
+00028b80: 6474 683d 6120 2f20 322c 206f 7269 656e  dth=a / 2, orien
+00028b90: 7461 7469 6f6e 3d39 3029 0a20 2020 2044  tation=90).    D
+00028ba0: 2e61 6464 5f70 6f72 7428 6e61 6d65 3d32  .add_port(name=2
+00028bb0: 2c20 6d69 6470 6f69 6e74 3d5b 642c 2061  , midpoint=[d, a
+00028bc0: 202f 2034 5d2c 2077 6964 7468 3d61 202f   / 4], width=a /
+00028bd0: 2032 2c20 6f72 6965 6e74 6174 696f 6e3d   2, orientation=
+00028be0: 3029 0a20 2020 2072 6574 7572 6e20 440a  0).    return D.
+00028bf0: 0a0a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..# ============
 00028c00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00028c10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028c20: 3d3d 3d0a 0a23 2068 6169 7270 696e 203d  ===..# hairpin =
-00028c30: 206f 7074 696d 616c 5f68 6169 7270 696e   optimal_hairpin
-00028c40: 2877 6964 7468 203d 2031 2c20 7069 7463  (width = 1, pitc
-00028c50: 6820 3d20 332c 206c 656e 6774 6820 3d20  h = 3, length = 
-00028c60: 3330 2c20 6e75 6d5f 7074 7320 3d20 3230  30, num_pts = 20
-00028c70: 290a 2320 7175 6963 6b70 6c6f 7428 6861  ).# quickplot(ha
-00028c80: 6972 7069 6e29 0a0a 0a23 2073 7465 7020  irpin)...# step 
-00028c90: 3d20 6f70 7469 6d61 6c5f 7374 6570 2873  = optimal_step(s
-00028ca0: 7461 7274 5f77 6964 7468 203d 2035 2c20  tart_width = 5, 
-00028cb0: 656e 645f 7769 6474 6820 3d20 312c 206e  end_width = 1, n
-00028cc0: 756d 5f70 7473 203d 2038 302c 2077 6964  um_pts = 80, wid
-00028cd0: 7468 5f74 6f6c 203d 2031 652d 3329 0a23  th_tol = 1e-3).#
-00028ce0: 2071 7569 636b 706c 6f74 2873 7465 7029   quickplot(step)
-00028cf0: 0a0a 0a23 2074 7572 6e20 3d20 6f70 7469  ...# turn = opti
-00028d00: 6d61 6c5f 3930 6465 6728 7769 6474 6820  mal_90deg(width 
-00028d10: 3d20 3930 2c20 6c65 6e67 7468 5f61 646a  = 90, length_adj
-00028d20: 7573 7420 3d20 3129 0a23 2071 7569 636b  ust = 1).# quick
-00028d30: 706c 6f74 2874 7572 6e29 0a0a 0a23 203d  plot(turn)...# =
-00028d40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028d50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028d60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 230a  =============.#.
-00028d90: 2320 5375 7065 7263 6f6e 6475 6374 696e  # Superconductin
-00028da0: 6720 6465 7669 6365 730a 230a 2320 3d3d  g devices.#.# ==
-00028db0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c40: 3d3d 0a23 2045 7861 6d70 6c65 2063 6f64  ==.# Example cod
+00028c50: 650a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e.# ============
+00028c60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028c90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028ca0: 3d3d 0a0a 2320 6861 6972 7069 6e20 3d20  ==..# hairpin = 
+00028cb0: 6f70 7469 6d61 6c5f 6861 6972 7069 6e28  optimal_hairpin(
+00028cc0: 7769 6474 6820 3d20 312c 2070 6974 6368  width = 1, pitch
+00028cd0: 203d 2033 2c20 6c65 6e67 7468 203d 2033   = 3, length = 3
+00028ce0: 302c 206e 756d 5f70 7473 203d 2032 3029  0, num_pts = 20)
+00028cf0: 0a23 2071 7569 636b 706c 6f74 2868 6169  .# quickplot(hai
+00028d00: 7270 696e 290a 0a0a 2320 7374 6570 203d  rpin)...# step =
+00028d10: 206f 7074 696d 616c 5f73 7465 7028 7374   optimal_step(st
+00028d20: 6172 745f 7769 6474 6820 3d20 352c 2065  art_width = 5, e
+00028d30: 6e64 5f77 6964 7468 203d 2031 2c20 6e75  nd_width = 1, nu
+00028d40: 6d5f 7074 7320 3d20 3830 2c20 7769 6474  m_pts = 80, widt
+00028d50: 685f 746f 6c20 3d20 3165 2d33 290a 2320  h_tol = 1e-3).# 
+00028d60: 7175 6963 6b70 6c6f 7428 7374 6570 290a  quickplot(step).
+00028d70: 0a0a 2320 7475 726e 203d 206f 7074 696d  ..# turn = optim
+00028d80: 616c 5f39 3064 6567 2877 6964 7468 203d  al_90deg(width =
+00028d90: 2039 302c 206c 656e 6774 685f 6164 6a75   90, length_adju
+00028da0: 7374 203d 2031 290a 2320 7175 6963 6b70  st = 1).# quickp
+00028db0: 6c6f 7428 7475 726e 290a 0a0a 2320 3d3d  lot(turn)...# ==
 00028dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00028dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00028de0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00028df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 0a40  ============...@
-00028e00: 6465 7669 6365 5f6c 7275 5f63 6163 6865  device_lru_cache
-00028e10: 0a64 6566 2073 6e73 7064 280a 2020 2020  .def snspd(.    
-00028e20: 7769 7265 5f77 6964 7468 3d30 2e32 2c0a  wire_width=0.2,.
-00028e30: 2020 2020 7769 7265 5f70 6974 6368 3d30      wire_pitch=0
-00028e40: 2e36 2c0a 2020 2020 7369 7a65 3d28 3130  .6,.    size=(10
-00028e50: 2c20 3829 2c0a 2020 2020 6e75 6d5f 7371  , 8),.    num_sq
-00028e60: 7561 7265 733d 4e6f 6e65 2c0a 2020 2020  uares=None,.    
-00028e70: 7475 726e 5f72 6174 696f 3d34 2c0a 2020  turn_ratio=4,.  
-00028e80: 2020 7465 726d 696e 616c 735f 7361 6d65    terminals_same
-00028e90: 5f73 6964 653d 4661 6c73 652c 0a20 2020  _side=False,.   
-00028ea0: 206c 6179 6572 3d30 2c0a 293a 0a20 2020   layer=0,.):.   
-00028eb0: 2022 2222 4372 6561 7465 7320 616e 206f   """Creates an o
-00028ec0: 7074 696d 616c 6c79 2d72 6f75 6e64 6564  ptimally-rounded
-00028ed0: 2053 4e53 5044 2e0a 0a20 2020 2050 6172   SNSPD...    Par
-00028ee0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00028ef0: 2d2d 2d2d 2d2d 0a20 2020 2077 6964 7468  ------.    width
-00028f00: 203a 2069 6e74 206f 7220 666c 6f61 740a   : int or float.
-00028f10: 2020 2020 2020 2020 5769 6474 6820 6f66          Width of
-00028f20: 2074 6865 2077 6972 652e 0a20 2020 2070   the wire..    p
-00028f30: 6974 6368 203a 2069 6e74 206f 7220 666c  itch : int or fl
-00028f40: 6f61 740a 2020 2020 2020 2020 4469 7374  oat.        Dist
-00028f50: 616e 6365 2062 6574 7765 656e 2074 776f  ance between two
-00028f60: 2061 646a 6163 656e 7420 7769 7265 732e   adjacent wires.
-00028f70: 204d 7573 7420 6265 2067 7265 6174 6572   Must be greater
-00028f80: 2074 6861 6e20 6077 6964 7468 602e 0a20   than `width`.. 
-00028f90: 2020 2073 697a 6520 3a20 4e6f 6e65 206f     size : None o
-00028fa0: 7220 6172 7261 792d 6c69 6b65 5b32 5d20  r array-like[2] 
-00028fb0: 6f66 2069 6e74 206f 7220 666c 6f61 740a  of int or float.
-00028fc0: 2020 2020 2020 2020 2877 6964 7468 2c20          (width, 
-00028fd0: 6865 6967 6874 2920 6f66 2074 6865 2072  height) of the r
-00028fe0: 6563 7461 6e67 6c65 2066 6f72 6d65 6420  ectangle formed 
-00028ff0: 6279 2074 6865 206f 7574 6572 2062 6f75  by the outer bou
-00029000: 6e64 6172 7920 6f66 2074 6865 0a20 2020  ndary of the.   
-00029010: 2020 2020 2053 4e53 5044 2e20 4d75 7374       SNSPD. Must
-00029020: 2062 6520 6e6f 6e65 2069 6620 606e 756d   be none if `num
-00029030: 5f73 7175 6172 6573 6020 6973 2073 7065  _squares` is spe
-00029040: 6369 6669 6564 2e0a 2020 2020 6e75 6d5f  cified..    num_
-00029050: 7371 7561 7265 7320 3a20 696e 7420 6f72  squares : int or
-00029060: 204e 6f6e 650a 2020 2020 2020 2020 546f   None.        To
-00029070: 7461 6c20 6e75 6d62 6572 206f 6620 7371  tal number of sq
-00029080: 7561 7265 7320 696e 7369 6465 2074 6865  uares inside the
-00029090: 2053 4e53 5044 206c 656e 6774 682e 204d   SNSPD length. M
-000290a0: 7573 7420 6265 206e 6f6e 6520 6966 0a20  ust be none if. 
-000290b0: 2020 2020 2020 2060 7369 7a65 6020 6973         `size` is
-000290c0: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
-000290d0: 7475 726e 5f72 6174 696f 203a 2069 6e74  turn_ratio : int
-000290e0: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
-000290f0: 2020 5370 6563 6966 6965 7320 686f 7720    Specifies how 
-00029100: 6d75 6368 206f 6620 7468 6520 534e 5350  much of the SNSP
-00029110: 4420 7769 6474 6820 6973 2064 6564 6963  D width is dedic
-00029120: 6174 6564 2074 6f20 7468 6520 3138 3020  ated to the 180 
-00029130: 6465 6772 6565 0a20 2020 2020 2020 2074  degree.        t
-00029140: 7572 6e2e 2041 2060 7475 726e 5f72 6174  urn. A `turn_rat
-00029150: 696f 6020 6f66 2031 3020 7769 6c6c 2072  io` of 10 will r
-00029160: 6573 756c 7420 696e 2032 3025 206f 6620  esult in 20% of 
-00029170: 7468 6520 7769 6474 6820 6265 696e 670a  the width being.
-00029180: 2020 2020 2020 2020 636f 6d70 7269 7365          comprise
-00029190: 6420 6f66 2074 6865 2074 7572 6e2e 0a20  d of the turn.. 
-000291a0: 2020 2074 6572 6d69 6e61 6c73 5f73 616d     terminals_sam
-000291b0: 655f 7369 6465 203a 2062 6f6f 6c0a 2020  e_side : bool.  
-000291c0: 2020 2020 2020 4966 2054 7275 652c 2062        If True, b
-000291d0: 6f74 6820 706f 7274 7320 7769 6c6c 2062  oth ports will b
-000291e0: 6520 6c6f 6361 7465 6420 6f6e 2074 6865  e located on the
-000291f0: 2073 616d 6520 7369 6465 206f 6620 7468   same side of th
-00029200: 6520 534e 5350 442e 0a20 2020 206c 6179  e SNSPD..    lay
-00029210: 6572 203a 2069 6e74 2c20 6172 7261 792d  er : int, array-
-00029220: 6c69 6b65 5b32 5d2c 206f 7220 7365 740a  like[2], or set.
-00029230: 2020 2020 2020 2020 5370 6563 6966 6963          Specific
-00029240: 206c 6179 6572 2873 2920 746f 2070 7574   layer(s) to put
-00029250: 2070 6f6c 7967 6f6e 2067 656f 6d65 7472   polygon geometr
-00029260: 7920 6f6e 2e0a 0a20 2020 2052 6574 7572  y on...    Retur
-00029270: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00029280: 2020 2044 203a 2044 6576 6963 650a 2020     D : Device.  
-00029290: 2020 2020 2020 4120 4465 7669 6365 2063        A Device c
-000292a0: 6f6e 7461 696e 696e 6720 616e 206f 7074  ontaining an opt
-000292b0: 696d 616c 6c79 2d72 6f75 6e64 6564 2053  imally-rounded S
-000292c0: 4e53 5044 2e0a 2020 2020 2222 220a 2020  NSPD..    """.  
-000292d0: 2020 2320 436f 6e76 656e 6965 6e63 6520    # Convenience 
-000292e0: 7465 7374 7320 746f 2061 7574 6f2d 7368  tests to auto-sh
-000292f0: 6170 6520 7468 6520 7369 7a65 2062 6173  ape the size bas
-00029300: 6564 0a20 2020 2023 206f 6e20 7468 6520  ed.    # on the 
-00029310: 6e75 6d62 6572 206f 6620 7371 7561 7265  number of square
-00029320: 730a 2020 2020 6966 206e 756d 5f73 7175  s.    if num_squ
-00029330: 6172 6573 2069 7320 6e6f 7420 4e6f 6e65  ares is not None
-00029340: 2061 6e64 2028 0a20 2020 2020 2020 2028   and (.        (
-00029350: 7369 7a65 2069 7320 4e6f 6e65 2920 6f72  size is None) or
-00029360: 2028 2873 697a 655b 305d 2069 7320 4e6f   ((size[0] is No
-00029370: 6e65 2920 616e 6420 2873 697a 655b 315d  ne) and (size[1]
-00029380: 2920 6973 204e 6f6e 6529 0a20 2020 2029  ) is None).    )
-00029390: 3a0a 2020 2020 2020 2020 7879 203d 206e  :.        xy = n
-000293a0: 702e 7371 7274 286e 756d 5f73 7175 6172  p.sqrt(num_squar
-000293b0: 6573 202a 2077 6972 655f 7069 7463 6820  es * wire_pitch 
-000293c0: 2a20 7769 7265 5f77 6964 7468 290a 2020  * wire_width).  
-000293d0: 2020 2020 2020 7369 7a65 203d 205b 7879        size = [xy
-000293e0: 2c20 7879 5d0a 2020 2020 2020 2020 6e75  , xy].        nu
-000293f0: 6d5f 7371 7561 7265 7320 3d20 4e6f 6e65  m_squares = None
-00029400: 0a20 2020 2069 6620 5b73 697a 655b 305d  .    if [size[0]
-00029410: 2c20 7369 7a65 5b31 5d2c 206e 756d 5f73  , size[1], num_s
-00029420: 7175 6172 6573 5d2e 636f 756e 7428 4e6f  quares].count(No
-00029430: 6e65 2920 213d 2031 3a0a 2020 2020 2020  ne) != 1:.      
-00029440: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00029450: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00029460: 225b 5048 4944 4c5d 2073 6e73 7064 2829  "[PHIDL] snspd()
-00029470: 2072 6571 7569 7265 7320 7468 6174 2065   requires that e
-00029480: 7861 6374 6c79 204f 4e45 2076 616c 7565  xactly ONE value
-00029490: 206f 6620 220a 2020 2020 2020 2020 2020   of ".          
-000294a0: 2020 2274 6865 2061 7267 756d 656e 7473    "the arguments
-000294b0: 2060 606e 756d 5f73 7175 6172 6573 6060   ``num_squares``
-000294c0: 2061 6e64 2060 6073 697a 6560 6020 6265   and ``size`` be
-000294d0: 204e 6f6e 6520 220a 2020 2020 2020 2020   None ".        
-000294e0: 2020 2020 2274 6f20 7072 6576 656e 7420      "to prevent 
-000294f0: 6f76 6572 636f 6e73 7472 6169 6e69 6e67  overconstraining
-00029500: 2c20 666f 7220 6578 616d 706c 653a 5c6e  , for example:\n
-00029510: 220a 2020 2020 2020 2020 2020 2020 223e  ".            ">
-00029520: 3e3e 2073 6e73 7064 2873 697a 6520 3d20  >> snspd(size = 
-00029530: 2833 2c20 4e6f 6e65 292c 206e 756d 5f73  (3, None), num_s
-00029540: 7175 6172 6573 203d 2032 3030 3029 220a  quares = 2000)".
-00029550: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
-00029560: 2073 697a 655b 305d 2069 7320 4e6f 6e65   size[0] is None
-00029570: 3a0a 2020 2020 2020 2020 7973 697a 6520  :.        ysize 
-00029580: 3d20 7369 7a65 5b31 5d0a 2020 2020 2020  = size[1].      
-00029590: 2020 7873 697a 6520 3d20 6e75 6d5f 7371    xsize = num_sq
-000295a0: 7561 7265 7320 2a20 7769 7265 5f70 6974  uares * wire_pit
-000295b0: 6368 202a 2077 6972 655f 7769 6474 6820  ch * wire_width 
-000295c0: 2f20 7973 697a 650a 2020 2020 656c 6966  / ysize.    elif
-000295d0: 2073 697a 655b 315d 2069 7320 4e6f 6e65   size[1] is None
-000295e0: 3a0a 2020 2020 2020 2020 7873 697a 6520  :.        xsize 
-000295f0: 3d20 7369 7a65 5b30 5d0a 2020 2020 2020  = size[0].      
-00029600: 2020 7973 697a 6520 3d20 6e75 6d5f 7371    ysize = num_sq
-00029610: 7561 7265 7320 2a20 7769 7265 5f70 6974  uares * wire_pit
-00029620: 6368 202a 2077 6972 655f 7769 6474 6820  ch * wire_width 
-00029630: 2f20 7873 697a 650a 2020 2020 656c 7365  / xsize.    else
-00029640: 3a0a 2020 2020 2020 2020 7873 697a 6520  :.        xsize 
-00029650: 3d20 7369 7a65 5b30 5d0a 2020 2020 2020  = size[0].      
-00029660: 2020 7973 697a 6520 3d20 7369 7a65 5b31    ysize = size[1
-00029670: 5d0a 0a20 2020 206e 756d 5f6d 6561 6e64  ]..    num_meand
-00029680: 6572 7320 3d20 696e 7428 6e70 2e63 6569  ers = int(np.cei
-00029690: 6c28 7973 697a 6520 2f20 7769 7265 5f70  l(ysize / wire_p
-000296a0: 6974 6368 2929 0a0a 2020 2020 4420 3d20  itch))..    D = 
-000296b0: 4465 7669 6365 286e 616d 653d 2273 6e73  Device(name="sns
-000296c0: 7064 2229 0a20 2020 2068 6169 7270 696e  pd").    hairpin
-000296d0: 203d 206f 7074 696d 616c 5f68 6169 7270   = optimal_hairp
-000296e0: 696e 280a 2020 2020 2020 2020 7769 6474  in(.        widt
-000296f0: 683d 7769 7265 5f77 6964 7468 2c0a 2020  h=wire_width,.  
-00029700: 2020 2020 2020 7069 7463 683d 7769 7265        pitch=wire
-00029710: 5f70 6974 6368 2c0a 2020 2020 2020 2020  _pitch,.        
-00029720: 7475 726e 5f72 6174 696f 3d74 7572 6e5f  turn_ratio=turn_
-00029730: 7261 7469 6f2c 0a20 2020 2020 2020 206c  ratio,.        l
-00029740: 656e 6774 683d 7873 697a 6520 2f20 322c  ength=xsize / 2,
-00029750: 0a20 2020 2020 2020 206e 756d 5f70 7473  .        num_pts
-00029760: 3d32 302c 0a20 2020 2020 2020 206c 6179  =20,.        lay
-00029770: 6572 3d6c 6179 6572 2c0a 2020 2020 290a  er=layer,.    ).
-00029780: 0a20 2020 2069 6620 2874 6572 6d69 6e61  .    if (termina
-00029790: 6c73 5f73 616d 655f 7369 6465 2069 7320  ls_same_side is 
-000297a0: 4661 6c73 6529 2061 6e64 2028 286e 756d  False) and ((num
-000297b0: 5f6d 6561 6e64 6572 7320 2520 3229 203d  _meanders % 2) =
-000297c0: 3d20 3029 3a0a 2020 2020 2020 2020 6e75  = 0):.        nu
-000297d0: 6d5f 6d65 616e 6465 7273 202b 3d20 310a  m_meanders += 1.
-000297e0: 2020 2020 656c 6966 2028 7465 726d 696e      elif (termin
-000297f0: 616c 735f 7361 6d65 5f73 6964 6520 6973  als_same_side is
-00029800: 2054 7275 6529 2061 6e64 2028 286e 756d   True) and ((num
-00029810: 5f6d 6561 6e64 6572 7320 2520 3229 203d  _meanders % 2) =
-00029820: 3d20 3129 3a0a 2020 2020 2020 2020 6e75  = 1):.        nu
-00029830: 6d5f 6d65 616e 6465 7273 202b 3d20 310a  m_meanders += 1.
-00029840: 0a20 2020 2073 7461 7274 5f6e 7720 3d20  .    start_nw = 
-00029850: 442e 6164 645f 7265 6628 636f 6d70 6173  D.add_ref(compas
-00029860: 7328 7369 7a65 3d5b 7873 697a 6520 2f20  s(size=[xsize / 
-00029870: 322c 2077 6972 655f 7769 6474 685d 2c20  2, wire_width], 
-00029880: 6c61 7965 723d 6c61 7965 7229 290a 0a20  layer=layer)).. 
-00029890: 2020 2068 705f 7072 6576 203d 2044 2e61     hp_prev = D.a
-000298a0: 6464 5f72 6566 2868 6169 7270 696e 290a  dd_ref(hairpin).
-000298b0: 2020 2020 6870 5f70 7265 762e 636f 6e6e      hp_prev.conn
-000298c0: 6563 7428 312c 2073 7461 7274 5f6e 772e  ect(1, start_nw.
-000298d0: 706f 7274 735b 2245 225d 290a 2020 2020  ports["E"]).    
-000298e0: 616c 7465 726e 6174 6520 3d20 5472 7565  alternate = True
-000298f0: 0a20 2020 2066 6f72 206e 2069 6e20 7261  .    for n in ra
-00029900: 6e67 6528 322c 206e 756d 5f6d 6561 6e64  nge(2, num_meand
-00029910: 6572 7329 3a0a 2020 2020 2020 2020 6870  ers):.        hp
-00029920: 203d 2044 2e61 6464 5f72 6566 2868 6169   = D.add_ref(hai
-00029930: 7270 696e 290a 2020 2020 2020 2020 6966  rpin).        if
-00029940: 2061 6c74 6572 6e61 7465 3a0a 2020 2020   alternate:.    
-00029950: 2020 2020 2020 2020 6870 2e63 6f6e 6e65          hp.conne
-00029960: 6374 2832 2c20 6870 5f70 7265 762e 706f  ct(2, hp_prev.po
-00029970: 7274 735b 325d 290a 2020 2020 2020 2020  rts[2]).        
-00029980: 2020 2020 6c61 7374 5f70 6f72 7420 3d20      last_port = 
-00029990: 6870 2e70 6f72 7473 5b31 5d0a 2020 2020  hp.ports[1].    
-000299a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000299b0: 2020 2020 2020 6870 2e63 6f6e 6e65 6374        hp.connect
-000299c0: 2831 2c20 6870 5f70 7265 762e 706f 7274  (1, hp_prev.port
-000299d0: 735b 315d 290a 2020 2020 2020 2020 2020  s[1]).          
-000299e0: 2020 6c61 7374 5f70 6f72 7420 3d20 6870    last_port = hp
-000299f0: 2e70 6f72 7473 5b32 5d0a 2020 2020 2020  .ports[2].      
-00029a00: 2020 6870 5f70 7265 7620 3d20 6870 0a20    hp_prev = hp. 
-00029a10: 2020 2020 2020 2061 6c74 6572 6e61 7465         alternate
-00029a20: 203d 206e 6f74 2061 6c74 6572 6e61 7465   = not alternate
-00029a30: 0a0a 2020 2020 6669 6e69 7368 5f73 6520  ..    finish_se 
-00029a40: 3d20 442e 6164 645f 7265 6628 636f 6d70  = D.add_ref(comp
-00029a50: 6173 7328 7369 7a65 3d5b 7873 697a 6520  ass(size=[xsize 
-00029a60: 2f20 322c 2077 6972 655f 7769 6474 685d  / 2, wire_width]
-00029a70: 2c20 6c61 7965 723d 6c61 7965 7229 290a  , layer=layer)).
-00029a80: 2020 2020 6669 6e69 7368 5f73 652e 636f      finish_se.co
-00029a90: 6e6e 6563 7428 2245 222c 206c 6173 745f  nnect("E", last_
-00029aa0: 706f 7274 290a 0a20 2020 2044 2e61 6464  port)..    D.add
-00029ab0: 5f70 6f72 7428 706f 7274 3d73 7461 7274  _port(port=start
-00029ac0: 5f6e 772e 706f 7274 735b 2257 225d 2c20  _nw.ports["W"], 
-00029ad0: 6e61 6d65 3d31 290a 2020 2020 442e 6164  name=1).    D.ad
-00029ae0: 645f 706f 7274 2870 6f72 743d 6669 6e69  d_port(port=fini
-00029af0: 7368 5f73 652e 706f 7274 735b 2257 225d  sh_se.ports["W"]
-00029b00: 2c20 6e61 6d65 3d32 290a 0a20 2020 2044  , name=2)..    D
-00029b10: 2e69 6e66 6f5b 226e 756d 5f73 7175 6172  .info["num_squar
-00029b20: 6573 225d 203d 206e 756d 5f6d 6561 6e64  es"] = num_meand
-00029b30: 6572 7320 2a20 2878 7369 7a65 202f 2077  ers * (xsize / w
-00029b40: 6972 655f 7769 6474 6829 0a20 2020 2044  ire_width).    D
-00029b50: 2e69 6e66 6f5b 2261 7265 6122 5d20 3d20  .info["area"] = 
-00029b60: 7873 697a 6520 2a20 7973 697a 650a 2020  xsize * ysize.  
-00029b70: 2020 442e 696e 666f 5b22 7369 7a65 225d    D.info["size"]
-00029b80: 203d 2028 7873 697a 652c 2079 7369 7a65   = (xsize, ysize
-00029b90: 290a 0a20 2020 2072 6574 7572 6e20 440a  )..    return D.
-00029ba0: 0a0a 6465 6620 736e 7370 645f 6578 7061  ..def snspd_expa
-00029bb0: 6e64 6564 280a 2020 2020 7769 7265 5f77  nded(.    wire_w
-00029bc0: 6964 7468 3d30 2e32 2c0a 2020 2020 7769  idth=0.2,.    wi
-00029bd0: 7265 5f70 6974 6368 3d30 2e36 2c0a 2020  re_pitch=0.6,.  
-00029be0: 2020 7369 7a65 3d28 3130 2c20 3829 2c0a    size=(10, 8),.
-00029bf0: 2020 2020 6e75 6d5f 7371 7561 7265 733d      num_squares=
-00029c00: 4e6f 6e65 2c0a 2020 2020 636f 6e6e 6563  None,.    connec
-00029c10: 746f 725f 7769 6474 683d 312c 0a20 2020  tor_width=1,.   
-00029c20: 2063 6f6e 6e65 6374 6f72 5f73 796d 6d65   connector_symme
-00029c30: 7472 6963 3d46 616c 7365 2c0a 2020 2020  tric=False,.    
-00029c40: 7475 726e 5f72 6174 696f 3d34 2c0a 2020  turn_ratio=4,.  
-00029c50: 2020 7465 726d 696e 616c 735f 7361 6d65    terminals_same
-00029c60: 5f73 6964 653d 4661 6c73 652c 0a20 2020  _side=False,.   
-00029c70: 206c 6179 6572 3d30 2c0a 293a 0a20 2020   layer=0,.):.   
-00029c80: 2022 2222 4372 6561 7465 7320 616e 206f   """Creates an o
-00029c90: 7074 696d 616c 6c79 2d72 6f75 6e64 6564  ptimally-rounded
-00029ca0: 2053 4e53 5044 2077 6974 6820 7769 7265   SNSPD with wire
-00029cb0: 7320 636f 6d69 6e67 206f 7574 206f 6620  s coming out of 
-00029cc0: 6974 2074 6861 740a 2020 2020 6578 7061  it that.    expa
-00029cd0: 6e64 2e0a 0a20 2020 2050 6172 616d 6574  nd...    Paramet
-00029ce0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00029cf0: 2d2d 0a20 2020 2077 6964 7468 203a 2069  --.    width : i
-00029d00: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
-00029d10: 2020 2020 5769 6474 6820 6f66 2074 6865      Width of the
-00029d20: 2077 6972 652e 0a20 2020 2070 6974 6368   wire..    pitch
-00029d30: 203a 2069 6e74 206f 7220 666c 6f61 740a   : int or float.
-00029d40: 2020 2020 2020 2020 4469 7374 616e 6365          Distance
-00029d50: 2062 6574 7765 656e 2074 776f 2061 646a   between two adj
-00029d60: 6163 656e 7420 7769 7265 732e 204d 7573  acent wires. Mus
-00029d70: 7420 6265 2067 7265 6174 6572 2074 6861  t be greater tha
-00029d80: 6e20 6077 6964 7468 602e 0a20 2020 2073  n `width`..    s
-00029d90: 697a 6520 3a20 4e6f 6e65 206f 7220 6172  ize : None or ar
-00029da0: 7261 792d 6c69 6b65 5b32 5d20 6f66 2069  ray-like[2] of i
-00029db0: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
-00029dc0: 2020 2020 2877 6964 7468 2c20 6865 6967      (width, heig
-00029dd0: 6874 2920 6f66 2074 6865 2072 6563 7461  ht) of the recta
-00029de0: 6e67 6c65 2066 6f72 6d65 6420 6279 2074  ngle formed by t
-00029df0: 6865 206f 7574 6572 2062 6f75 6e64 6172  he outer boundar
-00029e00: 7920 6f66 2074 6865 0a20 2020 2020 2020  y of the.       
-00029e10: 2053 4e53 5044 2e20 4d75 7374 2062 6520   SNSPD. Must be 
-00029e20: 6e6f 6e65 2069 6620 606e 756d 5f73 7175  none if `num_squ
-00029e30: 6172 6573 6020 6973 2073 7065 6369 6669  ares` is specifi
-00029e40: 6564 2e0a 2020 2020 6e75 6d5f 7371 7561  ed..    num_squa
-00029e50: 7265 7320 3a20 696e 7420 6f72 204e 6f6e  res : int or Non
-00029e60: 650a 2020 2020 2020 2020 546f 7461 6c20  e.        Total 
-00029e70: 6e75 6d62 6572 206f 6620 7371 7561 7265  number of square
-00029e80: 7320 696e 7369 6465 2074 6865 2053 4e53  s inside the SNS
-00029e90: 5044 206c 656e 6774 682e 204d 7573 7420  PD length. Must 
-00029ea0: 6265 206e 6f6e 6520 6966 0a20 2020 2020  be none if.     
-00029eb0: 2020 2060 7369 7a65 6020 6973 2073 7065     `size` is spe
-00029ec0: 6369 6669 6564 2e0a 2020 2020 636f 6e6e  cified..    conn
-00029ed0: 6563 746f 725f 7769 6474 6820 3a20 696e  ector_width : in
-00029ee0: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-00029ef0: 2020 2057 6964 7468 206f 6620 7468 6520     Width of the 
-00029f00: 636f 6e6e 6563 746f 7273 2e0a 2020 2020  connectors..    
-00029f10: 636f 6e6e 6563 746f 725f 7379 6d6d 6574  connector_symmet
-00029f20: 7269 6320 3a20 626f 6f6c 0a20 2020 2020  ric : bool.     
-00029f30: 2020 2049 6620 5472 7565 2c20 6d69 7272     If True, mirr
-00029f40: 6f72 7320 7468 6520 636f 6e6e 6563 746f  ors the connecto
-00029f50: 7273 2061 6372 6f73 7320 7468 6569 7220  rs across their 
-00029f60: 666c 6174 2065 6467 6520 616e 6420 6164  flat edge and ad
-00029f70: 6473 2074 6865 6d0a 2020 2020 2020 2020  ds them.        
-00029f80: 746f 2074 6865 2063 6f6e 6e65 6374 6f72  to the connector
-00029f90: 2067 656f 6d65 7472 792e 0a20 2020 2074   geometry..    t
-00029fa0: 7572 6e5f 7261 7469 6f20 3a20 696e 7420  urn_ratio : int 
-00029fb0: 6f72 2066 6c6f 6174 0a20 2020 2020 2020  or float.       
-00029fc0: 2053 7065 6369 6669 6573 2068 6f77 206d   Specifies how m
-00029fd0: 7563 6820 6f66 2074 6865 2053 4e53 5044  uch of the SNSPD
-00029fe0: 2077 6964 7468 2069 7320 6465 6469 6361   width is dedica
-00029ff0: 7465 6420 746f 2074 6865 2031 3830 2064  ted to the 180 d
-0002a000: 6567 7265 650a 2020 2020 2020 2020 7475  egree.        tu
-0002a010: 726e 2e20 4120 6074 7572 6e5f 7261 7469  rn. A `turn_rati
-0002a020: 6f60 206f 6620 3130 2077 696c 6c20 7265  o` of 10 will re
-0002a030: 7375 6c74 2069 6e20 3230 2520 6f66 2074  sult in 20% of t
-0002a040: 6865 2077 6964 7468 2062 6569 6e67 0a20  he width being. 
-0002a050: 2020 2020 2020 2063 6f6d 7072 6973 6564         comprised
-0002a060: 206f 6620 7468 6520 7475 726e 2e0a 2020   of the turn..  
-0002a070: 2020 7465 726d 696e 616c 735f 7361 6d65    terminals_same
-0002a080: 5f73 6964 6520 3a20 626f 6f6c 0a20 2020  _side : bool.   
-0002a090: 2020 2020 2049 6620 5472 7565 2c20 626f       If True, bo
-0002a0a0: 7468 2070 6f72 7473 2077 696c 6c20 6265  th ports will be
-0002a0b0: 206c 6f63 6174 6564 206f 6e20 7468 6520   located on the 
-0002a0c0: 7361 6d65 2073 6964 6520 6f66 2074 6865  same side of the
-0002a0d0: 2053 4e53 5044 2e0a 2020 2020 6c61 7965   SNSPD..    laye
-0002a0e0: 7220 3a20 696e 742c 2061 7272 6179 2d6c  r : int, array-l
-0002a0f0: 696b 655b 325d 2c20 6f72 2073 6574 0a20  ike[2], or set. 
-0002a100: 2020 2020 2020 2053 7065 6369 6669 6320         Specific 
-0002a110: 6c61 7965 7228 7329 2074 6f20 7075 7420  layer(s) to put 
-0002a120: 706f 6c79 676f 6e20 6765 6f6d 6574 7279  polygon geometry
-0002a130: 206f 6e2e 0a0a 2020 2020 5265 7475 726e   on...    Return
-0002a140: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-0002a150: 2020 4420 3a20 4465 7669 6365 0a20 2020    D : Device.   
-0002a160: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
-0002a170: 6e74 6169 6e69 6e67 2061 6e20 6f70 7469  ntaining an opti
-0002a180: 6d61 6c6c 792d 726f 756e 6465 6420 534e  mally-rounded SN
-0002a190: 5350 4420 7769 7468 2065 7870 616e 6469  SPD with expandi
-0002a1a0: 6e67 2069 6e70 7574 2f0a 2020 2020 2020  ng input/.      
-0002a1b0: 2020 6f75 7470 7574 2077 6972 6573 2e0a    output wires..
-0002a1c0: 2020 2020 2222 220a 2020 2020 4420 3d20      """.    D = 
-0002a1d0: 4465 7669 6365 2822 736e 7370 645f 6578  Device("snspd_ex
-0002a1e0: 7061 6e64 6564 2229 0a20 2020 2053 203d  panded").    S =
-0002a1f0: 2073 6e73 7064 280a 2020 2020 2020 2020   snspd(.        
-0002a200: 7769 7265 5f77 6964 7468 3d77 6972 655f  wire_width=wire_
-0002a210: 7769 6474 682c 0a20 2020 2020 2020 2077  width,.        w
-0002a220: 6972 655f 7069 7463 683d 7769 7265 5f70  ire_pitch=wire_p
-0002a230: 6974 6368 2c0a 2020 2020 2020 2020 7369  itch,.        si
-0002a240: 7a65 3d73 697a 652c 0a20 2020 2020 2020  ze=size,.       
-0002a250: 206e 756d 5f73 7175 6172 6573 3d6e 756d   num_squares=num
-0002a260: 5f73 7175 6172 6573 2c0a 2020 2020 2020  _squares,.      
-0002a270: 2020 7475 726e 5f72 6174 696f 3d74 7572    turn_ratio=tur
-0002a280: 6e5f 7261 7469 6f2c 0a20 2020 2020 2020  n_ratio,.       
-0002a290: 2074 6572 6d69 6e61 6c73 5f73 616d 655f   terminals_same_
-0002a2a0: 7369 6465 3d74 6572 6d69 6e61 6c73 5f73  side=terminals_s
-0002a2b0: 616d 655f 7369 6465 2c0a 2020 2020 2020  ame_side,.      
-0002a2c0: 2020 6c61 7965 723d 6c61 7965 722c 0a20    layer=layer,. 
-0002a2d0: 2020 2029 0a20 2020 2073 203d 2044 2e61     ).    s = D.a
-0002a2e0: 6464 5f72 6566 2853 290a 2020 2020 7374  dd_ref(S).    st
-0002a2f0: 6570 5f64 6576 6963 6520 3d20 6f70 7469  ep_device = opti
-0002a300: 6d61 6c5f 7374 6570 280a 2020 2020 2020  mal_step(.      
-0002a310: 2020 7374 6172 745f 7769 6474 683d 7769    start_width=wi
-0002a320: 7265 5f77 6964 7468 2c0a 2020 2020 2020  re_width,.      
-0002a330: 2020 656e 645f 7769 6474 683d 636f 6e6e    end_width=conn
-0002a340: 6563 746f 725f 7769 6474 682c 0a20 2020  ector_width,.   
-0002a350: 2020 2020 206e 756d 5f70 7473 3d31 3030       num_pts=100
-0002a360: 2c0a 2020 2020 2020 2020 616e 7469 6372  ,.        anticr
-0002a370: 6f77 6469 6e67 5f66 6163 746f 723d 322c  owding_factor=2,
-0002a380: 0a20 2020 2020 2020 2077 6964 7468 5f74  .        width_t
-0002a390: 6f6c 3d31 652d 332c 0a20 2020 2020 2020  ol=1e-3,.       
-0002a3a0: 2073 796d 6d65 7472 6963 3d63 6f6e 6e65   symmetric=conne
-0002a3b0: 6374 6f72 5f73 796d 6d65 7472 6963 2c0a  ctor_symmetric,.
-0002a3c0: 2020 2020 2020 2020 6c61 7965 723d 6c61          layer=la
-0002a3d0: 7965 722c 0a20 2020 2029 0a20 2020 2073  yer,.    ).    s
-0002a3e0: 7465 7031 203d 2044 2e61 6464 5f72 6566  tep1 = D.add_ref
-0002a3f0: 2873 7465 705f 6465 7669 6365 290a 2020  (step_device).  
-0002a400: 2020 7374 6570 3220 3d20 442e 6164 645f    step2 = D.add_
-0002a410: 7265 6628 7374 6570 5f64 6576 6963 6529  ref(step_device)
-0002a420: 0a20 2020 2073 7465 7031 2e63 6f6e 6e65  .    step1.conne
-0002a430: 6374 2870 6f72 743d 312c 2064 6573 7469  ct(port=1, desti
-0002a440: 6e61 7469 6f6e 3d73 2e70 6f72 7473 5b31  nation=s.ports[1
-0002a450: 5d29 0a20 2020 2073 7465 7032 2e63 6f6e  ]).    step2.con
-0002a460: 6e65 6374 2870 6f72 743d 312c 2064 6573  nect(port=1, des
-0002a470: 7469 6e61 7469 6f6e 3d73 2e70 6f72 7473  tination=s.ports
-0002a480: 5b32 5d29 0a20 2020 2044 2e61 6464 5f70  [2]).    D.add_p
-0002a490: 6f72 7428 6e61 6d65 3d31 2c20 706f 7274  ort(name=1, port
-0002a4a0: 3d73 7465 7031 2e70 6f72 7473 5b32 5d29  =step1.ports[2])
-0002a4b0: 0a20 2020 2044 2e61 6464 5f70 6f72 7428  .    D.add_port(
-0002a4c0: 6e61 6d65 3d32 2c20 706f 7274 3d73 7465  name=2, port=ste
-0002a4d0: 7032 2e70 6f72 7473 5b32 5d29 0a0a 2020  p2.ports[2])..  
-0002a4e0: 2020 442e 696e 666f 203d 2053 2e69 6e66    D.info = S.inf
-0002a4f0: 6f0a 2020 2020 532e 696e 666f 203d 207b  o.    S.info = {
-0002a500: 7d0a 0a20 2020 2072 6574 7572 6e20 440a  }..    return D.
-0002a510: 0a0a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..# ============
-0002a520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a560: 3d3d 0a23 2045 7861 6d70 6c65 2063 6f64  ==.# Example cod
-0002a570: 650a 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  e.# ============
-0002a580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028e00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 0a23  ============.#.#
+00028e10: 2053 7570 6572 636f 6e64 7563 7469 6e67   Superconducting
+00028e20: 2064 6576 6963 6573 0a23 0a23 203d 3d3d   devices.#.# ===
+00028e30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028e60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00028e70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a0a 4064  ===========...@d
+00028e80: 6576 6963 655f 6c72 755f 6361 6368 650a  evice_lru_cache.
+00028e90: 6465 6620 736e 7370 6428 0a20 2020 2077  def snspd(.    w
+00028ea0: 6972 655f 7769 6474 683d 302e 322c 0a20  ire_width=0.2,. 
+00028eb0: 2020 2077 6972 655f 7069 7463 683d 302e     wire_pitch=0.
+00028ec0: 362c 0a20 2020 2073 697a 653d 2831 302c  6,.    size=(10,
+00028ed0: 2038 292c 0a20 2020 206e 756d 5f73 7175   8),.    num_squ
+00028ee0: 6172 6573 3d4e 6f6e 652c 0a20 2020 2074  ares=None,.    t
+00028ef0: 7572 6e5f 7261 7469 6f3d 342c 0a20 2020  urn_ratio=4,.   
+00028f00: 2074 6572 6d69 6e61 6c73 5f73 616d 655f   terminals_same_
+00028f10: 7369 6465 3d46 616c 7365 2c0a 2020 2020  side=False,.    
+00028f20: 6c61 7965 723d 302c 0a29 3a0a 2020 2020  layer=0,.):.    
+00028f30: 2222 2243 7265 6174 6573 2061 6e20 6f70  """Creates an op
+00028f40: 7469 6d61 6c6c 792d 726f 756e 6465 6420  timally-rounded 
+00028f50: 534e 5350 442e 0a0a 2020 2020 5061 7261  SNSPD...    Para
+00028f60: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00028f70: 2d2d 2d2d 2d0a 2020 2020 7769 6474 6820  -----.    width 
+00028f80: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
+00028f90: 2020 2020 2020 2057 6964 7468 206f 6620         Width of 
+00028fa0: 7468 6520 7769 7265 2e0a 2020 2020 7069  the wire..    pi
+00028fb0: 7463 6820 3a20 696e 7420 6f72 2066 6c6f  tch : int or flo
+00028fc0: 6174 0a20 2020 2020 2020 2044 6973 7461  at.        Dista
+00028fd0: 6e63 6520 6265 7477 6565 6e20 7477 6f20  nce between two 
+00028fe0: 6164 6a61 6365 6e74 2077 6972 6573 2e20  adjacent wires. 
+00028ff0: 4d75 7374 2062 6520 6772 6561 7465 7220  Must be greater 
+00029000: 7468 616e 2060 7769 6474 6860 2e0a 2020  than `width`..  
+00029010: 2020 7369 7a65 203a 204e 6f6e 6520 6f72    size : None or
+00029020: 2061 7272 6179 2d6c 696b 655b 325d 206f   array-like[2] o
+00029030: 6620 696e 7420 6f72 2066 6c6f 6174 0a20  f int or float. 
+00029040: 2020 2020 2020 2028 7769 6474 682c 2068         (width, h
+00029050: 6569 6768 7429 206f 6620 7468 6520 7265  eight) of the re
+00029060: 6374 616e 676c 6520 666f 726d 6564 2062  ctangle formed b
+00029070: 7920 7468 6520 6f75 7465 7220 626f 756e  y the outer boun
+00029080: 6461 7279 206f 6620 7468 650a 2020 2020  dary of the.    
+00029090: 2020 2020 534e 5350 442e 204d 7573 7420      SNSPD. Must 
+000290a0: 6265 206e 6f6e 6520 6966 2060 6e75 6d5f  be none if `num_
+000290b0: 7371 7561 7265 7360 2069 7320 7370 6563  squares` is spec
+000290c0: 6966 6965 642e 0a20 2020 206e 756d 5f73  ified..    num_s
+000290d0: 7175 6172 6573 203a 2069 6e74 206f 7220  quares : int or 
+000290e0: 4e6f 6e65 0a20 2020 2020 2020 2054 6f74  None.        Tot
+000290f0: 616c 206e 756d 6265 7220 6f66 2073 7175  al number of squ
+00029100: 6172 6573 2069 6e73 6964 6520 7468 6520  ares inside the 
+00029110: 534e 5350 4420 6c65 6e67 7468 2e20 4d75  SNSPD length. Mu
+00029120: 7374 2062 6520 6e6f 6e65 2069 660a 2020  st be none if.  
+00029130: 2020 2020 2020 6073 697a 6560 2069 7320        `size` is 
+00029140: 7370 6563 6966 6965 642e 0a20 2020 2074  specified..    t
+00029150: 7572 6e5f 7261 7469 6f20 3a20 696e 7420  urn_ratio : int 
+00029160: 6f72 2066 6c6f 6174 0a20 2020 2020 2020  or float.       
+00029170: 2053 7065 6369 6669 6573 2068 6f77 206d   Specifies how m
+00029180: 7563 6820 6f66 2074 6865 2053 4e53 5044  uch of the SNSPD
+00029190: 2077 6964 7468 2069 7320 6465 6469 6361   width is dedica
+000291a0: 7465 6420 746f 2074 6865 2031 3830 2064  ted to the 180 d
+000291b0: 6567 7265 650a 2020 2020 2020 2020 7475  egree.        tu
+000291c0: 726e 2e20 4120 6074 7572 6e5f 7261 7469  rn. A `turn_rati
+000291d0: 6f60 206f 6620 3130 2077 696c 6c20 7265  o` of 10 will re
+000291e0: 7375 6c74 2069 6e20 3230 2520 6f66 2074  sult in 20% of t
+000291f0: 6865 2077 6964 7468 2062 6569 6e67 0a20  he width being. 
+00029200: 2020 2020 2020 2063 6f6d 7072 6973 6564         comprised
+00029210: 206f 6620 7468 6520 7475 726e 2e0a 2020   of the turn..  
+00029220: 2020 7465 726d 696e 616c 735f 7361 6d65    terminals_same
+00029230: 5f73 6964 6520 3a20 626f 6f6c 0a20 2020  _side : bool.   
+00029240: 2020 2020 2049 6620 5472 7565 2c20 626f       If True, bo
+00029250: 7468 2070 6f72 7473 2077 696c 6c20 6265  th ports will be
+00029260: 206c 6f63 6174 6564 206f 6e20 7468 6520   located on the 
+00029270: 7361 6d65 2073 6964 6520 6f66 2074 6865  same side of the
+00029280: 2053 4e53 5044 2e0a 2020 2020 6c61 7965   SNSPD..    laye
+00029290: 7220 3a20 696e 742c 2061 7272 6179 2d6c  r : int, array-l
+000292a0: 696b 655b 325d 2c20 6f72 2073 6574 0a20  ike[2], or set. 
+000292b0: 2020 2020 2020 2053 7065 6369 6669 6320         Specific 
+000292c0: 6c61 7965 7228 7329 2074 6f20 7075 7420  layer(s) to put 
+000292d0: 706f 6c79 676f 6e20 6765 6f6d 6574 7279  polygon geometry
+000292e0: 206f 6e2e 0a0a 2020 2020 5265 7475 726e   on...    Return
+000292f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00029300: 2020 4420 3a20 4465 7669 6365 0a20 2020    D : Device.   
+00029310: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
+00029320: 6e74 6169 6e69 6e67 2061 6e20 6f70 7469  ntaining an opti
+00029330: 6d61 6c6c 792d 726f 756e 6465 6420 534e  mally-rounded SN
+00029340: 5350 442e 0a20 2020 2022 2222 0a20 2020  SPD..    """.   
+00029350: 2023 2043 6f6e 7665 6e69 656e 6365 2074   # Convenience t
+00029360: 6573 7473 2074 6f20 6175 746f 2d73 6861  ests to auto-sha
+00029370: 7065 2074 6865 2073 697a 6520 6261 7365  pe the size base
+00029380: 640a 2020 2020 2320 6f6e 2074 6865 206e  d.    # on the n
+00029390: 756d 6265 7220 6f66 2073 7175 6172 6573  umber of squares
+000293a0: 0a20 2020 2069 6620 6e75 6d5f 7371 7561  .    if num_squa
+000293b0: 7265 7320 6973 206e 6f74 204e 6f6e 6520  res is not None 
+000293c0: 616e 6420 280a 2020 2020 2020 2020 2873  and (.        (s
+000293d0: 697a 6520 6973 204e 6f6e 6529 206f 7220  ize is None) or 
+000293e0: 2828 7369 7a65 5b30 5d20 6973 204e 6f6e  ((size[0] is Non
+000293f0: 6529 2061 6e64 2028 7369 7a65 5b31 5d29  e) and (size[1])
+00029400: 2069 7320 4e6f 6e65 290a 2020 2020 293a   is None).    ):
+00029410: 0a20 2020 2020 2020 2078 7920 3d20 6e70  .        xy = np
+00029420: 2e73 7172 7428 6e75 6d5f 7371 7561 7265  .sqrt(num_square
+00029430: 7320 2a20 7769 7265 5f70 6974 6368 202a  s * wire_pitch *
+00029440: 2077 6972 655f 7769 6474 6829 0a20 2020   wire_width).   
+00029450: 2020 2020 2073 697a 6520 3d20 5b78 792c       size = [xy,
+00029460: 2078 795d 0a20 2020 2020 2020 206e 756d   xy].        num
+00029470: 5f73 7175 6172 6573 203d 204e 6f6e 650a  _squares = None.
+00029480: 2020 2020 6966 205b 7369 7a65 5b30 5d2c      if [size[0],
+00029490: 2073 697a 655b 315d 2c20 6e75 6d5f 7371   size[1], num_sq
+000294a0: 7561 7265 735d 2e63 6f75 6e74 284e 6f6e  uares].count(Non
+000294b0: 6529 2021 3d20 313a 0a20 2020 2020 2020  e) != 1:.       
+000294c0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000294d0: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
+000294e0: 5b50 4849 444c 5d20 736e 7370 6428 2920  [PHIDL] snspd() 
+000294f0: 7265 7175 6972 6573 2074 6861 7420 6578  requires that ex
+00029500: 6163 746c 7920 4f4e 4520 7661 6c75 6520  actly ONE value 
+00029510: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
+00029520: 2022 7468 6520 6172 6775 6d65 6e74 7320   "the arguments 
+00029530: 6060 6e75 6d5f 7371 7561 7265 7360 6020  ``num_squares`` 
+00029540: 616e 6420 6060 7369 7a65 6060 2062 6520  and ``size`` be 
+00029550: 4e6f 6e65 2022 0a20 2020 2020 2020 2020  None ".         
+00029560: 2020 2022 746f 2070 7265 7665 6e74 206f     "to prevent o
+00029570: 7665 7263 6f6e 7374 7261 696e 696e 672c  verconstraining,
+00029580: 2066 6f72 2065 7861 6d70 6c65 3a5c 6e22   for example:\n"
+00029590: 0a20 2020 2020 2020 2020 2020 2022 3e3e  .            ">>
+000295a0: 3e20 736e 7370 6428 7369 7a65 203d 2028  > snspd(size = (
+000295b0: 332c 204e 6f6e 6529 2c20 6e75 6d5f 7371  3, None), num_sq
+000295c0: 7561 7265 7320 3d20 3230 3030 2922 0a20  uares = 2000)". 
+000295d0: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
+000295e0: 7369 7a65 5b30 5d20 6973 204e 6f6e 653a  size[0] is None:
+000295f0: 0a20 2020 2020 2020 2079 7369 7a65 203d  .        ysize =
+00029600: 2073 697a 655b 315d 0a20 2020 2020 2020   size[1].       
+00029610: 2078 7369 7a65 203d 206e 756d 5f73 7175   xsize = num_squ
+00029620: 6172 6573 202a 2077 6972 655f 7069 7463  ares * wire_pitc
+00029630: 6820 2a20 7769 7265 5f77 6964 7468 202f  h * wire_width /
+00029640: 2079 7369 7a65 0a20 2020 2065 6c69 6620   ysize.    elif 
+00029650: 7369 7a65 5b31 5d20 6973 204e 6f6e 653a  size[1] is None:
+00029660: 0a20 2020 2020 2020 2078 7369 7a65 203d  .        xsize =
+00029670: 2073 697a 655b 305d 0a20 2020 2020 2020   size[0].       
+00029680: 2079 7369 7a65 203d 206e 756d 5f73 7175   ysize = num_squ
+00029690: 6172 6573 202a 2077 6972 655f 7069 7463  ares * wire_pitc
+000296a0: 6820 2a20 7769 7265 5f77 6964 7468 202f  h * wire_width /
+000296b0: 2078 7369 7a65 0a20 2020 2065 6c73 653a   xsize.    else:
+000296c0: 0a20 2020 2020 2020 2078 7369 7a65 203d  .        xsize =
+000296d0: 2073 697a 655b 305d 0a20 2020 2020 2020   size[0].       
+000296e0: 2079 7369 7a65 203d 2073 697a 655b 315d   ysize = size[1]
+000296f0: 0a0a 2020 2020 6e75 6d5f 6d65 616e 6465  ..    num_meande
+00029700: 7273 203d 2069 6e74 286e 702e 6365 696c  rs = int(np.ceil
+00029710: 2879 7369 7a65 202f 2077 6972 655f 7069  (ysize / wire_pi
+00029720: 7463 6829 290a 0a20 2020 2044 203d 2044  tch))..    D = D
+00029730: 6576 6963 6528 6e61 6d65 3d22 736e 7370  evice(name="snsp
+00029740: 6422 290a 2020 2020 6861 6972 7069 6e20  d").    hairpin 
+00029750: 3d20 6f70 7469 6d61 6c5f 6861 6972 7069  = optimal_hairpi
+00029760: 6e28 0a20 2020 2020 2020 2077 6964 7468  n(.        width
+00029770: 3d77 6972 655f 7769 6474 682c 0a20 2020  =wire_width,.   
+00029780: 2020 2020 2070 6974 6368 3d77 6972 655f       pitch=wire_
+00029790: 7069 7463 682c 0a20 2020 2020 2020 2074  pitch,.        t
+000297a0: 7572 6e5f 7261 7469 6f3d 7475 726e 5f72  urn_ratio=turn_r
+000297b0: 6174 696f 2c0a 2020 2020 2020 2020 6c65  atio,.        le
+000297c0: 6e67 7468 3d78 7369 7a65 202f 2032 2c0a  ngth=xsize / 2,.
+000297d0: 2020 2020 2020 2020 6e75 6d5f 7074 733d          num_pts=
+000297e0: 3230 2c0a 2020 2020 2020 2020 6c61 7965  20,.        laye
+000297f0: 723d 6c61 7965 722c 0a20 2020 2029 0a0a  r=layer,.    )..
+00029800: 2020 2020 6966 2028 7465 726d 696e 616c      if (terminal
+00029810: 735f 7361 6d65 5f73 6964 6520 6973 2046  s_same_side is F
+00029820: 616c 7365 2920 616e 6420 2828 6e75 6d5f  alse) and ((num_
+00029830: 6d65 616e 6465 7273 2025 2032 2920 3d3d  meanders % 2) ==
+00029840: 2030 293a 0a20 2020 2020 2020 206e 756d   0):.        num
+00029850: 5f6d 6561 6e64 6572 7320 2b3d 2031 0a20  _meanders += 1. 
+00029860: 2020 2065 6c69 6620 2874 6572 6d69 6e61     elif (termina
+00029870: 6c73 5f73 616d 655f 7369 6465 2069 7320  ls_same_side is 
+00029880: 5472 7565 2920 616e 6420 2828 6e75 6d5f  True) and ((num_
+00029890: 6d65 616e 6465 7273 2025 2032 2920 3d3d  meanders % 2) ==
+000298a0: 2031 293a 0a20 2020 2020 2020 206e 756d   1):.        num
+000298b0: 5f6d 6561 6e64 6572 7320 2b3d 2031 0a0a  _meanders += 1..
+000298c0: 2020 2020 7374 6172 745f 6e77 203d 2044      start_nw = D
+000298d0: 2e61 6464 5f72 6566 2863 6f6d 7061 7373  .add_ref(compass
+000298e0: 2873 697a 653d 5b78 7369 7a65 202f 2032  (size=[xsize / 2
+000298f0: 2c20 7769 7265 5f77 6964 7468 5d2c 206c  , wire_width], l
+00029900: 6179 6572 3d6c 6179 6572 2929 0a0a 2020  ayer=layer))..  
+00029910: 2020 6870 5f70 7265 7620 3d20 442e 6164    hp_prev = D.ad
+00029920: 645f 7265 6628 6861 6972 7069 6e29 0a20  d_ref(hairpin). 
+00029930: 2020 2068 705f 7072 6576 2e63 6f6e 6e65     hp_prev.conne
+00029940: 6374 2831 2c20 7374 6172 745f 6e77 2e70  ct(1, start_nw.p
+00029950: 6f72 7473 5b22 4522 5d29 0a20 2020 2061  orts["E"]).    a
+00029960: 6c74 6572 6e61 7465 203d 2054 7275 650a  lternate = True.
+00029970: 2020 2020 666f 7220 6e20 696e 2072 616e      for n in ran
+00029980: 6765 2832 2c20 6e75 6d5f 6d65 616e 6465  ge(2, num_meande
+00029990: 7273 293a 0a20 2020 2020 2020 2068 7020  rs):.        hp 
+000299a0: 3d20 442e 6164 645f 7265 6628 6861 6972  = D.add_ref(hair
+000299b0: 7069 6e29 0a20 2020 2020 2020 2069 6620  pin).        if 
+000299c0: 616c 7465 726e 6174 653a 0a20 2020 2020  alternate:.     
+000299d0: 2020 2020 2020 2068 702e 636f 6e6e 6563         hp.connec
+000299e0: 7428 322c 2068 705f 7072 6576 2e70 6f72  t(2, hp_prev.por
+000299f0: 7473 5b32 5d29 0a20 2020 2020 2020 2020  ts[2]).         
+00029a00: 2020 206c 6173 745f 706f 7274 203d 2068     last_port = h
+00029a10: 702e 706f 7274 735b 315d 0a20 2020 2020  p.ports[1].     
+00029a20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00029a30: 2020 2020 2068 702e 636f 6e6e 6563 7428       hp.connect(
+00029a40: 312c 2068 705f 7072 6576 2e70 6f72 7473  1, hp_prev.ports
+00029a50: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+00029a60: 206c 6173 745f 706f 7274 203d 2068 702e   last_port = hp.
+00029a70: 706f 7274 735b 325d 0a20 2020 2020 2020  ports[2].       
+00029a80: 2068 705f 7072 6576 203d 2068 700a 2020   hp_prev = hp.  
+00029a90: 2020 2020 2020 616c 7465 726e 6174 6520        alternate 
+00029aa0: 3d20 6e6f 7420 616c 7465 726e 6174 650a  = not alternate.
+00029ab0: 0a20 2020 2066 696e 6973 685f 7365 203d  .    finish_se =
+00029ac0: 2044 2e61 6464 5f72 6566 2863 6f6d 7061   D.add_ref(compa
+00029ad0: 7373 2873 697a 653d 5b78 7369 7a65 202f  ss(size=[xsize /
+00029ae0: 2032 2c20 7769 7265 5f77 6964 7468 5d2c   2, wire_width],
+00029af0: 206c 6179 6572 3d6c 6179 6572 2929 0a20   layer=layer)). 
+00029b00: 2020 2066 696e 6973 685f 7365 2e63 6f6e     finish_se.con
+00029b10: 6e65 6374 2822 4522 2c20 6c61 7374 5f70  nect("E", last_p
+00029b20: 6f72 7429 0a0a 2020 2020 442e 6164 645f  ort)..    D.add_
+00029b30: 706f 7274 2870 6f72 743d 7374 6172 745f  port(port=start_
+00029b40: 6e77 2e70 6f72 7473 5b22 5722 5d2c 206e  nw.ports["W"], n
+00029b50: 616d 653d 3129 0a20 2020 2044 2e61 6464  ame=1).    D.add
+00029b60: 5f70 6f72 7428 706f 7274 3d66 696e 6973  _port(port=finis
+00029b70: 685f 7365 2e70 6f72 7473 5b22 5722 5d2c  h_se.ports["W"],
+00029b80: 206e 616d 653d 3229 0a0a 2020 2020 442e   name=2)..    D.
+00029b90: 696e 666f 5b22 6e75 6d5f 7371 7561 7265  info["num_square
+00029ba0: 7322 5d20 3d20 6e75 6d5f 6d65 616e 6465  s"] = num_meande
+00029bb0: 7273 202a 2028 7873 697a 6520 2f20 7769  rs * (xsize / wi
+00029bc0: 7265 5f77 6964 7468 290a 2020 2020 442e  re_width).    D.
+00029bd0: 696e 666f 5b22 6172 6561 225d 203d 2078  info["area"] = x
+00029be0: 7369 7a65 202a 2079 7369 7a65 0a20 2020  size * ysize.   
+00029bf0: 2044 2e69 6e66 6f5b 2273 697a 6522 5d20   D.info["size"] 
+00029c00: 3d20 2878 7369 7a65 2c20 7973 697a 6529  = (xsize, ysize)
+00029c10: 0a0a 2020 2020 7265 7475 726e 2044 0a0a  ..    return D..
+00029c20: 0a64 6566 2073 6e73 7064 5f65 7870 616e  .def snspd_expan
+00029c30: 6465 6428 0a20 2020 2077 6972 655f 7769  ded(.    wire_wi
+00029c40: 6474 683d 302e 322c 0a20 2020 2077 6972  dth=0.2,.    wir
+00029c50: 655f 7069 7463 683d 302e 362c 0a20 2020  e_pitch=0.6,.   
+00029c60: 2073 697a 653d 2831 302c 2038 292c 0a20   size=(10, 8),. 
+00029c70: 2020 206e 756d 5f73 7175 6172 6573 3d4e     num_squares=N
+00029c80: 6f6e 652c 0a20 2020 2063 6f6e 6e65 6374  one,.    connect
+00029c90: 6f72 5f77 6964 7468 3d31 2c0a 2020 2020  or_width=1,.    
+00029ca0: 636f 6e6e 6563 746f 725f 7379 6d6d 6574  connector_symmet
+00029cb0: 7269 633d 4661 6c73 652c 0a20 2020 2074  ric=False,.    t
+00029cc0: 7572 6e5f 7261 7469 6f3d 342c 0a20 2020  urn_ratio=4,.   
+00029cd0: 2074 6572 6d69 6e61 6c73 5f73 616d 655f   terminals_same_
+00029ce0: 7369 6465 3d46 616c 7365 2c0a 2020 2020  side=False,.    
+00029cf0: 6c61 7965 723d 302c 0a29 3a0a 2020 2020  layer=0,.):.    
+00029d00: 2222 2243 7265 6174 6573 2061 6e20 6f70  """Creates an op
+00029d10: 7469 6d61 6c6c 792d 726f 756e 6465 6420  timally-rounded 
+00029d20: 534e 5350 4420 7769 7468 2077 6972 6573  SNSPD with wires
+00029d30: 2063 6f6d 696e 6720 6f75 7420 6f66 2069   coming out of i
+00029d40: 7420 7468 6174 0a20 2020 2065 7870 616e  t that.    expan
+00029d50: 642e 0a0a 2020 2020 5061 7261 6d65 7465  d...    Paramete
+00029d60: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00029d70: 2d0a 2020 2020 7769 6474 6820 3a20 696e  -.    width : in
+00029d80: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
+00029d90: 2020 2057 6964 7468 206f 6620 7468 6520     Width of the 
+00029da0: 7769 7265 2e0a 2020 2020 7069 7463 6820  wire..    pitch 
+00029db0: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
+00029dc0: 2020 2020 2020 2044 6973 7461 6e63 6520         Distance 
+00029dd0: 6265 7477 6565 6e20 7477 6f20 6164 6a61  between two adja
+00029de0: 6365 6e74 2077 6972 6573 2e20 4d75 7374  cent wires. Must
+00029df0: 2062 6520 6772 6561 7465 7220 7468 616e   be greater than
+00029e00: 2060 7769 6474 6860 2e0a 2020 2020 7369   `width`..    si
+00029e10: 7a65 203a 204e 6f6e 6520 6f72 2061 7272  ze : None or arr
+00029e20: 6179 2d6c 696b 655b 325d 206f 6620 696e  ay-like[2] of in
+00029e30: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
+00029e40: 2020 2028 7769 6474 682c 2068 6569 6768     (width, heigh
+00029e50: 7429 206f 6620 7468 6520 7265 6374 616e  t) of the rectan
+00029e60: 676c 6520 666f 726d 6564 2062 7920 7468  gle formed by th
+00029e70: 6520 6f75 7465 7220 626f 756e 6461 7279  e outer boundary
+00029e80: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00029e90: 534e 5350 442e 204d 7573 7420 6265 206e  SNSPD. Must be n
+00029ea0: 6f6e 6520 6966 2060 6e75 6d5f 7371 7561  one if `num_squa
+00029eb0: 7265 7360 2069 7320 7370 6563 6966 6965  res` is specifie
+00029ec0: 642e 0a20 2020 206e 756d 5f73 7175 6172  d..    num_squar
+00029ed0: 6573 203a 2069 6e74 206f 7220 4e6f 6e65  es : int or None
+00029ee0: 0a20 2020 2020 2020 2054 6f74 616c 206e  .        Total n
+00029ef0: 756d 6265 7220 6f66 2073 7175 6172 6573  umber of squares
+00029f00: 2069 6e73 6964 6520 7468 6520 534e 5350   inside the SNSP
+00029f10: 4420 6c65 6e67 7468 2e20 4d75 7374 2062  D length. Must b
+00029f20: 6520 6e6f 6e65 2069 660a 2020 2020 2020  e none if.      
+00029f30: 2020 6073 697a 6560 2069 7320 7370 6563    `size` is spec
+00029f40: 6966 6965 642e 0a20 2020 2063 6f6e 6e65  ified..    conne
+00029f50: 6374 6f72 5f77 6964 7468 203a 2069 6e74  ctor_width : int
+00029f60: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
+00029f70: 2020 5769 6474 6820 6f66 2074 6865 2063    Width of the c
+00029f80: 6f6e 6e65 6374 6f72 732e 0a20 2020 2063  onnectors..    c
+00029f90: 6f6e 6e65 6374 6f72 5f73 796d 6d65 7472  onnector_symmetr
+00029fa0: 6963 203a 2062 6f6f 6c0a 2020 2020 2020  ic : bool.      
+00029fb0: 2020 4966 2054 7275 652c 206d 6972 726f    If True, mirro
+00029fc0: 7273 2074 6865 2063 6f6e 6e65 6374 6f72  rs the connector
+00029fd0: 7320 6163 726f 7373 2074 6865 6972 2066  s across their f
+00029fe0: 6c61 7420 6564 6765 2061 6e64 2061 6464  lat edge and add
+00029ff0: 7320 7468 656d 0a20 2020 2020 2020 2074  s them.        t
+0002a000: 6f20 7468 6520 636f 6e6e 6563 746f 7220  o the connector 
+0002a010: 6765 6f6d 6574 7279 2e0a 2020 2020 7475  geometry..    tu
+0002a020: 726e 5f72 6174 696f 203a 2069 6e74 206f  rn_ratio : int o
+0002a030: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
+0002a040: 5370 6563 6966 6965 7320 686f 7720 6d75  Specifies how mu
+0002a050: 6368 206f 6620 7468 6520 534e 5350 4420  ch of the SNSPD 
+0002a060: 7769 6474 6820 6973 2064 6564 6963 6174  width is dedicat
+0002a070: 6564 2074 6f20 7468 6520 3138 3020 6465  ed to the 180 de
+0002a080: 6772 6565 0a20 2020 2020 2020 2074 7572  gree.        tur
+0002a090: 6e2e 2041 2060 7475 726e 5f72 6174 696f  n. A `turn_ratio
+0002a0a0: 6020 6f66 2031 3020 7769 6c6c 2072 6573  ` of 10 will res
+0002a0b0: 756c 7420 696e 2032 3025 206f 6620 7468  ult in 20% of th
+0002a0c0: 6520 7769 6474 6820 6265 696e 670a 2020  e width being.  
+0002a0d0: 2020 2020 2020 636f 6d70 7269 7365 6420        comprised 
+0002a0e0: 6f66 2074 6865 2074 7572 6e2e 0a20 2020  of the turn..   
+0002a0f0: 2074 6572 6d69 6e61 6c73 5f73 616d 655f   terminals_same_
+0002a100: 7369 6465 203a 2062 6f6f 6c0a 2020 2020  side : bool.    
+0002a110: 2020 2020 4966 2054 7275 652c 2062 6f74      If True, bot
+0002a120: 6820 706f 7274 7320 7769 6c6c 2062 6520  h ports will be 
+0002a130: 6c6f 6361 7465 6420 6f6e 2074 6865 2073  located on the s
+0002a140: 616d 6520 7369 6465 206f 6620 7468 6520  ame side of the 
+0002a150: 534e 5350 442e 0a20 2020 206c 6179 6572  SNSPD..    layer
+0002a160: 203a 2069 6e74 2c20 6172 7261 792d 6c69   : int, array-li
+0002a170: 6b65 5b32 5d2c 206f 7220 7365 740a 2020  ke[2], or set.  
+0002a180: 2020 2020 2020 5370 6563 6966 6963 206c        Specific l
+0002a190: 6179 6572 2873 2920 746f 2070 7574 2070  ayer(s) to put p
+0002a1a0: 6f6c 7967 6f6e 2067 656f 6d65 7472 7920  olygon geometry 
+0002a1b0: 6f6e 2e0a 0a20 2020 2052 6574 7572 6e73  on...    Returns
+0002a1c0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0002a1d0: 2044 203a 2044 6576 6963 650a 2020 2020   D : Device.    
+0002a1e0: 2020 2020 4120 4465 7669 6365 2063 6f6e      A Device con
+0002a1f0: 7461 696e 696e 6720 616e 206f 7074 696d  taining an optim
+0002a200: 616c 6c79 2d72 6f75 6e64 6564 2053 4e53  ally-rounded SNS
+0002a210: 5044 2077 6974 6820 6578 7061 6e64 696e  PD with expandin
+0002a220: 6720 696e 7075 742f 0a20 2020 2020 2020  g input/.       
+0002a230: 206f 7574 7075 7420 7769 7265 732e 0a20   output wires.. 
+0002a240: 2020 2022 2222 0a20 2020 2044 203d 2044     """.    D = D
+0002a250: 6576 6963 6528 2273 6e73 7064 5f65 7870  evice("snspd_exp
+0002a260: 616e 6465 6422 290a 2020 2020 5320 3d20  anded").    S = 
+0002a270: 736e 7370 6428 0a20 2020 2020 2020 2077  snspd(.        w
+0002a280: 6972 655f 7769 6474 683d 7769 7265 5f77  ire_width=wire_w
+0002a290: 6964 7468 2c0a 2020 2020 2020 2020 7769  idth,.        wi
+0002a2a0: 7265 5f70 6974 6368 3d77 6972 655f 7069  re_pitch=wire_pi
+0002a2b0: 7463 682c 0a20 2020 2020 2020 2073 697a  tch,.        siz
+0002a2c0: 653d 7369 7a65 2c0a 2020 2020 2020 2020  e=size,.        
+0002a2d0: 6e75 6d5f 7371 7561 7265 733d 6e75 6d5f  num_squares=num_
+0002a2e0: 7371 7561 7265 732c 0a20 2020 2020 2020  squares,.       
+0002a2f0: 2074 7572 6e5f 7261 7469 6f3d 7475 726e   turn_ratio=turn
+0002a300: 5f72 6174 696f 2c0a 2020 2020 2020 2020  _ratio,.        
+0002a310: 7465 726d 696e 616c 735f 7361 6d65 5f73  terminals_same_s
+0002a320: 6964 653d 7465 726d 696e 616c 735f 7361  ide=terminals_sa
+0002a330: 6d65 5f73 6964 652c 0a20 2020 2020 2020  me_side,.       
+0002a340: 206c 6179 6572 3d6c 6179 6572 2c0a 2020   layer=layer,.  
+0002a350: 2020 290a 2020 2020 7320 3d20 442e 6164    ).    s = D.ad
+0002a360: 645f 7265 6628 5329 0a20 2020 2073 7465  d_ref(S).    ste
+0002a370: 705f 6465 7669 6365 203d 206f 7074 696d  p_device = optim
+0002a380: 616c 5f73 7465 7028 0a20 2020 2020 2020  al_step(.       
+0002a390: 2073 7461 7274 5f77 6964 7468 3d77 6972   start_width=wir
+0002a3a0: 655f 7769 6474 682c 0a20 2020 2020 2020  e_width,.       
+0002a3b0: 2065 6e64 5f77 6964 7468 3d63 6f6e 6e65   end_width=conne
+0002a3c0: 6374 6f72 5f77 6964 7468 2c0a 2020 2020  ctor_width,.    
+0002a3d0: 2020 2020 6e75 6d5f 7074 733d 3130 302c      num_pts=100,
+0002a3e0: 0a20 2020 2020 2020 2061 6e74 6963 726f  .        anticro
+0002a3f0: 7764 696e 675f 6661 6374 6f72 3d32 2c0a  wding_factor=2,.
+0002a400: 2020 2020 2020 2020 7769 6474 685f 746f          width_to
+0002a410: 6c3d 3165 2d33 2c0a 2020 2020 2020 2020  l=1e-3,.        
+0002a420: 7379 6d6d 6574 7269 633d 636f 6e6e 6563  symmetric=connec
+0002a430: 746f 725f 7379 6d6d 6574 7269 632c 0a20  tor_symmetric,. 
+0002a440: 2020 2020 2020 206c 6179 6572 3d6c 6179         layer=lay
+0002a450: 6572 2c0a 2020 2020 290a 2020 2020 7374  er,.    ).    st
+0002a460: 6570 3120 3d20 442e 6164 645f 7265 6628  ep1 = D.add_ref(
+0002a470: 7374 6570 5f64 6576 6963 6529 0a20 2020  step_device).   
+0002a480: 2073 7465 7032 203d 2044 2e61 6464 5f72   step2 = D.add_r
+0002a490: 6566 2873 7465 705f 6465 7669 6365 290a  ef(step_device).
+0002a4a0: 2020 2020 7374 6570 312e 636f 6e6e 6563      step1.connec
+0002a4b0: 7428 706f 7274 3d31 2c20 6465 7374 696e  t(port=1, destin
+0002a4c0: 6174 696f 6e3d 732e 706f 7274 735b 315d  ation=s.ports[1]
+0002a4d0: 290a 2020 2020 7374 6570 322e 636f 6e6e  ).    step2.conn
+0002a4e0: 6563 7428 706f 7274 3d31 2c20 6465 7374  ect(port=1, dest
+0002a4f0: 696e 6174 696f 6e3d 732e 706f 7274 735b  ination=s.ports[
+0002a500: 325d 290a 2020 2020 442e 6164 645f 706f  2]).    D.add_po
+0002a510: 7274 286e 616d 653d 312c 2070 6f72 743d  rt(name=1, port=
+0002a520: 7374 6570 312e 706f 7274 735b 325d 290a  step1.ports[2]).
+0002a530: 2020 2020 442e 6164 645f 706f 7274 286e      D.add_port(n
+0002a540: 616d 653d 322c 2070 6f72 743d 7374 6570  ame=2, port=step
+0002a550: 322e 706f 7274 735b 325d 290a 0a20 2020  2.ports[2])..   
+0002a560: 2044 2e69 6e66 6f20 3d20 532e 696e 666f   D.info = S.info
+0002a570: 0a20 2020 2053 2e69 6e66 6f20 3d20 7b7d  .    S.info = {}
+0002a580: 0a0a 2020 2020 7265 7475 726e 2044 0a0a  ..    return D..
+0002a590: 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .# =============
 0002a5a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002a5b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002a5c0: 3d3d 0a0a 2320 7320 3d20 736e 7370 6428  ==..# s = snspd(
-0002a5d0: 7769 7265 5f77 6964 7468 203d 2030 2e32  wire_width = 0.2
-0002a5e0: 2c20 7769 7265 5f70 6974 6368 203d 2030  , wire_pitch = 0
-0002a5f0: 2e36 2c20 7369 7a65 203d 205b 3130 2c33  .6, size = [10,3
-0002a600: 5d2c 2074 6572 6d69 6e61 6c73 5f73 616d  ], terminals_sam
-0002a610: 655f 7369 6465 203d 2054 7275 6529 0a23  e_side = True).#
-0002a620: 2071 7569 636b 706c 6f74 2873 290a 0a23   quickplot(s)..#
-0002a630: 2073 203d 2073 6e73 7064 2877 6972 655f   s = snspd(wire_
-0002a640: 7769 6474 6820 3d20 302e 322c 2077 6972  width = 0.2, wir
-0002a650: 655f 7069 7463 6820 3d20 302e 362c 2073  e_pitch = 0.6, s
-0002a660: 697a 6520 3d20 5b31 302c 204e 6f6e 655d  ize = [10, None]
-0002a670: 2c0a 2320 2020 2020 2020 2020 206e 756d  ,.#          num
-0002a680: 5f73 7175 6172 6573 203d 2031 3030 302c  _squares = 1000,
-0002a690: 2074 6572 6d69 6e61 6c73 5f73 616d 655f   terminals_same_
-0002a6a0: 7369 6465 203d 2054 7275 6529 0a23 2071  side = True).# q
-0002a6b0: 7569 636b 706c 6f74 2873 290a 0a0a 6465  uickplot(s)...de
-0002a6c0: 6620 736e 7370 645f 6361 6e64 656c 6162  f snspd_candelab
-0002a6d0: 7261 2820 2023 206e 6f71 613a 2043 3930  ra(  # noqa: C90
-0002a6e0: 310a 2020 2020 7769 7265 5f77 6964 7468  1.    wire_width
-0002a6f0: 3d30 2e35 322c 0a20 2020 2077 6972 655f  =0.52,.    wire_
-0002a700: 7069 7463 683d 302e 3536 2c0a 2020 2020  pitch=0.56,.    
-0002a710: 6861 7869 733d 3930 2c0a 2020 2020 7661  haxis=90,.    va
-0002a720: 7869 733d 3530 2c0a 2020 2020 6571 7561  xis=50,.    equa
-0002a730: 6c69 7a65 5f70 6174 685f 6c65 6e67 7468  lize_path_length
-0002a740: 733d 4661 6c73 652c 0a20 2020 2078 7769  s=False,.    xwi
-0002a750: 6e67 3d46 616c 7365 2c0a 2020 2020 6c61  ng=False,.    la
-0002a760: 7965 723d 302c 0a29 3a0a 2020 2020 2222  yer=0,.):.    ""
-0002a770: 2243 7265 6174 6573 2061 6e20 6f70 7469  "Creates an opti
-0002a780: 6d61 6c6c 792d 726f 756e 6465 6420 534e  mally-rounded SN
-0002a790: 5350 4420 7769 7468 206c 6f77 2063 7572  SPD with low cur
-0002a7a0: 7265 6e74 2063 726f 7764 696e 6720 616e  rent crowding an
-0002a7b0: 640a 2020 2020 6172 6274 6974 7261 7269  d.    arbtitrari
-0002a7c0: 6c79 2d68 6967 6820 6669 6c6c 2066 6163  ly-high fill fac
-0002a7d0: 746f 7220 6173 2064 6573 6372 6962 6564  tor as described
-0002a7e0: 2062 7920 5265 6464 7920 6574 2e20 616c   by Reddy et. al
-0002a7f0: 2e2c 0a20 2020 2041 504c 2050 686f 746f  .,.    APL Photo
-0002a800: 6e69 6373 2037 2c20 3035 3133 3032 2028  nics 7, 051302 (
-0002a810: 3230 3232 2920 2068 7474 7073 3a2f 2f64  2022)  https://d
-0002a820: 6f69 2e6f 7267 2f31 302e 3130 3633 2f35  oi.org/10.1063/5
-0002a830: 2e30 3038 3830 3037 0a0a 2020 2020 5061  .0088007..    Pa
-0002a840: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0002a850: 2d2d 2d2d 2d2d 2d0a 2020 2020 7769 7265  -------.    wire
-0002a860: 5f77 6964 7468 203a 2069 6e74 206f 7220  _width : int or 
-0002a870: 666c 6f61 740a 2020 2020 2020 2020 5769  float.        Wi
-0002a880: 6474 6820 6f66 2074 6865 2077 6972 652e  dth of the wire.
-0002a890: 0a20 2020 2077 6972 655f 7069 7463 6820  .    wire_pitch 
-0002a8a0: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
-0002a8b0: 2020 2020 2020 2044 6973 7461 6e63 6520         Distance 
-0002a8c0: 6265 7477 6565 6e20 7477 6f20 6164 6a61  between two adja
-0002a8d0: 6365 6e74 2077 6972 6573 2e20 4d75 7374  cent wires. Must
-0002a8e0: 2062 6520 6772 6561 7465 7220 7468 616e   be greater than
-0002a8f0: 2060 7769 6474 6860 2e0a 2020 2020 6861   `width`..    ha
-0002a900: 7869 7320 3a20 696e 7420 6f72 2066 6c6f  xis : int or flo
-0002a910: 6174 0a20 2020 2020 2020 204c 656e 6774  at.        Lengt
-0002a920: 6820 6f66 2068 6f72 697a 6f6e 7461 6c20  h of horizontal 
-0002a930: 6469 6167 6f6e 616c 206f 6620 7468 6520  diagonal of the 
-0002a940: 7268 6f6d 626f 6964 616c 2061 6374 6976  rhomboidal activ
-0002a950: 6520 6172 6561 2e0a 2020 2020 2020 2020  e area..        
-0002a960: 5468 6520 7061 7261 6d65 7465 7220 6068  The parameter `h
-0002a970: 6178 6973 6020 6973 2070 7269 6f72 6974  axis` is priorit
-0002a980: 697a 6564 206f 7665 7220 6076 6178 6973  ized over `vaxis
-0002a990: 602e 0a20 2020 2076 6178 6973 203a 2069  `..    vaxis : i
-0002a9a0: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
-0002a9b0: 2020 2020 4c65 6e67 7468 206f 6620 7665      Length of ve
-0002a9c0: 7274 6963 616c 2064 6961 676f 6e61 6c20  rtical diagonal 
-0002a9d0: 6f66 2074 6865 2072 686f 6d62 6f69 6461  of the rhomboida
-0002a9e0: 6c20 6163 7469 7665 2061 7265 612e 0a20  l active area.. 
-0002a9f0: 2020 2065 7175 616c 697a 655f 7061 7468     equalize_path
-0002aa00: 5f6c 656e 6774 6873 203a 2062 6f6f 6c0a  _lengths : bool.
-0002aa10: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-0002aa20: 2061 6464 7320 7769 7265 2073 6567 6d65   adds wire segme
-0002aa30: 6e74 7320 746f 2068 6169 7270 696e 2062  nts to hairpin b
-0002aa40: 656e 6473 2074 6f20 6571 7561 6c69 7a65  ends to equalize
-0002aa50: 2070 6174 6820 6c65 6e67 7468 730a 2020   path lengths.  
-0002aa60: 2020 2020 2020 6672 6f6d 2063 656e 7465        from cente
-0002aa70: 7220 746f 2063 656e 7465 7220 666f 7220  r to center for 
-0002aa80: 616c 6c20 7061 7261 6c6c 656c 2077 6972  all parallel wir
-0002aa90: 6573 2069 6e20 6163 7469 7665 2061 7265  es in active are
-0002aaa0: 612e 0a20 2020 2078 7769 6e67 203a 2062  a..    xwing : b
-0002aab0: 6f6f 6c0a 2020 2020 2020 2020 4966 2054  ool.        If T
-0002aac0: 7275 652c 2072 6570 6c61 6365 7320 3930  rue, replaces 90
-0002aad0: 2d64 6567 7265 6520 6265 6e64 7320 7769  -degree bends wi
-0002aae0: 7468 2031 3335 2d64 6567 7265 6520 6265  th 135-degree be
-0002aaf0: 6e64 732e 0a20 2020 206c 6179 6572 203a  nds..    layer :
-0002ab00: 2069 6e74 0a20 2020 2020 2020 2053 7065   int.        Spe
-0002ab10: 6369 6669 6320 6c61 7965 7220 746f 2070  cific layer to p
-0002ab20: 7574 2070 6f6c 7967 6f6e 2067 656f 6d65  ut polygon geome
-0002ab30: 7472 7920 6f6e 2e0a 0a20 2020 2052 6574  try on...    Ret
-0002ab40: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-0002ab50: 0a20 2020 2044 203a 2044 6576 6963 650a  .    D : Device.
-0002ab60: 2020 2020 2020 2020 4120 4465 7669 6365          A Device
-0002ab70: 2063 6f6e 7461 696e 696e 6720 616e 206f   containing an o
-0002ab80: 7074 696d 616c 6c79 2d72 6f75 6e64 6564  ptimally-rounded
-0002ab90: 2053 4e53 5044 2077 6974 6820 6d69 6e69   SNSPD with mini
-0002aba0: 6d69 7a65 6420 6375 7272 656e 740a 2020  mized current.  
-0002abb0: 2020 2020 2020 6372 6f77 6469 6e67 2066        crowding f
-0002abc0: 6f72 2061 6e79 2066 696c 6c20 6661 6374  or any fill fact
-0002abd0: 6f72 2e0a 2020 2020 2222 220a 0a20 2020  or..    """..   
-0002abe0: 2064 6566 206f 6666 5f61 7869 735f 7574   def off_axis_ut
-0002abf0: 7572 6e28 0a20 2020 2020 2020 2077 6972  urn(.        wir
-0002ac00: 655f 7769 6474 683d 302e 3532 2c0a 2020  e_width=0.52,.  
-0002ac10: 2020 2020 2020 7769 7265 5f70 6974 6368        wire_pitch
-0002ac20: 3d30 2e35 362c 0a20 2020 2020 2020 2070  =0.56,.        p
-0002ac30: 6661 6374 3d31 302e 3020 2f20 332c 0a20  fact=10.0 / 3,. 
-0002ac40: 2020 2020 2020 2073 6861 7270 3d46 616c         sharp=Fal
-0002ac50: 7365 2c0a 2020 2020 2020 2020 7061 645f  se,.        pad_
-0002ac60: 6c65 6e67 7468 3d30 2c0a 2020 2020 2020  length=0,.      
-0002ac70: 2020 6c61 7965 723d 302c 0a20 2020 2029    layer=0,.    )
-0002ac80: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-0002ac90: 7572 6e73 2070 6869 646c 2064 6576 6963  urns phidl devic
-0002aca0: 6520 6c6f 772d 6372 6f77 6469 6e67 2075  e low-crowding u
-0002acb0: 2d74 7572 6e20 666f 7220 6361 6e64 656c  -turn for candel
-0002acc0: 6162 7261 206d 6561 6e64 6572 2e22 2222  abra meander."""
-0002acd0: 0a20 2020 2020 2020 2062 6172 6320 3d20  .        barc = 
-0002ace0: 6f70 7469 6d61 6c5f 3930 6465 6728 7769  optimal_90deg(wi
-0002acf0: 6474 683d 7769 7265 5f77 6964 7468 2c20  dth=wire_width, 
-0002ad00: 6c61 7965 723d 6c61 7965 7229 0a20 2020  layer=layer).   
-0002ad10: 2020 2020 2069 6620 6e6f 7420 7368 6172       if not shar
-0002ad20: 703a 0a20 2020 2020 2020 2020 2020 2023  p:.            #
-0002ad30: 2046 6f72 206e 6f6e 2d72 6f75 6e64 6564   For non-rounded
-0002ad40: 206f 7574 6572 2072 6164 6969 0a20 2020   outer radii.   
-0002ad50: 2020 2020 2020 2020 2023 204e 6f74 2066           # Not f
-0002ad60: 756c 6c79 2069 6d70 6c65 6d65 6e74 6564  ully implemented
-0002ad70: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
-0002ad80: 7431 6d70 203d 205b 6261 7263 2e70 6f72  t1mp = [barc.por
-0002ad90: 7473 5b31 5d2e 782c 2062 6172 632e 706f  ts[1].x, barc.po
-0002ada0: 7274 735b 315d 2e79 5d0a 2020 2020 2020  rts[1].y].      
-0002adb0: 2020 2020 2020 706f 7274 316f 7220 3d20        port1or = 
-0002adc0: 6261 7263 2e70 6f72 7473 5b31 5d2e 6f72  barc.ports[1].or
-0002add0: 6965 6e74 6174 696f 6e0a 2020 2020 2020  ientation.      
-0002ade0: 2020 2020 2020 706f 7274 326d 7020 3d20        port2mp = 
-0002adf0: 5b62 6172 632e 706f 7274 735b 325d 2e78  [barc.ports[2].x
-0002ae00: 2c20 6261 7263 2e70 6f72 7473 5b32 5d2e  , barc.ports[2].
-0002ae10: 795d 0a20 2020 2020 2020 2020 2020 2070  y].            p
-0002ae20: 6f72 7432 6f72 203d 2062 6172 632e 706f  ort2or = barc.po
-0002ae30: 7274 735b 325d 2e6f 7269 656e 7461 7469  rts[2].orientati
-0002ae40: 6f6e 0a20 2020 2020 2020 2020 2020 2062  on.            b
-0002ae50: 6172 6320 3d20 626f 6f6c 6561 6e28 0a20  arc = boolean(. 
-0002ae60: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0002ae70: 3d62 6172 632c 0a20 2020 2020 2020 2020  =barc,.         
-0002ae80: 2020 2020 2020 2042 3d63 6f70 7928 6261         B=copy(ba
-0002ae90: 7263 292e 6d6f 7665 285b 2d77 6972 655f  rc).move([-wire_
-0002aea0: 7769 6474 682c 202d 7769 7265 5f77 6964  width, -wire_wid
-0002aeb0: 7468 5d29 2c0a 2020 2020 2020 2020 2020  th]),.          
-0002aec0: 2020 2020 2020 6f70 6572 6174 696f 6e3d        operation=
-0002aed0: 226e 6f74 222c 0a20 2020 2020 2020 2020  "not",.         
-0002aee0: 2020 2020 2020 206c 6179 6572 3d6c 6179         layer=lay
-0002aef0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0002af00: 290a 2020 2020 2020 2020 2020 2020 6261  ).            ba
-0002af10: 7263 2e61 6464 5f70 6f72 7428 0a20 2020  rc.add_port(.   
-0002af20: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-0002af30: 653d 312c 206d 6964 706f 696e 743d 706f  e=1, midpoint=po
-0002af40: 7274 316d 702c 2077 6964 7468 3d77 6972  rt1mp, width=wir
-0002af50: 655f 7769 6474 682c 206f 7269 656e 7461  e_width, orienta
-0002af60: 7469 6f6e 3d70 6f72 7431 6f72 0a20 2020  tion=port1or.   
-0002af70: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0002af80: 2020 2020 2020 2062 6172 632e 6164 645f         barc.add_
-0002af90: 706f 7274 280a 2020 2020 2020 2020 2020  port(.          
-0002afa0: 2020 2020 2020 6e61 6d65 3d32 2c20 6d69        name=2, mi
-0002afb0: 6470 6f69 6e74 3d70 6f72 7432 6d70 2c20  dpoint=port2mp, 
-0002afc0: 7769 6474 683d 7769 7265 5f77 6964 7468  width=wire_width
-0002afd0: 2c20 6f72 6965 6e74 6174 696f 6e3d 706f  , orientation=po
-0002afe0: 7274 326f 720a 2020 2020 2020 2020 2020  rt2or.          
-0002aff0: 2020 290a 2020 2020 2020 2020 7069 6e20    ).        pin 
-0002b000: 3d20 6f70 7469 6d61 6c5f 6861 6972 7069  = optimal_hairpi
-0002b010: 6e28 0a20 2020 2020 2020 2020 2020 2077  n(.            w
-0002b020: 6964 7468 3d77 6972 655f 7769 6474 682c  idth=wire_width,
-0002b030: 0a20 2020 2020 2020 2020 2020 2070 6974  .            pit
-0002b040: 6368 3d70 6661 6374 202a 2077 6972 655f  ch=pfact * wire_
-0002b050: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
-0002b060: 2020 206c 656e 6774 683d 3820 2a20 7769     length=8 * wi
-0002b070: 7265 5f77 6964 7468 2c0a 2020 2020 2020  re_width,.      
-0002b080: 2020 2020 2020 6c61 7965 723d 6c61 7965        layer=laye
-0002b090: 722c 0a20 2020 2020 2020 2029 0a20 2020  r,.        ).   
-0002b0a0: 2020 2020 2070 6173 203d 2063 6f6d 7061       pas = compa
-0002b0b0: 7373 2873 697a 653d 2877 6972 655f 7769  ss(size=(wire_wi
-0002b0c0: 6474 682c 2077 6972 655f 7069 7463 6829  dth, wire_pitch)
-0002b0d0: 2c20 6c61 7965 723d 6c61 7965 7229 0a20  , layer=layer). 
-0002b0e0: 2020 2020 2020 2044 203d 2044 6576 6963         D = Devic
-0002b0f0: 6528 290a 2020 2020 2020 2020 6172 6331  e().        arc1
-0002b100: 203d 2044 2e61 6464 5f72 6566 2862 6172   = D.add_ref(bar
-0002b110: 6329 0a20 2020 2020 2020 2061 7263 312e  c).        arc1.
-0002b120: 726f 7461 7465 2839 3029 0a20 2020 2020  rotate(90).     
-0002b130: 2020 2070 696e 3120 3d20 442e 6164 645f     pin1 = D.add_
-0002b140: 7265 6628 7069 6e29 0a20 2020 2020 2020  ref(pin).       
-0002b150: 2070 696e 312e 636f 6e6e 6563 7428 312c   pin1.connect(1,
-0002b160: 2061 7263 312e 706f 7274 735b 325d 290a   arc1.ports[2]).
-0002b170: 2020 2020 2020 2020 7061 7331 203d 2044          pas1 = D
-0002b180: 2e61 6464 5f72 6566 2870 6173 290a 2020  .add_ref(pas).  
-0002b190: 2020 2020 2020 7061 7331 2e63 6f6e 6e65        pas1.conne
-0002b1a0: 6374 2870 6173 312e 706f 7274 735b 224e  ct(pas1.ports["N
-0002b1b0: 225d 2c20 7069 6e31 2e70 6f72 7473 5b32  "], pin1.ports[2
-0002b1c0: 5d29 0a20 2020 2020 2020 2061 7263 3220  ]).        arc2 
-0002b1d0: 3d20 442e 6164 645f 7265 6628 6261 7263  = D.add_ref(barc
-0002b1e0: 290a 2020 2020 2020 2020 6172 6332 2e63  ).        arc2.c
-0002b1f0: 6f6e 6e65 6374 2832 2c20 7061 7331 2e70  onnect(2, pas1.p
-0002b200: 6f72 7473 5b22 5322 5d29 0a20 2020 2020  orts["S"]).     
-0002b210: 2020 2069 6620 7061 645f 6c65 6e67 7468     if pad_length
-0002b220: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-0002b230: 2020 7069 6e31 2e6d 6f76 6579 2870 6164    pin1.movey(pad
-0002b240: 5f6c 656e 6774 6820 2a20 302e 3529 0a20  _length * 0.5). 
-0002b250: 2020 2020 2020 2020 2020 2074 656d 7063             tempc
-0002b260: 203d 2044 2e61 6464 5f72 6566 280a 2020   = D.add_ref(.  
-0002b270: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0002b280: 6d70 6173 7328 0a20 2020 2020 2020 2020  mpass(.         
-0002b290: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-0002b2a0: 2870 696e 312e 706f 7274 735b 315d 2e77  (pin1.ports[1].w
-0002b2b0: 6964 7468 2c20 7069 6e31 2e70 6f72 7473  idth, pin1.ports
-0002b2c0: 5b31 5d2e 7920 2d20 6172 6331 2e70 6f72  [1].y - arc1.por
-0002b2d0: 7473 5b32 5d2e 7929 2c0a 2020 2020 2020  ts[2].y),.      
-0002b2e0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0002b2f0: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
-0002b300: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002b310: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0002b320: 2020 2020 2020 2074 656d 7063 2e63 6f6e         tempc.con
-0002b330: 6e65 6374 2822 4e22 2c20 7069 6e31 2e70  nect("N", pin1.p
-0002b340: 6f72 7473 5b31 5d29 0a20 2020 2020 2020  orts[1]).       
-0002b350: 2020 2020 2074 656d 7063 203d 2044 2e61       tempc = D.a
-0002b360: 6464 5f72 6566 280a 2020 2020 2020 2020  dd_ref(.        
-0002b370: 2020 2020 2020 2020 636f 6d70 6173 7328          compass(
-0002b380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b390: 2020 2020 2073 697a 653d 2870 696e 312e       size=(pin1.
-0002b3a0: 706f 7274 735b 325d 2e77 6964 7468 2c20  ports[2].width, 
-0002b3b0: 7069 6e31 2e70 6f72 7473 5b32 5d2e 7920  pin1.ports[2].y 
-0002b3c0: 2d20 7061 7331 2e70 6f72 7473 5b22 4e22  - pas1.ports["N"
-0002b3d0: 5d2e 7929 2c0a 2020 2020 2020 2020 2020  ].y),.          
-0002b3e0: 2020 2020 2020 2020 2020 6c61 7965 723d            layer=
-0002b3f0: 6c61 7965 722c 0a20 2020 2020 2020 2020  layer,.         
-0002b400: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002b410: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0002b420: 2020 2074 656d 7063 2e63 6f6e 6e65 6374     tempc.connect
-0002b430: 2822 4e22 2c20 7069 6e31 2e70 6f72 7473  ("N", pin1.ports
-0002b440: 5b32 5d29 0a20 2020 2020 2020 2044 2e61  [2]).        D.a
-0002b450: 6464 5f70 6f72 7428 0a20 2020 2020 2020  dd_port(.       
-0002b460: 2020 2020 206e 616d 653d 312c 0a20 2020       name=1,.   
-0002b470: 2020 2020 2020 2020 206d 6964 706f 696e           midpoin
-0002b480: 743d 6172 6331 2e70 6f72 7473 5b31 5d2e  t=arc1.ports[1].
-0002b490: 6d69 6470 6f69 6e74 2c0a 2020 2020 2020  midpoint,.      
-0002b4a0: 2020 2020 2020 7769 6474 683d 7769 7265        width=wire
-0002b4b0: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
-0002b4c0: 2020 2020 6f72 6965 6e74 6174 696f 6e3d      orientation=
-0002b4d0: 6172 6331 2e70 6f72 7473 5b31 5d2e 6f72  arc1.ports[1].or
-0002b4e0: 6965 6e74 6174 696f 6e2c 0a20 2020 2020  ientation,.     
-0002b4f0: 2020 2029 0a20 2020 2020 2020 2044 2e61     ).        D.a
-0002b500: 6464 5f70 6f72 7428 0a20 2020 2020 2020  dd_port(.       
-0002b510: 2020 2020 206e 616d 653d 322c 0a20 2020       name=2,.   
-0002b520: 2020 2020 2020 2020 206d 6964 706f 696e           midpoin
-0002b530: 743d 6172 6332 2e70 6f72 7473 5b31 5d2e  t=arc2.ports[1].
-0002b540: 6d69 6470 6f69 6e74 2c0a 2020 2020 2020  midpoint,.      
-0002b550: 2020 2020 2020 7769 6474 683d 7769 7265        width=wire
-0002b560: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
-0002b570: 2020 2020 6f72 6965 6e74 6174 696f 6e3d      orientation=
-0002b580: 6172 6332 2e70 6f72 7473 5b31 5d2e 6f72  arc2.ports[1].or
-0002b590: 6965 6e74 6174 696f 6e2c 0a20 2020 2020  ientation,.     
-0002b5a0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-0002b5b0: 7572 6e20 440a 0a20 2020 2064 6566 2078  urn D..    def x
-0002b5c0: 7769 6e67 5f75 7475 726e 280a 2020 2020  wing_uturn(.    
-0002b5d0: 2020 2020 7769 7265 5f77 6964 7468 3d30      wire_width=0
-0002b5e0: 2e35 322c 2077 6972 655f 7069 7463 683d  .52, wire_pitch=
-0002b5f0: 302e 3536 2c20 7066 6163 743d 3130 2e30  0.56, pfact=10.0
-0002b600: 202f 2033 2c20 7061 645f 6c65 6e67 7468   / 3, pad_length
-0002b610: 3d30 2c20 6c61 7965 723d 300a 2020 2020  =0, layer=0.    
-0002b620: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-0002b630: 7475 726e 7320 7068 6964 6c20 6465 7669  turns phidl devi
-0002b640: 6365 206c 6f77 2d63 726f 7764 696e 6720  ce low-crowding 
-0002b650: 752d 7475 726e 2066 6f72 2058 2d77 696e  u-turn for X-win
-0002b660: 6720 6d65 616e 6465 722e 2222 220a 2020  g meander.""".  
-0002b670: 2020 2020 2020 6261 7263 203d 2061 7263        barc = arc
-0002b680: 280a 2020 2020 2020 2020 2020 2020 7261  (.            ra
-0002b690: 6469 7573 3d77 6972 655f 7769 6474 6820  dius=wire_width 
-0002b6a0: 2a20 332c 2077 6964 7468 3d77 6972 655f  * 3, width=wire_
-0002b6b0: 7769 6474 682c 206c 6179 6572 3d6c 6179  width, layer=lay
-0002b6c0: 6572 2c20 7468 6574 613d 3435 0a20 2020  er, theta=45.   
-0002b6d0: 2020 2020 2029 2e72 6f74 6174 6528 3138       ).rotate(18
-0002b6e0: 3029 0a0a 2020 2020 2020 2020 7069 6e20  0)..        pin 
-0002b6f0: 3d20 6f70 7469 6d61 6c5f 6861 6972 7069  = optimal_hairpi
-0002b700: 6e28 0a20 2020 2020 2020 2020 2020 2077  n(.            w
-0002b710: 6964 7468 3d77 6972 655f 7769 6474 682c  idth=wire_width,
-0002b720: 0a20 2020 2020 2020 2020 2020 2070 6974  .            pit
-0002b730: 6368 3d70 6661 6374 202a 2077 6972 655f  ch=pfact * wire_
-0002b740: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
-0002b750: 2020 206c 656e 6774 683d 3135 202a 2077     length=15 * w
-0002b760: 6972 655f 7769 6474 682c 0a20 2020 2020  ire_width,.     
-0002b770: 2020 2020 2020 206c 6179 6572 3d6c 6179         layer=lay
-0002b780: 6572 2c0a 2020 2020 2020 2020 290a 0a20  er,.        ).. 
-0002b790: 2020 2020 2020 2070 6173 6c65 6e20 3d20         paslen = 
-0002b7a0: 7066 6163 7420 2a20 7769 7265 5f77 6964  pfact * wire_wid
-0002b7b0: 7468 202d 206e 702e 7371 7274 2832 2920  th - np.sqrt(2) 
-0002b7c0: 2a20 7769 7265 5f70 6974 6368 0a20 2020  * wire_pitch.   
-0002b7d0: 2020 2020 2070 6173 203d 2063 6f6d 7061       pas = compa
-0002b7e0: 7373 2873 697a 653d 2877 6972 655f 7769  ss(size=(wire_wi
-0002b7f0: 6474 682c 2061 6273 2870 6173 6c65 6e29  dth, abs(paslen)
-0002b800: 292c 206c 6179 6572 3d6c 6179 6572 290a  ), layer=layer).
-0002b810: 2020 2020 2020 2020 4474 656d 7020 3d20          Dtemp = 
-0002b820: 4465 7669 6365 2829 0a20 2020 2020 2020  Device().       
-0002b830: 2061 7263 3120 3d20 4474 656d 702e 6164   arc1 = Dtemp.ad
-0002b840: 645f 7265 6628 6261 7263 290a 2020 2020  d_ref(barc).    
-0002b850: 2020 2020 6172 6331 2e72 6f74 6174 6528      arc1.rotate(
-0002b860: 3930 290a 2020 2020 2020 2020 7069 6e31  90).        pin1
-0002b870: 203d 2044 7465 6d70 2e61 6464 5f72 6566   = Dtemp.add_ref
-0002b880: 2870 696e 290a 2020 2020 2020 2020 7061  (pin).        pa
-0002b890: 7331 203d 2044 7465 6d70 2e61 6464 5f72  s1 = Dtemp.add_r
-0002b8a0: 6566 2870 6173 290a 2020 2020 2020 2020  ef(pas).        
-0002b8b0: 6172 6332 203d 2044 7465 6d70 2e61 6464  arc2 = Dtemp.add
+0002a5c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a5d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a5e0: 3d0a 2320 4578 616d 706c 6520 636f 6465  =.# Example code
+0002a5f0: 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .# =============
+0002a600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002a640: 3d0a 0a23 2073 203d 2073 6e73 7064 2877  =..# s = snspd(w
+0002a650: 6972 655f 7769 6474 6820 3d20 302e 322c  ire_width = 0.2,
+0002a660: 2077 6972 655f 7069 7463 6820 3d20 302e   wire_pitch = 0.
+0002a670: 362c 2073 697a 6520 3d20 5b31 302c 335d  6, size = [10,3]
+0002a680: 2c20 7465 726d 696e 616c 735f 7361 6d65  , terminals_same
+0002a690: 5f73 6964 6520 3d20 5472 7565 290a 2320  _side = True).# 
+0002a6a0: 7175 6963 6b70 6c6f 7428 7329 0a0a 2320  quickplot(s)..# 
+0002a6b0: 7320 3d20 736e 7370 6428 7769 7265 5f77  s = snspd(wire_w
+0002a6c0: 6964 7468 203d 2030 2e32 2c20 7769 7265  idth = 0.2, wire
+0002a6d0: 5f70 6974 6368 203d 2030 2e36 2c20 7369  _pitch = 0.6, si
+0002a6e0: 7a65 203d 205b 3130 2c20 4e6f 6e65 5d2c  ze = [10, None],
+0002a6f0: 0a23 2020 2020 2020 2020 2020 6e75 6d5f  .#          num_
+0002a700: 7371 7561 7265 7320 3d20 3130 3030 2c20  squares = 1000, 
+0002a710: 7465 726d 696e 616c 735f 7361 6d65 5f73  terminals_same_s
+0002a720: 6964 6520 3d20 5472 7565 290a 2320 7175  ide = True).# qu
+0002a730: 6963 6b70 6c6f 7428 7329 0a0a 0a64 6566  ickplot(s)...def
+0002a740: 2073 6e73 7064 5f63 616e 6465 6c61 6272   snspd_candelabr
+0002a750: 6128 2020 2320 6e6f 7161 3a20 4339 3031  a(  # noqa: C901
+0002a760: 0a20 2020 2077 6972 655f 7769 6474 683d  .    wire_width=
+0002a770: 302e 3532 2c0a 2020 2020 7769 7265 5f70  0.52,.    wire_p
+0002a780: 6974 6368 3d30 2e35 362c 0a20 2020 2068  itch=0.56,.    h
+0002a790: 6178 6973 3d39 302c 0a20 2020 2076 6178  axis=90,.    vax
+0002a7a0: 6973 3d35 302c 0a20 2020 2065 7175 616c  is=50,.    equal
+0002a7b0: 697a 655f 7061 7468 5f6c 656e 6774 6873  ize_path_lengths
+0002a7c0: 3d46 616c 7365 2c0a 2020 2020 7877 696e  =False,.    xwin
+0002a7d0: 673d 4661 6c73 652c 0a20 2020 206c 6179  g=False,.    lay
+0002a7e0: 6572 3d30 2c0a 293a 0a20 2020 2022 2222  er=0,.):.    """
+0002a7f0: 4372 6561 7465 7320 616e 206f 7074 696d  Creates an optim
+0002a800: 616c 6c79 2d72 6f75 6e64 6564 2053 4e53  ally-rounded SNS
+0002a810: 5044 2077 6974 6820 6c6f 7720 6375 7272  PD with low curr
+0002a820: 656e 7420 6372 6f77 6469 6e67 2061 6e64  ent crowding and
+0002a830: 0a20 2020 2061 7262 7469 7472 6172 696c  .    arbtitraril
+0002a840: 792d 6869 6768 2066 696c 6c20 6661 6374  y-high fill fact
+0002a850: 6f72 2061 7320 6465 7363 7269 6265 6420  or as described 
+0002a860: 6279 2052 6564 6479 2065 742e 2061 6c2e  by Reddy et. al.
+0002a870: 2c0a 2020 2020 4150 4c20 5068 6f74 6f6e  ,.    APL Photon
+0002a880: 6963 7320 372c 2030 3531 3330 3220 2832  ics 7, 051302 (2
+0002a890: 3032 3229 2020 6874 7470 733a 2f2f 646f  022)  https://do
+0002a8a0: 692e 6f72 672f 3130 2e31 3036 332f 352e  i.org/10.1063/5.
+0002a8b0: 3030 3838 3030 370a 0a20 2020 2050 6172  0088007..    Par
+0002a8c0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0002a8d0: 2d2d 2d2d 2d2d 0a20 2020 2077 6972 655f  ------.    wire_
+0002a8e0: 7769 6474 6820 3a20 696e 7420 6f72 2066  width : int or f
+0002a8f0: 6c6f 6174 0a20 2020 2020 2020 2057 6964  loat.        Wid
+0002a900: 7468 206f 6620 7468 6520 7769 7265 2e0a  th of the wire..
+0002a910: 2020 2020 7769 7265 5f70 6974 6368 203a      wire_pitch :
+0002a920: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
+0002a930: 2020 2020 2020 4469 7374 616e 6365 2062        Distance b
+0002a940: 6574 7765 656e 2074 776f 2061 646a 6163  etween two adjac
+0002a950: 656e 7420 7769 7265 732e 204d 7573 7420  ent wires. Must 
+0002a960: 6265 2067 7265 6174 6572 2074 6861 6e20  be greater than 
+0002a970: 6077 6964 7468 602e 0a20 2020 2068 6178  `width`..    hax
+0002a980: 6973 203a 2069 6e74 206f 7220 666c 6f61  is : int or floa
+0002a990: 740a 2020 2020 2020 2020 4c65 6e67 7468  t.        Length
+0002a9a0: 206f 6620 686f 7269 7a6f 6e74 616c 2064   of horizontal d
+0002a9b0: 6961 676f 6e61 6c20 6f66 2074 6865 2072  iagonal of the r
+0002a9c0: 686f 6d62 6f69 6461 6c20 6163 7469 7665  homboidal active
+0002a9d0: 2061 7265 612e 0a20 2020 2020 2020 2054   area..        T
+0002a9e0: 6865 2070 6172 616d 6574 6572 2060 6861  he parameter `ha
+0002a9f0: 7869 7360 2069 7320 7072 696f 7269 7469  xis` is prioriti
+0002aa00: 7a65 6420 6f76 6572 2060 7661 7869 7360  zed over `vaxis`
+0002aa10: 2e0a 2020 2020 7661 7869 7320 3a20 696e  ..    vaxis : in
+0002aa20: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
+0002aa30: 2020 204c 656e 6774 6820 6f66 2076 6572     Length of ver
+0002aa40: 7469 6361 6c20 6469 6167 6f6e 616c 206f  tical diagonal o
+0002aa50: 6620 7468 6520 7268 6f6d 626f 6964 616c  f the rhomboidal
+0002aa60: 2061 6374 6976 6520 6172 6561 2e0a 2020   active area..  
+0002aa70: 2020 6571 7561 6c69 7a65 5f70 6174 685f    equalize_path_
+0002aa80: 6c65 6e67 7468 7320 3a20 626f 6f6c 0a20  lengths : bool. 
+0002aa90: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+0002aaa0: 6164 6473 2077 6972 6520 7365 676d 656e  adds wire segmen
+0002aab0: 7473 2074 6f20 6861 6972 7069 6e20 6265  ts to hairpin be
+0002aac0: 6e64 7320 746f 2065 7175 616c 697a 6520  nds to equalize 
+0002aad0: 7061 7468 206c 656e 6774 6873 0a20 2020  path lengths.   
+0002aae0: 2020 2020 2066 726f 6d20 6365 6e74 6572       from center
+0002aaf0: 2074 6f20 6365 6e74 6572 2066 6f72 2061   to center for a
+0002ab00: 6c6c 2070 6172 616c 6c65 6c20 7769 7265  ll parallel wire
+0002ab10: 7320 696e 2061 6374 6976 6520 6172 6561  s in active area
+0002ab20: 2e0a 2020 2020 7877 696e 6720 3a20 626f  ..    xwing : bo
+0002ab30: 6f6c 0a20 2020 2020 2020 2049 6620 5472  ol.        If Tr
+0002ab40: 7565 2c20 7265 706c 6163 6573 2039 302d  ue, replaces 90-
+0002ab50: 6465 6772 6565 2062 656e 6473 2077 6974  degree bends wit
+0002ab60: 6820 3133 352d 6465 6772 6565 2062 656e  h 135-degree ben
+0002ab70: 6473 2e0a 2020 2020 6c61 7965 7220 3a20  ds..    layer : 
+0002ab80: 696e 740a 2020 2020 2020 2020 5370 6563  int.        Spec
+0002ab90: 6966 6963 206c 6179 6572 2074 6f20 7075  ific layer to pu
+0002aba0: 7420 706f 6c79 676f 6e20 6765 6f6d 6574  t polygon geomet
+0002abb0: 7279 206f 6e2e 0a0a 2020 2020 5265 7475  ry on...    Retu
+0002abc0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0002abd0: 2020 2020 4420 3a20 4465 7669 6365 0a20      D : Device. 
+0002abe0: 2020 2020 2020 2041 2044 6576 6963 6520         A Device 
+0002abf0: 636f 6e74 6169 6e69 6e67 2061 6e20 6f70  containing an op
+0002ac00: 7469 6d61 6c6c 792d 726f 756e 6465 6420  timally-rounded 
+0002ac10: 534e 5350 4420 7769 7468 206d 696e 696d  SNSPD with minim
+0002ac20: 697a 6564 2063 7572 7265 6e74 0a20 2020  ized current.   
+0002ac30: 2020 2020 2063 726f 7764 696e 6720 666f       crowding fo
+0002ac40: 7220 616e 7920 6669 6c6c 2066 6163 746f  r any fill facto
+0002ac50: 722e 0a20 2020 2022 2222 0a0a 2020 2020  r..    """..    
+0002ac60: 6465 6620 6f66 665f 6178 6973 5f75 7475  def off_axis_utu
+0002ac70: 726e 280a 2020 2020 2020 2020 7769 7265  rn(.        wire
+0002ac80: 5f77 6964 7468 3d30 2e35 322c 0a20 2020  _width=0.52,.   
+0002ac90: 2020 2020 2077 6972 655f 7069 7463 683d       wire_pitch=
+0002aca0: 302e 3536 2c0a 2020 2020 2020 2020 7066  0.56,.        pf
+0002acb0: 6163 743d 3130 2e30 202f 2033 2c0a 2020  act=10.0 / 3,.  
+0002acc0: 2020 2020 2020 7368 6172 703d 4661 6c73        sharp=Fals
+0002acd0: 652c 0a20 2020 2020 2020 2070 6164 5f6c  e,.        pad_l
+0002ace0: 656e 6774 683d 302c 0a20 2020 2020 2020  ength=0,.       
+0002acf0: 206c 6179 6572 3d30 2c0a 2020 2020 293a   layer=0,.    ):
+0002ad00: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0002ad10: 726e 7320 7068 6964 6c20 6465 7669 6365  rns phidl device
+0002ad20: 206c 6f77 2d63 726f 7764 696e 6720 752d   low-crowding u-
+0002ad30: 7475 726e 2066 6f72 2063 616e 6465 6c61  turn for candela
+0002ad40: 6272 6120 6d65 616e 6465 722e 2222 220a  bra meander.""".
+0002ad50: 2020 2020 2020 2020 6261 7263 203d 206f          barc = o
+0002ad60: 7074 696d 616c 5f39 3064 6567 2877 6964  ptimal_90deg(wid
+0002ad70: 7468 3d77 6972 655f 7769 6474 682c 206c  th=wire_width, l
+0002ad80: 6179 6572 3d6c 6179 6572 290a 2020 2020  ayer=layer).    
+0002ad90: 2020 2020 6966 206e 6f74 2073 6861 7270      if not sharp
+0002ada0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0002adb0: 466f 7220 6e6f 6e2d 726f 756e 6465 6420  For non-rounded 
+0002adc0: 6f75 7465 7220 7261 6469 690a 2020 2020  outer radii.    
+0002add0: 2020 2020 2020 2020 2320 4e6f 7420 6675          # Not fu
+0002ade0: 6c6c 7920 696d 706c 656d 656e 7465 640a  lly implemented.
+0002adf0: 2020 2020 2020 2020 2020 2020 706f 7274              port
+0002ae00: 316d 7020 3d20 5b62 6172 632e 706f 7274  1mp = [barc.port
+0002ae10: 735b 315d 2e78 2c20 6261 7263 2e70 6f72  s[1].x, barc.por
+0002ae20: 7473 5b31 5d2e 795d 0a20 2020 2020 2020  ts[1].y].       
+0002ae30: 2020 2020 2070 6f72 7431 6f72 203d 2062       port1or = b
+0002ae40: 6172 632e 706f 7274 735b 315d 2e6f 7269  arc.ports[1].ori
+0002ae50: 656e 7461 7469 6f6e 0a20 2020 2020 2020  entation.       
+0002ae60: 2020 2020 2070 6f72 7432 6d70 203d 205b       port2mp = [
+0002ae70: 6261 7263 2e70 6f72 7473 5b32 5d2e 782c  barc.ports[2].x,
+0002ae80: 2062 6172 632e 706f 7274 735b 325d 2e79   barc.ports[2].y
+0002ae90: 5d0a 2020 2020 2020 2020 2020 2020 706f  ].            po
+0002aea0: 7274 326f 7220 3d20 6261 7263 2e70 6f72  rt2or = barc.por
+0002aeb0: 7473 5b32 5d2e 6f72 6965 6e74 6174 696f  ts[2].orientatio
+0002aec0: 6e0a 2020 2020 2020 2020 2020 2020 6261  n.            ba
+0002aed0: 7263 203d 2062 6f6f 6c65 616e 280a 2020  rc = boolean(.  
+0002aee0: 2020 2020 2020 2020 2020 2020 2020 413d                A=
+0002aef0: 6261 7263 2c0a 2020 2020 2020 2020 2020  barc,.          
+0002af00: 2020 2020 2020 423d 636f 7079 2862 6172        B=copy(bar
+0002af10: 6329 2e6d 6f76 6528 5b2d 7769 7265 5f77  c).move([-wire_w
+0002af20: 6964 7468 2c20 2d77 6972 655f 7769 6474  idth, -wire_widt
+0002af30: 685d 292c 0a20 2020 2020 2020 2020 2020  h]),.           
+0002af40: 2020 2020 206f 7065 7261 7469 6f6e 3d22       operation="
+0002af50: 6e6f 7422 2c0a 2020 2020 2020 2020 2020  not",.          
+0002af60: 2020 2020 2020 6c61 7965 723d 6c61 7965        layer=laye
+0002af70: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
+0002af80: 0a20 2020 2020 2020 2020 2020 2062 6172  .            bar
+0002af90: 632e 6164 645f 706f 7274 280a 2020 2020  c.add_port(.    
+0002afa0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0002afb0: 3d31 2c20 6d69 6470 6f69 6e74 3d70 6f72  =1, midpoint=por
+0002afc0: 7431 6d70 2c20 7769 6474 683d 7769 7265  t1mp, width=wire
+0002afd0: 5f77 6964 7468 2c20 6f72 6965 6e74 6174  _width, orientat
+0002afe0: 696f 6e3d 706f 7274 316f 720a 2020 2020  ion=port1or.    
+0002aff0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002b000: 2020 2020 2020 6261 7263 2e61 6464 5f70        barc.add_p
+0002b010: 6f72 7428 0a20 2020 2020 2020 2020 2020  ort(.           
+0002b020: 2020 2020 206e 616d 653d 322c 206d 6964       name=2, mid
+0002b030: 706f 696e 743d 706f 7274 326d 702c 2077  point=port2mp, w
+0002b040: 6964 7468 3d77 6972 655f 7769 6474 682c  idth=wire_width,
+0002b050: 206f 7269 656e 7461 7469 6f6e 3d70 6f72   orientation=por
+0002b060: 7432 6f72 0a20 2020 2020 2020 2020 2020  t2or.           
+0002b070: 2029 0a20 2020 2020 2020 2070 696e 203d   ).        pin =
+0002b080: 206f 7074 696d 616c 5f68 6169 7270 696e   optimal_hairpin
+0002b090: 280a 2020 2020 2020 2020 2020 2020 7769  (.            wi
+0002b0a0: 6474 683d 7769 7265 5f77 6964 7468 2c0a  dth=wire_width,.
+0002b0b0: 2020 2020 2020 2020 2020 2020 7069 7463              pitc
+0002b0c0: 683d 7066 6163 7420 2a20 7769 7265 5f77  h=pfact * wire_w
+0002b0d0: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
+0002b0e0: 2020 6c65 6e67 7468 3d38 202a 2077 6972    length=8 * wir
+0002b0f0: 655f 7769 6474 682c 0a20 2020 2020 2020  e_width,.       
+0002b100: 2020 2020 206c 6179 6572 3d6c 6179 6572       layer=layer
+0002b110: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0002b120: 2020 2020 7061 7320 3d20 636f 6d70 6173      pas = compas
+0002b130: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
+0002b140: 7468 2c20 7769 7265 5f70 6974 6368 292c  th, wire_pitch),
+0002b150: 206c 6179 6572 3d6c 6179 6572 290a 2020   layer=layer).  
+0002b160: 2020 2020 2020 4420 3d20 4465 7669 6365        D = Device
+0002b170: 2829 0a20 2020 2020 2020 2061 7263 3120  ().        arc1 
+0002b180: 3d20 442e 6164 645f 7265 6628 6261 7263  = D.add_ref(barc
+0002b190: 290a 2020 2020 2020 2020 6172 6331 2e72  ).        arc1.r
+0002b1a0: 6f74 6174 6528 3930 290a 2020 2020 2020  otate(90).      
+0002b1b0: 2020 7069 6e31 203d 2044 2e61 6464 5f72    pin1 = D.add_r
+0002b1c0: 6566 2870 696e 290a 2020 2020 2020 2020  ef(pin).        
+0002b1d0: 7069 6e31 2e63 6f6e 6e65 6374 2831 2c20  pin1.connect(1, 
+0002b1e0: 6172 6331 2e70 6f72 7473 5b32 5d29 0a20  arc1.ports[2]). 
+0002b1f0: 2020 2020 2020 2070 6173 3120 3d20 442e         pas1 = D.
+0002b200: 6164 645f 7265 6628 7061 7329 0a20 2020  add_ref(pas).   
+0002b210: 2020 2020 2070 6173 312e 636f 6e6e 6563       pas1.connec
+0002b220: 7428 7061 7331 2e70 6f72 7473 5b22 4e22  t(pas1.ports["N"
+0002b230: 5d2c 2070 696e 312e 706f 7274 735b 325d  ], pin1.ports[2]
+0002b240: 290a 2020 2020 2020 2020 6172 6332 203d  ).        arc2 =
+0002b250: 2044 2e61 6464 5f72 6566 2862 6172 6329   D.add_ref(barc)
+0002b260: 0a20 2020 2020 2020 2061 7263 322e 636f  .        arc2.co
+0002b270: 6e6e 6563 7428 322c 2070 6173 312e 706f  nnect(2, pas1.po
+0002b280: 7274 735b 2253 225d 290a 2020 2020 2020  rts["S"]).      
+0002b290: 2020 6966 2070 6164 5f6c 656e 6774 6820    if pad_length 
+0002b2a0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+0002b2b0: 2070 696e 312e 6d6f 7665 7928 7061 645f   pin1.movey(pad_
+0002b2c0: 6c65 6e67 7468 202a 2030 2e35 290a 2020  length * 0.5).  
+0002b2d0: 2020 2020 2020 2020 2020 7465 6d70 6320            tempc 
+0002b2e0: 3d20 442e 6164 645f 7265 6628 0a20 2020  = D.add_ref(.   
+0002b2f0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0002b300: 7061 7373 280a 2020 2020 2020 2020 2020  pass(.          
+0002b310: 2020 2020 2020 2020 2020 7369 7a65 3d28            size=(
+0002b320: 7069 6e31 2e70 6f72 7473 5b31 5d2e 7769  pin1.ports[1].wi
+0002b330: 6474 682c 2070 696e 312e 706f 7274 735b  dth, pin1.ports[
+0002b340: 315d 2e79 202d 2061 7263 312e 706f 7274  1].y - arc1.port
+0002b350: 735b 325d 2e79 292c 0a20 2020 2020 2020  s[2].y),.       
+0002b360: 2020 2020 2020 2020 2020 2020 206c 6179               lay
+0002b370: 6572 3d6c 6179 6572 2c0a 2020 2020 2020  er=layer,.      
+0002b380: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002b390: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002b3a0: 2020 2020 2020 7465 6d70 632e 636f 6e6e        tempc.conn
+0002b3b0: 6563 7428 224e 222c 2070 696e 312e 706f  ect("N", pin1.po
+0002b3c0: 7274 735b 315d 290a 2020 2020 2020 2020  rts[1]).        
+0002b3d0: 2020 2020 7465 6d70 6320 3d20 442e 6164      tempc = D.ad
+0002b3e0: 645f 7265 6628 0a20 2020 2020 2020 2020  d_ref(.         
+0002b3f0: 2020 2020 2020 2063 6f6d 7061 7373 280a         compass(.
+0002b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b410: 2020 2020 7369 7a65 3d28 7069 6e31 2e70      size=(pin1.p
+0002b420: 6f72 7473 5b32 5d2e 7769 6474 682c 2070  orts[2].width, p
+0002b430: 696e 312e 706f 7274 735b 325d 2e79 202d  in1.ports[2].y -
+0002b440: 2070 6173 312e 706f 7274 735b 224e 225d   pas1.ports["N"]
+0002b450: 2e79 292c 0a20 2020 2020 2020 2020 2020  .y),.           
+0002b460: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
+0002b470: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+0002b480: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002b490: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0002b4a0: 2020 7465 6d70 632e 636f 6e6e 6563 7428    tempc.connect(
+0002b4b0: 224e 222c 2070 696e 312e 706f 7274 735b  "N", pin1.ports[
+0002b4c0: 325d 290a 2020 2020 2020 2020 442e 6164  2]).        D.ad
+0002b4d0: 645f 706f 7274 280a 2020 2020 2020 2020  d_port(.        
+0002b4e0: 2020 2020 6e61 6d65 3d31 2c0a 2020 2020      name=1,.    
+0002b4f0: 2020 2020 2020 2020 6d69 6470 6f69 6e74          midpoint
+0002b500: 3d61 7263 312e 706f 7274 735b 315d 2e6d  =arc1.ports[1].m
+0002b510: 6964 706f 696e 742c 0a20 2020 2020 2020  idpoint,.       
+0002b520: 2020 2020 2077 6964 7468 3d77 6972 655f       width=wire_
+0002b530: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
+0002b540: 2020 206f 7269 656e 7461 7469 6f6e 3d61     orientation=a
+0002b550: 7263 312e 706f 7274 735b 315d 2e6f 7269  rc1.ports[1].ori
+0002b560: 656e 7461 7469 6f6e 2c0a 2020 2020 2020  entation,.      
+0002b570: 2020 290a 2020 2020 2020 2020 442e 6164    ).        D.ad
+0002b580: 645f 706f 7274 280a 2020 2020 2020 2020  d_port(.        
+0002b590: 2020 2020 6e61 6d65 3d32 2c0a 2020 2020      name=2,.    
+0002b5a0: 2020 2020 2020 2020 6d69 6470 6f69 6e74          midpoint
+0002b5b0: 3d61 7263 322e 706f 7274 735b 315d 2e6d  =arc2.ports[1].m
+0002b5c0: 6964 706f 696e 742c 0a20 2020 2020 2020  idpoint,.       
+0002b5d0: 2020 2020 2077 6964 7468 3d77 6972 655f       width=wire_
+0002b5e0: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
+0002b5f0: 2020 206f 7269 656e 7461 7469 6f6e 3d61     orientation=a
+0002b600: 7263 322e 706f 7274 735b 315d 2e6f 7269  rc2.ports[1].ori
+0002b610: 656e 7461 7469 6f6e 2c0a 2020 2020 2020  entation,.      
+0002b620: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0002b630: 726e 2044 0a0a 2020 2020 6465 6620 7877  rn D..    def xw
+0002b640: 696e 675f 7574 7572 6e28 0a20 2020 2020  ing_uturn(.     
+0002b650: 2020 2077 6972 655f 7769 6474 683d 302e     wire_width=0.
+0002b660: 3532 2c20 7769 7265 5f70 6974 6368 3d30  52, wire_pitch=0
+0002b670: 2e35 362c 2070 6661 6374 3d31 302e 3020  .56, pfact=10.0 
+0002b680: 2f20 332c 2070 6164 5f6c 656e 6774 683d  / 3, pad_length=
+0002b690: 302c 206c 6179 6572 3d30 0a20 2020 2029  0, layer=0.    )
+0002b6a0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+0002b6b0: 7572 6e73 2070 6869 646c 2064 6576 6963  urns phidl devic
+0002b6c0: 6520 6c6f 772d 6372 6f77 6469 6e67 2075  e low-crowding u
+0002b6d0: 2d74 7572 6e20 666f 7220 582d 7769 6e67  -turn for X-wing
+0002b6e0: 206d 6561 6e64 6572 2e22 2222 0a20 2020   meander.""".   
+0002b6f0: 2020 2020 2062 6172 6320 3d20 6172 6328       barc = arc(
+0002b700: 0a20 2020 2020 2020 2020 2020 2072 6164  .            rad
+0002b710: 6975 733d 7769 7265 5f77 6964 7468 202a  ius=wire_width *
+0002b720: 2033 2c20 7769 6474 683d 7769 7265 5f77   3, width=wire_w
+0002b730: 6964 7468 2c20 6c61 7965 723d 6c61 7965  idth, layer=laye
+0002b740: 722c 2074 6865 7461 3d34 350a 2020 2020  r, theta=45.    
+0002b750: 2020 2020 292e 726f 7461 7465 2831 3830      ).rotate(180
+0002b760: 290a 0a20 2020 2020 2020 2070 696e 203d  )..        pin =
+0002b770: 206f 7074 696d 616c 5f68 6169 7270 696e   optimal_hairpin
+0002b780: 280a 2020 2020 2020 2020 2020 2020 7769  (.            wi
+0002b790: 6474 683d 7769 7265 5f77 6964 7468 2c0a  dth=wire_width,.
+0002b7a0: 2020 2020 2020 2020 2020 2020 7069 7463              pitc
+0002b7b0: 683d 7066 6163 7420 2a20 7769 7265 5f77  h=pfact * wire_w
+0002b7c0: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
+0002b7d0: 2020 6c65 6e67 7468 3d31 3520 2a20 7769    length=15 * wi
+0002b7e0: 7265 5f77 6964 7468 2c0a 2020 2020 2020  re_width,.      
+0002b7f0: 2020 2020 2020 6c61 7965 723d 6c61 7965        layer=laye
+0002b800: 722c 0a20 2020 2020 2020 2029 0a0a 2020  r,.        )..  
+0002b810: 2020 2020 2020 7061 736c 656e 203d 2070        paslen = p
+0002b820: 6661 6374 202a 2077 6972 655f 7769 6474  fact * wire_widt
+0002b830: 6820 2d20 6e70 2e73 7172 7428 3229 202a  h - np.sqrt(2) *
+0002b840: 2077 6972 655f 7069 7463 680a 2020 2020   wire_pitch.    
+0002b850: 2020 2020 7061 7320 3d20 636f 6d70 6173      pas = compas
+0002b860: 7328 7369 7a65 3d28 7769 7265 5f77 6964  s(size=(wire_wid
+0002b870: 7468 2c20 6162 7328 7061 736c 656e 2929  th, abs(paslen))
+0002b880: 2c20 6c61 7965 723d 6c61 7965 7229 0a20  , layer=layer). 
+0002b890: 2020 2020 2020 2044 7465 6d70 203d 2044         Dtemp = D
+0002b8a0: 6576 6963 6528 290a 2020 2020 2020 2020  evice().        
+0002b8b0: 6172 6331 203d 2044 7465 6d70 2e61 6464  arc1 = Dtemp.add
 0002b8c0: 5f72 6566 2862 6172 6329 0a20 2020 2020  _ref(barc).     
-0002b8d0: 2020 2069 6620 7061 736c 656e 203e 2030     if paslen > 0
-0002b8e0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-0002b8f0: 7331 2e63 6f6e 6e65 6374 2870 6173 312e  s1.connect(pas1.
-0002b900: 706f 7274 735b 2253 225d 2c20 6172 6331  ports["S"], arc1
-0002b910: 2e70 6f72 7473 5b32 5d29 0a20 2020 2020  .ports[2]).     
-0002b920: 2020 2020 2020 2070 696e 312e 636f 6e6e         pin1.conn
-0002b930: 6563 7428 312c 2070 6173 312e 706f 7274  ect(1, pas1.port
-0002b940: 735b 224e 225d 290a 2020 2020 2020 2020  s["N"]).        
-0002b950: 2020 2020 6172 6332 2e63 6f6e 6e65 6374      arc2.connect
-0002b960: 2832 2c20 7069 6e31 2e70 6f72 7473 5b32  (2, pin1.ports[2
-0002b970: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-0002b980: 0a20 2020 2020 2020 2020 2020 2070 696e  .            pin
-0002b990: 312e 636f 6e6e 6563 7428 312c 2061 7263  1.connect(1, arc
-0002b9a0: 312e 706f 7274 735b 325d 290a 2020 2020  1.ports[2]).    
-0002b9b0: 2020 2020 2020 2020 7061 7331 2e63 6f6e          pas1.con
-0002b9c0: 6e65 6374 2822 4e22 2c20 7069 6e31 2e70  nect("N", pin1.p
-0002b9d0: 6f72 7473 5b32 5d29 0a20 2020 2020 2020  orts[2]).       
-0002b9e0: 2020 2020 2061 7263 322e 636f 6e6e 6563       arc2.connec
-0002b9f0: 7428 322c 2070 6173 312e 706f 7274 735b  t(2, pas1.ports[
-0002ba00: 2253 225d 290a 2020 2020 2020 2020 6966  "S"]).        if
-0002ba10: 2070 6164 5f6c 656e 6774 6820 3e20 303a   pad_length > 0:
-0002ba20: 0a20 2020 2020 2020 2020 2020 2070 696e  .            pin
-0002ba30: 312e 6d6f 7665 285b 7061 645f 6c65 6e67  1.move([pad_leng
-0002ba40: 7468 202a 2030 2e35 202f 206e 702e 7371  th * 0.5 / np.sq
-0002ba50: 7274 2832 292c 2070 6164 5f6c 656e 6774  rt(2), pad_lengt
-0002ba60: 6820 2a20 302e 3520 2f20 6e70 2e73 7172  h * 0.5 / np.sqr
-0002ba70: 7428 3229 5d29 0a20 2020 2020 2020 2020  t(2)]).         
-0002ba80: 2020 2069 6620 7061 736c 656e 203e 2030     if paslen > 0
-0002ba90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002baa0: 2020 696e 6478 3120 3d20 320a 2020 2020    indx1 = 2.    
-0002bab0: 2020 2020 2020 2020 2020 2020 696e 6478              indx
-0002bac0: 3220 3d20 310a 2020 2020 2020 2020 2020  2 = 1.          
-0002bad0: 2020 2020 2020 6d79 6172 6320 3d20 6172        myarc = ar
-0002bae0: 6332 0a20 2020 2020 2020 2020 2020 2065  c2.            e
-0002baf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0002bb00: 2020 2020 2069 6e64 7831 203d 2031 0a20       indx1 = 1. 
-0002bb10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002bb20: 6e64 7832 203d 2032 0a20 2020 2020 2020  ndx2 = 2.       
-0002bb30: 2020 2020 2020 2020 206d 7961 7263 203d           myarc =
-0002bb40: 2061 7263 310a 2020 2020 2020 2020 2020   arc1.          
-0002bb50: 2020 636f 6d70 6469 7374 203d 206e 702e    compdist = np.
-0002bb60: 7371 7274 280a 2020 2020 2020 2020 2020  sqrt(.          
-0002bb70: 2020 2020 2020 6e70 2e73 756d 286e 702e        np.sum(np.
-0002bb80: 7371 7561 7265 2870 696e 312e 706f 7274  square(pin1.port
-0002bb90: 735b 696e 6478 315d 2e6d 6964 706f 696e  s[indx1].midpoin
-0002bba0: 7420 2d20 6d79 6172 632e 706f 7274 735b  t - myarc.ports[
-0002bbb0: 325d 2e6d 6964 706f 696e 7429 290a 2020  2].midpoint)).  
-0002bbc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0002bbd0: 2020 2020 2020 2020 7465 6d70 6320 3d20          tempc = 
-0002bbe0: 4474 656d 702e 6164 645f 7265 6628 0a20  Dtemp.add_ref(. 
-0002bbf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002bc00: 6f6d 7061 7373 2873 697a 653d 2870 696e  ompass(size=(pin
-0002bc10: 312e 706f 7274 735b 696e 6478 315d 2e77  1.ports[indx1].w
-0002bc20: 6964 7468 2c20 636f 6d70 6469 7374 292c  idth, compdist),
-0002bc30: 206c 6179 6572 3d6c 6179 6572 290a 2020   layer=layer).  
-0002bc40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0002bc50: 2020 2020 2020 2020 7465 6d70 632e 636f          tempc.co
-0002bc60: 6e6e 6563 7428 224e 222c 2070 696e 312e  nnect("N", pin1.
-0002bc70: 706f 7274 735b 696e 6478 315d 290a 2020  ports[indx1]).  
-0002bc80: 2020 2020 2020 2020 2020 636f 6d70 6469            compdi
-0002bc90: 7374 203d 206e 702e 7371 7274 280a 2020  st = np.sqrt(.  
-0002bca0: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-0002bcb0: 2e73 756d 286e 702e 7371 7561 7265 2870  .sum(np.square(p
-0002bcc0: 696e 312e 706f 7274 735b 696e 6478 325d  in1.ports[indx2]
-0002bcd0: 2e6d 6964 706f 696e 7420 2d20 7061 7331  .midpoint - pas1
-0002bce0: 2e70 6f72 7473 5b22 4e22 5d2e 6d69 6470  .ports["N"].midp
-0002bcf0: 6f69 6e74 2929 0a20 2020 2020 2020 2020  oint)).         
-0002bd00: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002bd10: 2074 656d 7063 203d 2044 7465 6d70 2e61   tempc = Dtemp.a
-0002bd20: 6464 5f72 6566 280a 2020 2020 2020 2020  dd_ref(.        
-0002bd30: 2020 2020 2020 2020 636f 6d70 6173 7328          compass(
-0002bd40: 7369 7a65 3d28 7069 6e31 2e70 6f72 7473  size=(pin1.ports
-0002bd50: 5b69 6e64 7832 5d2e 7769 6474 682c 2063  [indx2].width, c
-0002bd60: 6f6d 7064 6973 7429 2c20 6c61 7965 723d  ompdist), layer=
-0002bd70: 6c61 7965 7229 0a20 2020 2020 2020 2020  layer).         
-0002bd80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002bd90: 2074 656d 7063 2e63 6f6e 6e65 6374 2822   tempc.connect("
-0002bda0: 4e22 2c20 7069 6e31 2e70 6f72 7473 5b69  N", pin1.ports[i
-0002bdb0: 6e64 7832 5d29 0a0a 2020 2020 2020 2020  ndx2])..        
-0002bdc0: 4474 656d 702e 6164 645f 706f 7274 280a  Dtemp.add_port(.
-0002bdd0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0002bde0: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-0002bdf0: 6d69 6470 6f69 6e74 3d61 7263 312e 706f  midpoint=arc1.po
-0002be00: 7274 735b 315d 2e6d 6964 706f 696e 742c  rts[1].midpoint,
-0002be10: 0a20 2020 2020 2020 2020 2020 2077 6964  .            wid
-0002be20: 7468 3d77 6972 655f 7769 6474 682c 0a20  th=wire_width,. 
-0002be30: 2020 2020 2020 2020 2020 206f 7269 656e             orien
-0002be40: 7461 7469 6f6e 3d61 7263 312e 706f 7274  tation=arc1.port
-0002be50: 735b 315d 2e6f 7269 656e 7461 7469 6f6e  s[1].orientation
-0002be60: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0002be70: 2020 2020 4474 656d 702e 6164 645f 706f      Dtemp.add_po
-0002be80: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-0002be90: 6e61 6d65 3d32 2c0a 2020 2020 2020 2020  name=2,.        
-0002bea0: 2020 2020 6d69 6470 6f69 6e74 3d61 7263      midpoint=arc
-0002beb0: 322e 706f 7274 735b 315d 2e6d 6964 706f  2.ports[1].midpo
-0002bec0: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-0002bed0: 2077 6964 7468 3d77 6972 655f 7769 6474   width=wire_widt
-0002bee0: 682c 0a20 2020 2020 2020 2020 2020 206f  h,.            o
-0002bef0: 7269 656e 7461 7469 6f6e 3d61 7263 322e  rientation=arc2.
-0002bf00: 706f 7274 735b 315d 2e6f 7269 656e 7461  ports[1].orienta
-0002bf10: 7469 6f6e 2c0a 2020 2020 2020 2020 290a  tion,.        ).
-0002bf20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002bf30: 4474 656d 700a 0a20 2020 2044 203d 2044  Dtemp..    D = D
-0002bf40: 6576 6963 6528 6e61 6d65 3d22 736e 7370  evice(name="snsp
-0002bf50: 645f 6361 6e64 656c 6162 7261 2229 0a20  d_candelabra"). 
-0002bf60: 2020 2069 6620 7877 696e 673a 0a20 2020     if xwing:.   
-0002bf70: 2020 2020 2044 7465 6d70 203d 2078 7769       Dtemp = xwi
-0002bf80: 6e67 5f75 7475 726e 2877 6972 655f 7769  ng_uturn(wire_wi
-0002bf90: 6474 683d 7769 7265 5f77 6964 7468 2c20  dth=wire_width, 
-0002bfa0: 7769 7265 5f70 6974 6368 3d77 6972 655f  wire_pitch=wire_
-0002bfb0: 7069 7463 682c 206c 6179 6572 3d6c 6179  pitch, layer=lay
-0002bfc0: 6572 290a 2020 2020 656c 7365 3a0a 2020  er).    else:.  
-0002bfd0: 2020 2020 2020 4474 656d 7020 3d20 6f66        Dtemp = of
-0002bfe0: 665f 6178 6973 5f75 7475 726e 280a 2020  f_axis_uturn(.  
-0002bff0: 2020 2020 2020 2020 2020 7769 7265 5f77            wire_w
-0002c000: 6964 7468 3d77 6972 655f 7769 6474 682c  idth=wire_width,
-0002c010: 2077 6972 655f 7069 7463 683d 7769 7265   wire_pitch=wire
-0002c020: 5f70 6974 6368 2c20 6c61 7965 723d 6c61  _pitch, layer=la
-0002c030: 7965 720a 2020 2020 2020 2020 290a 2020  yer.        ).  
-0002c040: 2020 4474 656d 705f 6d69 7272 6f72 6564    Dtemp_mirrored
-0002c050: 203d 2064 6565 7063 6f70 7928 4474 656d   = deepcopy(Dtem
-0002c060: 7029 2e6d 6972 726f 7228 5b30 2c20 305d  p).mirror([0, 0]
-0002c070: 2c20 5b30 2c20 315d 290a 2020 2020 7061  , [0, 1]).    pa
-0002c080: 6464 696e 6720 3d20 4474 656d 702e 7873  dding = Dtemp.xs
-0002c090: 697a 650a 2020 2020 6d61 786c 6c20 3d20  ize.    maxll = 
-0002c0a0: 6861 7869 7320 2d20 3220 2a20 7061 6464  haxis - 2 * padd
-0002c0b0: 696e 670a 2020 2020 646c 6c20 3d20 6162  ing.    dll = ab
-0002c0c0: 7328 4474 656d 702e 706f 7274 735b 315d  s(Dtemp.ports[1]
-0002c0d0: 2e78 202d 2044 7465 6d70 2e70 6f72 7473  .x - Dtemp.ports
-0002c0e0: 5b32 5d2e 7829 202b 2077 6972 655f 7069  [2].x) + wire_pi
-0002c0f0: 7463 680a 2020 2020 6861 6c66 5f6e 756d  tch.    half_num
-0002c100: 5f6d 6561 6e64 6572 7320 3d20 696e 7428  _meanders = int(
-0002c110: 6e70 2e63 6569 6c28 302e 3520 2a20 7661  np.ceil(0.5 * va
-0002c120: 7869 7320 2f20 7769 7265 5f70 6974 6368  xis / wire_pitch
-0002c130: 2929 202b 2032 0a0a 2020 2020 6966 2078  )) + 2..    if x
-0002c140: 7769 6e67 3a0a 2020 2020 2020 2020 6265  wing:.        be
-0002c150: 6e64 203d 2044 2e61 6464 5f72 6566 280a  nd = D.add_ref(.
-0002c160: 2020 2020 2020 2020 2020 2020 6172 6328              arc(
-0002c170: 7261 6469 7573 3d77 6972 655f 7769 6474  radius=wire_widt
-0002c180: 6820 2a20 332c 2077 6964 7468 3d77 6972  h * 3, width=wir
-0002c190: 655f 7769 6474 682c 2074 6865 7461 3d39  e_width, theta=9
-0002c1a0: 302c 206c 6179 6572 3d6c 6179 6572 290a  0, layer=layer).
-0002c1b0: 2020 2020 2020 2020 292e 726f 7461 7465          ).rotate
-0002c1c0: 2831 3830 290a 2020 2020 656c 7365 3a0a  (180).    else:.
-0002c1d0: 2020 2020 2020 2020 6265 6e64 203d 2044          bend = D
-0002c1e0: 2e61 6464 5f72 6566 286f 7074 696d 616c  .add_ref(optimal
-0002c1f0: 5f39 3064 6567 2877 6964 7468 3d77 6972  _90deg(width=wir
-0002c200: 655f 7769 6474 682c 206c 6179 6572 3d6c  e_width, layer=l
-0002c210: 6179 6572 2929 0a20 2020 2069 6620 286d  ayer)).    if (m
-0002c220: 6178 6c6c 202d 2064 6c6c 202a 2068 616c  axll - dll * hal
-0002c230: 665f 6e75 6d5f 6d65 616e 6465 7273 2920  f_num_meanders) 
-0002c240: 3c3d 2030 2e30 3a0a 2020 2020 2020 2020  <= 0.0:.        
-0002c250: 7768 696c 6520 286d 6178 6c6c 202d 2064  while (maxll - d
-0002c260: 6c6c 202a 2068 616c 665f 6e75 6d5f 6d65  ll * half_num_me
-0002c270: 616e 6465 7273 2920 3c3d 2030 2e30 3a0a  anders) <= 0.0:.
-0002c280: 2020 2020 2020 2020 2020 2020 6861 6c66              half
-0002c290: 5f6e 756d 5f6d 6561 6e64 6572 7320 3d20  _num_meanders = 
-0002c2a0: 6861 6c66 5f6e 756d 5f6d 6561 6e64 6572  half_num_meander
-0002c2b0: 7320 2d20 310a 2020 2020 6670 6173 203d  s - 1.    fpas =
-0002c2c0: 2044 2e61 6464 5f72 6566 280a 2020 2020   D.add_ref(.    
-0002c2d0: 2020 2020 636f 6d70 6173 7328 7369 7a65      compass(size
-0002c2e0: 3d28 302e 3520 2a20 286d 6178 6c6c 202d  =(0.5 * (maxll -
-0002c2f0: 2064 6c6c 202a 2068 616c 665f 6e75 6d5f   dll * half_num_
-0002c300: 6d65 616e 6465 7273 292c 2077 6972 655f  meanders), wire_
-0002c310: 7769 6474 6829 2c20 6c61 7965 723d 6c61  width), layer=la
-0002c320: 7965 7229 0a20 2020 2029 0a20 2020 2044  yer).    ).    D
-0002c330: 2e6d 6f76 6578 282d 6265 6e64 2e70 6f72  .movex(-bend.por
-0002c340: 7473 5b31 5d2e 7829 0a20 2020 2066 7061  ts[1].x).    fpa
-0002c350: 732e 636f 6e6e 6563 7428 6670 6173 2e70  s.connect(fpas.p
-0002c360: 6f72 7473 5b22 5722 5d2c 2062 656e 642e  orts["W"], bend.
-0002c370: 706f 7274 735b 325d 290a 2020 2020 6c6c  ports[2]).    ll
-0002c380: 203d 2044 2e78 7369 7a65 202a 2032 202d   = D.xsize * 2 -
-0002c390: 2077 6972 655f 7769 6474 680a 2020 2020   wire_width.    
-0002c3a0: 6966 2065 7175 616c 697a 655f 7061 7468  if equalize_path
-0002c3b0: 5f6c 656e 6774 6873 3a0a 2020 2020 2020  _lengths:.      
-0002c3c0: 2020 6966 2078 7769 6e67 3a0a 2020 2020    if xwing:.    
-0002c3d0: 2020 2020 2020 2020 4474 656d 7020 3d20          Dtemp = 
-0002c3e0: 7877 696e 675f 7574 7572 6e28 0a20 2020  xwing_uturn(.   
-0002c3f0: 2020 2020 2020 2020 2020 2020 2077 6972               wir
-0002c400: 655f 7769 6474 683d 7769 7265 5f77 6964  e_width=wire_wid
-0002c410: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0002c420: 2020 2020 7769 7265 5f70 6974 6368 3d77      wire_pitch=w
-0002c430: 6972 655f 7069 7463 682c 0a20 2020 2020  ire_pitch,.     
-0002c440: 2020 2020 2020 2020 2020 2070 6164 5f6c             pad_l
-0002c450: 656e 6774 683d 286d 6178 6c6c 202d 206c  ength=(maxll - l
-0002c460: 6c20 2d20 646c 6c29 202a 2065 7175 616c  l - dll) * equal
-0002c470: 697a 655f 7061 7468 5f6c 656e 6774 6873  ize_path_lengths
-0002c480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c490: 2020 6c61 7965 723d 6c61 7965 722c 0a20    layer=layer,. 
-0002c4a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002c4b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0002c4c0: 2020 2020 2020 2044 7465 6d70 203d 206f         Dtemp = o
-0002c4d0: 6666 5f61 7869 735f 7574 7572 6e28 0a20  ff_axis_uturn(. 
-0002c4e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0002c4f0: 6972 655f 7769 6474 683d 7769 7265 5f77  ire_width=wire_w
-0002c500: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
-0002c510: 2020 2020 2020 7769 7265 5f70 6974 6368        wire_pitch
-0002c520: 3d77 6972 655f 7069 7463 682c 0a20 2020  =wire_pitch,.   
-0002c530: 2020 2020 2020 2020 2020 2020 2070 6164               pad
-0002c540: 5f6c 656e 6774 683d 286d 6178 6c6c 202d  _length=(maxll -
-0002c550: 206c 6c20 2d20 646c 6c29 202a 2065 7175   ll - dll) * equ
-0002c560: 616c 697a 655f 7061 7468 5f6c 656e 6774  alize_path_lengt
-0002c570: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-0002c580: 2020 2020 6c61 7965 723d 6c61 7965 722c      layer=layer,
-0002c590: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0002c5a0: 2020 2075 7475 726e 203d 2044 2e61 6464     uturn = D.add
-0002c5b0: 5f72 6566 2844 7465 6d70 290a 2020 2020  _ref(Dtemp).    
-0002c5c0: 7574 7572 6e2e 636f 6e6e 6563 7428 312c  uturn.connect(1,
-0002c5d0: 2066 7061 732e 706f 7274 735b 2245 225d   fpas.ports["E"]
-0002c5e0: 290a 2020 2020 6469 725f 6c65 6674 203d  ).    dir_left =
-0002c5f0: 2054 7275 650a 0a20 2020 2074 7572 6e5f   True..    turn_
-0002c600: 7061 6464 696e 6720 3d20 6d61 786c 6c20  padding = maxll 
-0002c610: 2d20 6c6c 202d 2032 202a 2064 6c6c 0a0a  - ll - 2 * dll..
-0002c620: 2020 2020 7768 696c 6520 6c6c 203c 206d      while ll < m
-0002c630: 6178 6c6c 202d 2064 6c6c 3a0a 2020 2020  axll - dll:.    
-0002c640: 2020 2020 6c6c 203d 206c 6c20 2b20 646c      ll = ll + dl
-0002c650: 6c0a 2020 2020 2020 2020 6966 2065 7175  l.        if equ
-0002c660: 616c 697a 655f 7061 7468 5f6c 656e 6774  alize_path_lengt
-0002c670: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
-0002c680: 6966 2078 7769 6e67 3a0a 2020 2020 2020  if xwing:.      
-0002c690: 2020 2020 2020 2020 2020 4474 656d 7020            Dtemp 
-0002c6a0: 3d20 7877 696e 675f 7574 7572 6e28 0a20  = xwing_uturn(. 
-0002c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c6c0: 2020 2077 6972 655f 7769 6474 683d 7769     wire_width=wi
-0002c6d0: 7265 5f77 6964 7468 2c0a 2020 2020 2020  re_width,.      
-0002c6e0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-0002c6f0: 7265 5f70 6974 6368 3d77 6972 655f 7069  re_pitch=wire_pi
-0002c700: 7463 682c 0a20 2020 2020 2020 2020 2020  tch,.           
-0002c710: 2020 2020 2020 2020 2070 6164 5f6c 656e           pad_len
-0002c720: 6774 683d 7475 726e 5f70 6164 6469 6e67  gth=turn_padding
-0002c730: 202a 2065 7175 616c 697a 655f 7061 7468   * equalize_path
-0002c740: 5f6c 656e 6774 6873 2c0a 2020 2020 2020  _lengths,.      
-0002c750: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0002c760: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
-0002c770: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002c780: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0002c790: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0002c7a0: 7465 6d70 203d 206f 6666 5f61 7869 735f  temp = off_axis_
-0002c7b0: 7574 7572 6e28 0a20 2020 2020 2020 2020  uturn(.         
-0002c7c0: 2020 2020 2020 2020 2020 2077 6972 655f             wire_
-0002c7d0: 7769 6474 683d 7769 7265 5f77 6964 7468  width=wire_width
-0002c7e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c7f0: 2020 2020 2020 7769 7265 5f70 6974 6368        wire_pitch
-0002c800: 3d77 6972 655f 7069 7463 682c 0a20 2020  =wire_pitch,.   
-0002c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c820: 2070 6164 5f6c 656e 6774 683d 7475 726e   pad_length=turn
-0002c830: 5f70 6164 6469 6e67 202a 2065 7175 616c  _padding * equal
-0002c840: 697a 655f 7061 7468 5f6c 656e 6774 6873  ize_path_lengths
-0002c850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c860: 2020 2020 2020 6c61 7965 723d 6c61 7965        layer=laye
-0002c870: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0002c880: 2020 2029 0a20 2020 2020 2020 2074 7572     ).        tur
-0002c890: 6e5f 7061 6464 696e 6720 3d20 7475 726e  n_padding = turn
-0002c8a0: 5f70 6164 6469 6e67 202d 2064 6c6c 0a20  _padding - dll. 
-0002c8b0: 2020 2020 2020 206e 6577 7061 7320 3d20         newpas = 
-0002c8c0: 442e 6164 645f 7265 6628 636f 6d70 6173  D.add_ref(compas
-0002c8d0: 7328 7369 7a65 3d28 6c6c 2c20 7769 7265  s(size=(ll, wire
-0002c8e0: 5f77 6964 7468 292c 206c 6179 6572 3d6c  _width), layer=l
-0002c8f0: 6179 6572 2929 0a20 2020 2020 2020 2069  ayer)).        i
-0002c900: 6620 6469 725f 6c65 6674 3a0a 2020 2020  f dir_left:.    
-0002c910: 2020 2020 2020 2020 6e65 7770 6173 2e63          newpas.c
-0002c920: 6f6e 6e65 6374 286e 6577 7061 732e 706f  onnect(newpas.po
-0002c930: 7274 735b 2245 225d 2c20 7574 7572 6e2e  rts["E"], uturn.
-0002c940: 706f 7274 735b 325d 290a 2020 2020 2020  ports[2]).      
-0002c950: 2020 2020 2020 6966 2065 7175 616c 697a        if equaliz
-0002c960: 655f 7061 7468 5f6c 656e 6774 6873 3a0a  e_path_lengths:.
-0002c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c980: 7574 7572 6e20 3d20 442e 6164 645f 7265  uturn = D.add_re
-0002c990: 6628 4474 656d 702e 6d69 7272 6f72 285b  f(Dtemp.mirror([
-0002c9a0: 302c 2030 5d2c 205b 302c 2031 5d29 290a  0, 0], [0, 1])).
-0002c9b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0002c9c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002c9d0: 2020 7574 7572 6e20 3d20 442e 6164 645f    uturn = D.add_
-0002c9e0: 7265 6628 4474 656d 705f 6d69 7272 6f72  ref(Dtemp_mirror
-0002c9f0: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-0002ca00: 7574 7572 6e2e 636f 6e6e 6563 7428 312c  uturn.connect(1,
-0002ca10: 206e 6577 7061 732e 706f 7274 735b 2257   newpas.ports["W
-0002ca20: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-0002ca30: 6469 725f 6c65 6674 203d 2046 616c 7365  dir_left = False
-0002ca40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0002ca50: 2020 2020 2020 2020 2020 206e 6577 7061             newpa
-0002ca60: 732e 636f 6e6e 6563 7428 6e65 7770 6173  s.connect(newpas
-0002ca70: 2e70 6f72 7473 5b22 5722 5d2c 2075 7475  .ports["W"], utu
-0002ca80: 726e 2e70 6f72 7473 5b32 5d29 0a20 2020  rn.ports[2]).   
-0002ca90: 2020 2020 2020 2020 2075 7475 726e 203d           uturn =
-0002caa0: 2044 2e61 6464 5f72 6566 2844 7465 6d70   D.add_ref(Dtemp
-0002cab0: 290a 2020 2020 2020 2020 2020 2020 7574  ).            ut
-0002cac0: 7572 6e2e 636f 6e6e 6563 7428 312c 206e  urn.connect(1, n
-0002cad0: 6577 7061 732e 706f 7274 735b 2245 225d  ewpas.ports["E"]
-0002cae0: 290a 2020 2020 2020 2020 2020 2020 6469  ).            di
-0002caf0: 725f 6c65 6674 203d 2054 7275 650a 0a20  r_left = True.. 
-0002cb00: 2020 206e 6577 7061 7320 3d20 442e 6164     newpas = D.ad
-0002cb10: 645f 7265 6628 636f 6d70 6173 7328 7369  d_ref(compass(si
-0002cb20: 7a65 3d28 6c6c 202f 2032 2c20 7769 7265  ze=(ll / 2, wire
-0002cb30: 5f77 6964 7468 292c 206c 6179 6572 3d6c  _width), layer=l
-0002cb40: 6179 6572 2929 0a20 2020 2069 6620 6469  ayer)).    if di
-0002cb50: 725f 6c65 6674 3a0a 2020 2020 2020 2020  r_left:.        
-0002cb60: 6e65 7770 6173 2e63 6f6e 6e65 6374 286e  newpas.connect(n
-0002cb70: 6577 7061 732e 706f 7274 735b 2245 225d  ewpas.ports["E"]
-0002cb80: 2c20 7574 7572 6e2e 706f 7274 735b 325d  , uturn.ports[2]
-0002cb90: 290a 2020 2020 2020 2020 6469 725f 6c65  ).        dir_le
-0002cba0: 6674 203d 2046 616c 7365 0a20 2020 2065  ft = False.    e
-0002cbb0: 6c73 653a 0a20 2020 2020 2020 206e 6577  lse:.        new
-0002cbc0: 7061 732e 636f 6e6e 6563 7428 6e65 7770  pas.connect(newp
-0002cbd0: 6173 2e70 6f72 7473 5b22 5722 5d2c 2075  as.ports["W"], u
-0002cbe0: 7475 726e 2e70 6f72 7473 5b32 5d29 0a20  turn.ports[2]). 
-0002cbf0: 2020 2020 2020 2064 6972 5f6c 6566 7420         dir_left 
-0002cc00: 3d20 5472 7565 0a0a 2020 2020 442e 6d6f  = True..    D.mo
-0002cc10: 7665 7828 2d44 2e78 290a 2020 2020 6966  vex(-D.x).    if
-0002cc20: 206e 6f74 2078 7769 6e67 3a0a 2020 2020   not xwing:.    
-0002cc30: 2020 2020 6265 6e64 2e6d 6f76 6578 282d      bend.movex(-
-0002cc40: 6265 6e64 2e70 6f72 7473 5b31 5d2e 7829  bend.ports[1].x)
-0002cc50: 0a20 2020 2069 6620 2866 7061 732e 706f  .    if (fpas.po
-0002cc60: 7274 735b 2257 225d 2e78 202d 2062 656e  rts["W"].x - ben
-0002cc70: 642e 706f 7274 735b 325d 2e78 2920 3e20  d.ports[2].x) > 
-0002cc80: 303a 0a20 2020 2020 2020 2074 656d 7063  0:.        tempc
-0002cc90: 203d 2044 2e61 6464 5f72 6566 280a 2020   = D.add_ref(.  
-0002cca0: 2020 2020 2020 2020 2020 636f 6d70 6173            compas
-0002ccb0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-0002ccc0: 2020 2073 697a 653d 2866 7061 732e 706f     size=(fpas.po
-0002ccd0: 7274 735b 2257 225d 2e78 202d 2062 656e  rts["W"].x - ben
-0002cce0: 642e 706f 7274 735b 325d 2e78 2c20 6265  d.ports[2].x, be
-0002ccf0: 6e64 2e70 6f72 7473 5b32 5d2e 7769 6474  nd.ports[2].widt
-0002cd00: 6829 2c0a 2020 2020 2020 2020 2020 2020  h),.            
-0002cd10: 2020 2020 6c61 7965 723d 6c61 7965 722c      layer=layer,
-0002cd20: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0002cd30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002cd40: 2074 656d 7063 2e63 6f6e 6e65 6374 2822   tempc.connect("
-0002cd50: 4522 2c20 6670 6173 2e70 6f72 7473 5b22  E", fpas.ports["
-0002cd60: 5722 5d29 0a20 2020 2044 2e6d 6f76 6528  W"]).    D.move(
-0002cd70: 5b2d 442e 782c 202d 442e 796d 696e 202d  [-D.x, -D.ymin -
-0002cd80: 2077 6972 655f 7769 6474 6820 2a20 302e   wire_width * 0.
-0002cd90: 355d 290a 2020 2020 442e 6164 645f 706f  5]).    D.add_po
-0002cda0: 7274 286e 616d 653d 312c 2070 6f72 743d  rt(name=1, port=
-0002cdb0: 6265 6e64 2e70 6f72 7473 5b31 5d29 0a20  bend.ports[1]). 
-0002cdc0: 2020 2069 6620 6469 725f 6c65 6674 3a0a     if dir_left:.
-0002cdd0: 2020 2020 2020 2020 442e 6164 645f 706f          D.add_po
-0002cde0: 7274 286e 616d 653d 322c 2070 6f72 743d  rt(name=2, port=
-0002cdf0: 6e65 7770 6173 2e70 6f72 7473 5b22 4522  newpas.ports["E"
-0002ce00: 5d29 0a20 2020 2065 6c73 653a 0a20 2020  ]).    else:.   
-0002ce10: 2020 2020 2044 2e61 6464 5f70 6f72 7428       D.add_port(
-0002ce20: 6e61 6d65 3d32 2c20 706f 7274 3d6e 6577  name=2, port=new
-0002ce30: 7061 732e 706f 7274 735b 2257 225d 290a  pas.ports["W"]).
-0002ce40: 0a20 2020 2044 6f75 7420 3d20 4465 7669  .    Dout = Devi
-0002ce50: 6365 2829 0a20 2020 2044 3120 3d20 446f  ce().    D1 = Do
-0002ce60: 7574 2e61 6464 5f72 6566 2844 290a 2020  ut.add_ref(D).  
-0002ce70: 2020 4432 203d 2044 6f75 742e 6164 645f    D2 = Dout.add_
-0002ce80: 7265 6628 636f 7079 2844 292e 726f 7461  ref(copy(D).rota
-0002ce90: 7465 2831 3830 2929 0a20 2020 2074 656d  te(180)).    tem
-0002cea0: 7063 203d 2044 6f75 742e 6164 645f 7265  pc = Dout.add_re
-0002ceb0: 6628 0a20 2020 2020 2020 2063 6f6d 7061  f(.        compa
-0002cec0: 7373 280a 2020 2020 2020 2020 2020 2020  ss(.            
-0002ced0: 7369 7a65 3d28 6162 7328 4431 2e70 6f72  size=(abs(D1.por
-0002cee0: 7473 5b32 5d2e 7820 2d20 4432 2e70 6f72  ts[2].x - D2.por
-0002cef0: 7473 5b32 5d2e 7829 2c20 4431 2e70 6f72  ts[2].x), D1.por
-0002cf00: 7473 5b32 5d2e 7769 6474 6829 2c20 6c61  ts[2].width), la
-0002cf10: 7965 723d 6c61 7965 720a 2020 2020 2020  yer=layer.      
-0002cf20: 2020 290a 2020 2020 290a 2020 2020 6966    ).    ).    if
-0002cf30: 2044 312e 706f 7274 735b 325d 2e78 203e   D1.ports[2].x >
-0002cf40: 2044 322e 706f 7274 735b 325d 2e78 3a0a   D2.ports[2].x:.
-0002cf50: 2020 2020 2020 2020 7465 6d70 632e 636f          tempc.co
-0002cf60: 6e6e 6563 7428 2245 222c 2044 312e 706f  nnect("E", D1.po
-0002cf70: 7274 735b 325d 290a 2020 2020 656c 7365  rts[2]).    else
-0002cf80: 3a0a 2020 2020 2020 2020 7465 6d70 632e  :.        tempc.
-0002cf90: 636f 6e6e 6563 7428 2257 222c 2044 312e  connect("W", D1.
-0002cfa0: 706f 7274 735b 325d 290a 2020 2020 446f  ports[2]).    Do
-0002cfb0: 7574 2e61 6464 5f70 6f72 7428 6e61 6d65  ut.add_port(name
-0002cfc0: 3d31 2c20 706f 7274 3d44 312e 706f 7274  =1, port=D1.port
-0002cfd0: 735b 315d 290a 2020 2020 446f 7574 2e61  s[1]).    Dout.a
-0002cfe0: 6464 5f70 6f72 7428 6e61 6d65 3d32 2c20  dd_port(name=2, 
-0002cff0: 706f 7274 3d44 322e 706f 7274 735b 315d  port=D2.ports[1]
-0002d000: 290a 2020 2020 7265 7475 726e 2044 6f75  ).    return Dou
-0002d010: 740a 0a0a 6465 6620 7974 726f 6e5f 726f  t...def ytron_ro
-0002d020: 756e 6428 0a20 2020 2072 686f 3d31 2c0a  und(.    rho=1,.
-0002d030: 2020 2020 6172 6d5f 6c65 6e67 7468 733d      arm_lengths=
-0002d040: 2835 3030 2c20 3330 3029 2c0a 2020 2020  (500, 300),.    
-0002d050: 736f 7572 6365 5f6c 656e 6774 683d 3530  source_length=50
-0002d060: 302c 0a20 2020 2061 726d 5f77 6964 7468  0,.    arm_width
-0002d070: 733d 2832 3030 2c20 3230 3029 2c0a 2020  s=(200, 200),.  
-0002d080: 2020 7468 6574 613d 322e 352c 0a20 2020    theta=2.5,.   
-0002d090: 2074 6865 7461 5f72 6573 6f6c 7574 696f   theta_resolutio
-0002d0a0: 6e3d 3130 2c0a 2020 2020 6c61 7965 723d  n=10,.    layer=
-0002d0b0: 302c 0a29 3a0a 2020 2020 2222 2259 7472  0,.):.    """Ytr
-0002d0c0: 6f6e 2073 7472 7563 7475 7265 2066 6f72  on structure for
-0002d0d0: 2073 7570 6572 636f 6e64 7563 7469 6e67   superconducting
-0002d0e0: 206e 616e 6f77 6972 6573 0a0a 2020 2020   nanowires..    
-0002d0f0: 4d63 4361 7567 6861 6e2c 2041 2e20 4e2e  McCaughan, A. N.
-0002d100: 2c20 4162 6562 652c 204e 2e20 532e 2c20  , Abebe, N. S., 
-0002d110: 5a68 616f 2c20 512e 2d59 2e20 2620 4265  Zhao, Q.-Y. & Be
-0002d120: 7267 6772 656e 2c20 4b2e 204b 2e0a 2020  rggren, K. K..  
-0002d130: 2020 5573 696e 6720 4765 6f6d 6574 7279    Using Geometry
-0002d140: 2054 6f20 5365 6e73 6520 4375 7272 656e   To Sense Curren
-0002d150: 742e 204e 616e 6f20 4c65 7474 2e20 3136  t. Nano Lett. 16
-0002d160: 2c20 3736 3236 e280 9337 3633 3120 2832  , 7626...7631 (2
-0002d170: 3031 3629 2e0a 2020 2020 6874 7470 3a2f  016)..    http:/
-0002d180: 2f64 782e 646f 692e 6f72 672f 3130 2e31  /dx.doi.org/10.1
-0002d190: 3032 312f 6163 732e 6e61 6e6f 6c65 7474  021/acs.nanolett
-0002d1a0: 2e36 6230 3335 3933 0a0a 2020 2020 5061  .6b03593..    Pa
-0002d1b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0002d1c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7268 6f20  -------.    rho 
-0002d1d0: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
-0002d1e0: 2020 2020 2020 2052 6164 6975 7320 6f66         Radius of
-0002d1f0: 2063 7572 7661 7475 7265 206f 6620 7974   curvature of yt
-0002d200: 726f 6e20 696e 7465 7273 6563 7469 6f6e  ron intersection
-0002d210: 2070 6f69 6e74 0a20 2020 2061 726d 5f6c   point.    arm_l
-0002d220: 656e 6774 6873 203a 2061 7272 6179 2d6c  engths : array-l
-0002d230: 696b 655b 325d 206f 6620 696e 7420 6f72  ike[2] of int or
-0002d240: 2066 6c6f 6174 0a20 2020 2020 2020 204c   float.        L
-0002d250: 656e 6774 6873 206f 6620 7468 6520 6c65  engths of the le
-0002d260: 6674 2061 6e64 2072 6967 6874 2061 726d  ft and right arm
-0002d270: 7320 6f66 2074 6865 2079 5472 6f6e 2c20  s of the yTron, 
-0002d280: 7265 7370 6563 7469 7665 6c79 2e0a 2020  respectively..  
-0002d290: 2020 736f 7572 6365 5f6c 656e 6774 6820    source_length 
-0002d2a0: 3a20 696e 7420 6f72 2066 6c6f 6174 0a20  : int or float. 
-0002d2b0: 2020 2020 2020 204c 656e 6774 6820 6f66         Length of
-0002d2c0: 2074 6865 2073 6f75 7263 6520 6f66 2074   the source of t
-0002d2d0: 6865 2079 5472 6f6e 2e0a 2020 2020 6172  he yTron..    ar
-0002d2e0: 6d5f 7769 6474 6873 203a 2061 7272 6179  m_widths : array
-0002d2f0: 2d6c 696b 655b 325d 206f 6620 696e 7420  -like[2] of int 
-0002d300: 6f72 2066 6c6f 6174 0a20 2020 2020 2020  or float.       
-0002d310: 2057 6964 7468 7320 6f66 2074 6865 206c   Widths of the l
-0002d320: 6566 7420 616e 6420 7269 6768 7420 6172  eft and right ar
-0002d330: 6d73 206f 6620 7468 6520 7954 726f 6e2c  ms of the yTron,
-0002d340: 2072 6573 7065 6374 6976 656c 792e 0a20   respectively.. 
-0002d350: 2020 2074 6865 7461 203a 2069 6e74 206f     theta : int o
-0002d360: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
-0002d370: 416e 676c 6520 6265 7477 6565 6e20 7468  Angle between th
-0002d380: 6520 7477 6f20 7954 726f 6e20 6172 6d73  e two yTron arms
-0002d390: 2e0a 2020 2020 7468 6574 615f 7265 736f  ..    theta_reso
-0002d3a0: 6c75 7469 6f6e 203a 2069 6e74 206f 7220  lution : int or 
-0002d3b0: 666c 6f61 740a 2020 2020 2020 2020 416e  float.        An
-0002d3c0: 676c 6520 7265 736f 6c75 7469 6f6e 2066  gle resolution f
-0002d3d0: 6f72 2063 7572 7661 7475 7265 206f 6620  or curvature of 
-0002d3e0: 7974 726f 6e20 696e 7465 7273 6563 7469  ytron intersecti
-0002d3f0: 6f6e 2070 6f69 6e74 0a20 2020 206c 6179  on point.    lay
-0002d400: 6572 203a 2069 6e74 2c20 6172 7261 792d  er : int, array-
-0002d410: 6c69 6b65 5b32 5d2c 206f 7220 7365 740a  like[2], or set.
-0002d420: 2020 2020 2020 2020 5370 6563 6966 6963          Specific
-0002d430: 206c 6179 6572 2873 2920 746f 2070 7574   layer(s) to put
-0002d440: 2070 6f6c 7967 6f6e 2067 656f 6d65 7472   polygon geometr
-0002d450: 7920 6f6e 2e0a 0a20 2020 2052 6574 7572  y on...    Retur
-0002d460: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0002d470: 2020 2044 203a 2044 6576 6963 650a 2020     D : Device.  
-0002d480: 2020 2020 2020 4120 4465 7669 6365 2063        A Device c
-0002d490: 6f6e 7461 696e 696e 6720 6120 7954 726f  ontaining a yTro
-0002d4a0: 6e20 6765 6f6d 6574 7279 2e0a 2020 2020  n geometry..    
-0002d4b0: 2222 220a 2020 2020 2320 3d3d 3d3d 3d3d  """.    # ======
-0002d4c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002d4d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002d4e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002d4f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002d500: 3d3d 3d3d 0a20 2020 2023 2020 4372 6561  ====.    #  Crea
-0002d510: 7465 2074 6865 2062 6173 6963 2067 656f  te the basic geo
-0002d520: 6d65 7472 790a 2020 2020 2320 3d3d 3d3d  metry.    # ====
-0002d530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002b8d0: 2020 2061 7263 312e 726f 7461 7465 2839     arc1.rotate(9
+0002b8e0: 3029 0a20 2020 2020 2020 2070 696e 3120  0).        pin1 
+0002b8f0: 3d20 4474 656d 702e 6164 645f 7265 6628  = Dtemp.add_ref(
+0002b900: 7069 6e29 0a20 2020 2020 2020 2070 6173  pin).        pas
+0002b910: 3120 3d20 4474 656d 702e 6164 645f 7265  1 = Dtemp.add_re
+0002b920: 6628 7061 7329 0a20 2020 2020 2020 2061  f(pas).        a
+0002b930: 7263 3220 3d20 4474 656d 702e 6164 645f  rc2 = Dtemp.add_
+0002b940: 7265 6628 6261 7263 290a 2020 2020 2020  ref(barc).      
+0002b950: 2020 6966 2070 6173 6c65 6e20 3e20 303a    if paslen > 0:
+0002b960: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+0002b970: 312e 636f 6e6e 6563 7428 7061 7331 2e70  1.connect(pas1.p
+0002b980: 6f72 7473 5b22 5322 5d2c 2061 7263 312e  orts["S"], arc1.
+0002b990: 706f 7274 735b 325d 290a 2020 2020 2020  ports[2]).      
+0002b9a0: 2020 2020 2020 7069 6e31 2e63 6f6e 6e65        pin1.conne
+0002b9b0: 6374 2831 2c20 7061 7331 2e70 6f72 7473  ct(1, pas1.ports
+0002b9c0: 5b22 4e22 5d29 0a20 2020 2020 2020 2020  ["N"]).         
+0002b9d0: 2020 2061 7263 322e 636f 6e6e 6563 7428     arc2.connect(
+0002b9e0: 322c 2070 696e 312e 706f 7274 735b 325d  2, pin1.ports[2]
+0002b9f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0002ba00: 2020 2020 2020 2020 2020 2020 7069 6e31              pin1
+0002ba10: 2e63 6f6e 6e65 6374 2831 2c20 6172 6331  .connect(1, arc1
+0002ba20: 2e70 6f72 7473 5b32 5d29 0a20 2020 2020  .ports[2]).     
+0002ba30: 2020 2020 2020 2070 6173 312e 636f 6e6e         pas1.conn
+0002ba40: 6563 7428 224e 222c 2070 696e 312e 706f  ect("N", pin1.po
+0002ba50: 7274 735b 325d 290a 2020 2020 2020 2020  rts[2]).        
+0002ba60: 2020 2020 6172 6332 2e63 6f6e 6e65 6374      arc2.connect
+0002ba70: 2832 2c20 7061 7331 2e70 6f72 7473 5b22  (2, pas1.ports["
+0002ba80: 5322 5d29 0a20 2020 2020 2020 2069 6620  S"]).        if 
+0002ba90: 7061 645f 6c65 6e67 7468 203e 2030 3a0a  pad_length > 0:.
+0002baa0: 2020 2020 2020 2020 2020 2020 7069 6e31              pin1
+0002bab0: 2e6d 6f76 6528 5b70 6164 5f6c 656e 6774  .move([pad_lengt
+0002bac0: 6820 2a20 302e 3520 2f20 6e70 2e73 7172  h * 0.5 / np.sqr
+0002bad0: 7428 3229 2c20 7061 645f 6c65 6e67 7468  t(2), pad_length
+0002bae0: 202a 2030 2e35 202f 206e 702e 7371 7274   * 0.5 / np.sqrt
+0002baf0: 2832 295d 290a 2020 2020 2020 2020 2020  (2)]).          
+0002bb00: 2020 6966 2070 6173 6c65 6e20 3e20 303a    if paslen > 0:
+0002bb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bb20: 2069 6e64 7831 203d 2032 0a20 2020 2020   indx1 = 2.     
+0002bb30: 2020 2020 2020 2020 2020 2069 6e64 7832             indx2
+0002bb40: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+0002bb50: 2020 2020 206d 7961 7263 203d 2061 7263       myarc = arc
+0002bb60: 320a 2020 2020 2020 2020 2020 2020 656c  2.            el
+0002bb70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002bb80: 2020 2020 696e 6478 3120 3d20 310a 2020      indx1 = 1.  
+0002bb90: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0002bba0: 6478 3220 3d20 320a 2020 2020 2020 2020  dx2 = 2.        
+0002bbb0: 2020 2020 2020 2020 6d79 6172 6320 3d20          myarc = 
+0002bbc0: 6172 6331 0a20 2020 2020 2020 2020 2020  arc1.           
+0002bbd0: 2063 6f6d 7064 6973 7420 3d20 6e70 2e73   compdist = np.s
+0002bbe0: 7172 7428 0a20 2020 2020 2020 2020 2020  qrt(.           
+0002bbf0: 2020 2020 206e 702e 7375 6d28 6e70 2e73       np.sum(np.s
+0002bc00: 7175 6172 6528 7069 6e31 2e70 6f72 7473  quare(pin1.ports
+0002bc10: 5b69 6e64 7831 5d2e 6d69 6470 6f69 6e74  [indx1].midpoint
+0002bc20: 202d 206d 7961 7263 2e70 6f72 7473 5b32   - myarc.ports[2
+0002bc30: 5d2e 6d69 6470 6f69 6e74 2929 0a20 2020  ].midpoint)).   
+0002bc40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0002bc50: 2020 2020 2020 2074 656d 7063 203d 2044         tempc = D
+0002bc60: 7465 6d70 2e61 6464 5f72 6566 280a 2020  temp.add_ref(.  
+0002bc70: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0002bc80: 6d70 6173 7328 7369 7a65 3d28 7069 6e31  mpass(size=(pin1
+0002bc90: 2e70 6f72 7473 5b69 6e64 7831 5d2e 7769  .ports[indx1].wi
+0002bca0: 6474 682c 2063 6f6d 7064 6973 7429 2c20  dth, compdist), 
+0002bcb0: 6c61 7965 723d 6c61 7965 7229 0a20 2020  layer=layer).   
+0002bcc0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0002bcd0: 2020 2020 2020 2074 656d 7063 2e63 6f6e         tempc.con
+0002bce0: 6e65 6374 2822 4e22 2c20 7069 6e31 2e70  nect("N", pin1.p
+0002bcf0: 6f72 7473 5b69 6e64 7831 5d29 0a20 2020  orts[indx1]).   
+0002bd00: 2020 2020 2020 2020 2063 6f6d 7064 6973           compdis
+0002bd10: 7420 3d20 6e70 2e73 7172 7428 0a20 2020  t = np.sqrt(.   
+0002bd20: 2020 2020 2020 2020 2020 2020 206e 702e               np.
+0002bd30: 7375 6d28 6e70 2e73 7175 6172 6528 7069  sum(np.square(pi
+0002bd40: 6e31 2e70 6f72 7473 5b69 6e64 7832 5d2e  n1.ports[indx2].
+0002bd50: 6d69 6470 6f69 6e74 202d 2070 6173 312e  midpoint - pas1.
+0002bd60: 706f 7274 735b 224e 225d 2e6d 6964 706f  ports["N"].midpo
+0002bd70: 696e 7429 290a 2020 2020 2020 2020 2020  int)).          
+0002bd80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0002bd90: 7465 6d70 6320 3d20 4474 656d 702e 6164  tempc = Dtemp.ad
+0002bda0: 645f 7265 6628 0a20 2020 2020 2020 2020  d_ref(.         
+0002bdb0: 2020 2020 2020 2063 6f6d 7061 7373 2873         compass(s
+0002bdc0: 697a 653d 2870 696e 312e 706f 7274 735b  ize=(pin1.ports[
+0002bdd0: 696e 6478 325d 2e77 6964 7468 2c20 636f  indx2].width, co
+0002bde0: 6d70 6469 7374 292c 206c 6179 6572 3d6c  mpdist), layer=l
+0002bdf0: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+0002be00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0002be10: 7465 6d70 632e 636f 6e6e 6563 7428 224e  tempc.connect("N
+0002be20: 222c 2070 696e 312e 706f 7274 735b 696e  ", pin1.ports[in
+0002be30: 6478 325d 290a 0a20 2020 2020 2020 2044  dx2])..        D
+0002be40: 7465 6d70 2e61 6464 5f70 6f72 7428 0a20  temp.add_port(. 
+0002be50: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+0002be60: 312c 0a20 2020 2020 2020 2020 2020 206d  1,.            m
+0002be70: 6964 706f 696e 743d 6172 6331 2e70 6f72  idpoint=arc1.por
+0002be80: 7473 5b31 5d2e 6d69 6470 6f69 6e74 2c0a  ts[1].midpoint,.
+0002be90: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+0002bea0: 683d 7769 7265 5f77 6964 7468 2c0a 2020  h=wire_width,.  
+0002beb0: 2020 2020 2020 2020 2020 6f72 6965 6e74            orient
+0002bec0: 6174 696f 6e3d 6172 6331 2e70 6f72 7473  ation=arc1.ports
+0002bed0: 5b31 5d2e 6f72 6965 6e74 6174 696f 6e2c  [1].orientation,
+0002bee0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002bef0: 2020 2044 7465 6d70 2e61 6464 5f70 6f72     Dtemp.add_por
+0002bf00: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
+0002bf10: 616d 653d 322c 0a20 2020 2020 2020 2020  ame=2,.         
+0002bf20: 2020 206d 6964 706f 696e 743d 6172 6332     midpoint=arc2
+0002bf30: 2e70 6f72 7473 5b31 5d2e 6d69 6470 6f69  .ports[1].midpoi
+0002bf40: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+0002bf50: 7769 6474 683d 7769 7265 5f77 6964 7468  width=wire_width
+0002bf60: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+0002bf70: 6965 6e74 6174 696f 6e3d 6172 6332 2e70  ientation=arc2.p
+0002bf80: 6f72 7473 5b31 5d2e 6f72 6965 6e74 6174  orts[1].orientat
+0002bf90: 696f 6e2c 0a20 2020 2020 2020 2029 0a0a  ion,.        )..
+0002bfa0: 2020 2020 2020 2020 7265 7475 726e 2044          return D
+0002bfb0: 7465 6d70 0a0a 2020 2020 4420 3d20 4465  temp..    D = De
+0002bfc0: 7669 6365 286e 616d 653d 2273 6e73 7064  vice(name="snspd
+0002bfd0: 5f63 616e 6465 6c61 6272 6122 290a 2020  _candelabra").  
+0002bfe0: 2020 6966 2078 7769 6e67 3a0a 2020 2020    if xwing:.    
+0002bff0: 2020 2020 4474 656d 7020 3d20 7877 696e      Dtemp = xwin
+0002c000: 675f 7574 7572 6e28 7769 7265 5f77 6964  g_uturn(wire_wid
+0002c010: 7468 3d77 6972 655f 7769 6474 682c 2077  th=wire_width, w
+0002c020: 6972 655f 7069 7463 683d 7769 7265 5f70  ire_pitch=wire_p
+0002c030: 6974 6368 2c20 6c61 7965 723d 6c61 7965  itch, layer=laye
+0002c040: 7229 0a20 2020 2065 6c73 653a 0a20 2020  r).    else:.   
+0002c050: 2020 2020 2044 7465 6d70 203d 206f 6666       Dtemp = off
+0002c060: 5f61 7869 735f 7574 7572 6e28 0a20 2020  _axis_uturn(.   
+0002c070: 2020 2020 2020 2020 2077 6972 655f 7769           wire_wi
+0002c080: 6474 683d 7769 7265 5f77 6964 7468 2c20  dth=wire_width, 
+0002c090: 7769 7265 5f70 6974 6368 3d77 6972 655f  wire_pitch=wire_
+0002c0a0: 7069 7463 682c 206c 6179 6572 3d6c 6179  pitch, layer=lay
+0002c0b0: 6572 0a20 2020 2020 2020 2029 0a20 2020  er.        ).   
+0002c0c0: 2044 7465 6d70 5f6d 6972 726f 7265 6420   Dtemp_mirrored 
+0002c0d0: 3d20 6465 6570 636f 7079 2844 7465 6d70  = deepcopy(Dtemp
+0002c0e0: 292e 6d69 7272 6f72 285b 302c 2030 5d2c  ).mirror([0, 0],
+0002c0f0: 205b 302c 2031 5d29 0a20 2020 2070 6164   [0, 1]).    pad
+0002c100: 6469 6e67 203d 2044 7465 6d70 2e78 7369  ding = Dtemp.xsi
+0002c110: 7a65 0a20 2020 206d 6178 6c6c 203d 2068  ze.    maxll = h
+0002c120: 6178 6973 202d 2032 202a 2070 6164 6469  axis - 2 * paddi
+0002c130: 6e67 0a20 2020 2064 6c6c 203d 2061 6273  ng.    dll = abs
+0002c140: 2844 7465 6d70 2e70 6f72 7473 5b31 5d2e  (Dtemp.ports[1].
+0002c150: 7820 2d20 4474 656d 702e 706f 7274 735b  x - Dtemp.ports[
+0002c160: 325d 2e78 2920 2b20 7769 7265 5f70 6974  2].x) + wire_pit
+0002c170: 6368 0a20 2020 2068 616c 665f 6e75 6d5f  ch.    half_num_
+0002c180: 6d65 616e 6465 7273 203d 2069 6e74 286e  meanders = int(n
+0002c190: 702e 6365 696c 2830 2e35 202a 2076 6178  p.ceil(0.5 * vax
+0002c1a0: 6973 202f 2077 6972 655f 7069 7463 6829  is / wire_pitch)
+0002c1b0: 2920 2b20 320a 0a20 2020 2069 6620 7877  ) + 2..    if xw
+0002c1c0: 696e 673a 0a20 2020 2020 2020 2062 656e  ing:.        ben
+0002c1d0: 6420 3d20 442e 6164 645f 7265 6628 0a20  d = D.add_ref(. 
+0002c1e0: 2020 2020 2020 2020 2020 2061 7263 2872             arc(r
+0002c1f0: 6164 6975 733d 7769 7265 5f77 6964 7468  adius=wire_width
+0002c200: 202a 2033 2c20 7769 6474 683d 7769 7265   * 3, width=wire
+0002c210: 5f77 6964 7468 2c20 7468 6574 613d 3930  _width, theta=90
+0002c220: 2c20 6c61 7965 723d 6c61 7965 7229 0a20  , layer=layer). 
+0002c230: 2020 2020 2020 2029 2e72 6f74 6174 6528         ).rotate(
+0002c240: 3138 3029 0a20 2020 2065 6c73 653a 0a20  180).    else:. 
+0002c250: 2020 2020 2020 2062 656e 6420 3d20 442e         bend = D.
+0002c260: 6164 645f 7265 6628 6f70 7469 6d61 6c5f  add_ref(optimal_
+0002c270: 3930 6465 6728 7769 6474 683d 7769 7265  90deg(width=wire
+0002c280: 5f77 6964 7468 2c20 6c61 7965 723d 6c61  _width, layer=la
+0002c290: 7965 7229 290a 2020 2020 6966 2028 6d61  yer)).    if (ma
+0002c2a0: 786c 6c20 2d20 646c 6c20 2a20 6861 6c66  xll - dll * half
+0002c2b0: 5f6e 756d 5f6d 6561 6e64 6572 7329 203c  _num_meanders) <
+0002c2c0: 3d20 302e 303a 0a20 2020 2020 2020 2077  = 0.0:.        w
+0002c2d0: 6869 6c65 2028 6d61 786c 6c20 2d20 646c  hile (maxll - dl
+0002c2e0: 6c20 2a20 6861 6c66 5f6e 756d 5f6d 6561  l * half_num_mea
+0002c2f0: 6e64 6572 7329 203c 3d20 302e 303a 0a20  nders) <= 0.0:. 
+0002c300: 2020 2020 2020 2020 2020 2068 616c 665f             half_
+0002c310: 6e75 6d5f 6d65 616e 6465 7273 203d 2068  num_meanders = h
+0002c320: 616c 665f 6e75 6d5f 6d65 616e 6465 7273  alf_num_meanders
+0002c330: 202d 2031 0a20 2020 2066 7061 7320 3d20   - 1.    fpas = 
+0002c340: 442e 6164 645f 7265 6628 0a20 2020 2020  D.add_ref(.     
+0002c350: 2020 2063 6f6d 7061 7373 2873 697a 653d     compass(size=
+0002c360: 2830 2e35 202a 2028 6d61 786c 6c20 2d20  (0.5 * (maxll - 
+0002c370: 646c 6c20 2a20 6861 6c66 5f6e 756d 5f6d  dll * half_num_m
+0002c380: 6561 6e64 6572 7329 2c20 7769 7265 5f77  eanders), wire_w
+0002c390: 6964 7468 292c 206c 6179 6572 3d6c 6179  idth), layer=lay
+0002c3a0: 6572 290a 2020 2020 290a 2020 2020 442e  er).    ).    D.
+0002c3b0: 6d6f 7665 7828 2d62 656e 642e 706f 7274  movex(-bend.port
+0002c3c0: 735b 315d 2e78 290a 2020 2020 6670 6173  s[1].x).    fpas
+0002c3d0: 2e63 6f6e 6e65 6374 2866 7061 732e 706f  .connect(fpas.po
+0002c3e0: 7274 735b 2257 225d 2c20 6265 6e64 2e70  rts["W"], bend.p
+0002c3f0: 6f72 7473 5b32 5d29 0a20 2020 206c 6c20  orts[2]).    ll 
+0002c400: 3d20 442e 7873 697a 6520 2a20 3220 2d20  = D.xsize * 2 - 
+0002c410: 7769 7265 5f77 6964 7468 0a20 2020 2069  wire_width.    i
+0002c420: 6620 6571 7561 6c69 7a65 5f70 6174 685f  f equalize_path_
+0002c430: 6c65 6e67 7468 733a 0a20 2020 2020 2020  lengths:.       
+0002c440: 2069 6620 7877 696e 673a 0a20 2020 2020   if xwing:.     
+0002c450: 2020 2020 2020 2044 7465 6d70 203d 2078         Dtemp = x
+0002c460: 7769 6e67 5f75 7475 726e 280a 2020 2020  wing_uturn(.    
+0002c470: 2020 2020 2020 2020 2020 2020 7769 7265              wire
+0002c480: 5f77 6964 7468 3d77 6972 655f 7769 6474  _width=wire_widt
+0002c490: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0002c4a0: 2020 2077 6972 655f 7069 7463 683d 7769     wire_pitch=wi
+0002c4b0: 7265 5f70 6974 6368 2c0a 2020 2020 2020  re_pitch,.      
+0002c4c0: 2020 2020 2020 2020 2020 7061 645f 6c65            pad_le
+0002c4d0: 6e67 7468 3d28 6d61 786c 6c20 2d20 6c6c  ngth=(maxll - ll
+0002c4e0: 202d 2064 6c6c 2920 2a20 6571 7561 6c69   - dll) * equali
+0002c4f0: 7a65 5f70 6174 685f 6c65 6e67 7468 732c  ze_path_lengths,
+0002c500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c510: 206c 6179 6572 3d6c 6179 6572 2c0a 2020   layer=layer,.  
+0002c520: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002c530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002c540: 2020 2020 2020 4474 656d 7020 3d20 6f66        Dtemp = of
+0002c550: 665f 6178 6973 5f75 7475 726e 280a 2020  f_axis_uturn(.  
+0002c560: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+0002c570: 7265 5f77 6964 7468 3d77 6972 655f 7769  re_width=wire_wi
+0002c580: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
+0002c590: 2020 2020 2077 6972 655f 7069 7463 683d       wire_pitch=
+0002c5a0: 7769 7265 5f70 6974 6368 2c0a 2020 2020  wire_pitch,.    
+0002c5b0: 2020 2020 2020 2020 2020 2020 7061 645f              pad_
+0002c5c0: 6c65 6e67 7468 3d28 6d61 786c 6c20 2d20  length=(maxll - 
+0002c5d0: 6c6c 202d 2064 6c6c 2920 2a20 6571 7561  ll - dll) * equa
+0002c5e0: 6c69 7a65 5f70 6174 685f 6c65 6e67 7468  lize_path_length
+0002c5f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0002c600: 2020 206c 6179 6572 3d6c 6179 6572 2c0a     layer=layer,.
+0002c610: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002c620: 2020 7574 7572 6e20 3d20 442e 6164 645f    uturn = D.add_
+0002c630: 7265 6628 4474 656d 7029 0a20 2020 2075  ref(Dtemp).    u
+0002c640: 7475 726e 2e63 6f6e 6e65 6374 2831 2c20  turn.connect(1, 
+0002c650: 6670 6173 2e70 6f72 7473 5b22 4522 5d29  fpas.ports["E"])
+0002c660: 0a20 2020 2064 6972 5f6c 6566 7420 3d20  .    dir_left = 
+0002c670: 5472 7565 0a0a 2020 2020 7475 726e 5f70  True..    turn_p
+0002c680: 6164 6469 6e67 203d 206d 6178 6c6c 202d  adding = maxll -
+0002c690: 206c 6c20 2d20 3220 2a20 646c 6c0a 0a20   ll - 2 * dll.. 
+0002c6a0: 2020 2077 6869 6c65 206c 6c20 3c20 6d61     while ll < ma
+0002c6b0: 786c 6c20 2d20 646c 6c3a 0a20 2020 2020  xll - dll:.     
+0002c6c0: 2020 206c 6c20 3d20 6c6c 202b 2064 6c6c     ll = ll + dll
+0002c6d0: 0a20 2020 2020 2020 2069 6620 6571 7561  .        if equa
+0002c6e0: 6c69 7a65 5f70 6174 685f 6c65 6e67 7468  lize_path_length
+0002c6f0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+0002c700: 6620 7877 696e 673a 0a20 2020 2020 2020  f xwing:.       
+0002c710: 2020 2020 2020 2020 2044 7465 6d70 203d           Dtemp =
+0002c720: 2078 7769 6e67 5f75 7475 726e 280a 2020   xwing_uturn(.  
+0002c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c740: 2020 7769 7265 5f77 6964 7468 3d77 6972    wire_width=wir
+0002c750: 655f 7769 6474 682c 0a20 2020 2020 2020  e_width,.       
+0002c760: 2020 2020 2020 2020 2020 2020 2077 6972               wir
+0002c770: 655f 7069 7463 683d 7769 7265 5f70 6974  e_pitch=wire_pit
+0002c780: 6368 2c0a 2020 2020 2020 2020 2020 2020  ch,.            
+0002c790: 2020 2020 2020 2020 7061 645f 6c65 6e67          pad_leng
+0002c7a0: 7468 3d74 7572 6e5f 7061 6464 696e 6720  th=turn_padding 
+0002c7b0: 2a20 6571 7561 6c69 7a65 5f70 6174 685f  * equalize_path_
+0002c7c0: 6c65 6e67 7468 732c 0a20 2020 2020 2020  lengths,.       
+0002c7d0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
+0002c7e0: 6572 3d6c 6179 6572 2c0a 2020 2020 2020  er=layer,.      
+0002c7f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002c800: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002c810: 2020 2020 2020 2020 2020 2020 2020 4474                Dt
+0002c820: 656d 7020 3d20 6f66 665f 6178 6973 5f75  emp = off_axis_u
+0002c830: 7475 726e 280a 2020 2020 2020 2020 2020  turn(.          
+0002c840: 2020 2020 2020 2020 2020 7769 7265 5f77            wire_w
+0002c850: 6964 7468 3d77 6972 655f 7769 6474 682c  idth=wire_width,
+0002c860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c870: 2020 2020 2077 6972 655f 7069 7463 683d       wire_pitch=
+0002c880: 7769 7265 5f70 6974 6368 2c0a 2020 2020  wire_pitch,.    
+0002c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c8a0: 7061 645f 6c65 6e67 7468 3d74 7572 6e5f  pad_length=turn_
+0002c8b0: 7061 6464 696e 6720 2a20 6571 7561 6c69  padding * equali
+0002c8c0: 7a65 5f70 6174 685f 6c65 6e67 7468 732c  ze_path_lengths,
+0002c8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c8e0: 2020 2020 206c 6179 6572 3d6c 6179 6572       layer=layer
+0002c8f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c900: 2020 290a 2020 2020 2020 2020 7475 726e    ).        turn
+0002c910: 5f70 6164 6469 6e67 203d 2074 7572 6e5f  _padding = turn_
+0002c920: 7061 6464 696e 6720 2d20 646c 6c0a 2020  padding - dll.  
+0002c930: 2020 2020 2020 6e65 7770 6173 203d 2044        newpas = D
+0002c940: 2e61 6464 5f72 6566 2863 6f6d 7061 7373  .add_ref(compass
+0002c950: 2873 697a 653d 286c 6c2c 2077 6972 655f  (size=(ll, wire_
+0002c960: 7769 6474 6829 2c20 6c61 7965 723d 6c61  width), layer=la
+0002c970: 7965 7229 290a 2020 2020 2020 2020 6966  yer)).        if
+0002c980: 2064 6972 5f6c 6566 743a 0a20 2020 2020   dir_left:.     
+0002c990: 2020 2020 2020 206e 6577 7061 732e 636f         newpas.co
+0002c9a0: 6e6e 6563 7428 6e65 7770 6173 2e70 6f72  nnect(newpas.por
+0002c9b0: 7473 5b22 4522 5d2c 2075 7475 726e 2e70  ts["E"], uturn.p
+0002c9c0: 6f72 7473 5b32 5d29 0a20 2020 2020 2020  orts[2]).       
+0002c9d0: 2020 2020 2069 6620 6571 7561 6c69 7a65       if equalize
+0002c9e0: 5f70 6174 685f 6c65 6e67 7468 733a 0a20  _path_lengths:. 
+0002c9f0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0002ca00: 7475 726e 203d 2044 2e61 6464 5f72 6566  turn = D.add_ref
+0002ca10: 2844 7465 6d70 2e6d 6972 726f 7228 5b30  (Dtemp.mirror([0
+0002ca20: 2c20 305d 2c20 5b30 2c20 315d 2929 0a20  , 0], [0, 1])). 
+0002ca30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0002ca40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ca50: 2075 7475 726e 203d 2044 2e61 6464 5f72   uturn = D.add_r
+0002ca60: 6566 2844 7465 6d70 5f6d 6972 726f 7265  ef(Dtemp_mirrore
+0002ca70: 6429 0a20 2020 2020 2020 2020 2020 2075  d).            u
+0002ca80: 7475 726e 2e63 6f6e 6e65 6374 2831 2c20  turn.connect(1, 
+0002ca90: 6e65 7770 6173 2e70 6f72 7473 5b22 5722  newpas.ports["W"
+0002caa0: 5d29 0a20 2020 2020 2020 2020 2020 2064  ]).            d
+0002cab0: 6972 5f6c 6566 7420 3d20 4661 6c73 650a  ir_left = False.
+0002cac0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002cad0: 2020 2020 2020 2020 2020 6e65 7770 6173            newpas
+0002cae0: 2e63 6f6e 6e65 6374 286e 6577 7061 732e  .connect(newpas.
+0002caf0: 706f 7274 735b 2257 225d 2c20 7574 7572  ports["W"], utur
+0002cb00: 6e2e 706f 7274 735b 325d 290a 2020 2020  n.ports[2]).    
+0002cb10: 2020 2020 2020 2020 7574 7572 6e20 3d20          uturn = 
+0002cb20: 442e 6164 645f 7265 6628 4474 656d 7029  D.add_ref(Dtemp)
+0002cb30: 0a20 2020 2020 2020 2020 2020 2075 7475  .            utu
+0002cb40: 726e 2e63 6f6e 6e65 6374 2831 2c20 6e65  rn.connect(1, ne
+0002cb50: 7770 6173 2e70 6f72 7473 5b22 4522 5d29  wpas.ports["E"])
+0002cb60: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+0002cb70: 5f6c 6566 7420 3d20 5472 7565 0a0a 2020  _left = True..  
+0002cb80: 2020 6e65 7770 6173 203d 2044 2e61 6464    newpas = D.add
+0002cb90: 5f72 6566 2863 6f6d 7061 7373 2873 697a  _ref(compass(siz
+0002cba0: 653d 286c 6c20 2f20 322c 2077 6972 655f  e=(ll / 2, wire_
+0002cbb0: 7769 6474 6829 2c20 6c61 7965 723d 6c61  width), layer=la
+0002cbc0: 7965 7229 290a 2020 2020 6966 2064 6972  yer)).    if dir
+0002cbd0: 5f6c 6566 743a 0a20 2020 2020 2020 206e  _left:.        n
+0002cbe0: 6577 7061 732e 636f 6e6e 6563 7428 6e65  ewpas.connect(ne
+0002cbf0: 7770 6173 2e70 6f72 7473 5b22 4522 5d2c  wpas.ports["E"],
+0002cc00: 2075 7475 726e 2e70 6f72 7473 5b32 5d29   uturn.ports[2])
+0002cc10: 0a20 2020 2020 2020 2064 6972 5f6c 6566  .        dir_lef
+0002cc20: 7420 3d20 4661 6c73 650a 2020 2020 656c  t = False.    el
+0002cc30: 7365 3a0a 2020 2020 2020 2020 6e65 7770  se:.        newp
+0002cc40: 6173 2e63 6f6e 6e65 6374 286e 6577 7061  as.connect(newpa
+0002cc50: 732e 706f 7274 735b 2257 225d 2c20 7574  s.ports["W"], ut
+0002cc60: 7572 6e2e 706f 7274 735b 325d 290a 2020  urn.ports[2]).  
+0002cc70: 2020 2020 2020 6469 725f 6c65 6674 203d        dir_left =
+0002cc80: 2054 7275 650a 0a20 2020 2044 2e6d 6f76   True..    D.mov
+0002cc90: 6578 282d 442e 7829 0a20 2020 2069 6620  ex(-D.x).    if 
+0002cca0: 6e6f 7420 7877 696e 673a 0a20 2020 2020  not xwing:.     
+0002ccb0: 2020 2062 656e 642e 6d6f 7665 7828 2d62     bend.movex(-b
+0002ccc0: 656e 642e 706f 7274 735b 315d 2e78 290a  end.ports[1].x).
+0002ccd0: 2020 2020 6966 2028 6670 6173 2e70 6f72      if (fpas.por
+0002cce0: 7473 5b22 5722 5d2e 7820 2d20 6265 6e64  ts["W"].x - bend
+0002ccf0: 2e70 6f72 7473 5b32 5d2e 7829 203e 2030  .ports[2].x) > 0
+0002cd00: 3a0a 2020 2020 2020 2020 7465 6d70 6320  :.        tempc 
+0002cd10: 3d20 442e 6164 645f 7265 6628 0a20 2020  = D.add_ref(.   
+0002cd20: 2020 2020 2020 2020 2063 6f6d 7061 7373           compass
+0002cd30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002cd40: 2020 7369 7a65 3d28 6670 6173 2e70 6f72    size=(fpas.por
+0002cd50: 7473 5b22 5722 5d2e 7820 2d20 6265 6e64  ts["W"].x - bend
+0002cd60: 2e70 6f72 7473 5b32 5d2e 782c 2062 656e  .ports[2].x, ben
+0002cd70: 642e 706f 7274 735b 325d 2e77 6964 7468  d.ports[2].width
+0002cd80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0002cd90: 2020 206c 6179 6572 3d6c 6179 6572 2c0a     layer=layer,.
+0002cda0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002cdb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002cdc0: 7465 6d70 632e 636f 6e6e 6563 7428 2245  tempc.connect("E
+0002cdd0: 222c 2066 7061 732e 706f 7274 735b 2257  ", fpas.ports["W
+0002cde0: 225d 290a 2020 2020 442e 6d6f 7665 285b  "]).    D.move([
+0002cdf0: 2d44 2e78 2c20 2d44 2e79 6d69 6e20 2d20  -D.x, -D.ymin - 
+0002ce00: 7769 7265 5f77 6964 7468 202a 2030 2e35  wire_width * 0.5
+0002ce10: 5d29 0a20 2020 2044 2e61 6464 5f70 6f72  ]).    D.add_por
+0002ce20: 7428 6e61 6d65 3d31 2c20 706f 7274 3d62  t(name=1, port=b
+0002ce30: 656e 642e 706f 7274 735b 315d 290a 2020  end.ports[1]).  
+0002ce40: 2020 6966 2064 6972 5f6c 6566 743a 0a20    if dir_left:. 
+0002ce50: 2020 2020 2020 2044 2e61 6464 5f70 6f72         D.add_por
+0002ce60: 7428 6e61 6d65 3d32 2c20 706f 7274 3d6e  t(name=2, port=n
+0002ce70: 6577 7061 732e 706f 7274 735b 2245 225d  ewpas.ports["E"]
+0002ce80: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+0002ce90: 2020 2020 442e 6164 645f 706f 7274 286e      D.add_port(n
+0002cea0: 616d 653d 322c 2070 6f72 743d 6e65 7770  ame=2, port=newp
+0002ceb0: 6173 2e70 6f72 7473 5b22 5722 5d29 0a0a  as.ports["W"])..
+0002cec0: 2020 2020 446f 7574 203d 2044 6576 6963      Dout = Devic
+0002ced0: 6528 290a 2020 2020 4431 203d 2044 6f75  e().    D1 = Dou
+0002cee0: 742e 6164 645f 7265 6628 4429 0a20 2020  t.add_ref(D).   
+0002cef0: 2044 3220 3d20 446f 7574 2e61 6464 5f72   D2 = Dout.add_r
+0002cf00: 6566 2863 6f70 7928 4429 2e72 6f74 6174  ef(copy(D).rotat
+0002cf10: 6528 3138 3029 290a 2020 2020 7465 6d70  e(180)).    temp
+0002cf20: 6320 3d20 446f 7574 2e61 6464 5f72 6566  c = Dout.add_ref
+0002cf30: 280a 2020 2020 2020 2020 636f 6d70 6173  (.        compas
+0002cf40: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
+0002cf50: 697a 653d 2861 6273 2844 312e 706f 7274  ize=(abs(D1.port
+0002cf60: 735b 325d 2e78 202d 2044 322e 706f 7274  s[2].x - D2.port
+0002cf70: 735b 325d 2e78 292c 2044 312e 706f 7274  s[2].x), D1.port
+0002cf80: 735b 325d 2e77 6964 7468 292c 206c 6179  s[2].width), lay
+0002cf90: 6572 3d6c 6179 6572 0a20 2020 2020 2020  er=layer.       
+0002cfa0: 2029 0a20 2020 2029 0a20 2020 2069 6620   ).    ).    if 
+0002cfb0: 4431 2e70 6f72 7473 5b32 5d2e 7820 3e20  D1.ports[2].x > 
+0002cfc0: 4432 2e70 6f72 7473 5b32 5d2e 783a 0a20  D2.ports[2].x:. 
+0002cfd0: 2020 2020 2020 2074 656d 7063 2e63 6f6e         tempc.con
+0002cfe0: 6e65 6374 2822 4522 2c20 4431 2e70 6f72  nect("E", D1.por
+0002cff0: 7473 5b32 5d29 0a20 2020 2065 6c73 653a  ts[2]).    else:
+0002d000: 0a20 2020 2020 2020 2074 656d 7063 2e63  .        tempc.c
+0002d010: 6f6e 6e65 6374 2822 5722 2c20 4431 2e70  onnect("W", D1.p
+0002d020: 6f72 7473 5b32 5d29 0a20 2020 2044 6f75  orts[2]).    Dou
+0002d030: 742e 6164 645f 706f 7274 286e 616d 653d  t.add_port(name=
+0002d040: 312c 2070 6f72 743d 4431 2e70 6f72 7473  1, port=D1.ports
+0002d050: 5b31 5d29 0a20 2020 2044 6f75 742e 6164  [1]).    Dout.ad
+0002d060: 645f 706f 7274 286e 616d 653d 322c 2070  d_port(name=2, p
+0002d070: 6f72 743d 4432 2e70 6f72 7473 5b31 5d29  ort=D2.ports[1])
+0002d080: 0a20 2020 2072 6574 7572 6e20 446f 7574  .    return Dout
+0002d090: 0a0a 0a64 6566 2079 7472 6f6e 5f72 6f75  ...def ytron_rou
+0002d0a0: 6e64 280a 2020 2020 7268 6f3d 312c 0a20  nd(.    rho=1,. 
+0002d0b0: 2020 2061 726d 5f6c 656e 6774 6873 3d28     arm_lengths=(
+0002d0c0: 3530 302c 2033 3030 292c 0a20 2020 2073  500, 300),.    s
+0002d0d0: 6f75 7263 655f 6c65 6e67 7468 3d35 3030  ource_length=500
+0002d0e0: 2c0a 2020 2020 6172 6d5f 7769 6474 6873  ,.    arm_widths
+0002d0f0: 3d28 3230 302c 2032 3030 292c 0a20 2020  =(200, 200),.   
+0002d100: 2074 6865 7461 3d32 2e35 2c0a 2020 2020   theta=2.5,.    
+0002d110: 7468 6574 615f 7265 736f 6c75 7469 6f6e  theta_resolution
+0002d120: 3d31 302c 0a20 2020 206c 6179 6572 3d30  =10,.    layer=0
+0002d130: 2c0a 293a 0a20 2020 2022 2222 5974 726f  ,.):.    """Ytro
+0002d140: 6e20 7374 7275 6374 7572 6520 666f 7220  n structure for 
+0002d150: 7375 7065 7263 6f6e 6475 6374 696e 6720  superconducting 
+0002d160: 6e61 6e6f 7769 7265 730a 0a20 2020 204d  nanowires..    M
+0002d170: 6343 6175 6768 616e 2c20 412e 204e 2e2c  cCaughan, A. N.,
+0002d180: 2041 6265 6265 2c20 4e2e 2053 2e2c 205a   Abebe, N. S., Z
+0002d190: 6861 6f2c 2051 2e2d 592e 2026 2042 6572  hao, Q.-Y. & Ber
+0002d1a0: 6767 7265 6e2c 204b 2e20 4b2e 0a20 2020  ggren, K. K..   
+0002d1b0: 2055 7369 6e67 2047 656f 6d65 7472 7920   Using Geometry 
+0002d1c0: 546f 2053 656e 7365 2043 7572 7265 6e74  To Sense Current
+0002d1d0: 2e20 4e61 6e6f 204c 6574 742e 2031 362c  . Nano Lett. 16,
+0002d1e0: 2037 3632 36e2 8093 3736 3331 2028 3230   7626...7631 (20
+0002d1f0: 3136 292e 0a20 2020 2068 7474 703a 2f2f  16)..    http://
+0002d200: 6478 2e64 6f69 2e6f 7267 2f31 302e 3130  dx.doi.org/10.10
+0002d210: 3231 2f61 6373 2e6e 616e 6f6c 6574 742e  21/acs.nanolett.
+0002d220: 3662 3033 3539 330a 0a20 2020 2050 6172  6b03593..    Par
+0002d230: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0002d240: 2d2d 2d2d 2d2d 0a20 2020 2072 686f 203a  ------.    rho :
+0002d250: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
+0002d260: 2020 2020 2020 5261 6469 7573 206f 6620        Radius of 
+0002d270: 6375 7276 6174 7572 6520 6f66 2079 7472  curvature of ytr
+0002d280: 6f6e 2069 6e74 6572 7365 6374 696f 6e20  on intersection 
+0002d290: 706f 696e 740a 2020 2020 6172 6d5f 6c65  point.    arm_le
+0002d2a0: 6e67 7468 7320 3a20 6172 7261 792d 6c69  ngths : array-li
+0002d2b0: 6b65 5b32 5d20 6f66 2069 6e74 206f 7220  ke[2] of int or 
+0002d2c0: 666c 6f61 740a 2020 2020 2020 2020 4c65  float.        Le
+0002d2d0: 6e67 7468 7320 6f66 2074 6865 206c 6566  ngths of the lef
+0002d2e0: 7420 616e 6420 7269 6768 7420 6172 6d73  t and right arms
+0002d2f0: 206f 6620 7468 6520 7954 726f 6e2c 2072   of the yTron, r
+0002d300: 6573 7065 6374 6976 656c 792e 0a20 2020  espectively..   
+0002d310: 2073 6f75 7263 655f 6c65 6e67 7468 203a   source_length :
+0002d320: 2069 6e74 206f 7220 666c 6f61 740a 2020   int or float.  
+0002d330: 2020 2020 2020 4c65 6e67 7468 206f 6620        Length of 
+0002d340: 7468 6520 736f 7572 6365 206f 6620 7468  the source of th
+0002d350: 6520 7954 726f 6e2e 0a20 2020 2061 726d  e yTron..    arm
+0002d360: 5f77 6964 7468 7320 3a20 6172 7261 792d  _widths : array-
+0002d370: 6c69 6b65 5b32 5d20 6f66 2069 6e74 206f  like[2] of int o
+0002d380: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
+0002d390: 5769 6474 6873 206f 6620 7468 6520 6c65  Widths of the le
+0002d3a0: 6674 2061 6e64 2072 6967 6874 2061 726d  ft and right arm
+0002d3b0: 7320 6f66 2074 6865 2079 5472 6f6e 2c20  s of the yTron, 
+0002d3c0: 7265 7370 6563 7469 7665 6c79 2e0a 2020  respectively..  
+0002d3d0: 2020 7468 6574 6120 3a20 696e 7420 6f72    theta : int or
+0002d3e0: 2066 6c6f 6174 0a20 2020 2020 2020 2041   float.        A
+0002d3f0: 6e67 6c65 2062 6574 7765 656e 2074 6865  ngle between the
+0002d400: 2074 776f 2079 5472 6f6e 2061 726d 732e   two yTron arms.
+0002d410: 0a20 2020 2074 6865 7461 5f72 6573 6f6c  .    theta_resol
+0002d420: 7574 696f 6e20 3a20 696e 7420 6f72 2066  ution : int or f
+0002d430: 6c6f 6174 0a20 2020 2020 2020 2041 6e67  loat.        Ang
+0002d440: 6c65 2072 6573 6f6c 7574 696f 6e20 666f  le resolution fo
+0002d450: 7220 6375 7276 6174 7572 6520 6f66 2079  r curvature of y
+0002d460: 7472 6f6e 2069 6e74 6572 7365 6374 696f  tron intersectio
+0002d470: 6e20 706f 696e 740a 2020 2020 6c61 7965  n point.    laye
+0002d480: 7220 3a20 696e 742c 2061 7272 6179 2d6c  r : int, array-l
+0002d490: 696b 655b 325d 2c20 6f72 2073 6574 0a20  ike[2], or set. 
+0002d4a0: 2020 2020 2020 2053 7065 6369 6669 6320         Specific 
+0002d4b0: 6c61 7965 7228 7329 2074 6f20 7075 7420  layer(s) to put 
+0002d4c0: 706f 6c79 676f 6e20 6765 6f6d 6574 7279  polygon geometry
+0002d4d0: 206f 6e2e 0a0a 2020 2020 5265 7475 726e   on...    Return
+0002d4e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0002d4f0: 2020 4420 3a20 4465 7669 6365 0a20 2020    D : Device.   
+0002d500: 2020 2020 2041 2044 6576 6963 6520 636f       A Device co
+0002d510: 6e74 6169 6e69 6e67 2061 2079 5472 6f6e  ntaining a yTron
+0002d520: 2067 656f 6d65 7472 792e 0a20 2020 2022   geometry..    "
+0002d530: 2222 0a20 2020 2023 203d 3d3d 3d3d 3d3d  "".    # =======
 0002d540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002d550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002d560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002d570: 3d3d 3d3d 3d3d 0a20 2020 2074 6865 7461  ======.    theta
-0002d580: 203d 2074 6865 7461 202a 2070 6920 2f20   = theta * pi / 
-0002d590: 3138 300a 2020 2020 7468 6574 615f 7265  180.    theta_re
-0002d5a0: 736f 6c75 7469 6f6e 203d 2074 6865 7461  solution = theta
-0002d5b0: 5f72 6573 6f6c 7574 696f 6e20 2a20 7069  _resolution * pi
-0002d5c0: 202f 2031 3830 0a20 2020 2074 6865 7461   / 180.    theta
-0002d5d0: 6c69 7374 203d 206e 702e 6c69 6e73 7061  list = np.linspa
-0002d5e0: 6365 280a 2020 2020 2020 2020 2d28 7069  ce(.        -(pi
-0002d5f0: 202d 2074 6865 7461 292c 202d 7468 6574   - theta), -thet
-0002d600: 612c 2069 6e74 2828 7069 202d 2032 202a  a, int((pi - 2 *
-0002d610: 2074 6865 7461 2920 2f20 7468 6574 615f   theta) / theta_
-0002d620: 7265 736f 6c75 7469 6f6e 2920 2b20 320a  resolution) + 2.
-0002d630: 2020 2020 290a 2020 2020 7365 6d69 6369      ).    semici
-0002d640: 7263 6c65 5f78 203d 2072 686f 202a 2063  rcle_x = rho * c
-0002d650: 6f73 2874 6865 7461 6c69 7374 290a 2020  os(thetalist).  
-0002d660: 2020 7365 6d69 6369 7263 6c65 5f79 203d    semicircle_y =
-0002d670: 2072 686f 202a 2073 696e 2874 6865 7461   rho * sin(theta
-0002d680: 6c69 7374 2920 2b20 7268 6f0a 0a20 2020  list) + rho..   
-0002d690: 2023 2052 6573 7420 6f66 2079 5472 6f6e   # Rest of yTron
-0002d6a0: 0a20 2020 2078 6320 3d20 7268 6f20 2a20  .    xc = rho * 
-0002d6b0: 636f 7328 7468 6574 6129 0a20 2020 2079  cos(theta).    y
-0002d6c0: 6320 3d20 7268 6f20 2a20 7369 6e28 7468  c = rho * sin(th
-0002d6d0: 6574 6129 0a20 2020 2061 726d 5f78 5f6c  eta).    arm_x_l
-0002d6e0: 6566 7420 3d20 6172 6d5f 6c65 6e67 7468  eft = arm_length
-0002d6f0: 735b 305d 202a 2073 696e 2874 6865 7461  s[0] * sin(theta
-0002d700: 290a 2020 2020 6172 6d5f 795f 6c65 6674  ).    arm_y_left
-0002d710: 203d 2061 726d 5f6c 656e 6774 6873 5b30   = arm_lengths[0
-0002d720: 5d20 2a20 636f 7328 7468 6574 6129 0a20  ] * cos(theta). 
-0002d730: 2020 2061 726d 5f78 5f72 6967 6874 203d     arm_x_right =
-0002d740: 2061 726d 5f6c 656e 6774 6873 5b31 5d20   arm_lengths[1] 
-0002d750: 2a20 7369 6e28 7468 6574 6129 0a20 2020  * sin(theta).   
-0002d760: 2061 726d 5f79 5f72 6967 6874 203d 2061   arm_y_right = a
-0002d770: 726d 5f6c 656e 6774 6873 5b31 5d20 2a20  rm_lengths[1] * 
-0002d780: 636f 7328 7468 6574 6129 0a0a 2020 2020  cos(theta)..    
-0002d790: 2320 5772 6974 6520 6f75 7420 7820 616e  # Write out x an
-0002d7a0: 6420 7920 636f 6f72 6473 2066 6f72 2079  d y coords for y
-0002d7b0: 5472 6f6e 2070 6f6c 7967 6f6e 0a20 2020  Tron polygon.   
-0002d7c0: 2078 7074 7320 3d20 7365 6d69 6369 7263   xpts = semicirc
-0002d7d0: 6c65 5f78 2e74 6f6c 6973 7428 2920 2b20  le_x.tolist() + 
-0002d7e0: 5b0a 2020 2020 2020 2020 7863 202b 2061  [.        xc + a
-0002d7f0: 726d 5f78 5f72 6967 6874 2c0a 2020 2020  rm_x_right,.    
-0002d800: 2020 2020 7863 202b 2061 726d 5f78 5f72      xc + arm_x_r
-0002d810: 6967 6874 202b 2061 726d 5f77 6964 7468  ight + arm_width
-0002d820: 735b 315d 2c0a 2020 2020 2020 2020 7863  s[1],.        xc
-0002d830: 202b 2061 726d 5f77 6964 7468 735b 315d   + arm_widths[1]
-0002d840: 2c0a 2020 2020 2020 2020 7863 202b 2061  ,.        xc + a
-0002d850: 726d 5f77 6964 7468 735b 315d 2c0a 2020  rm_widths[1],.  
-0002d860: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-0002d870: 202d 2878 6320 2b20 6172 6d5f 7769 6474   -(xc + arm_widt
-0002d880: 6873 5b30 5d29 2c0a 2020 2020 2020 2020  hs[0]),.        
-0002d890: 2d28 7863 202b 2061 726d 5f77 6964 7468  -(xc + arm_width
-0002d8a0: 735b 305d 292c 0a20 2020 2020 2020 202d  s[0]),.        -
-0002d8b0: 2878 6320 2b20 6172 6d5f 785f 6c65 6674  (xc + arm_x_left
-0002d8c0: 202b 2061 726d 5f77 6964 7468 735b 305d   + arm_widths[0]
-0002d8d0: 292c 0a20 2020 2020 2020 202d 2878 6320  ),.        -(xc 
-0002d8e0: 2b20 6172 6d5f 785f 6c65 6674 292c 0a20  + arm_x_left),. 
-0002d8f0: 2020 205d 0a20 2020 2079 7074 7320 3d20     ].    ypts = 
-0002d900: 7365 6d69 6369 7263 6c65 5f79 2e74 6f6c  semicircle_y.tol
-0002d910: 6973 7428 2920 2b20 5b0a 2020 2020 2020  ist() + [.      
-0002d920: 2020 7963 202b 2061 726d 5f79 5f72 6967    yc + arm_y_rig
-0002d930: 6874 2c0a 2020 2020 2020 2020 7963 202b  ht,.        yc +
-0002d940: 2061 726d 5f79 5f72 6967 6874 2c0a 2020   arm_y_right,.  
-0002d950: 2020 2020 2020 7963 2c0a 2020 2020 2020        yc,.      
-0002d960: 2020 7963 202d 2073 6f75 7263 655f 6c65    yc - source_le
-0002d970: 6e67 7468 2c0a 2020 2020 2020 2020 7963  ngth,.        yc
-0002d980: 202d 2073 6f75 7263 655f 6c65 6e67 7468   - source_length
-0002d990: 2c0a 2020 2020 2020 2020 7963 202d 2073  ,.        yc - s
-0002d9a0: 6f75 7263 655f 6c65 6e67 7468 2c0a 2020  ource_length,.  
-0002d9b0: 2020 2020 2020 7963 2c0a 2020 2020 2020        yc,.      
-0002d9c0: 2020 7963 202b 2061 726d 5f79 5f6c 6566    yc + arm_y_lef
-0002d9d0: 742c 0a20 2020 2020 2020 2079 6320 2b20  t,.        yc + 
-0002d9e0: 6172 6d5f 795f 6c65 6674 2c0a 2020 2020  arm_y_left,.    
-0002d9f0: 5d0a 0a20 2020 2023 203d 3d3d 3d3d 3d3d  ]..    # =======
-0002da00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002da10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002da20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002da30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002da40: 3d3d 3d0a 2020 2020 2320 2043 7265 6174  ===.    #  Creat
-0002da50: 6520 6120 626c 616e 6b20 6465 7669 6365  e a blank device
-0002da60: 2c20 6164 6420 7468 6520 6765 6f6d 6574  , add the geomet
-0002da70: 7279 2c20 616e 6420 6465 6669 6e65 2074  ry, and define t
-0002da80: 6865 2070 6f72 7473 0a20 2020 2023 203d  he ports.    # =
+0002d570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002d580: 3d3d 3d0a 2020 2020 2320 2043 7265 6174  ===.    #  Creat
+0002d590: 6520 7468 6520 6261 7369 6320 6765 6f6d  e the basic geom
+0002d5a0: 6574 7279 0a20 2020 2023 203d 3d3d 3d3d  etry.    # =====
+0002d5b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002d5c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002d5d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002d5e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002d5f0: 3d3d 3d3d 3d0a 2020 2020 7468 6574 6120  =====.    theta 
+0002d600: 3d20 7468 6574 6120 2a20 7069 202f 2031  = theta * pi / 1
+0002d610: 3830 0a20 2020 2074 6865 7461 5f72 6573  80.    theta_res
+0002d620: 6f6c 7574 696f 6e20 3d20 7468 6574 615f  olution = theta_
+0002d630: 7265 736f 6c75 7469 6f6e 202a 2070 6920  resolution * pi 
+0002d640: 2f20 3138 300a 2020 2020 7468 6574 616c  / 180.    thetal
+0002d650: 6973 7420 3d20 6e70 2e6c 696e 7370 6163  ist = np.linspac
+0002d660: 6528 0a20 2020 2020 2020 202d 2870 6920  e(.        -(pi 
+0002d670: 2d20 7468 6574 6129 2c20 2d74 6865 7461  - theta), -theta
+0002d680: 2c20 696e 7428 2870 6920 2d20 3220 2a20  , int((pi - 2 * 
+0002d690: 7468 6574 6129 202f 2074 6865 7461 5f72  theta) / theta_r
+0002d6a0: 6573 6f6c 7574 696f 6e29 202b 2032 0a20  esolution) + 2. 
+0002d6b0: 2020 2029 0a20 2020 2073 656d 6963 6972     ).    semicir
+0002d6c0: 636c 655f 7820 3d20 7268 6f20 2a20 636f  cle_x = rho * co
+0002d6d0: 7328 7468 6574 616c 6973 7429 0a20 2020  s(thetalist).   
+0002d6e0: 2073 656d 6963 6972 636c 655f 7920 3d20   semicircle_y = 
+0002d6f0: 7268 6f20 2a20 7369 6e28 7468 6574 616c  rho * sin(thetal
+0002d700: 6973 7429 202b 2072 686f 0a0a 2020 2020  ist) + rho..    
+0002d710: 2320 5265 7374 206f 6620 7954 726f 6e0a  # Rest of yTron.
+0002d720: 2020 2020 7863 203d 2072 686f 202a 2063      xc = rho * c
+0002d730: 6f73 2874 6865 7461 290a 2020 2020 7963  os(theta).    yc
+0002d740: 203d 2072 686f 202a 2073 696e 2874 6865   = rho * sin(the
+0002d750: 7461 290a 2020 2020 6172 6d5f 785f 6c65  ta).    arm_x_le
+0002d760: 6674 203d 2061 726d 5f6c 656e 6774 6873  ft = arm_lengths
+0002d770: 5b30 5d20 2a20 7369 6e28 7468 6574 6129  [0] * sin(theta)
+0002d780: 0a20 2020 2061 726d 5f79 5f6c 6566 7420  .    arm_y_left 
+0002d790: 3d20 6172 6d5f 6c65 6e67 7468 735b 305d  = arm_lengths[0]
+0002d7a0: 202a 2063 6f73 2874 6865 7461 290a 2020   * cos(theta).  
+0002d7b0: 2020 6172 6d5f 785f 7269 6768 7420 3d20    arm_x_right = 
+0002d7c0: 6172 6d5f 6c65 6e67 7468 735b 315d 202a  arm_lengths[1] *
+0002d7d0: 2073 696e 2874 6865 7461 290a 2020 2020   sin(theta).    
+0002d7e0: 6172 6d5f 795f 7269 6768 7420 3d20 6172  arm_y_right = ar
+0002d7f0: 6d5f 6c65 6e67 7468 735b 315d 202a 2063  m_lengths[1] * c
+0002d800: 6f73 2874 6865 7461 290a 0a20 2020 2023  os(theta)..    #
+0002d810: 2057 7269 7465 206f 7574 2078 2061 6e64   Write out x and
+0002d820: 2079 2063 6f6f 7264 7320 666f 7220 7954   y coords for yT
+0002d830: 726f 6e20 706f 6c79 676f 6e0a 2020 2020  ron polygon.    
+0002d840: 7870 7473 203d 2073 656d 6963 6972 636c  xpts = semicircl
+0002d850: 655f 782e 746f 6c69 7374 2829 202b 205b  e_x.tolist() + [
+0002d860: 0a20 2020 2020 2020 2078 6320 2b20 6172  .        xc + ar
+0002d870: 6d5f 785f 7269 6768 742c 0a20 2020 2020  m_x_right,.     
+0002d880: 2020 2078 6320 2b20 6172 6d5f 785f 7269     xc + arm_x_ri
+0002d890: 6768 7420 2b20 6172 6d5f 7769 6474 6873  ght + arm_widths
+0002d8a0: 5b31 5d2c 0a20 2020 2020 2020 2078 6320  [1],.        xc 
+0002d8b0: 2b20 6172 6d5f 7769 6474 6873 5b31 5d2c  + arm_widths[1],
+0002d8c0: 0a20 2020 2020 2020 2078 6320 2b20 6172  .        xc + ar
+0002d8d0: 6d5f 7769 6474 6873 5b31 5d2c 0a20 2020  m_widths[1],.   
+0002d8e0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
+0002d8f0: 2d28 7863 202b 2061 726d 5f77 6964 7468  -(xc + arm_width
+0002d900: 735b 305d 292c 0a20 2020 2020 2020 202d  s[0]),.        -
+0002d910: 2878 6320 2b20 6172 6d5f 7769 6474 6873  (xc + arm_widths
+0002d920: 5b30 5d29 2c0a 2020 2020 2020 2020 2d28  [0]),.        -(
+0002d930: 7863 202b 2061 726d 5f78 5f6c 6566 7420  xc + arm_x_left 
+0002d940: 2b20 6172 6d5f 7769 6474 6873 5b30 5d29  + arm_widths[0])
+0002d950: 2c0a 2020 2020 2020 2020 2d28 7863 202b  ,.        -(xc +
+0002d960: 2061 726d 5f78 5f6c 6566 7429 2c0a 2020   arm_x_left),.  
+0002d970: 2020 5d0a 2020 2020 7970 7473 203d 2073    ].    ypts = s
+0002d980: 656d 6963 6972 636c 655f 792e 746f 6c69  emicircle_y.toli
+0002d990: 7374 2829 202b 205b 0a20 2020 2020 2020  st() + [.       
+0002d9a0: 2079 6320 2b20 6172 6d5f 795f 7269 6768   yc + arm_y_righ
+0002d9b0: 742c 0a20 2020 2020 2020 2079 6320 2b20  t,.        yc + 
+0002d9c0: 6172 6d5f 795f 7269 6768 742c 0a20 2020  arm_y_right,.   
+0002d9d0: 2020 2020 2079 632c 0a20 2020 2020 2020       yc,.       
+0002d9e0: 2079 6320 2d20 736f 7572 6365 5f6c 656e   yc - source_len
+0002d9f0: 6774 682c 0a20 2020 2020 2020 2079 6320  gth,.        yc 
+0002da00: 2d20 736f 7572 6365 5f6c 656e 6774 682c  - source_length,
+0002da10: 0a20 2020 2020 2020 2079 6320 2d20 736f  .        yc - so
+0002da20: 7572 6365 5f6c 656e 6774 682c 0a20 2020  urce_length,.   
+0002da30: 2020 2020 2079 632c 0a20 2020 2020 2020       yc,.       
+0002da40: 2079 6320 2b20 6172 6d5f 795f 6c65 6674   yc + arm_y_left
+0002da50: 2c0a 2020 2020 2020 2020 7963 202b 2061  ,.        yc + a
+0002da60: 726d 5f79 5f6c 6566 742c 0a20 2020 205d  rm_y_left,.    ]
+0002da70: 0a0a 2020 2020 2320 3d3d 3d3d 3d3d 3d3d  ..    # ========
+0002da80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002da90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002daa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002dab0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dad0: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 4420  =========.    D 
-0002dae0: 3d20 4465 7669 6365 286e 616d 653d 2279  = Device(name="y
-0002daf0: 7472 6f6e 2229 0a20 2020 2044 2e61 6464  tron").    D.add
-0002db00: 5f70 6f6c 7967 6f6e 285b 7870 7473 2c20  _polygon([xpts, 
-0002db10: 7970 7473 5d2c 206c 6179 6572 3d6c 6179  ypts], layer=lay
-0002db20: 6572 290a 2020 2020 442e 6164 645f 706f  er).    D.add_po
-0002db30: 7274 280a 2020 2020 2020 2020 6e61 6d65  rt(.        name
-0002db40: 3d22 6c65 6674 222c 0a20 2020 2020 2020  ="left",.       
-0002db50: 206d 6964 706f 696e 743d 5b2d 2878 6320   midpoint=[-(xc 
-0002db60: 2b20 6172 6d5f 785f 6c65 6674 202b 2061  + arm_x_left + a
-0002db70: 726d 5f77 6964 7468 735b 305d 202f 2032  rm_widths[0] / 2
-0002db80: 292c 2079 6320 2b20 6172 6d5f 795f 6c65  ), yc + arm_y_le
-0002db90: 6674 5d2c 0a20 2020 2020 2020 2077 6964  ft],.        wid
-0002dba0: 7468 3d61 726d 5f77 6964 7468 735b 305d  th=arm_widths[0]
-0002dbb0: 2c0a 2020 2020 2020 2020 6f72 6965 6e74  ,.        orient
-0002dbc0: 6174 696f 6e3d 3930 2c0a 2020 2020 290a  ation=90,.    ).
-0002dbd0: 2020 2020 442e 6164 645f 706f 7274 280a      D.add_port(.
-0002dbe0: 2020 2020 2020 2020 6e61 6d65 3d22 7269          name="ri
-0002dbf0: 6768 7422 2c0a 2020 2020 2020 2020 6d69  ght",.        mi
-0002dc00: 6470 6f69 6e74 3d5b 7863 202b 2061 726d  dpoint=[xc + arm
-0002dc10: 5f78 5f72 6967 6874 202b 2061 726d 5f77  _x_right + arm_w
-0002dc20: 6964 7468 735b 315d 202f 2032 2c20 7963  idths[1] / 2, yc
-0002dc30: 202b 2061 726d 5f79 5f72 6967 6874 5d2c   + arm_y_right],
-0002dc40: 0a20 2020 2020 2020 2077 6964 7468 3d61  .        width=a
-0002dc50: 726d 5f77 6964 7468 735b 315d 2c0a 2020  rm_widths[1],.  
-0002dc60: 2020 2020 2020 6f72 6965 6e74 6174 696f        orientatio
-0002dc70: 6e3d 3930 2c0a 2020 2020 290a 2020 2020  n=90,.    ).    
-0002dc80: 442e 6164 645f 706f 7274 280a 2020 2020  D.add_port(.    
-0002dc90: 2020 2020 6e61 6d65 3d22 736f 7572 6365      name="source
-0002dca0: 222c 0a20 2020 2020 2020 206d 6964 706f  ",.        midpo
-0002dcb0: 696e 743d 5b30 202b 2028 6172 6d5f 7769  int=[0 + (arm_wi
-0002dcc0: 6474 6873 5b31 5d20 2d20 6172 6d5f 7769  dths[1] - arm_wi
-0002dcd0: 6474 6873 5b30 5d29 202f 2032 2c20 2d73  dths[0]) / 2, -s
-0002dce0: 6f75 7263 655f 6c65 6e67 7468 202b 2079  ource_length + y
-0002dcf0: 635d 2c0a 2020 2020 2020 2020 7769 6474  c],.        widt
-0002dd00: 683d 6172 6d5f 7769 6474 6873 5b30 5d20  h=arm_widths[0] 
-0002dd10: 2b20 6172 6d5f 7769 6474 6873 5b31 5d20  + arm_widths[1] 
-0002dd20: 2b20 3220 2a20 7863 2c0a 2020 2020 2020  + 2 * xc,.      
-0002dd30: 2020 6f72 6965 6e74 6174 696f 6e3d 2d39    orientation=-9
-0002dd40: 302c 0a20 2020 2029 0a0a 2020 2020 2320  0,.    )..    # 
-0002dd50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dd80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002dd90: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2023  ==========.    #
-0002dda0: 2020 5265 636f 7264 2061 6e79 2070 6172    Record any par
-0002ddb0: 616d 6574 6572 7320 796f 7520 6d61 7920  ameters you may 
-0002ddc0: 7761 6e74 2074 6f20 6163 6365 7373 206c  want to access l
-0002ddd0: 6174 6572 0a20 2020 2023 203d 3d3d 3d3d  ater.    # =====
+0002dac0: 3d3d 0a20 2020 2023 2020 4372 6561 7465  ==.    #  Create
+0002dad0: 2061 2062 6c61 6e6b 2064 6576 6963 652c   a blank device,
+0002dae0: 2061 6464 2074 6865 2067 656f 6d65 7472   add the geometr
+0002daf0: 792c 2061 6e64 2064 6566 696e 6520 7468  y, and define th
+0002db00: 6520 706f 7274 730a 2020 2020 2320 3d3d  e ports.    # ==
+0002db10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002db20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002db30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002db40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002db50: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2044 203d  ========.    D =
+0002db60: 2044 6576 6963 6528 6e61 6d65 3d22 7974   Device(name="yt
+0002db70: 726f 6e22 290a 2020 2020 442e 6164 645f  ron").    D.add_
+0002db80: 706f 6c79 676f 6e28 5b78 7074 732c 2079  polygon([xpts, y
+0002db90: 7074 735d 2c20 6c61 7965 723d 6c61 7965  pts], layer=laye
+0002dba0: 7229 0a20 2020 2044 2e61 6464 5f70 6f72  r).    D.add_por
+0002dbb0: 7428 0a20 2020 2020 2020 206e 616d 653d  t(.        name=
+0002dbc0: 226c 6566 7422 2c0a 2020 2020 2020 2020  "left",.        
+0002dbd0: 6d69 6470 6f69 6e74 3d5b 2d28 7863 202b  midpoint=[-(xc +
+0002dbe0: 2061 726d 5f78 5f6c 6566 7420 2b20 6172   arm_x_left + ar
+0002dbf0: 6d5f 7769 6474 6873 5b30 5d20 2f20 3229  m_widths[0] / 2)
+0002dc00: 2c20 7963 202b 2061 726d 5f79 5f6c 6566  , yc + arm_y_lef
+0002dc10: 745d 2c0a 2020 2020 2020 2020 7769 6474  t],.        widt
+0002dc20: 683d 6172 6d5f 7769 6474 6873 5b30 5d2c  h=arm_widths[0],
+0002dc30: 0a20 2020 2020 2020 206f 7269 656e 7461  .        orienta
+0002dc40: 7469 6f6e 3d39 302c 0a20 2020 2029 0a20  tion=90,.    ). 
+0002dc50: 2020 2044 2e61 6464 5f70 6f72 7428 0a20     D.add_port(. 
+0002dc60: 2020 2020 2020 206e 616d 653d 2272 6967         name="rig
+0002dc70: 6874 222c 0a20 2020 2020 2020 206d 6964  ht",.        mid
+0002dc80: 706f 696e 743d 5b78 6320 2b20 6172 6d5f  point=[xc + arm_
+0002dc90: 785f 7269 6768 7420 2b20 6172 6d5f 7769  x_right + arm_wi
+0002dca0: 6474 6873 5b31 5d20 2f20 322c 2079 6320  dths[1] / 2, yc 
+0002dcb0: 2b20 6172 6d5f 795f 7269 6768 745d 2c0a  + arm_y_right],.
+0002dcc0: 2020 2020 2020 2020 7769 6474 683d 6172          width=ar
+0002dcd0: 6d5f 7769 6474 6873 5b31 5d2c 0a20 2020  m_widths[1],.   
+0002dce0: 2020 2020 206f 7269 656e 7461 7469 6f6e       orientation
+0002dcf0: 3d39 302c 0a20 2020 2029 0a20 2020 2044  =90,.    ).    D
+0002dd00: 2e61 6464 5f70 6f72 7428 0a20 2020 2020  .add_port(.     
+0002dd10: 2020 206e 616d 653d 2273 6f75 7263 6522     name="source"
+0002dd20: 2c0a 2020 2020 2020 2020 6d69 6470 6f69  ,.        midpoi
+0002dd30: 6e74 3d5b 3020 2b20 2861 726d 5f77 6964  nt=[0 + (arm_wid
+0002dd40: 7468 735b 315d 202d 2061 726d 5f77 6964  ths[1] - arm_wid
+0002dd50: 7468 735b 305d 2920 2f20 322c 202d 736f  ths[0]) / 2, -so
+0002dd60: 7572 6365 5f6c 656e 6774 6820 2b20 7963  urce_length + yc
+0002dd70: 5d2c 0a20 2020 2020 2020 2077 6964 7468  ],.        width
+0002dd80: 3d61 726d 5f77 6964 7468 735b 305d 202b  =arm_widths[0] +
+0002dd90: 2061 726d 5f77 6964 7468 735b 315d 202b   arm_widths[1] +
+0002dda0: 2032 202a 2078 632c 0a20 2020 2020 2020   2 * xc,.       
+0002ddb0: 206f 7269 656e 7461 7469 6f6e 3d2d 3930   orientation=-90
+0002ddc0: 2c0a 2020 2020 290a 0a20 2020 2023 203d  ,.    )..    # =
+0002ddd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002dde0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002ddf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002de00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002de10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002de20: 3d3d 3d3d 3d0a 2020 2020 442e 696e 666f  =====.    D.info
-0002de30: 5b22 7268 6f22 5d20 3d20 7268 6f0a 2020  ["rho"] = rho.  
-0002de40: 2020 442e 696e 666f 5b22 6c65 6674 5f77    D.info["left_w
-0002de50: 6964 7468 225d 203d 2061 726d 5f77 6964  idth"] = arm_wid
-0002de60: 7468 735b 305d 0a20 2020 2044 2e69 6e66  ths[0].    D.inf
-0002de70: 6f5b 2272 6967 6874 5f77 6964 7468 225d  o["right_width"]
-0002de80: 203d 2061 726d 5f77 6964 7468 735b 315d   = arm_widths[1]
-0002de90: 0a20 2020 2044 2e69 6e66 6f5b 2273 6f75  .    D.info["sou
-0002dea0: 7263 655f 7769 6474 6822 5d20 3d20 6172  rce_width"] = ar
-0002deb0: 6d5f 7769 6474 6873 5b30 5d20 2b20 6172  m_widths[0] + ar
-0002dec0: 6d5f 7769 6474 6873 5b31 5d20 2b20 3220  m_widths[1] + 2 
-0002ded0: 2a20 7863 0a0a 2020 2020 7265 7475 726e  * xc..    return
-0002dee0: 2044 0a0a 0a23 203d 3d3d 3d3d 3d3d 3d3d   D...# =========
-0002def0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df30: 3d3d 3d3d 3d0a 2320 4578 616d 706c 6520  =====.# Example 
-0002df40: 636f 6465 0a23 203d 3d3d 3d3d 3d3d 3d3d  code.# =========
-0002df50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002de10: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2320  =========.    # 
+0002de20: 2052 6563 6f72 6420 616e 7920 7061 7261   Record any para
+0002de30: 6d65 7465 7273 2079 6f75 206d 6179 2077  meters you may w
+0002de40: 616e 7420 746f 2061 6363 6573 7320 6c61  ant to access la
+0002de50: 7465 720a 2020 2020 2320 3d3d 3d3d 3d3d  ter.    # ======
+0002de60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002de70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002de80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002de90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002dea0: 3d3d 3d3d 0a20 2020 2044 2e69 6e66 6f5b  ====.    D.info[
+0002deb0: 2272 686f 225d 203d 2072 686f 0a20 2020  "rho"] = rho.   
+0002dec0: 2044 2e69 6e66 6f5b 226c 6566 745f 7769   D.info["left_wi
+0002ded0: 6474 6822 5d20 3d20 6172 6d5f 7769 6474  dth"] = arm_widt
+0002dee0: 6873 5b30 5d0a 2020 2020 442e 696e 666f  hs[0].    D.info
+0002def0: 5b22 7269 6768 745f 7769 6474 6822 5d20  ["right_width"] 
+0002df00: 3d20 6172 6d5f 7769 6474 6873 5b31 5d0a  = arm_widths[1].
+0002df10: 2020 2020 442e 696e 666f 5b22 736f 7572      D.info["sour
+0002df20: 6365 5f77 6964 7468 225d 203d 2061 726d  ce_width"] = arm
+0002df30: 5f77 6964 7468 735b 305d 202b 2061 726d  _widths[0] + arm
+0002df40: 5f77 6964 7468 735b 315d 202b 2032 202a  _widths[1] + 2 *
+0002df50: 2078 630a 0a20 2020 2072 6574 7572 6e20   xc..    return 
+0002df60: 440a 0a0a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  D...# ==========
 0002df70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002df80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0002df90: 3d3d 3d3d 3d0a 0a23 2079 203d 2079 7472  =====..# y = ytr
-0002dfa0: 6f6e 5f72 6f75 6e64 2872 686f 203d 2031  on_round(rho = 1
-0002dfb0: 2c20 6172 6d5f 6c65 6e67 7468 7320 3d20  , arm_lengths = 
-0002dfc0: 2835 3030 2c33 3030 292c 2020 736f 7572  (500,300),  sour
-0002dfd0: 6365 5f6c 656e 6774 6820 3d20 3530 302c  ce_length = 500,
-0002dfe0: 0a23 2061 726d 5f77 6964 7468 7320 3d20  .# arm_widths = 
-0002dff0: 2832 3030 2c20 3230 3029 2c20 7468 6574  (200, 200), thet
-0002e000: 6120 3d20 322e 352c 2074 6865 7461 5f72  a = 2.5, theta_r
-0002e010: 6573 6f6c 7574 696f 6e20 3d20 3130 2c0a  esolution = 10,.
-0002e020: 2320 6c61 7965 7220 3d20 3029 0a23 2071  # layer = 0).# q
-0002e030: 7569 636b 706c 6f74 2879 290a 0a0a 2320  uickplot(y)...# 
-0002e040: 2525 0a                                  %%.
+0002df90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002dfa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002dfb0: 3d3d 3d3d 0a23 2045 7861 6d70 6c65 2063  ====.# Example c
+0002dfc0: 6f64 650a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  ode.# ==========
+0002dfd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002dfe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002dff0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002e000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0002e010: 3d3d 3d3d 0a0a 2320 7920 3d20 7974 726f  ====..# y = ytro
+0002e020: 6e5f 726f 756e 6428 7268 6f20 3d20 312c  n_round(rho = 1,
+0002e030: 2061 726d 5f6c 656e 6774 6873 203d 2028   arm_lengths = (
+0002e040: 3530 302c 3330 3029 2c20 2073 6f75 7263  500,300),  sourc
+0002e050: 655f 6c65 6e67 7468 203d 2035 3030 2c0a  e_length = 500,.
+0002e060: 2320 6172 6d5f 7769 6474 6873 203d 2028  # arm_widths = (
+0002e070: 3230 302c 2032 3030 292c 2074 6865 7461  200, 200), theta
+0002e080: 203d 2032 2e35 2c20 7468 6574 615f 7265   = 2.5, theta_re
+0002e090: 736f 6c75 7469 6f6e 203d 2031 302c 0a23  solution = 10,.#
+0002e0a0: 206c 6179 6572 203d 2030 290a 2320 7175   layer = 0).# qu
+0002e0b0: 6963 6b70 6c6f 7428 7929 0a0a 0a23 2025  ickplot(y)...# %
+0002e0c0: 250a                                     %.
```

### Comparing `phidl-1.6.3/phidl/path.py` & `phidl-1.6.4/phidl/path.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/phidl_tutorial_example.py` & `phidl-1.6.4/phidl/phidl_tutorial_example.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/quickplotter.py` & `phidl-1.6.4/phidl/quickplotter.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/routing.py` & `phidl-1.6.4/phidl/routing.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl/utilities.py` & `phidl-1.6.4/phidl/utilities.py`

 * *Files identical despite different names*

### Comparing `phidl-1.6.3/phidl.egg-info/PKG-INFO` & `phidl-1.6.4/phidl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 Metadata-Version: 2.1
 Name: phidl
-Version: 1.6.3
+Version: 1.6.4
 Summary: PHIDL
 Author: Adam McCaughan
 Author-email: amccaugh@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pytest](https://github.com/amccaugh/phidl/actions/workflows/pytest.yml/badge.svg)](https://github.com/amccaugh/phidl/actions/workflows/pytest.yml)
 [![pre-commit](https://github.com/amccaugh/phidl/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/amccaugh/phidl/actions/workflows/pre-commit.yml)
 
 # PHIDL
 GDS scripting for Python that's intuitive, fast, and powerful.
 
 - [**Installation / requirements**](#installation--requirements)
 - [**Tutorial + examples**](https://phidl.readthedocs.io/en/latest/tutorials.html) (or [try an interactive notebook](https://mybinder.org/v2/gh/amccaugh/phidl/master?filepath=phidl_tutorial_example.ipynb))
 - [**Geometry library + function documentation**](https://phidl.readthedocs.io/en/latest/geometry_reference.html)
-- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on Feb 9, 2023)
-    - Huge new routing rewrite for `phidl.routing`, including automatic manhattan routing with custom cross-sections!  See [the routing documentation](https://phidl.readthedocs.io/en/latest/tutorials/routing.html) for details. Big thanks to Jeffrey Holzgrafe @jolzgrafe for this contribution
-    - `Path`s can now be used to produce sharp angles, in addition to smooth bends. See [the Path documentation](https://phidl.readthedocs.io/en/latest/tutorials/waveguides.html#Sharp/angular-paths)
-
-```python
-import phidl.routing as pr
-D_left = pr.route_smooth(port1, port2, radius=8, layer = 2)
-D_right = pr.route_sharp(port1, port2, layer = 2)
-```
-
-![phidl example image](https://amccaugh.github.io/phidl/readme_9.png)
+- [Changelog](https://github.com/amccaugh/phidl/blob/master/CHANGELOG.md) (latest update 1.6.3 on July 20, 2023)
+    - New `pg.fill_rectangle()` [examples and documentation](https://phidl.readthedocs.io/en/latest/geometry_reference.html#Fill-tool)
 
 # Citation
 
 If you found PHIDL useful, please consider citing it in (just one!) of your publications -- we appreciate it greatly. ([BibTeX](https://raw.githubusercontent.com/amccaugh/phidl/master/CITATION.bib))
  - McCaughan, A. N., et. al. PHIDL: Python-based layout and geometry creation for nanolithography. *J. Vac. Sci. Technol. B* 39, 062601 (2021). http://dx.doi.org/10.1116/6.0001203
 
 # Gallery
@@ -100,9 +89,7 @@
 There are also handy functions to help pack shapes into as small an area as possible:
 
 ```
 pg.packer(D_list, spacing = 1.25, aspect_ratio = (2,1))
 ```
 
 ![phidl example image](https://amccaugh.github.io/phidl/packer.png)
-
-
```

### Comparing `phidl-1.6.3/setup.py` & `phidl-1.6.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="phidl",
-    version="1.6.3",
+    version="1.6.4",
     description="PHIDL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     author="Adam McCaughan",
     author_email="amccaugh@gmail.com",
     packages=["phidl"],
```

