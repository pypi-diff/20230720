# Comparing `tmp/track_generator-0.5.1.tar.gz` & `tmp/track_generator-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track_generator-0.5.1.tar", last modified: Fri Jul  7 09:00:08 2023, max compression
+gzip compressed data, was "track_generator-0.5.3.tar", last modified: Thu Jul 20 09:10:01 2023, max compression
```

## Comparing `track_generator-0.5.1.tar` & `track_generator-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 08:59:58.000000 track_generator-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 09:00:08.035945 track_generator-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 08:59:58.000000 track_generator-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 09:00:08.035945 track_generator-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 08:59:58.000000 track_generator-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.031945 track_generator-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 08:59:58.000000 track_generator-0.5.1/tests/test_track_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/coordinate_system.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gazebo_model_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/model.config.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/model.sdf.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/setup.bash.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/track.material.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     4464 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3763 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/ground_truth_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gui/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gui/qml/
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/qml/track_live_view.qml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/track_live_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14575 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/painter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/segment_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/segment_templates/crosswalk.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/segment_templates/intersection.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/starter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26049 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9571 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-07-07 08:59:58.000000 track_generator-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 09:09:49.000000 track_generator-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 09:10:01.178404 track_generator-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-20 09:09:49.000000 track_generator-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 09:10:01.178404 track_generator-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 09:09:49.000000 track_generator-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.174404 track_generator-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 09:09:49.000000 track_generator-0.5.3/tests/test_track_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/coordinate_system.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gazebo_model_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/model.config.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/model.sdf.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/setup.bash.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/track.material.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3875 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/ground_truth_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gui/qml/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/qml/track_live_view.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/track_live_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12318 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/painter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/segment_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/segment_templates/crosswalk.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/segment_templates/intersection.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2531 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/starter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27240 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7283 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/xsd/track.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83595 2023-07-20 09:09:49.000000 track_generator-0.5.3/versioneer.py
```

### Comparing `track_generator-0.5.1/setup.py` & `track_generator-0.5.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     description=("Track generator"),
     license="GPL 3.0",
     keywords="svg model vehicles track",
     url="https://github.com/twyleg/track_generator",
     packages=find_packages(),
     include_package_data=True,
     long_description=read("README.md"),
-    install_requires=["pytransform3d", "numpy", "drawsvg==1.9", "watchdog~=3.0.0", "pyside6~=6.5.1"],
+    long_description_content_type='text/markdown',
+    install_requires=[
+        "pytransform3d~=3.2.0",
+        "drawsvg~=2.2.0",
+        "watchdog~=3.0.0",
+        "pyside6==6.4.0.1",
+        "xmlschema~=2.3.1",
+    ],
     entry_points={
         "console_scripts": [
             "track_generator = track_generator.starter:start",
         ]
     },
 )
```

### Comparing `track_generator-0.5.1/track_generator/coordinate_system.py` & `track_generator-0.5.3/track_generator/coordinate_system.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # Copyright (C) 2022 twyleg
 import numpy as np
 import pytransform3d.rotations as pyrot
 import pytransform3d.transformations as pytr
-from typing import Optional, List
+from typing import List, Union
 
 
 class WorldCoordinateSystem:
     def __init__(self):
         self.local_to_world = pytr.transform_from(
             pyrot.matrix_from_axis_angle(np.array([0.0, 0.0, 1.0, 0.0])), np.array([0.0, 0.0, 0.0])
         )
 
 
 class CartesianSystem2d:
-    def __init__(self, x: float, y: float, yaw: float, parent: Optional["CartesianSystem"] = WorldCoordinateSystem()):
+    def __init__(
+        self,
+        x: float,
+        y: float,
+        yaw: float,
+        parent: Union["CartesianSystem2d", WorldCoordinateSystem] = WorldCoordinateSystem(),
+    ):
         p = np.array([x, y, 0.0])
         a = np.array([0.0, 0.0, 1.0, np.deg2rad(yaw)])
         local_to_parent = pytr.transform_from(pyrot.matrix_from_axis_angle(a), p)
         parent_to_world = parent.local_to_world
-        self.local_to_world = pytr.concat(local_to_parent, parent_to_world)
+        self.local_to_world: np.ndarray = pytr.concat(local_to_parent, parent_to_world)
 
 
 class Point2d:
     def __init__(self, x_l: float, y_l: float, local_coordinate_system: CartesianSystem2d):
         self.local_coordinate_system = local_coordinate_system
         self.x_l = x_l
         self.y_l = y_l
@@ -34,11 +40,7 @@
         self.y_w = point_world[1]
 
     def __str__(self):
         return f"Local: ({self.x_l},{self.y_l}), World: ({self.x_w},{self.y_w})"
 
 
 Polygon = List[Point2d]
-
-# class Polygon(List[Point2d]):
-#     def __init__(self, *args):
-#         super().__init__(self, *args)
```

### Comparing `track_generator-0.5.1/track_generator/gazebo_model_templates/model.sdf.template` & `track_generator-0.5.3/track_generator/gazebo_model_templates/model.sdf.template`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.1/track_generator/generator.py` & `track_generator-0.5.3/track_generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 import os
 from pathlib import Path
 from typing import List, Callable
 
 from track_generator import xml_reader
 from track_generator.painter import Painter
 from track_generator.gazebo_model_generator import GazeboModelGenerator
-from track_generator.gui.track_live_view import TrackLiveView
 from track_generator.ground_truth_generator import GroundTruthGenerator
 
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 
 def _create_output_directory_if_required(output_dirpath: Path):
-    output_dirpath.mkdir(exist_ok=True)
+    output_dirpath.mkdir(parents=True, exist_ok=True)
 
 
 def _get_track_name_from_file_path(track_filepath: Path) -> str:
     filename = os.path.basename(track_filepath)
     filename_without_extension, _ = os.path.splitext(filename)
     return filename_without_extension
 
 
 def generate_track(
     track_filepaths: List[Path],
     root_output_dirpath: Path,
     generate_png=False,
     generate_gazebo_project=False,
     generate_ground_truth=False,
-) -> List[str]:
+) -> List[Path]:
     """
     Generate tracks (SVG, Gazebo project, etc) from given track files (XML)
     :param track_filepaths: List of track files
     :param root_output_dirpath: The output directory to write results to. Subdirectories for every track will be
     generated.
     :param generate_png: Flag whether a png image should be created for the track
     :param generate_gazebo_project:Flag whether gazebo project files should be created for the track
@@ -71,17 +70,14 @@
 
 
 class FileChangedHandler(FileSystemEventHandler):
     def __init__(self, input_filepath: Path, callback: Callable):
         self.input_filepath = input_filepath
         self.callback = callback
 
-    # def on_any_event(self, event) -> None:
-    #     pass
-
     def on_closed(self, event) -> None:
         event_filepath = Path(event.src_path)
         if event_filepath == self.input_filepath:
             self.callback()
         return None
 
 
@@ -91,15 +87,17 @@
     :param track_file: Track file
     :param root_output_directory: The output directory to write results to. Subdirectories for every track will be
     generated.
     :return: Output directory for the track
     """
     track_file_directory = track_file.parent
     track_name = _get_track_name_from_file_path(track_file)
-    output_file_path = os.path.join(root_output_directory, track_name, f"{track_name}.svg")
+    output_file_path = root_output_directory / track_name / f"{track_name}.svg"
+    from track_generator.gui.track_live_view import TrackLiveView
+
     track_live_view = TrackLiveView(output_file_path)
 
     def update():
         print(f"Track file changed, regenerating track ({track_file})")
         generate_track([track_file], root_output_directory, generate_png=False, generate_gazebo_project=False)
         track_live_view.update()
```

