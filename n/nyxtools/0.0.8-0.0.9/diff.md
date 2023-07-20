# Comparing `tmp/nyxtools-0.0.8.tar.gz` & `tmp/nyxtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyxtools-0.0.8.tar", last modified: Tue Apr  5 11:56:24 2022, max compression
+gzip compressed data, was "nyxtools-0.0.9.tar", last modified: Fri May 20 19:33:35 2022, max compression
```

## Comparing `nyxtools-0.0.8.tar` & `nyxtools-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:24.002489 nyxtools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-05 11:56:13.000000 nyxtools-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-04-05 11:56:13.000000 nyxtools-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-04-05 11:56:13.000000 nyxtools-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-04-05 11:56:13.000000 nyxtools-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-04-05 11:56:24.002489 nyxtools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-04-05 11:56:13.000000 nyxtools-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:23.994489 nyxtools-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:23.998489 nyxtools-0.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-04-05 11:56:13.000000 nyxtools-0.0.8/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:24.002489 nyxtools-0.0.8/nyxtools/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-05 11:56:24.002489 nyxtools-0.0.8/nyxtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11619 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/flyer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/flyer_eiger2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:24.002489 nyxtools-0.0.8/nyxtools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     9319 2022-04-05 11:56:13.000000 nyxtools-0.0.8/nyxtools/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 11:56:24.002489 nyxtools-0.0.8/nyxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-05 11:56:23.000000 nyxtools-0.0.8/nyxtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-05 11:56:13.000000 nyxtools-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-04-05 11:56:24.002489 nyxtools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-04-05 11:56:13.000000 nyxtools-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68542 2022-04-05 11:56:13.000000 nyxtools-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.467238 nyxtools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-20 19:33:27.000000 nyxtools-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-05-20 19:33:27.000000 nyxtools-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-05-20 19:33:27.000000 nyxtools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-20 19:33:27.000000 nyxtools-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-05-20 19:33:35.467238 nyxtools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-05-20 19:33:27.000000 nyxtools-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.467238 nyxtools-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.467238 nyxtools-0.0.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-20 19:33:27.000000 nyxtools-0.0.9/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.471238 nyxtools-0.0.9/nyxtools/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-20 19:33:35.471238 nyxtools-0.0.9/nyxtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11619 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/flyer_eiger2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.467238 nyxtools-0.0.9/nyxtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9319 2022-05-20 19:33:27.000000 nyxtools-0.0.9/nyxtools/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 19:33:35.467238 nyxtools-0.0.9/nyxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-20 19:33:35.000000 nyxtools-0.0.9/nyxtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-20 19:33:27.000000 nyxtools-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-20 19:33:35.471238 nyxtools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-05-20 19:33:27.000000 nyxtools-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68542 2022-05-20 19:33:27.000000 nyxtools-0.0.9/versioneer.py
```

### Comparing `nyxtools-0.0.8/CONTRIBUTING.rst` & `nyxtools-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/LICENSE` & `nyxtools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/PKG-INFO` & `nyxtools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyxtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common code for the NYX beamline at NSLS-II.
 Home-page: https://github.com/JunAishima/nyxtools
 Author: Brookhaven National Laboratory
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nyxtools-0.0.8/docs/Makefile` & `nyxtools-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/docs/make.bat` & `nyxtools-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/docs/source/conf.py` & `nyxtools-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/docs/source/min_versions.rst` & `nyxtools-0.0.9/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools/flyer.py` & `nyxtools-0.0.9/nyxtools/flyer.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools/flyer_eiger2.py` & `nyxtools-0.0.9/nyxtools/flyer_eiger2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import logging
 import time as ttime
 
 from mxtools.flyer import MXFlyer
-from ophyd.sim import NullStatus
 from ophyd.status import SubscriptionStatus
 
 logger = logging.getLogger(__name__)
 DEFAULT_DATUM_DICT = {"data": None, "omega": None}
 
 
 class NYXEiger2Flyer(MXFlyer):
     def __init__(self, vector, zebra, detector=None) -> None:
         super().__init__(vector, zebra, detector)
         self.name = "NYXEiger2Flyer"
 
     def kickoff(self):
         self.detector.stage()
