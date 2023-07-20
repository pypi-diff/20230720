# Comparing `tmp/track_generator-0.5.3.tar.gz` & `tmp/track_generator-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track_generator-0.5.3.tar", last modified: Thu Jul 20 09:10:01 2023, max compression
+gzip compressed data, was "track_generator-0.5.4.tar", last modified: Thu Jul 20 09:18:03 2023, max compression
```

## Comparing `track_generator-0.5.3.tar` & `track_generator-0.5.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 09:09:49.000000 track_generator-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 09:10:01.178404 track_generator-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-20 09:09:49.000000 track_generator-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 09:10:01.178404 track_generator-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 09:09:49.000000 track_generator-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.174404 track_generator-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 09:09:49.000000 track_generator-0.5.3/tests/test_track_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/coordinate_system.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gazebo_model_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/model.config.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/model.sdf.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/setup.bash.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gazebo_model_templates/track.material.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3875 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/ground_truth_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gui/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/gui/qml/
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/qml/track_live_view.qml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/gui/track_live_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12318 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/painter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/segment_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/segment_templates/crosswalk.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/segment_templates/intersection.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2531 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/starter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27240 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7283 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-20 09:09:49.000000 track_generator-0.5.3/track_generator/xsd/track.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:10:01.178404 track_generator-0.5.3/track_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 09:10:01.000000 track_generator-0.5.3/track_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83595 2023-07-20 09:09:49.000000 track_generator-0.5.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 09:17:50.000000 track_generator-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-20 09:18:03.629572 track_generator-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-20 09:17:50.000000 track_generator-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 09:18:03.629572 track_generator-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 09:17:50.000000 track_generator-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.625573 track_generator-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 09:17:50.000000 track_generator-0.5.4/tests/test_track_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/coordinate_system.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gazebo_model_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/gazebo_model_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gazebo_model_templates/model.config.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gazebo_model_templates/model.sdf.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gazebo_model_templates/setup.bash.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gazebo_model_templates/track.material.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3875 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/ground_truth_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/gui/qml/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gui/qml/track_live_view.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/gui/track_live_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12318 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/painter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/segment_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/segment_templates/crosswalk.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/segment_templates/intersection.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2531 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/starter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27240 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7283 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-20 09:17:50.000000 track_generator-0.5.4/track_generator/xsd/track.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:18:03.629572 track_generator-0.5.4/track_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 09:18:03.000000 track_generator-0.5.4/track_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83595 2023-07-20 09:17:50.000000 track_generator-0.5.4/versioneer.py
```

### Comparing `track_generator-0.5.3/PKG-INFO` & `track_generator-0.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: track_generator
-Version: 0.5.3
-Summary: Track generator
-Home-page: https://github.com/twyleg/track_generator
-Author: Torsten Wylegala
-Author-email: mail@twyleg.de
-License: GPL 3.0
-Keywords: svg model vehicles track
-Description-Content-Type: text/markdown
-
 [![Build status](https://github.com/twyleg/track_generator/actions/workflows/checks.yml/badge.svg)]()
 [![GitHub latest commit](https://badgen.net/github/last-commit/twyleg/track_generator)](https://GitHub.com/twyleg/track_generator/commit/)
 [![PyPI download month](https://img.shields.io/pypi/dm/track-generator)](https://pypi.python.org/pypi/track-generator/)
 [![PyPi version](https://badgen.net/pypi/v/track-generator/)](https://pypi.org/project/track-generator)
 [![Documentation Status](https://readthedocs.org/projects/track-generator/badge/?version=latest)](http://track-generator.readthedocs.io/?badge=latest)
 
 Track Generator
@@ -22,15 +11,15 @@
 from a parametric description (XML).
 
 For example, the following track was generated based on the parametric description
 that follows:
 
 **Output (SVG, optional PNG):**
 
-![track definition example](docs/source/_static/img/svg/doc_track_example.svg)
+![track definition example](https://raw.githubusercontent.com/twyleg/track_generator/master/docs/source/_static/img/svg/doc_track_example.svg)
 
 **Track definition file (XML):**
 
 ```xml
     <TrackDefinition version="0.0.1">
         <Size width="5.0" height="6.0"/>
         <Origin x="0" y="0"/>
@@ -82,15 +71,15 @@
 
     track_generator generate_track_live <TRACK_DEFINITION_FILE>
 
 Examples
 ========
 
 Examples that demonstrate the usage of the tool can be found in the
-[examples/](examples/) directory.
+[examples/](https://github.com/twyleg/track_generator/tree/master/examples) directory.
 
 Documentation
 =============
 
 Check the readthedocs site for more details:
 
 https://track-generator.readthedocs.io/en/latest/
```

### Comparing `track_generator-0.5.3/README.md` & `track_generator-0.5.4/track_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: track-generator
+Version: 0.5.4
+Summary: Track generator
+Home-page: https://github.com/twyleg/track_generator
+Author: Torsten Wylegala
+Author-email: mail@twyleg.de
+License: GPL 3.0
+Keywords: svg model vehicles track
+Description-Content-Type: text/markdown
+
 [![Build status](https://github.com/twyleg/track_generator/actions/workflows/checks.yml/badge.svg)]()
 [![GitHub latest commit](https://badgen.net/github/last-commit/twyleg/track_generator)](https://GitHub.com/twyleg/track_generator/commit/)
 [![PyPI download month](https://img.shields.io/pypi/dm/track-generator)](https://pypi.python.org/pypi/track-generator/)
 [![PyPi version](https://badgen.net/pypi/v/track-generator/)](https://pypi.org/project/track-generator)
 [![Documentation Status](https://readthedocs.org/projects/track-generator/badge/?version=latest)](http://track-generator.readthedocs.io/?badge=latest)
 
 Track Generator
@@ -11,15 +22,15 @@
 from a parametric description (XML).
 
 For example, the following track was generated based on the parametric description
 that follows:
 
 **Output (SVG, optional PNG):**
 
-![track definition example](docs/source/_static/img/svg/doc_track_example.svg)
+![track definition example](https://raw.githubusercontent.com/twyleg/track_generator/master/docs/source/_static/img/svg/doc_track_example.svg)
 
 **Track definition file (XML):**
 
 ```xml
     <TrackDefinition version="0.0.1">
         <Size width="5.0" height="6.0"/>
         <Origin x="0" y="0"/>
@@ -71,15 +82,15 @@
 
     track_generator generate_track_live <TRACK_DEFINITION_FILE>
 
 Examples
 ========
 
 Examples that demonstrate the usage of the tool can be found in the
-[examples/](examples/) directory.
+[examples/](https://github.com/twyleg/track_generator/tree/master/examples) directory.
 
 Documentation
 =============
 
 Check the readthedocs site for more details:
 
 https://track-generator.readthedocs.io/en/latest/
```

### Comparing `track_generator-0.5.3/setup.py` & `track_generator-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/coordinate_system.py` & `track_generator-0.5.4/track_generator/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/gazebo_model_generator.py` & `track_generator-0.5.4/track_generator/gazebo_model_generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/gazebo_model_templates/model.sdf.template` & `track_generator-0.5.4/track_generator/gazebo_model_templates/model.sdf.template`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/generator.py` & `track_generator-0.5.4/track_generator/generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/ground_truth_generator.py` & `track_generator-0.5.4/track_generator/ground_truth_generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/gui/qml/track_live_view.qml` & `track_generator-0.5.4/track_generator/gui/qml/track_live_view.qml`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/gui/track_live_view.py` & `track_generator-0.5.4/track_generator/gui/track_live_view.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/painter.py` & `track_generator-0.5.4/track_generator/painter.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/segment_templates/crosswalk.svg` & `track_generator-0.5.4/track_generator/segment_templates/crosswalk.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/segment_templates/intersection.svg` & `track_generator-0.5.4/track_generator/segment_templates/intersection.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/starter.py` & `track_generator-0.5.4/track_generator/starter.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/track.py` & `track_generator-0.5.4/track_generator/track.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/xml_reader.py` & `track_generator-0.5.4/track_generator/xml_reader.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator/xsd/track.xsd` & `track_generator-0.5.4/track_generator/xsd/track.xsd`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/track_generator.egg-info/PKG-INFO` & `track_generator-0.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: track-generator
-Version: 0.5.3
+Name: track_generator
+Version: 0.5.4
 Summary: Track generator
 Home-page: https://github.com/twyleg/track_generator
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: svg model vehicles track
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 from a parametric description (XML).
 
 For example, the following track was generated based on the parametric description
 that follows:
 
 **Output (SVG, optional PNG):**
 
-![track definition example](docs/source/_static/img/svg/doc_track_example.svg)
+![track definition example](https://raw.githubusercontent.com/twyleg/track_generator/master/docs/source/_static/img/svg/doc_track_example.svg)
 
 **Track definition file (XML):**
 
 ```xml
     <TrackDefinition version="0.0.1">
         <Size width="5.0" height="6.0"/>
         <Origin x="0" y="0"/>
@@ -82,15 +82,15 @@
 
     track_generator generate_track_live <TRACK_DEFINITION_FILE>
 
 Examples
 ========
 
 Examples that demonstrate the usage of the tool can be found in the
-[examples/](examples/) directory.
+[examples/](https://github.com/twyleg/track_generator/tree/master/examples) directory.
 
 Documentation
 =============
 
 Check the readthedocs site for more details:
 
 https://track-generator.readthedocs.io/en/latest/
```

### Comparing `track_generator-0.5.3/track_generator.egg-info/SOURCES.txt` & `track_generator-0.5.4/track_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.3/versioneer.py` & `track_generator-0.5.4/versioneer.py`

 * *Files identical despite different names*

