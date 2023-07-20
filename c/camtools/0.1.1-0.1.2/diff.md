# Comparing `tmp/camtools-0.1.1.tar.gz` & `tmp/camtools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camtools-0.1.1.tar", last modified: Wed Jul 19 03:32:35 2023, max compression
+gzip compressed data, was "camtools-0.1.2.tar", last modified: Thu Jul 20 17:12:40 2023, max compression
```

## Comparing `camtools-0.1.1.tar` & `camtools-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxr-x   0 yixing    (1000) yixing    (1000)        0 2023-07-19 03:32:35.806830 camtools-0.1.1/
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     1067 2023-04-12 05:26:11.000000 camtools-0.1.1/LICENSE
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     7010 2023-07-19 03:32:35.806830 camtools-0.1.1/PKG-INFO
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     6640 2023-07-19 03:25:17.000000 camtools-0.1.1/README.md
-drwxrwxr-x   0 yixing    (1000) yixing    (1000)        0 2023-07-19 03:32:35.806830 camtools-0.1.1/camtools/
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      404 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/__init__.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     7453 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/camera.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)    29606 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/colmap.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     1773 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/colormap.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)    11072 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/convert.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     1638 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/geometry.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)    26652 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/image.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     8261 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/io.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     8890 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/metric.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     1441 2023-04-12 05:26:11.000000 camtools-0.1.1/camtools/normalize.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     4419 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/plot.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     6919 2023-07-04 15:36:56.000000 camtools-0.1.1/camtools/project.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     4396 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/raycast.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     3423 2023-07-18 08:00:41.000000 camtools-0.1.1/camtools/sanity.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     5323 2023-07-18 05:08:41.000000 camtools-0.1.1/camtools/solver.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      498 2023-04-12 05:26:11.000000 camtools-0.1.1/camtools/stat.py
-drwxrwxr-x   0 yixing    (1000) yixing    (1000)        0 2023-07-19 03:32:35.806830 camtools-0.1.1/camtools.egg-info/
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     7010 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/PKG-INFO
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      582 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/SOURCES.txt
--rw-rw-r--   0 yixing    (1000) yixing    (1000)        1 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/dependency_links.txt
--rw-rw-r--   0 yixing    (1000) yixing    (1000)       47 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/entry_points.txt
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      105 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/requires.txt
--rw-rw-r--   0 yixing    (1000) yixing    (1000)        9 2023-07-19 03:32:35.000000 camtools-0.1.1/camtools.egg-info/top_level.txt
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      612 2023-07-19 03:31:41.000000 camtools-0.1.1/pyproject.toml
--rw-rw-r--   0 yixing    (1000) yixing    (1000)       38 2023-07-19 03:32:35.806830 camtools-0.1.1/setup.cfg
--rw-rw-r--   0 yixing    (1000) yixing    (1000)      488 2023-07-18 06:38:21.000000 camtools-0.1.1/setup.py
-drwxrwxr-x   0 yixing    (1000) yixing    (1000)        0 2023-07-19 03:32:35.806830 camtools-0.1.1/test/
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     3351 2023-07-18 05:08:41.000000 camtools-0.1.1/test/test_convert.py
--rw-rw-r--   0 yixing    (1000) yixing    (1000)     1972 2023-07-18 05:08:41.000000 camtools-0.1.1/test/test_image.py
+drwxr-xr-x   0 yixing     (501) staff       (20)        0 2023-07-20 17:12:40.237156 camtools-0.1.2/
+-rw-r--r--   0 yixing     (501) staff       (20)     1067 2023-01-06 06:00:58.000000 camtools-0.1.2/LICENSE
+-rw-r--r--   0 yixing     (501) staff       (20)     7523 2023-07-20 17:12:40.237025 camtools-0.1.2/PKG-INFO
+-rw-r--r--   0 yixing     (501) staff       (20)     7153 2023-07-20 17:10:31.000000 camtools-0.1.2/README.md
+drwxr-xr-x   0 yixing     (501) staff       (20)        0 2023-07-20 17:12:40.234967 camtools-0.1.2/camtools/
+-rw-r--r--   0 yixing     (501) staff       (20)      404 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/__init__.py
+-rw-r--r--   0 yixing     (501) staff       (20)     7453 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/camera.py
+-rw-r--r--   0 yixing     (501) staff       (20)    29606 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/colmap.py
+-rw-r--r--   0 yixing     (501) staff       (20)     1773 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/colormap.py
+-rw-r--r--   0 yixing     (501) staff       (20)    11072 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/convert.py
+-rw-r--r--   0 yixing     (501) staff       (20)     1638 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/geometry.py
+-rw-r--r--   0 yixing     (501) staff       (20)    26652 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/image.py
+-rw-r--r--   0 yixing     (501) staff       (20)     8261 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/io.py
+-rw-r--r--   0 yixing     (501) staff       (20)     8890 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/metric.py
+-rw-r--r--   0 yixing     (501) staff       (20)     1441 2023-01-06 06:00:58.000000 camtools-0.1.2/camtools/normalize.py
+-rw-r--r--   0 yixing     (501) staff       (20)     4419 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/plot.py
+-rw-r--r--   0 yixing     (501) staff       (20)     6919 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/project.py
+-rw-r--r--   0 yixing     (501) staff       (20)     4396 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/raycast.py
+-rw-r--r--   0 yixing     (501) staff       (20)     3423 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/sanity.py
+-rw-r--r--   0 yixing     (501) staff       (20)     5323 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/solver.py
+-rw-r--r--   0 yixing     (501) staff       (20)      498 2023-01-06 06:00:58.000000 camtools-0.1.2/camtools/stat.py
+drwxr-xr-x   0 yixing     (501) staff       (20)        0 2023-07-20 17:12:40.236289 camtools-0.1.2/camtools/tools/
+-rw-r--r--   0 yixing     (501) staff       (20)       54 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/tools/__init__.py
+-rw-r--r--   0 yixing     (501) staff       (20)     1802 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/tools/cli.py
+-rw-r--r--   0 yixing     (501) staff       (20)     7344 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/tools/crop_boarders.py
+-rw-r--r--   0 yixing     (501) staff       (20)    18062 2023-07-20 17:08:40.000000 camtools-0.1.2/camtools/tools/draw_bboxes.py
+drwxr-xr-x   0 yixing     (501) staff       (20)        0 2023-07-20 17:12:40.235764 camtools-0.1.2/camtools.egg-info/
+-rw-r--r--   0 yixing     (501) staff       (20)     7523 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/PKG-INFO
+-rw-r--r--   0 yixing     (501) staff       (20)      710 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/SOURCES.txt
+-rw-r--r--   0 yixing     (501) staff       (20)        1 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/dependency_links.txt
+-rw-r--r--   0 yixing     (501) staff       (20)       47 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/entry_points.txt
+-rw-r--r--   0 yixing     (501) staff       (20)      105 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/requires.txt
+-rw-r--r--   0 yixing     (501) staff       (20)        9 2023-07-20 17:12:40.000000 camtools-0.1.2/camtools.egg-info/top_level.txt
+-rw-r--r--   0 yixing     (501) staff       (20)      673 2023-07-20 17:10:49.000000 camtools-0.1.2/pyproject.toml
+-rw-r--r--   0 yixing     (501) staff       (20)       38 2023-07-20 17:12:40.237191 camtools-0.1.2/setup.cfg
+-rw-r--r--   0 yixing     (501) staff       (20)      488 2023-07-20 17:08:40.000000 camtools-0.1.2/setup.py
+drwxr-xr-x   0 yixing     (501) staff       (20)        0 2023-07-20 17:12:40.236829 camtools-0.1.2/test/
+-rw-r--r--   0 yixing     (501) staff       (20)     1172 2023-07-20 17:10:31.000000 camtools-0.1.2/test/test_cli.py
+-rw-r--r--   0 yixing     (501) staff       (20)     3351 2023-07-20 17:08:40.000000 camtools-0.1.2/test/test_convert.py
+-rw-r--r--   0 yixing     (501) staff       (20)     1972 2023-07-20 17:08:40.000000 camtools-0.1.2/test/test_image.py
```

### Comparing `camtools-0.1.1/LICENSE` & `camtools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/PKG-INFO` & `camtools-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-Metadata-Version: 2.1
-Name: camtools
-Version: 0.1.1
-Summary: CamTools: Camera Tools for Computer Vision.
-License: MIT
-Project-URL: Homepage, https://github.com/yxlao/camtools
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # CamTools: Camera Tools for Computer Vision
 
 CamTools is a useful tool for handling cameras in computer vision. It can be
 used for plotting, converting, projecting, ray casting, and doing more with
 camera parameters. It follows the standard camera coordinate system with clear
 and easy-to-use APIs.
 
 <a href="https://github.com/yxlao/camtools/actions/workflows/formatter.yml">