-
-        def zebra_callback(*args, **kwargs):
-            logger.debug(f"args: {args},  kwargs: {kwargs}\n")
-            self.zebra.pc.arm_signal.put(1)
-            return NullStatus()
-
         st = self.vector.move()
-        st.add_callback(zebra_callback)
-
         return st
 
+    def update_parameters(self, **kwargs):
+        super().update_parameters(**kwargs)
+        self.zebra.pc.arm_signal.put(1)
+        ttime.sleep(1)
+
     def complete(self):
         st_vector = self.vector.track_move()
 
         def detector_callback(value, old_value, **kwargs):
             logger.debug(f"DETECTOR status {old_value} -> {value}")
             # if old_value == "Acquiring" and value == "Done":
             if old_value == 1 and value == 0:
@@ -41,40 +37,44 @@
                 return False
 
         st_detector = SubscriptionStatus(self.detector.cam.acquire, detector_callback, run=True)
 
         return st_vector & st_detector
 
     def detector_arm(self, **kwargs):
+        logger.debug("flyer detector arm")
         kwargs["det_distance_m"] /= 1000
         super().detector_arm(**kwargs)
+        logger.debug("flyer detector arm done")
 
     def configure_vector(self, **kwargs):
+        logger.debug("configuring vector")
         angle_start = kwargs["angle_start"]
         scan_width = kwargs["scan_width"]
         exposure_ms = kwargs["exposure_period_per_image"] * 1.0e3
         num_images = kwargs["num_images"]
-        x_mm = (kwargs["x_start_um"] / 1000, kwargs["x_start_um"] / 1000)
-        y_mm = (kwargs["y_start_um"] / 1000, kwargs["y_start_um"] / 1000)
-        z_mm = (kwargs["z_start_um"] / 1000, kwargs["z_start_um"] / 1000)
+        x_mm = (kwargs["x_start_um"] / 1000, kwargs["x_end_um"] / 1000)
+        y_mm = (kwargs["y_start_um"] / 1000, kwargs["y_end_um"] / 1000)
+        z_mm = (kwargs["z_start_um"] / 1000, kwargs["z_end_um"] / 1000)
         o = (angle_start, angle_start + scan_width)
-        buffer_time_ms = 50
+        buffer_time_ms = 0
         shutter_lag_time_ms = 2
         shutter_time_ms = 2
         self.vector.prepare_move(
             o,
             x_mm,
             y_mm,
             z_mm,
             exposure_ms,
             num_images,
             buffer_time_ms,
             shutter_lag_time_ms,
             shutter_time_ms,
         )
+        logger.debug("configure done")
 
     def zebra_daq_prep(self):
         self.zebra.reset.put(1)
         ttime.sleep(2.0)
         self.zebra.out1.put(31)
         self.zebra.m1_set_pos.put(1)
         self.zebra.m2_set_pos.put(1)
```

### Comparing `nyxtools-0.0.8/nyxtools/handlers.py` & `nyxtools-0.0.9/nyxtools/handlers.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools/pilatus.py` & `nyxtools-0.0.9/nyxtools/pilatus.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools/robot.py` & `nyxtools-0.0.9/nyxtools/robot.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools/vector.py` & `nyxtools-0.0.9/nyxtools/vector.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/nyxtools.egg-info/PKG-INFO` & `nyxtools-0.0.9/nyxtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyxtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common code for the NYX beamline at NSLS-II.
 Home-page: https://github.com/JunAishima/nyxtools
 Author: Brookhaven National Laboratory
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nyxtools-0.0.8/nyxtools.egg-info/SOURCES.txt` & `nyxtools-0.0.9/nyxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/setup.py` & `nyxtools-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `nyxtools-0.0.8/versioneer.py` & `nyxtools-0.0.9/versioneer.py`

 * *Files identical despite different names*