### Comparing `track_generator-0.5.1/track_generator/ground_truth_generator.py` & `track_generator-0.5.3/track_generator/ground_truth_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
+from pathlib import Path
 from xml.etree import cElementTree as ET, ElementTree
 from xml.etree import ElementTree
 from xml.dom import minidom
 
 from track_generator.track import (
     Segment,
     Track,
     Start,
     Straight,
-    Arc,
+    Turn,
     Crosswalk,
     Intersection,
     Gap,
     ParkingArea,
     TrafficIsland,
     Clothoid,
 )
 
 
 class GroundTruthGenerator:
-    def __init__(self, track_name: str, output_directory: str):
+    def __init__(self, track_name: str, output_directory: Path):
         self.track_name = track_name
         self.output_directory = output_directory
         self.root = ET.Element("GroundTruth", {"version": "0.0.1"})
         self.points = ET.SubElement(self.root, "Points")
 
     def generate_ground_truth(self, track: Track):
         for segment in track.segments:
             self.generate_segment(segment)
-        with open(self.output_directory + "ground_truth.xml", "w") as f:
+        with open(self.output_directory / "ground_truth.xml", "w") as f:
             f.write(minidom.parseString(ET.tostring(self.root, "utf-8")).toprettyxml(indent="\t"))
 
     def generate_segment(self, segment: Segment):
         if isinstance(segment, Start):
             pass
         elif isinstance(segment, (Straight, ParkingArea, Gap, Crosswalk)):
             self.generate_straight(segment)
-        elif isinstance(segment, Arc):
-            self.generate_arc(segment)
+        elif isinstance(segment, Turn):
+            self.generate_turn(segment)
         elif isinstance(segment, Intersection):
             self.generate_intersection(segment)
         elif isinstance(segment, TrafficIsland):
             self.generate_traffic_island(segment)
         elif isinstance(segment, Clothoid):
             self.generate_clothoid(segment)
         else:
@@ -49,15 +50,17 @@
     def generate_straight(self, segment: Straight):
         for i, _ in enumerate(segment.center_line_polygon):
             self.write_points(
                 [segment.left_line_polygon[i].x_w, segment.left_line_polygon[i].y_w],
                 [segment.right_line_polygon[i].x_w, segment.right_line_polygon[i].y_w],
             )
 
-    def generate_arc(self, segment: Arc):
+    def generate_turn(self, segment: Turn):
+        assert segment.start_point_left
+        assert segment.start_point_right
         self.write_points(
             [segment.start_point_left.x_w, segment.start_point_left.y_w],
             [segment.start_point_right.x_w, segment.start_point_right.y_w],
         )
 
     def generate_intersection(self, segment: Intersection):
         for i, _ in enumerate(segment.corner_line_polygons[0]):
```

### Comparing `track_generator-0.5.1/track_generator/gui/qml/track_live_view.qml` & `track_generator-0.5.3/track_generator/gui/qml/track_live_view.qml`

 * *Files 20% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 	Image {
 		id: img
 
 		fillMode: Image.PreserveAspectFit
 		anchors.fill: parent
 		cache: false
-		source: model.filename
+		source: model.filepath
 		sourceSize.height: height
 		sourceSize.width: width
 
 		width: parent.width
 		height: parent.height
 
 		function reload() {
 			console.log('Reloading image!')
 			source = ""
-			source = model.filename
+			source = model.filepath
 		}
 	}
 
 	Connections {
 		target: model
 
 		function onReloadImage() {
```

### Comparing `track_generator-0.5.1/track_generator/painter.py` & `track_generator-0.5.3/track_generator/painter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,397 +1,343 @@
 # Copyright (C) 2022 twyleg
-import os
 import math
-import drawSvg as draw
+import drawsvg as draw
 
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Tuple
 from track_generator.track import (
     Track,
     Start,
     Straight,
-    Arc,
+    Turn,
     Crosswalk,
     Intersection,
     Gap,
     ParkingArea,
     TrafficIsland,
     Clothoid,
+    BackgroundColor,
+    BackgroundImage,
 )
 from track_generator.coordinate_system import Point2d, Polygon
 
 DEFAULT_LINE_WIDTH = 0.020
 DEFAULT_TRACK_WIDTH = 0.800
+DEFAULT_LANE_WIDTH = 0.380
 
 DEFAULT_TRACK_COLOR = "#000000"
 DEFAULT_LINE_COLOR = "#ffffff"
 
 
+class SvgPoint:
+    IMAGE_HEIGHT = 0.0
+
+    def __init__(self, point: Point2d) -> None:
+        self.point = point
+        self.x = point.x_w
+        self.y = self.IMAGE_HEIGHT - point.y_w
+
+    @property
+    def p(self) -> Tuple[float, float]:
+        return self.x, self.y
+
+
 class Painter:
     def __init__(self):
         self.d: Optional[draw.Drawing] = None
+        self.dash_style = "stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0"
+
+        self.default_track_background_style = {
+            "fill": "none",
+            "stroke": DEFAULT_TRACK_COLOR,
+            "stroke_width": DEFAULT_TRACK_WIDTH,
+        }
+
+        self.default_center_line_style = {
+            "fill": "none",
+            "stroke": DEFAULT_LINE_COLOR,
+            "stroke_width": DEFAULT_LINE_WIDTH,
+            "style": self.dash_style,
+        }
+
+        self.default_outer_line_style = {
+            "fill": "none",
+            "stroke": DEFAULT_LINE_COLOR,
+            "stroke_width": DEFAULT_LINE_WIDTH,
+        }
+
+    @classmethod
+    def direction_angle_to_svg_arc_angle(cls, direction_angle: float, cw: bool):
+        rotation_angle = -90.0 if cw else 90.0
+        return -direction_angle + rotation_angle
 
     def draw_polygon(self, polygon: Polygon, **kwargs) -> None:
-        if len(polygon) < 2:
-            return
-        for i in range(1, len(polygon)):
-            p0 = polygon[i - 1]
-            p1 = polygon[i]
-            self.d.append(draw.Line(p0.x_w, p0.y_w, p1.x_w, p1.y_w, **kwargs))
+        assert self.d
+        points = []
+        for point in polygon:
+            points.extend([*SvgPoint(point).p])
+        self.d.append(draw.Lines(*points, **kwargs))
 
     def draw_point(self, p: Point2d):