-  <img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+<img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml/badge.svg" alt="Unit Test">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/pypi.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/pypi.yml/badge.svg" alt="PyPI">
 </a>
 
 ## What can you do with CamTools?
 
 1. Plot cameras. Useful for debugging 3D reconstruction and NeRFs!
 
    ```python
@@ -37,14 +30,15 @@
       <img src="./camtools/assets/camera_frames.png" width="360" />
    </p>
 
 2. Convert camera parameters.
 
    ```python
    pose = ct.convert.T_to_pose(T)     # Convert T to pose
+   T    = ct.convert.T_to_pose(pose)  # Convert pose to T
    R, t = ct.convert.T_to_R_t(T)      # Convert T to R and t
    C    = ct.convert.pose_to_C(pose)  # Convert pose to camera center
    K, T = ct.convert.P_to_K_T(P)      # Decompose projection matrix to K and T
                                       # And more...
    ```
 
 3. Projection and ray casting.
@@ -101,26 +95,35 @@
    - Solve line intersections.
    - COLMAP tools.
    - Points normalization.
    - ...
 
 ## Installation
 
+To install CamTools, simply do:
+
 ```bash
-# Option 1: install from pip.
 pip install camtools
+```
 
-# Option 2: install from git.
-pip install git+https://github.com/yxlao/camtools.git
+Alternatively, you can install CamTools from source with one of the following
+methods:
 
-# Option 3: install from source.
+```bash
 git clone https://github.com/yxlao/camtools.git
 cd camtools
-pip install -e .  # Dev mode, if you want to modify camtools.
-pip install .     # Install mode, if you want to use camtools only.
+
+# Installation mode, if you want to use camtools only.
+pip install .
+
+# Dev mode, if you want to modify camtools on the fly.
+pip install -e .
+
+# Dev mode and dev dependencies, if you want to modify camtools and run tests.
+pip install -e .[dev]
 ```
 
 ## Camera coordinate system
 
 We follow the standard OpenCV-style camera coordinate system as shown below.
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,50 +1,47 @@
-Metadata-Version: 2.1 Name: camtools Version: 0.1.1 Summary: CamTools: Camera
-Tools for Computer Vision. License: MIT Project-URL: Homepage, https://
-github.com/yxlao/camtools Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE # CamTools: Camera Tools for Computer Vision CamTools is a useful tool
-for handling cameras in computer vision. It can be used for plotting,
-converting, projecting, ray casting, and doing more with camera parameters. It
-follows the standard camera coordinate system with clear and easy-to-use APIs.
-[Formatter] ## What can you do with CamTools? 1. Plot cameras. Useful for
-debugging 3D reconstruction and NeRFs! ```python import camtools as ct import
-open3d as o3d cameras = ct.camera.create_camera_ray_frames(Ks, Ts)
+# CamTools: Camera Tools for Computer Vision CamTools is a useful tool for
+handling cameras in computer vision. It can be used for plotting, converting,
+projecting, ray casting, and doing more with camera parameters. It follows the
+standard camera coordinate system with clear and easy-to-use APIs. [Formatter]
+[Unit_Test] [PyPI] ## What can you do with CamTools? 1. Plot cameras. Useful
+for debugging 3D reconstruction and NeRFs! ```python import camtools as ct
+import open3d as o3d cameras = ct.camera.create_camera_ray_frames(Ks, Ts)
 o3d.visualization.draw_geometries([cameras]) ```
                      [./camtools/assets/camera_frames.png]
 2. Convert camera parameters. ```python pose = ct.convert.T_to_pose(T) #
-Convert T to pose R, t = ct.convert.T_to_R_t(T) # Convert T to R and t C =
-ct.convert.pose_to_C(pose) # Convert pose to camera center K, T =
-ct.convert.P_to_K_T(P) # Decompose projection matrix to K and T # And more...
-``` 3. Projection and ray casting. ```python # Project 3D points to pixels.
-pixels = ct.project.points_to_pixel(points, K, T) # Back-project depth image to
-3D points. points = ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a
-triangle mesh to depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks,
-Ts, height, width) # And more... ``` 4. Image and depth I/O with no surprises.
-Strict type checks and range checks are enforced. The image and depth I/O APIs
-are specifically designed to solve the following pain points: - Is my image of
-type `float32` or `uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it
-RGB or BGR? - Does my image have an alpha channel? - When saving depth image as
-integer-based `.png`, is it correctly scaled? ```python ct.io.imread()
-ct.io.imwrite() ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line
-tools `ct` (runs in terminal). ```bash # Crop image boarders. ct crop-boarders
-*.png --pad_pixel 10 --skip_cropped --same_crop # Draw synchronized bounding
-boxes interactively. ct draw-bboxes path/to/a.png path/to/b.png # For more
-command-line tools. ct --help ```
+Convert T to pose T = ct.convert.T_to_pose(pose) # Convert pose to T R, t =
+ct.convert.T_to_R_t(T) # Convert T to R and t C = ct.convert.pose_to_C(pose) #
+Convert pose to camera center K, T = ct.convert.P_to_K_T(P) # Decompose
+projection matrix to K and T # And more... ``` 3. Projection and ray casting.
+```python # Project 3D points to pixels. pixels = ct.project.points_to_pixel
+(points, K, T) # Back-project depth image to 3D points. points =
+ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a triangle mesh to
+depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks, Ts, height, width)
+# And more... ``` 4. Image and depth I/O with no surprises. Strict type checks
+and range checks are enforced. The image and depth I/O APIs are specifically
+designed to solve the following pain points: - Is my image of type `float32` or
+`uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it RGB or BGR? -
+Does my image have an alpha channel? - When saving depth image as integer-based
+`.png`, is it correctly scaled? ```python ct.io.imread() ct.io.imwrite()
+ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line tools `ct` (runs
+in terminal). ```bash # Crop image boarders. ct crop-boarders *.png --pad_pixel
+10 --skip_cropped --same_crop # Draw synchronized bounding boxes interactively.
+ct draw-bboxes path/to/a.png path/to/b.png # For more command-line tools. ct --
+help ```
   [https://user-images.githubusercontent.com/1501945/241416210-e11ff3bf-22e6-
                           46c0-8ba0-d177a0015323.png]
 6. And more. - Solve line intersections. - COLMAP tools. - Points