-        self.d.append(draw.Circle(p.x_w, p.y_w, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
-
-        self.d.append(draw.Text(f"{p.x_w:.3f}\n{p.y_w:.3f}", 0.1, p.x_w + 0.032, p.y_w, fill="red"))
+        assert self.d
+        svg_p = SvgPoint(p)
+        self.d.append(draw.Circle(*svg_p.p, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
+        self.d.append(draw.Text(f"{p.x_w:.3f}\n{p.y_w:.3f}", 0.1, svg_p.x + 0.032, svg_p.y, fill="red"))
 
     def draw_arc_center_point(self, p: Point2d, radian_angle, radius):
-        self.d.append(draw.Circle(p.x_w, p.y_w, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
-
+        assert self.d
+        svg_p = SvgPoint(p)
+        self.d.append(draw.Circle(*svg_p.p, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
         self.d.append(
             draw.Text(
                 f"{p.x_w:.3f}\n{p.y_w:.3f}\nr={radius:.3f}\na={radian_angle:.1f}°",
                 0.1,
-                p.x_w + 0.032,
-                p.y_w,
+                svg_p.x + 0.032,
+                svg_p.y,
                 fill="red",
             )
         )
 
     def draw_start_verbose(self, segment: Start):
         self.draw_point(segment.start_point)
 
     def draw_straight(self, segment: Straight):
-        self.draw_polygon(
-            segment.center_line_polygon,
-            fill=DEFAULT_TRACK_COLOR,
-            stroke=DEFAULT_TRACK_COLOR,
-            stroke_width=DEFAULT_TRACK_WIDTH,
-        )
-        self.draw_polygon(
-            segment.center_line_polygon,
-            stroke=DEFAULT_LINE_COLOR,
-            stroke_width=DEFAULT_LINE_WIDTH,
-            fill="none",
-            style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0,fill-opacity:0",
-        )
-        # stroke-miterlimit:4;stroke-dasharray:0.08,0.16;stroke-dashoffset:0;stroke-width:0.02
-
-        self.draw_polygon(
-            segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
-        )
-        self.draw_polygon(
-            segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
-        )
+        self.draw_polygon(segment.center_line_polygon, **self.default_track_background_style)
+        self.draw_polygon(segment.center_line_polygon, **self.default_center_line_style)
+        self.draw_polygon(segment.left_line_polygon, **self.default_outer_line_style)
+        self.draw_polygon(segment.right_line_polygon, **self.default_outer_line_style)
 
     def draw_straight_verbose(self, segment: Straight):
         self.draw_point(segment.center_line_polygon[0])
         self.draw_point(segment.left_line_polygon[0])
         self.draw_point(segment.right_line_polygon[0])
 
-    def draw_arc(self, segment: Arc):
-        end_angle = segment.direction_angle
-        start_angle = segment.start_direction_angle
-
-        if segment.direction_clockwise:
-            final_end_angle = end_angle + 90
-            final_start_angle = start_angle + 90
-        else:
-            final_end_angle = end_angle - 90
-            final_start_angle = start_angle - 90
+    def draw_turn(self, segment: Turn):
+        assert segment.direction_angle is not None
+        assert segment.start_direction_angle is not None
+        assert segment.center_point
+        assert self.d
+
+        start_angle = self.direction_angle_to_svg_arc_angle(segment.start_direction_angle, segment.direction_clockwise)
+        end_angle = self.direction_angle_to_svg_arc_angle(segment.direction_angle, segment.direction_clockwise)
+
+        svg_center_point = SvgPoint(segment.center_point).p
 
         self.d.append(
             draw.Arc(
-                segment.center_point.x_w,
-                segment.center_point.y_w,
+                *svg_center_point,
                 math.fabs(segment.radius),
-                final_start_angle,
-                final_end_angle,
+                start_angle,
+                end_angle,
                 cw=segment.direction_clockwise,
-                stroke=DEFAULT_TRACK_COLOR,
-                stroke_width=DEFAULT_TRACK_WIDTH,
-                fill="none",
+                **self.default_track_background_style,
             )
         )
 
         self.d.append(
             draw.Arc(
-                segment.center_point.x_w,
-                segment.center_point.y_w,
-                math.fabs(segment.radius) - 0.380,
-                final_start_angle,
-                final_end_angle,
+                *svg_center_point,
+                math.fabs(segment.radius) - DEFAULT_LANE_WIDTH,
+                start_angle,
+                end_angle,
                 cw=segment.direction_clockwise,
-                stroke=DEFAULT_LINE_COLOR,
-                stroke_width=DEFAULT_LINE_WIDTH,
-                fill="none",
+                **self.default_outer_line_style,
             )
         )
 
         self.d.append(
             draw.Arc(
-                segment.center_point.x_w,
-                segment.center_point.y_w,
-                math.fabs(segment.radius) + 0.380,
-                final_start_angle,
-                final_end_angle,
+                *svg_center_point,
+                math.fabs(segment.radius) + DEFAULT_LANE_WIDTH,
+                start_angle,
+                end_angle,
                 cw=segment.direction_clockwise,
-                stroke=DEFAULT_LINE_COLOR,
-                stroke_width=DEFAULT_LINE_WIDTH,
-                fill="none",
+                **self.default_outer_line_style,
             )
         )
 
         self.d.append(
             draw.Arc(
-                segment.center_point.x_w,
-                segment.center_point.y_w,
+                *svg_center_point,
                 math.fabs(segment.radius),
-                final_start_angle,
-                final_end_angle,
+                start_angle,
+                end_angle,
                 cw=segment.direction_clockwise,
-                stroke=DEFAULT_LINE_COLOR,
-                stroke_width=DEFAULT_LINE_WIDTH,
-                fill="none",
-                style="stroke-miterlimit:4;stroke-dasharray:0.160,0.160;stroke-dashoffset:0",
+                **self.default_center_line_style,
             )
         )
 
-    def draw_arc_verbose(self, segment: Arc):
-        end_angle = segment.direction_angle
-        start_angle = segment.start_direction_angle
-
-        if segment.direction_clockwise:
-            final_end_angle = end_angle + 90
-            final_start_angle = start_angle + 90
-        else:
-            final_end_angle = end_angle - 90
-            final_start_angle = start_angle - 90
+    def draw_turn_verbose(self, segment: Turn):
+        assert segment.direction_angle is not None
+        assert segment.start_direction_angle is not None
+        assert segment.center_point
+        assert segment.start_point_center
+        assert segment.start_point_left
+        assert segment.start_point_right
+        assert self.d
+
+        start_angle = self.direction_angle_to_svg_arc_angle(segment.start_direction_angle, segment.direction_clockwise)
+        end_angle = self.direction_angle_to_svg_arc_angle(segment.direction_angle, segment.direction_clockwise)
+
+        svg_center_point = SvgPoint(segment.center_point).p
 
         p = draw.Path(fill="none", stroke="blue", stroke_width=DEFAULT_LINE_WIDTH)
         p.arc(
-            segment.center_point.x_w,
-            segment.center_point.y_w,
+            *svg_center_point,
             math.fabs(segment.radius),
-            final_end_angle,
-            final_start_angle,
-            cw=not segment.direction_clockwise,
+            start_angle,
+            end_angle,
+            cw=segment.direction_clockwise,
         )
         p.arc(
-            segment.center_point.x_w,
-            segment.center_point.y_w,
+            *svg_center_point,
             0,
-            final_start_angle,
-            final_end_angle,
+            start_angle,
+            end_angle,
             cw=segment.direction_clockwise,
-            includeL=True,
+            include_l=True,
         )
         p.Z()
         self.d.append(p)
 
         self.draw_arc_center_point(segment.center_point, segment.radian_angle, segment.radius)
         self.draw_point(segment.start_point_center)
         self.draw_point(segment.start_point_left)
         self.draw_point(segment.start_point_right)
 
     def draw_crosswalk(self, segment: Crosswalk):
-        self.draw_polygon(
-            segment.center_line_polygon, fill="#eeee00", stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH
-        )
-        self.draw_polygon(
-            segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
-        )
-        self.draw_polygon(
-            segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
-        )
+        self.draw_polygon(segment.center_line_polygon, **self.default_track_background_style)
+        self.draw_polygon(segment.left_line_polygon, **self.default_outer_line_style)
+        self.draw_polygon(segment.right_line_polygon, **self.default_outer_line_style)
 
         for polygon in segment.line_polygons:
             self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill="none")
 
     def draw_intersection(self, segment: Intersection):
         for polygon in segment.base_line_polygons:
-            self.draw_polygon(polygon, fill="#eeee00", stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH)
+            self.draw_polygon(polygon, **self.default_track_background_style)
 
         for polygon in segment.corner_line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
+            self.draw_polygon(polygon, **self.default_outer_line_style)
 
         for polygon in segment.stop_line_polygons:
             self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH * 2, fill="none")
 
         for polygon in segment.center_line_polygons:
-            self.draw_polygon(
-                polygon,
-                stroke=DEFAULT_LINE_COLOR,
-                stroke_width=DEFAULT_LINE_WIDTH,
-                fill="none",
-                style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0",
-            )
+            self.draw_polygon(polygon, **self.default_center_line_style)
 
     def draw_traffic_island(self, segment: TrafficIsland):
-        self.d.append(
-            draw.Lines(
-                segment.background_polygon[0].x_w,
-                segment.background_polygon[0].y_w,
-                segment.background_polygon[1].x_w,
-                segment.background_polygon[1].y_w,
-                segment.background_polygon[2].x_w,
-                segment.background_polygon[2].y_w,
-                segment.background_polygon[3].x_w,
-                segment.background_polygon[3].y_w,
-                segment.background_polygon[4].x_w,
-                segment.background_polygon[4].y_w,
-                segment.background_polygon[5].x_w,
-                segment.background_polygon[5].y_w,
-                segment.background_polygon[6].x_w,
-                segment.background_polygon[6].y_w,
-                segment.background_polygon[7].x_w,
-                segment.background_polygon[7].y_w,
-                close=False,
-                fill=DEFAULT_TRACK_COLOR,
-            )
-        )
+        assert self.d
+        self.draw_polygon(segment.background_polygon)
 
         for polygon in segment.line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
+            self.draw_polygon(polygon, **self.default_outer_line_style)
 
         for polygon in segment.crosswalk_lines_polygons:
             self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill="none")
 
     def draw_parking_area(self, segment: ParkingArea):
+        assert self.d
         self.draw_straight(segment)
 
         for polygon in segment.outline_polygon:
-            # Background
-            self.d.append(
-                draw.Lines(
-                    polygon[0].x_w,
-                    polygon[0].y_w,
-                    polygon[1].x_w,
-                    polygon[1].y_w,
-                    polygon[2].x_w,
-                    polygon[2].y_w,
-                    polygon[3].x_w,
-                    polygon[3].y_w,
-                    close=False,
-                    fill=DEFAULT_TRACK_COLOR,
-                )
+            self.draw_polygon(
+                polygon, fill=DEFAULT_TRACK_COLOR, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH
             )
-            # Outline
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
         for polygon in segment.spot_seperator_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
+            self.draw_polygon(polygon, **self.default_outer_line_style)
 
         for polygon in segment.blocker_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
+            self.draw_polygon(polygon, **self.default_outer_line_style)
 
     def draw_clothoid(self, segment: Clothoid):
-        background: tuple(float) = ()
-        for p in segment.background_polygon:
-            background += (p.x_w, p.y_w)
-        self.d.append(
-            draw.Lines(
-                background[0],
-                background[1],
-                *background,
-                fill=DEFAULT_TRACK_COLOR,
-                stroke=DEFAULT_TRACK_COLOR,
-                stroke_width=2 * DEFAULT_LINE_WIDTH,
-            )
-        )
-        middle_line: tuple(float) = ()
-        for p in segment.lines[0]:
-            middle_line += (p.x_w, p.y_w)
-        self.d.append(
-            draw.Lines(
-                *middle_line,
-                fill="none",
-                stroke=DEFAULT_LINE_COLOR,
-                stroke_width=DEFAULT_LINE_WIDTH,
-                style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0",
-            )
-        )
-        left_line: tuple(float) = ()
-        for p in segment.lines[1]:
-            left_line += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(*left_line, fill="none", stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
-        right_line: tuple(float) = ()
-        for p in segment.lines[2]:
-            right_line += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(*right_line, fill="none", stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
+        assert self.d
+        self.draw_polygon(segment.lines[0], **self.default_track_background_style)
+        self.draw_polygon(segment.lines[0], **self.default_center_line_style)
+        self.draw_polygon(segment.lines[1], **self.default_outer_line_style)
+        self.draw_polygon(segment.lines[2], **self.default_outer_line_style)
 
     def draw_template_based_segment(self, segment, template_file_path: str):
+        assert self.d
+        svg_start_point_center = SvgPoint(segment.start_point_center)
         self.d.append(
             draw.Image(
-                segment.start_point_center.x_w - (segment.width / 2.0),
-                segment.start_point_center.y_w,
+                svg_start_point_center.x - (segment.width / 2.0),
+                svg_start_point_center.y,
                 segment.width,
                 segment.height,
                 template_file_path,
                 embed=True,
-                transform=f"rotate({-(segment.direction_angle - 90.0)} , {segment.start_point_center.x_w}, {-segment.start_point_center.y_w})",
+                transform=f"rotate({-segment.direction_angle + 90.0} , {svg_start_point_center.x}, {svg_start_point_center.y})",
             )
         )
 
     def draw_segment(self, segment):
         if isinstance(segment, Start):
             pass
         elif isinstance(segment, Gap):
             pass
         elif isinstance(segment, Crosswalk):
             self.draw_crosswalk(segment)
         elif isinstance(segment, ParkingArea):
             self.draw_parking_area(segment)
         elif isinstance(segment, Straight):
             self.draw_straight(segment)
-        elif isinstance(segment, Arc):
-            self.draw_arc(segment)
+        elif isinstance(segment, Turn):
+            self.draw_turn(segment)
         elif isinstance(segment, Intersection):
             self.draw_intersection(segment)
         elif isinstance(segment, TrafficIsland):
             self.draw_traffic_island(segment)
         elif isinstance(segment, Clothoid):
             self.draw_clothoid(segment)
         else:
             raise RuntimeError()
 
     def draw_segment_verbose(self, segment):
         if isinstance(segment, Start):
             pass
         elif isinstance(segment, Straight):
             self.draw_straight_verbose(segment)
-        elif isinstance(segment, Arc):
-            self.draw_arc_verbose(segment)
+        elif isinstance(segment, Turn):
+            self.draw_turn_verbose(segment)
 
     def draw_track(self, track: Track):
+        SvgPoint.IMAGE_HEIGHT = track.height
         self.d = draw.Drawing(track.width, track.height, origin=track.origin, displayInline=False)
-        self.d.setPixelScale(1000)
-        self.d.append(
-            draw.Rectangle(
-                0,
-                0,
-                track.width,
-                track.height,
-                fill=track.background.color.color,
-                fill_opacity=track.background.color.opacity,
-            )
-        )
+        self.d.set_pixel_scale(1000)
 
-        if track.background.image:
-            img = track.background.image
+        if isinstance(track.background, BackgroundColor):
+            self.d.append(
+                draw.Rectangle(
+                    0,
+                    0,
+                    track.width,
+                    track.height,
+                    fill=track.background.color,
+                    fill_opacity=track.background.opacity,
+                )
+            )
+        elif isinstance(track.background, BackgroundImage):
+            img = track.background
             self.d.append(
-                draw.Image(img.x, img.y, img.width, img.height, img.file, embed=True, preserveAspectRatio="none")
+                draw.Image(img.x, img.y, img.width, img.height, img.filepath, embed=True, preserveAspectRatio="none")
             )
 
         for segment in track.segments:
             self.draw_segment(segment)
 
     def draw_track_verbose(self, track: Track):
         for segment in track.segments:
             self.draw_segment_verbose(segment)
 
-    def save_svg(self, track_name: str, output_directory: str, file_name_postfix: str = ""):
-        output_file_path = os.path.join(output_directory, track_name)
-        self.d.saveSvg(f"{output_file_path}{file_name_postfix}.svg")
-
-    def save_png(self, track_name: str, output_directory: str):
-        output_file_path = os.path.join(output_directory, track_name)
-        self.d.setPixelScale(1000)
-        self.d.savePng(f"{output_file_path}.png")
+    def save_svg(self, track_name: str, output_directory: Path, file_name_postfix: str = ""):
+        assert self.d
+        output_file_path = output_directory / track_name
+        self.d.save_svg(f"{output_file_path}{file_name_postfix}.svg")
+
+    def save_png(self, track_name: str, output_directory: Path):
+        assert self.d
+        output_file_path = output_directory / track_name
+        self.d.set_pixel_scale(1000)
+        self.d.save_png(f"{output_file_path}.png")
```

### Comparing `track_generator-0.5.1/track_generator/segment_templates/crosswalk.svg` & `track_generator-0.5.3/track_generator/segment_templates/crosswalk.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.1/track_generator/segment_templates/intersection.svg` & `track_generator-0.5.3/track_generator/segment_templates/intersection.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.1/track_generator/starter.py` & `track_generator-0.5.3/track_generator/starter.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         help='Output directory for generated tracks. Default="./"',
     )
     parser.add_argument("--png", action="store_true", help="Generate output PNG (SVG only by default).")
     parser.add_argument("--gazebo", action="store_true", help="Generate Gazebo model for track.")
     parser.add_argument("--ground_truth", action="store_true", help="Generate ground truth data for track.")
     args = parser.parse_args(sys.argv[2:])
 
-    generator.generate_track(args.track_files, args.output, args.png, args.gazebo, args.ground_truth)
+    track_file_filepaths = [Path(filepath) for filepath in args.track_files]
+    output_dirpath = Path(args.output)
+
+    generator.generate_track(track_file_filepaths, output_dirpath, args.png, args.gazebo, args.ground_truth)
 
 
 def subcommand_generate_track_live():
     parser = argparse.ArgumentParser(description="Generates a track")
     parser.add_argument(
         "track_file", metavar="track_file", type=str, help="a track file (XML) to generate the track from"
     )
@@ -38,15 +41,16 @@
         dest="output",
         default=Path.cwd() / "output",
         help='Output directory for generated tracks. Default="./"',
     )
     args = parser.parse_args(sys.argv[2:])
 
     track_filepath = Path(args.track_file)
-    generator.generate_track_live(track_filepath, args.output)
+    output_dirpath = Path(args.output)
+    generator.generate_track_live(track_filepath, output_dirpath)
 
 
 def subcommand_generate_trajectory():
     """TODO: Implement"""
     pass
```

### Comparing `track_generator-0.5.1/track_generator/track.py` & `track_generator-0.5.3/track_generator/track.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (C) 2022 twyleg
+from pathlib import Path
+
 import numpy
 from enum import Enum
 from math import tan, factorial, sqrt, sin, cos, radians, pi
-from typing import Any, List, Tuple, Optional
+from typing import Any, List, Tuple, Optional, Union
 from track_generator.coordinate_system import Polygon, Point2d, CartesianSystem2d
 
 LINE_WIDTH = 0.020
 TRACK_WIDTH = 0.800
 LINE_OFFSET = (TRACK_WIDTH / 2) - LINE_WIDTH
 
 CROSSWALK_LINE_WIDTH = 0.03
@@ -21,16 +23,19 @@
 class IntersectionDirection(Enum):
     RIGHT = "right"
     LEFT = "left"
     STRAIGHT = "straight"
 
 
 class ClothoidDirection(Enum):
-    LEFT = -1
-    RIGHT = 1
+    LEFT = "left"
+    RIGHT = "right"
+
+    def __int__(self) -> int:
+        return -1 if self == self.LEFT else 1
 
 
 class ClothoidType(Enum):
     OPEND = "opend"
     CLOSING = "closing"
 
 
@@ -46,41 +51,37 @@
         y = line_freq * i + pack_width
         polygons.append([Point2d(0, +y, coordinate_system), Point2d(length, +y, coordinate_system)])
         polygons.append([Point2d(0, -y, coordinate_system), Point2d(length, -y, coordinate_system)])
 
     return polygons
 
 
-class Background:
-    class Color:
-        def __init__(self, color: str, opacity: float):
-            self.color = color
-            self.opacity = opacity
-
-    class Image:
-        def __init__(self, file: str, x: float, y: float, width: float, height: float):
-            self.file = file
-            self.x = x
-            self.y = y
-            self.width = width
-            self.height = height
-
-    def __init__(self, color: Color = None, image: Image = None):
-        self.color: Optional[Background.Color] = color
-        self.image: Optional[Background.Image] = image
+class BackgroundColor:
+    def __init__(self, color: str, opacity: float):
+        self.color = color
+        self.opacity = opacity
+
+
+class BackgroundImage:
+    def __init__(self, filepath: Path, x: float, y: float, width: float, height: float):
+        self.filepath = filepath
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
 
 
 class Track:
     def __init__(
         self,
         version: str,
         width: float,
         height: float,
         origin: Tuple[float, float],
-        background: Background,
+        background: Union[BackgroundColor, BackgroundImage],
         segments: List[Any],
     ):
         self.version = version
         self.width = width
         self.height = height
         self.origin = origin
         self.background = background
@@ -92,15 +93,15 @@
                 self.segments[i].calc()
             else:
                 prev_segment = self.segments[i - 1]
                 self.segments[i].calc(prev_segment)
 
 
 class Segment:
-    def __init__(self):
+    def __init__(self) -> None:
         self.direction_angle: Optional[float] = None
         self.start_coordinate_system: Optional[CartesianSystem2d] = None
         self.end_coordinate_system: Optional[CartesianSystem2d] = None
 
     def calc(self, prev_segment):
         self.start_coordinate_system = prev_segment.end_coordinate_system
         self.direction_angle = prev_segment.direction_angle
@@ -110,15 +111,15 @@
     def __init__(self, x: float, y: float, direction_angle: float):
         self.start_coordinate_system = CartesianSystem2d(x, y, direction_angle)
         self.direction_angle = direction_angle
         self.start_point = Point2d(0, 0, self.start_coordinate_system)
         self.end_coordinate_system = self.start_coordinate_system
 
     def __str__(self) -> str:
-        return f"Start: end_point={self.end_point}, direction_angle={self.direction_angle}"
+        return f"Start: direction_angle={self.direction_angle}"
 
     def calc(self) -> None:
         pass
 
 
 class Straight(Segment):
     def __init__(self, length: float):
@@ -127,20 +128,21 @@
 
         self.center_line_polygon: Polygon = []
         self.left_line_polygon: Polygon = []
         self.right_line_polygon: Polygon = []
 
     def __str__(self) -> str:
         return (
-            f"Straight: sp={self.center_line_polygon[0][0]}, ep={self.center_line_polygon[0][1]},"
+            f"Straight: sp={self.center_line_polygon[0]}, ep={self.center_line_polygon[0]},"
             f" length={self.length}, direction_angle={self.direction_angle}"
         )
 
     def calc(self, prev_segment) -> None:
         super().calc(prev_segment)
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.end_coordinate_system = CartesianSystem2d(self.length, 0.0, 0.0, self.start_coordinate_system)
 
         self.center_line_polygon = [
             Point2d(0.0, 0.0, self.start_coordinate_system),
             Point2d(self.length, 0.0, self.start_coordinate_system),
         ]
 
@@ -151,46 +153,48 @@
 
         self.right_line_polygon = [
             Point2d(0.0, +LINE_OFFSET, self.start_coordinate_system),
             Point2d(self.length, +LINE_OFFSET, self.start_coordinate_system),
         ]
 
 
-class Arc(Segment):
+class Turn(Segment):
     def __init__(self, radius: float, radian_angle: float, direction_clockwise: bool):
         super().__init__()
         self.radius = radius
         self.radian_angle = radian_angle
         self.direction_clockwise = direction_clockwise
-        self.start_direction_angle: Optional[float] = None
 
+        self.start_direction_angle: Optional[float] = None
         self.start_point_center: Optional[Point2d] = None
         self.start_point_left: Optional[Point2d] = None
         self.start_point_right: Optional[Point2d] = None
         self.end_point_center: Optional[Point2d] = None
         self.center_point: Optional[Point2d] = None
 
     def __str__(self) -> str:
         return (
-            f"Arc: sp={self.start_point_center}, ep={self.end_point_center}, cp={self.center_point},"
+            f"Turn: sp={self.start_point_center}, ep={self.end_point_center}, cp={self.center_point},"
             f" start_direction_angle={self.start_direction_angle}, direction_angle={self.direction_angle},"
             f" cw={self.direction_clockwise}, angle={self.radian_angle}, radius={self.radius}"
         )
 
     def calc(self, prev_segment) -> None:
         super().calc(prev_segment)
 
         signed_radian_angle = -self.radian_angle if self.direction_clockwise else self.radian_angle
         center_offset = self.radius if self.direction_clockwise else -self.radius
 
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         center_coordinate_system = CartesianSystem2d(
             0.0, -center_offset, signed_radian_angle, self.start_coordinate_system
         )
         self.end_coordinate_system = CartesianSystem2d(0.0, center_offset, 0.0, center_coordinate_system)
 
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.start_point_center = Point2d(0.0, 0.0, self.start_coordinate_system)
         self.start_point_left = Point2d(0.0, -LINE_OFFSET, self.start_coordinate_system)
         self.start_point_right = Point2d(0.0, +LINE_OFFSET, self.start_coordinate_system)
 
         self.end_point_center = Point2d(0.0, 0.0, self.end_coordinate_system)
         self.center_point = Point2d(0.0, 0.0, center_coordinate_system)
 
@@ -201,28 +205,30 @@
 class Crosswalk(Straight):
     def __init__(self, length: float):
         super().__init__(length)
         self.line_polygons: List[Polygon] = []
 
     def calc(self, prev_segment) -> None:
         super().calc(prev_segment)
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.line_polygons = calc_crosswalk_lines(self.length, TRACK_WIDTH, self.start_coordinate_system)
 
 
 class Intersection(Segment):
     def __init__(self, length: float, direction: IntersectionDirection):
         super().__init__()
         self.length = length
         self.direction = direction
         self.base_line_polygons: List[Polygon] = []
         self.corner_line_polygons: List[Polygon] = []
         self.stop_line_polygons: List[Polygon] = []
         self.center_line_polygons: List[Polygon] = []
 
     def calc_base_lines(self) -> None:
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.base_line_polygons.append(
             [
                 Point2d(0.0, 0.0, self.start_coordinate_system),
                 Point2d(self.length, 0.0, self.start_coordinate_system),
             ]
         )
         self.base_line_polygons.append(
@@ -230,15 +236,15 @@
                 Point2d(self.length / 2, -self.length / 2, self.start_coordinate_system),
                 Point2d(self.length / 2, +self.length / 2, self.start_coordinate_system),
             ]
         )
 
     def calc_corner_lines(self) -> None:
         center_x = self.length / 2.0
-
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.corner_line_polygons.append(
             [
                 Point2d(0, -LINE_OFFSET, self.start_coordinate_system),
                 Point2d(center_x - LINE_OFFSET, -LINE_OFFSET, self.start_coordinate_system),
                 Point2d(center_x - LINE_OFFSET, -self.length / 2, self.start_coordinate_system),
             ]
         )
@@ -265,15 +271,15 @@
                 Point2d(center_x + LINE_OFFSET, +LINE_OFFSET, self.start_coordinate_system),
                 Point2d(center_x + LINE_OFFSET, +self.length / 2, self.start_coordinate_system),
             ]
         )
 
     def calc_stop_lines(self) -> None:
         center_x = self.length / 2.0
-
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.stop_line_polygons.append(
             [
                 Point2d(center_x - LINE_OFFSET, 0, self.start_coordinate_system),
                 Point2d(center_x - LINE_OFFSET, -LINE_OFFSET, self.start_coordinate_system),
             ]
         )
 
@@ -282,15 +288,15 @@
                 Point2d(center_x + LINE_OFFSET, 0, self.start_coordinate_system),
                 Point2d(center_x + LINE_OFFSET, +LINE_OFFSET, self.start_coordinate_system),
             ]
         )
 
     def calc_center_lines(self) -> None:
         center_x = self.length / 2.0
-
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.center_line_polygons.append(
             [
                 Point2d(0, 0, self.start_coordinate_system),
                 Point2d(center_x - LINE_OFFSET, 0, self.start_coordinate_system),
             ]
         )
 
@@ -319,14 +325,16 @@
         super().calc(prev_segment)
         if self.direction == IntersectionDirection.RIGHT:
             new_end = [self.length / 2, -self.length / 2, -90]
         elif self.direction == IntersectionDirection.STRAIGHT:
             new_end = [self.length, 0, 0]
         else:
             new_end = [self.length / 2, self.length / 2, 90]
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
+        assert isinstance(self.direction_angle, float)
         self.end_coordinate_system = CartesianSystem2d(new_end[0], new_end[1], new_end[2], self.start_coordinate_system)
         self.direction_angle += new_end[2]
 
         self.calc_base_lines()
         self.calc_corner_lines()
         self.calc_stop_lines()
         self.calc_center_lines()
@@ -341,14 +349,16 @@
         super().calc(prev_segment)
         if self.direction == IntersectionDirection.RIGHT:
             new_end = [self.length / 2, -self.length / 2, -90]
         elif self.direction == IntersectionDirection.STRAIGHT:
             new_end = [self.length, 0, 0]
         else:
             new_end = [self.length / 2, self.length / 2, 90]
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
+        assert isinstance(self.direction_angle, float)
         self.end_coordinate_system = CartesianSystem2d(new_end[0], new_end[1], new_end[2], self.start_coordinate_system)
         self.direction_angle += new_end[2]
 
 
 class ParkingArea(Straight):
     class ParkingLot:
         class Spot:
@@ -463,15 +473,15 @@
         self.curvature = curvature
         self.background_polygon: Polygon = []
         self.line_polygons: List[Polygon] = []
         self.crosswalk_lines_polygons: List[Polygon] = []
 
     def calc_lane(self, side: Side):
         side_factor = 1 if side == Side.LEFT else -1
-
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.line_polygons.append(
             [
                 Point2d(0.0, 0.0, self.start_coordinate_system),
                 Point2d(self.curve_segment_length, side_factor * self.island_width / 2, self.start_coordinate_system),
                 Point2d(
                     self.curve_segment_length + self.crosswalk_length,
                     side_factor * self.island_width / 2,
@@ -499,14 +509,15 @@
                     side_factor * LINE_OFFSET,
                     self.start_coordinate_system,
                 ),
             ]
         )
 
     def calc_background(self):
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         self.background_polygon = [
             Point2d(0.0, TRACK_WIDTH / 2, self.start_coordinate_system),
             Point2d(self.curve_segment_length, TRACK_WIDTH / 2 + self.island_width / 2, self.start_coordinate_system),
             Point2d(
                 self.curve_segment_length + self.crosswalk_length,
                 TRACK_WIDTH / 2 + self.island_width / 2,
                 self.start_coordinate_system,
@@ -525,14 +536,15 @@
             Point2d(
                 self.curve_segment_length, -(TRACK_WIDTH / 2 + self.island_width / 2), self.start_coordinate_system
             ),
             Point2d(0.0, -TRACK_WIDTH / 2, self.start_coordinate_system),
         ]
 
     def calc_crosswalk_lines(self):
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         width = TRACK_WIDTH / 2 - LINE_WIDTH
         self.crosswalk_lines_polygons = calc_crosswalk_lines(
             self.crosswalk_length,
             width,
             CartesianSystem2d(
                 self.curve_segment_length, +(self.island_width / 2 + LINE_OFFSET / 2), 0.0, self.start_coordinate_system
             ),
@@ -544,14 +556,15 @@
             CartesianSystem2d(
                 self.curve_segment_length, -(self.island_width / 2 + LINE_OFFSET / 2), 0.0, self.start_coordinate_system
             ),
         )
 
     def calc(self, prev_segment):
         super().calc(prev_segment)
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
         overall_length = 2 * self.curve_segment_length + self.crosswalk_length
         self.end_coordinate_system = CartesianSystem2d(overall_length, 0.0, 0.0, self.start_coordinate_system)
 
         self.calc_background()
         self.calc_lane(Side.LEFT)
         self.calc_lane(Side.RIGHT)
         self.calc_crosswalk_lines()
@@ -562,30 +575,30 @@
         super().__init__()
         self.a = a
         self.angle = angle
         self.angle_offset = angle_offset
         self.direction = direction
         self.type = type
         self.lines: List[Polygon] = []
-        self.background_polygon: List[Polygon] = []
+        self.background_polygon: Polygon = []
 
     def get_int(self, number: float) -> int:
         return int(number + 0.5 if number >= 0 else number - 0.5)
 
     def move_point(self, point: List[float], postponmet: List[float]) -> List[float]:
         return [point[0] + postponmet[0], point[1] + postponmet[1], point[2]]
 
     def rotate_point(self, point: List[float], radian: float) -> List[float]:
         return [
             point[0] * cos(radian) + point[1] * sin(radian),
             -point[0] * sin(radian) + point[1] * cos(radian),
             point[2],
         ]
 
-    def get_clothoid_point(self, length: float, direction: float) -> List[List[float]]:
+    def get_clothoid_point(self, length: float, direction: float) -> List[float]:
         toggle = 1
         x = 0
         y = 0
         for loops in range(20):
             x_ = (
                 toggle
                 * length ** (1 + 4 * loops)
@@ -598,27 +611,27 @@
             )
             x += x_
             y += y_
             toggle *= -1
         return [x, y * direction, length]
 
     def get_inverted_points(self, points: List[List[float]]) -> List[List[float]]:
-        angle = radians(self.angle) * self.direction.value
+        angle = radians(self.angle) * int(self.direction)
         new_points = []
         start = points[0]
         end = self.move_point(points[-1], [-start[0], -start[1]])
         for point in points:
             point = self.move_point(point, [-start[0], -start[1]])
             point = [(-point[0] + end[0]), (point[1] - end[1]), point[2]]
             point = self.rotate_point(point, angle)
             new_points.append(self.move_point(point, [start[0], start[1]]))
         return new_points[::-1]
 
     def get_clothoid(self) -> List[List[float]]:
-        direction = self.direction.value * -1
+        direction = int(self.direction) * -1
         arc_length_start = self.a * sqrt(2 * radians(self.angle_offset))
         arc_length_end = self.a * sqrt(2 * radians(self.angle_offset + self.angle))
         points = []
         distance = 0.04
         l = [
             i * distance
             for i in range(self.get_int(arc_length_start / distance), self.get_int(arc_length_end / distance) + 1)
@@ -630,21 +643,24 @@
         for i, point in enumerate(points):
             points[i] = self.rotate_point(self.move_point(point, first_point), radians(self.angle_offset) * direction)
         return points
 
     def get_moved_clothoid(self, points: List[List[float]], offset: float) -> List[List[float]]:
         new_points = []
         for point in points:
-            angle = (point[2] ** 2 / (2 * self.a**2) - radians(self.angle_offset)) * self.direction.value
+            angle = (point[2] ** 2 / (2 * self.a**2) - radians(self.angle_offset)) * int(self.direction)
             new_points.append([point[0] + offset * sin(angle), point[1] + offset * cos(angle), point[2]])
         return new_points
 
     def calc(self, prev_segment: Segment) -> None:
         super().calc(prev_segment)
-        direction = self.direction.value * -1
+        assert isinstance(self.start_coordinate_system, CartesianSystem2d)
+        assert isinstance(self.direction_angle, float)
+
+        direction = int(self.direction) * -1
         self.direction_angle += self.angle * direction
 
         middle_points = self.get_clothoid()
         left_lane_points = self.get_moved_clothoid(middle_points, +LINE_OFFSET)
         right_line_points = self.get_moved_clothoid(middle_points, -LINE_OFFSET)
 
         if self.type == ClothoidType.OPEND:
```

### Comparing `track_generator-0.5.1/track_generator/xml_reader.py` & `track_generator-0.5.3/track_generator/xml_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,84 @@
 # Copyright (C) 2022 twyleg
 import os
 import xml.etree.ElementTree as ET
 from pathlib import Path
+from typing import Union
 
+from xmlschema import XMLSchema
 from track_generator.track import *
 
+# mypy: disable-error-code="union-attr"
 
-class ElementMissingException(Exception):
-    def __init__(self, element_name: str, parent_element: ET.Element):
-        self.element_name = element_name
-        self.parent_element = parent_element
-
-    def __str__(self):
-        return f'ElementMissingException: missing element="{self.element_name}" in parent element "{self.parent_element.tag}"'
-
-
-class AttributeMissingException(Exception):
-    def __init__(self, attribute_name: str, element: ET.Element):
-        self.attribute_name = attribute_name
-        self.element = element
 
-    def __str__(self):
-        return f'AttributeMissingException: missing attribute="{self.attribute_name}" in element "{self.element.tag}""'
+FILE_DIR = Path(__file__).parent
 
 
 def read_track(xml_input_filepath: Path) -> Track:
+    print(f"Reading track: {xml_input_filepath}")
+    schema = XMLSchema(FILE_DIR / "xsd/track.xsd")
+    schema.validate(xml_input_filepath)
+
     tree = ET.parse(xml_input_filepath)
     root = tree.getroot()
 
     version = _read_root(root)
     width, height = _read_size(root)
     x, y = _read_origin(root)
     background = _read_background(root, xml_input_filepath)
     segments = _read_segments(root)
 
     return Track(version, width, height, (x, y), background, segments)
 
 
 def _read_root(root: ET.Element) -> str:
-    version = root.get("version")
-
-    if version is None:
-        raise AttributeMissingException("version", root)
-
+    version = root.attrib["version"]
     return version
 
 
 def _read_size(root: ET.Element) -> Tuple[float, float]:
     size_element = root.find("Size")
-
-    if size_element is None:
-        raise ElementMissingException("Size", root)
-
-    width = size_element.get("width")
-    height = size_element.get("height")
-
-    if width is None:
-        raise AttributeMissingException("width", size_element)
-
-    if height is None:
-        raise AttributeMissingException("height", size_element)
-
+    width = size_element.attrib["width"]
+    height = size_element.attrib["height"]
     return float(width), float(height)
 
 
 def _read_origin(root: ET.Element) -> Tuple[float, float]:
     origin_element = root.find("Origin")
-
-    if origin_element is None:
-        raise ElementMissingException("Origin", root)
-
-    x = origin_element.get("x")
-    y = origin_element.get("y")
-
-    if x is None:
-        raise AttributeMissingException("x", origin_element)
-
-    if y is None:
-        raise AttributeMissingException("y", origin_element)
-
+    x = origin_element.attrib["x"]
+    y = origin_element.attrib["y"]
     return float(x), float(y)
 
 
-def _read_background(root: ET.Element, xml_filepath: Path) -> Background:
+def _read_background(root: ET.Element, xml_filepath: Path) -> Union[BackgroundColor, BackgroundImage]:
     background_element = root.find("Background")
-
-    if background_element is None:
-        raise ElementMissingException("Background", root)
-
-    color = background_element.get("color")
-    opacity = background_element.get("opacity")
-
-    if color is None:
-        raise AttributeMissingException("color", background_element)
-
-    if opacity is None:
-        raise AttributeMissingException("opacity", background_element)
-
-    background_color = Background.Color(color, float(opacity))
-
     background_image_element = root.find("BackgroundImage")
-    background_image = None
+    if background_element is not None:
+        color = background_element.attrib["color"]
+        opacity = background_element.attrib["opacity"]
+        return BackgroundColor(color, float(opacity))
+    elif background_image_element is not None:
+        file = Path(background_image_element.attrib["file"])
+        x = float(background_image_element.attrib["x"])
+        y = float(background_image_element.attrib["y"])
+        width = float(background_image_element.attrib["width"])
+        height = float(background_image_element.attrib["height"])
+
+        if not file.is_absolute():
+            xml_file_basedir = Path(xml_filepath).parent
+            file = xml_file_basedir / file
 
-    if background_image_element is not None:
-        file = background_image_element.get("file")
-        x = float(background_image_element.get("x"))
-        y = float(background_image_element.get("y"))
-        width = float(background_image_element.get("width"))
-        height = float(background_image_element.get("height"))
-
-        if not os.path.isabs(file):
-            xml_file_basedir = os.path.dirname(xml_filepath)
-            file = os.path.join(xml_file_basedir, file)
+        return BackgroundImage(file, x, y, width, height)
 
-        background_image = Background.Image(file, x, y, width, height)
-
-    return Background(background_color, background_image)
+    raise RuntimeError("Here be dragons - XSD prevents us from getting here!")
 
 
 def _read_segments(root: ET.Element):
     segments_element = root.find("Segments")
 
-    if segments_element is None:
-        raise ElementMissingException("Segments", root)
-
     segments = []
 
     for segment_element in segments_element:
         if segment_element.tag == "Start":
             segments.append(_read_start_element(segment_element))
         elif segment_element.tag in ["Straight", "BlockedArea"]:
             segments.append(_read_straight_element(segment_element))
@@ -146,104 +97,71 @@
         elif segment_element.tag == "Clothoid":
             segments.append(_read_clothoid_element(segment_element))
 
     return segments
 
 
 def _read_start_element(start_element: ET.Element):
-    x = start_element.get("x")
-    y = start_element.get("y")
-    direction_angle = start_element.get("direction_angle")
-
-    if x is None:
-        raise AttributeMissingException("x", start_element)
-    elif y is None:
-        raise AttributeMissingException("y", start_element)
-    elif direction_angle is None:
-        raise AttributeMissingException("direction_angle", start_element)
-
+    x = start_element.attrib["x"]
+    y = start_element.attrib["y"]
+    direction_angle = start_element.attrib["direction_angle"]
     return Start(float(x), float(y), float(direction_angle))
 
 
 def _read_straight_element(straight_element: ET.Element):
-    length = straight_element.get("length")
-
-    if length is None:
-        raise AttributeMissingException("length", straight_element)
-
+    length = straight_element.attrib["length"]
     return Straight(float(length))
 
 
 def _read_turn_element(turn_element: ET.Element):
-    direction = turn_element.get("direction")
-    radius = turn_element.get("radius")
-    radian = turn_element.get("radian")
-
-    if direction is None:
-        raise AttributeMissingException("direction", turn_element)
-    elif radius is None:
-        raise AttributeMissingException("radius", turn_element)
-    elif radian is None:
-        raise AttributeMissingException("radian", turn_element)
-
+    direction = turn_element.attrib["direction"]
+    radius = turn_element.attrib["radius"]
+    radian = turn_element.attrib["radian"]
     cw = True if direction == "right" else False
-
-    return Arc(float(radius), float(radian), cw)
+    return Turn(float(radius), float(radian), cw)
 
 
 def _read_crosswalk_element(crosswalk_element: ET.Element):
-    length = crosswalk_element.get("length")
-
-    if length is None:
-        raise AttributeMissingException("length", crosswalk_element)
-
+    length = crosswalk_element.attrib["length"]
     return Crosswalk(float(length))
 
 
 def _read_intersection_element(intersection_element: ET.Element):
-    length = intersection_element.get("length")
-    direction = IntersectionDirection(str(intersection_element.get("direction")))
-    if length is None:
-        raise AttributeMissingException("length", intersection_element)
+    length = intersection_element.attrib["length"]
+    direction = IntersectionDirection(intersection_element.attrib["direction"])
     return Intersection(float(length), direction)
 
 
 def _read_gap_element(straight_element: ET.Element):
-    length = straight_element.get("length")
-    direction = IntersectionDirection(str(straight_element.get("direction")))
-    if length is None:
-        raise AttributeMissingException("length", straight_element)
-
+    length = straight_element.attrib["length"]
+    direction = IntersectionDirection(straight_element.attrib["direction"])
     return Gap(float(length), direction)
 
 
 def _read_spot_element(spot_element: ET.Element) -> ParkingArea.ParkingLot.Spot:
-    type = spot_element.get("type")
-    length = spot_element.get("length")
+    type = spot_element.attrib["type"]
+    length = spot_element.attrib["length"]
     return ParkingArea.ParkingLot.Spot(type, float(length))
 
 
 def _read_parking_lot_element(parking_lot_element: ET.Element) -> ParkingArea.ParkingLot:
-    start = parking_lot_element.get("start")
-    depth = parking_lot_element.get("depth")
-    opening_ending_angle = parking_lot_element.get("opening_ending_angle")
+    start = parking_lot_element.attrib["start"]
+    depth = parking_lot_element.attrib["depth"]
+    opening_ending_angle = parking_lot_element.attrib["opening_ending_angle"]
     spots: List[ParkingArea.ParkingLot.Spot] = []
 
     for spot_element in parking_lot_element:
         spot = _read_spot_element(spot_element)
         spots.append(spot)
 
     return ParkingArea.ParkingLot(float(start), float(depth), float(opening_ending_angle), spots)
 
 
 def _read_parking_area_element(parking_area_element: ET.Element):
-    length = parking_area_element.get("length")
-
-    if length is None:
-        raise AttributeMissingException("length", parking_area_element)
+    length = parking_area_element.attrib["length"]
 
     right_lots: List[ParkingArea.ParkingLot] = []
     left_lots: List[ParkingArea.ParkingLot] = []
 
     right_lots_element = parking_area_element.find("RightLots")
     for parking_lot_element in right_lots_element:
         parking_lot = _read_parking_lot_element(parking_lot_element)
@@ -254,23 +172,23 @@
         parking_lot = _read_parking_lot_element(parking_lot_element)
         left_lots.append(parking_lot)
 
     return ParkingArea(float(length), right_lots, left_lots)
 
 
 def _read_traffic_island_element(traffic_island_element: ET.Element):
-    island_width = traffic_island_element.get("island_width")
-    crosswalk_length = traffic_island_element.get("crosswalk_length")
-    curve_segment_length = traffic_island_element.get("curve_segment_length")
-    curvature = traffic_island_element.get("curvature")
+    island_width = traffic_island_element.attrib["island_width"]
+    crosswalk_length = traffic_island_element.attrib["crosswalk_length"]
+    curve_segment_length = traffic_island_element.attrib["curve_segment_length"]
+    curvature = traffic_island_element.attrib["curvature"]
 
     return TrafficIsland(float(island_width), float(crosswalk_length), float(curve_segment_length), float(curvature))
 
 
 def _read_clothoid_element(clothoid_element: ET.Element) -> Clothoid:
-    a = clothoid_element.get("a")
-    angle = clothoid_element.get("angle")
-    angle_offset = clothoid_element.get("angle_offset")
-    direction = ClothoidDirection.RIGHT if clothoid_element.get("direction") == "right" else ClothoidDirection.LEFT
-    type = ClothoidType(str(clothoid_element.get("type")))
+    a = clothoid_element.attrib["a"]
+    angle = clothoid_element.attrib["angle"]
+    angle_offset = clothoid_element.attrib["angle_offset"]
+    direction = ClothoidDirection(clothoid_element.attrib["direction"])
+    type = ClothoidType(str(clothoid_element.attrib["type"]))
 
     return Clothoid(float(a), float(angle), float(angle_offset), direction, ClothoidType(type))
```

### Comparing `track_generator-0.5.1/track_generator.egg-info/SOURCES.txt` & `track_generator-0.5.3/track_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 track_generator/gazebo_model_templates/model.sdf.template
 track_generator/gazebo_model_templates/setup.bash.template
 track_generator/gazebo_model_templates/track.material.template
 track_generator/gui/__init__.py
 track_generator/gui/track_live_view.py
 track_generator/gui/qml/track_live_view.qml
 track_generator/segment_templates/crosswalk.svg
-track_generator/segment_templates/intersection.svg
+track_generator/segment_templates/intersection.svg
+track_generator/xsd/track.xsd
```

### Comparing `track_generator-0.5.1/versioneer.py` & `track_generator-0.5.3/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,16 @@
 """
 # pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
+# mypy: ignore-errors
+
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
```