-normalization. - ... ## Installation ```bash # Option 1: install from pip. pip
-install camtools # Option 2: install from git. pip install git+https://
-github.com/yxlao/camtools.git # Option 3: install from source. git clone https:
-//github.com/yxlao/camtools.git cd camtools pip install -e . # Dev mode, if you
-want to modify camtools. pip install . # Install mode, if you want to use
-camtools only. ``` ## Camera coordinate system We follow the standard OpenCV-
-style camera coordinate system as shown below.
+normalization. - ... ## Installation To install CamTools, simply do: ```bash
+pip install camtools ``` Alternatively, you can install CamTools from source
+with one of the following methods: ```bash git clone https://github.com/yxlao/
+camtools.git cd camtools # Installation mode, if you want to use camtools only.
+pip install . # Dev mode, if you want to modify camtools on the fly. pip
+install -e . # Dev mode and dev dependencies, if you want to modify camtools
+and run tests. pip install -e .[dev] ``` ## Camera coordinate system We follow
+the standard OpenCV-style camera coordinate system as shown below.
                   [./camtools/assets/camera_coordinates.svg]
 - **Camera coordinate:** right-handed, with $Z$ pointing away from the camera
 towards the view direction and $Y$ axis pointing down. Note that this is
 different from the Blender convention, where $Z$ points towards the opposite
 view direction and the $Y$ axis points up. - **Image coordinate:** starts from
 the top-left corner of the image, with $x$ pointing right (corresponding to the
 image width) and $y$ pointing down (corresponding to the image height). This is
```

### Comparing `camtools-0.1.1/README.md` & `camtools-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,35 @@
+Metadata-Version: 2.1
+Name: camtools
+Version: 0.1.2
+Summary: CamTools: Camera Tools for Computer Vision.
+License: MIT
+Project-URL: Homepage, https://github.com/yxlao/camtools
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # CamTools: Camera Tools for Computer Vision
 
 CamTools is a useful tool for handling cameras in computer vision. It can be
 used for plotting, converting, projecting, ray casting, and doing more with
 camera parameters. It follows the standard camera coordinate system with clear
 and easy-to-use APIs.
 
 <a href="https://github.com/yxlao/camtools/actions/workflows/formatter.yml">
-  <img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+<img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml/badge.svg" alt="Unit Test">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/pypi.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/pypi.yml/badge.svg" alt="PyPI">
 </a>
 
 ## What can you do with CamTools?
 
 1. Plot cameras. Useful for debugging 3D reconstruction and NeRFs!
 
    ```python
@@ -24,14 +43,15 @@
       <img src="./camtools/assets/camera_frames.png" width="360" />
    </p>
 
 2. Convert camera parameters.
 
    ```python
    pose = ct.convert.T_to_pose(T)     # Convert T to pose
+   T    = ct.convert.T_to_pose(pose)  # Convert pose to T
    R, t = ct.convert.T_to_R_t(T)      # Convert T to R and t
    C    = ct.convert.pose_to_C(pose)  # Convert pose to camera center
    K, T = ct.convert.P_to_K_T(P)      # Decompose projection matrix to K and T
                                       # And more...
    ```
 
 3. Projection and ray casting.
@@ -88,26 +108,35 @@
    - Solve line intersections.
    - COLMAP tools.
    - Points normalization.
    - ...
 
 ## Installation
 
+To install CamTools, simply do:
+
 ```bash
-# Option 1: install from pip.
 pip install camtools
+```
 
-# Option 2: install from git.
-pip install git+https://github.com/yxlao/camtools.git
+Alternatively, you can install CamTools from source with one of the following
+methods:
 
-# Option 3: install from source.
+```bash
 git clone https://github.com/yxlao/camtools.git
 cd camtools
-pip install -e .  # Dev mode, if you want to modify camtools.
-pip install .     # Install mode, if you want to use camtools only.
+
+# Installation mode, if you want to use camtools only.
+pip install .
+
+# Dev mode, if you want to modify camtools on the fly.
+pip install -e .
+
+# Dev mode and dev dependencies, if you want to modify camtools and run tests.
+pip install -e .[dev]
 ```
 
 ## Camera coordinate system
 
 We follow the standard OpenCV-style camera coordinate system as shown below.
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,45 +1,53 @@
-# CamTools: Camera Tools for Computer Vision CamTools is a useful tool for
-handling cameras in computer vision. It can be used for plotting, converting,
-projecting, ray casting, and doing more with camera parameters. It follows the
-standard camera coordinate system with clear and easy-to-use APIs. [Formatter]
-## What can you do with CamTools? 1. Plot cameras. Useful for debugging 3D
-reconstruction and NeRFs! ```python import camtools as ct import open3d as o3d
-cameras = ct.camera.create_camera_ray_frames(Ks, Ts)
-o3d.visualization.draw_geometries([cameras]) ```
+Metadata-Version: 2.1 Name: camtools Version: 0.1.2 Summary: CamTools: Camera
+Tools for Computer Vision. License: MIT Project-URL: Homepage, https://
+github.com/yxlao/camtools Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE # CamTools: Camera Tools for Computer Vision CamTools is a useful tool
+for handling cameras in computer vision. It can be used for plotting,
+converting, projecting, ray casting, and doing more with camera parameters. It
+follows the standard camera coordinate system with clear and easy-to-use APIs.
+[Formatter] [Unit_Test] [PyPI] ## What can you do with CamTools? 1. Plot
+cameras. Useful for debugging 3D reconstruction and NeRFs! ```python import
+camtools as ct import open3d as o3d cameras =
+ct.camera.create_camera_ray_frames(Ks, Ts) o3d.visualization.draw_geometries(
+[cameras]) ```
                      [./camtools/assets/camera_frames.png]
 2. Convert camera parameters. ```python pose = ct.convert.T_to_pose(T) #
-Convert T to pose R, t = ct.convert.T_to_R_t(T) # Convert T to R and t C =
-ct.convert.pose_to_C(pose) # Convert pose to camera center K, T =
-ct.convert.P_to_K_T(P) # Decompose projection matrix to K and T # And more...
-``` 3. Projection and ray casting. ```python # Project 3D points to pixels.
-pixels = ct.project.points_to_pixel(points, K, T) # Back-project depth image to
-3D points. points = ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a
-triangle mesh to depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks,
-Ts, height, width) # And more... ``` 4. Image and depth I/O with no surprises.
-Strict type checks and range checks are enforced. The image and depth I/O APIs
-are specifically designed to solve the following pain points: - Is my image of
-type `float32` or `uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it
-RGB or BGR? - Does my image have an alpha channel? - When saving depth image as
-integer-based `.png`, is it correctly scaled? ```python ct.io.imread()
-ct.io.imwrite() ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line
-tools `ct` (runs in terminal). ```bash # Crop image boarders. ct crop-boarders
-*.png --pad_pixel 10 --skip_cropped --same_crop # Draw synchronized bounding
-boxes interactively. ct draw-bboxes path/to/a.png path/to/b.png # For more
-command-line tools. ct --help ```
+Convert T to pose T = ct.convert.T_to_pose(pose) # Convert pose to T R, t =
+ct.convert.T_to_R_t(T) # Convert T to R and t C = ct.convert.pose_to_C(pose) #
+Convert pose to camera center K, T = ct.convert.P_to_K_T(P) # Decompose
+projection matrix to K and T # And more... ``` 3. Projection and ray casting.
+```python # Project 3D points to pixels. pixels = ct.project.points_to_pixel
+(points, K, T) # Back-project depth image to 3D points. points =
+ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a triangle mesh to
+depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks, Ts, height, width)
+# And more... ``` 4. Image and depth I/O with no surprises. Strict type checks
+and range checks are enforced. The image and depth I/O APIs are specifically
+designed to solve the following pain points: - Is my image of type `float32` or
+`uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it RGB or BGR? -
+Does my image have an alpha channel? - When saving depth image as integer-based
+`.png`, is it correctly scaled? ```python ct.io.imread() ct.io.imwrite()
+ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line tools `ct` (runs
+in terminal). ```bash # Crop image boarders. ct crop-boarders *.png --pad_pixel
+10 --skip_cropped --same_crop # Draw synchronized bounding boxes interactively.
+ct draw-bboxes path/to/a.png path/to/b.png # For more command-line tools. ct --
+help ```
   [https://user-images.githubusercontent.com/1501945/241416210-e11ff3bf-22e6-
                           46c0-8ba0-d177a0015323.png]
 6. And more. - Solve line intersections. - COLMAP tools. - Points
-normalization. - ... ## Installation ```bash # Option 1: install from pip. pip
-install camtools # Option 2: install from git. pip install git+https://
-github.com/yxlao/camtools.git # Option 3: install from source. git clone https:
-//github.com/yxlao/camtools.git cd camtools pip install -e . # Dev mode, if you
-want to modify camtools. pip install . # Install mode, if you want to use
-camtools only. ``` ## Camera coordinate system We follow the standard OpenCV-
-style camera coordinate system as shown below.
+normalization. - ... ## Installation To install CamTools, simply do: ```bash
+pip install camtools ``` Alternatively, you can install CamTools from source
+with one of the following methods: ```bash git clone https://github.com/yxlao/
+camtools.git cd camtools # Installation mode, if you want to use camtools only.
+pip install . # Dev mode, if you want to modify camtools on the fly. pip
+install -e . # Dev mode and dev dependencies, if you want to modify camtools
+and run tests. pip install -e .[dev] ``` ## Camera coordinate system We follow
+the standard OpenCV-style camera coordinate system as shown below.
                   [./camtools/assets/camera_coordinates.svg]
 - **Camera coordinate:** right-handed, with $Z$ pointing away from the camera
 towards the view direction and $Y$ axis pointing down. Note that this is
 different from the Blender convention, where $Z$ points towards the opposite
 view direction and the $Y$ axis points up. - **Image coordinate:** starts from
 the top-left corner of the image, with $x$ pointing right (corresponding to the
 image width) and $y$ pointing down (corresponding to the image height). This is
```

### Comparing `camtools-0.1.1/camtools/camera.py` & `camtools-0.1.2/camtools/camera.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/colmap.py` & `camtools-0.1.2/camtools/colmap.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/colormap.py` & `camtools-0.1.2/camtools/colormap.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/convert.py` & `camtools-0.1.2/camtools/convert.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/geometry.py` & `camtools-0.1.2/camtools/geometry.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/image.py` & `camtools-0.1.2/camtools/image.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/io.py` & `camtools-0.1.2/camtools/io.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/metric.py` & `camtools-0.1.2/camtools/metric.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/normalize.py` & `camtools-0.1.2/camtools/normalize.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/plot.py` & `camtools-0.1.2/camtools/plot.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/project.py` & `camtools-0.1.2/camtools/project.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/raycast.py` & `camtools-0.1.2/camtools/raycast.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/sanity.py` & `camtools-0.1.2/camtools/sanity.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools/solver.py` & `camtools-0.1.2/camtools/solver.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/camtools.egg-info/PKG-INFO` & `camtools-0.1.2/camtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camtools
-Version: 0.1.1
+Version: 0.1.2
 Summary: CamTools: Camera Tools for Computer Vision.
 License: MIT
 Project-URL: Homepage, https://github.com/yxlao/camtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
@@ -15,15 +15,21 @@
 
 CamTools is a useful tool for handling cameras in computer vision. It can be
 used for plotting, converting, projecting, ray casting, and doing more with
 camera parameters. It follows the standard camera coordinate system with clear
 and easy-to-use APIs.
 
 <a href="https://github.com/yxlao/camtools/actions/workflows/formatter.yml">
-  <img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+<img src="https://github.com/yxlao/camtools/actions/workflows/formatter.yml/badge.svg" alt="Formatter">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/unit_test.yml/badge.svg" alt="Unit Test">
+</a>
+<a href="https://github.com/yxlao/camtools/actions/workflows/pypi.yml">
+<img src="https://github.com/yxlao/camtools/actions/workflows/pypi.yml/badge.svg" alt="PyPI">
 </a>
 
 ## What can you do with CamTools?
 
 1. Plot cameras. Useful for debugging 3D reconstruction and NeRFs!
 
    ```python
@@ -37,14 +43,15 @@
       <img src="./camtools/assets/camera_frames.png" width="360" />
    </p>
 
 2. Convert camera parameters.
 
    ```python
    pose = ct.convert.T_to_pose(T)     # Convert T to pose
+   T    = ct.convert.T_to_pose(pose)  # Convert pose to T
    R, t = ct.convert.T_to_R_t(T)      # Convert T to R and t
    C    = ct.convert.pose_to_C(pose)  # Convert pose to camera center
    K, T = ct.convert.P_to_K_T(P)      # Decompose projection matrix to K and T
                                       # And more...
    ```
 
 3. Projection and ray casting.
@@ -101,26 +108,35 @@
    - Solve line intersections.
    - COLMAP tools.
    - Points normalization.
    - ...
 
 ## Installation
 
+To install CamTools, simply do:
+
 ```bash
-# Option 1: install from pip.
 pip install camtools
+```
 
-# Option 2: install from git.
-pip install git+https://github.com/yxlao/camtools.git
+Alternatively, you can install CamTools from source with one of the following
+methods:
 
-# Option 3: install from source.
+```bash
 git clone https://github.com/yxlao/camtools.git
 cd camtools
-pip install -e .  # Dev mode, if you want to modify camtools.
-pip install .     # Install mode, if you want to use camtools only.
+
+# Installation mode, if you want to use camtools only.
+pip install .
+
+# Dev mode, if you want to modify camtools on the fly.
+pip install -e .
+
+# Dev mode and dev dependencies, if you want to modify camtools and run tests.
+pip install -e .[dev]
 ```
 
 ## Camera coordinate system
 
 We follow the standard OpenCV-style camera coordinate system as shown below.
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,50 +1,53 @@
-Metadata-Version: 2.1 Name: camtools Version: 0.1.1 Summary: CamTools: Camera
+Metadata-Version: 2.1 Name: camtools Version: 0.1.2 Summary: CamTools: Camera
 Tools for Computer Vision. License: MIT Project-URL: Homepage, https://
 github.com/yxlao/camtools Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE # CamTools: Camera Tools for Computer Vision CamTools is a useful tool
 for handling cameras in computer vision. It can be used for plotting,
 converting, projecting, ray casting, and doing more with camera parameters. It
 follows the standard camera coordinate system with clear and easy-to-use APIs.
-[Formatter] ## What can you do with CamTools? 1. Plot cameras. Useful for
-debugging 3D reconstruction and NeRFs! ```python import camtools as ct import
-open3d as o3d cameras = ct.camera.create_camera_ray_frames(Ks, Ts)
-o3d.visualization.draw_geometries([cameras]) ```
+[Formatter] [Unit_Test] [PyPI] ## What can you do with CamTools? 1. Plot
+cameras. Useful for debugging 3D reconstruction and NeRFs! ```python import
+camtools as ct import open3d as o3d cameras =
+ct.camera.create_camera_ray_frames(Ks, Ts) o3d.visualization.draw_geometries(
+[cameras]) ```
                      [./camtools/assets/camera_frames.png]
 2. Convert camera parameters. ```python pose = ct.convert.T_to_pose(T) #
-Convert T to pose R, t = ct.convert.T_to_R_t(T) # Convert T to R and t C =
-ct.convert.pose_to_C(pose) # Convert pose to camera center K, T =
-ct.convert.P_to_K_T(P) # Decompose projection matrix to K and T # And more...
-``` 3. Projection and ray casting. ```python # Project 3D points to pixels.
-pixels = ct.project.points_to_pixel(points, K, T) # Back-project depth image to
-3D points. points = ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a
-triangle mesh to depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks,
-Ts, height, width) # And more... ``` 4. Image and depth I/O with no surprises.
-Strict type checks and range checks are enforced. The image and depth I/O APIs
-are specifically designed to solve the following pain points: - Is my image of
-type `float32` or `uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it
-RGB or BGR? - Does my image have an alpha channel? - When saving depth image as
-integer-based `.png`, is it correctly scaled? ```python ct.io.imread()
-ct.io.imwrite() ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line
-tools `ct` (runs in terminal). ```bash # Crop image boarders. ct crop-boarders
-*.png --pad_pixel 10 --skip_cropped --same_crop # Draw synchronized bounding
-boxes interactively. ct draw-bboxes path/to/a.png path/to/b.png # For more
-command-line tools. ct --help ```
+Convert T to pose T = ct.convert.T_to_pose(pose) # Convert pose to T R, t =
+ct.convert.T_to_R_t(T) # Convert T to R and t C = ct.convert.pose_to_C(pose) #
+Convert pose to camera center K, T = ct.convert.P_to_K_T(P) # Decompose
+projection matrix to K and T # And more... ``` 3. Projection and ray casting.
+```python # Project 3D points to pixels. pixels = ct.project.points_to_pixel
+(points, K, T) # Back-project depth image to 3D points. points =
+ct.project.im_depth_to_points(im_depth, K, T) # Ray cast a triangle mesh to
+depth image. im_depth = ct.raycast.mesh_to_depths(mesh, Ks, Ts, height, width)
+# And more... ``` 4. Image and depth I/O with no surprises. Strict type checks
+and range checks are enforced. The image and depth I/O APIs are specifically
+designed to solve the following pain points: - Is my image of type `float32` or
+`uint8`? - Does it have range `[0, 1]` or `[0, 255]`? - Is it RGB or BGR? -
+Does my image have an alpha channel? - When saving depth image as integer-based
+`.png`, is it correctly scaled? ```python ct.io.imread() ct.io.imwrite()
+ct.io.imread_detph() ct.io.imwrite_depth() ``` 5. Command-line tools `ct` (runs
+in terminal). ```bash # Crop image boarders. ct crop-boarders *.png --pad_pixel
+10 --skip_cropped --same_crop # Draw synchronized bounding boxes interactively.
+ct draw-bboxes path/to/a.png path/to/b.png # For more command-line tools. ct --
+help ```
   [https://user-images.githubusercontent.com/1501945/241416210-e11ff3bf-22e6-
                           46c0-8ba0-d177a0015323.png]
 6. And more. - Solve line intersections. - COLMAP tools. - Points
-normalization. - ... ## Installation ```bash # Option 1: install from pip. pip
-install camtools # Option 2: install from git. pip install git+https://
-github.com/yxlao/camtools.git # Option 3: install from source. git clone https:
-//github.com/yxlao/camtools.git cd camtools pip install -e . # Dev mode, if you
-want to modify camtools. pip install . # Install mode, if you want to use
-camtools only. ``` ## Camera coordinate system We follow the standard OpenCV-
-style camera coordinate system as shown below.
+normalization. - ... ## Installation To install CamTools, simply do: ```bash
+pip install camtools ``` Alternatively, you can install CamTools from source
+with one of the following methods: ```bash git clone https://github.com/yxlao/
+camtools.git cd camtools # Installation mode, if you want to use camtools only.
+pip install . # Dev mode, if you want to modify camtools on the fly. pip
+install -e . # Dev mode and dev dependencies, if you want to modify camtools
+and run tests. pip install -e .[dev] ``` ## Camera coordinate system We follow
+the standard OpenCV-style camera coordinate system as shown below.
                   [./camtools/assets/camera_coordinates.svg]
 - **Camera coordinate:** right-handed, with $Z$ pointing away from the camera
 towards the view direction and $Y$ axis pointing down. Note that this is
 different from the Blender convention, where $Z$ points towards the opposite
 view direction and the $Y$ axis points up. - **Image coordinate:** starts from
 the top-left corner of the image, with $x$ pointing right (corresponding to the
 image width) and $y$ pointing down (corresponding to the image height). This is
```

### Comparing `camtools-0.1.1/pyproject.toml` & `camtools-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,18 @@
   "matplotlib>=3.3.4",
 ]
 description = "CamTools: Camera Tools for Computer Vision."
 license = {text = "MIT"}
 name = "camtools"
 readme = "README.md"
 requires-python = ">=3.6.0"
-version = "0.1.1"
+version = "0.1.2"
+
+[tool.setuptools]
+packages = ["camtools", "camtools.tools"]
 
 [project.urls]
 Homepage = "https://github.com/yxlao/camtools"
 
 [project.optional-dependencies]
 dev = [
   "black>=22.1.0",
```

### Comparing `camtools-0.1.1/test/test_convert.py` & `camtools-0.1.2/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `camtools-0.1.1/test/test_image.py` & `camtools-0.1.2/test/test_image.py`

 * *Files identical despite different names*

