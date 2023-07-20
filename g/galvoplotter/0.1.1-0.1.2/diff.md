# Comparing `tmp/galvoplotter-0.1.1.tar.gz` & `tmp/galvoplotter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galvoplotter-0.1.1.tar", last modified: Thu Jul 13 08:05:56 2023, max compression
+gzip compressed data, was "galvoplotter-0.1.2.tar", last modified: Thu Jul 20 10:18:55 2023, max compression
```

## Comparing `galvoplotter-0.1.1.tar` & `galvoplotter-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.409263 galvoplotter-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-06-28 05:27:33.000000 galvoplotter-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    11320 2023-07-13 08:05:56.410263 galvoplotter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10492 2023-07-13 08:04:21.000000 galvoplotter-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.381261 galvoplotter-0.1.1/examples/
--rw-rw-rw-   0        0        0        0 2023-06-28 03:52:49.000000 galvoplotter-0.1.1/examples/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/examples/gpio_detect.py
--rw-rw-rw-   0        0        0     1655 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/joystick.py
--rw-rw-rw-   0        0        0     1764 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/examples/light_circle_abort.py
--rw-rw-rw-   0        0        0      368 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/light_simple_cross.py
--rw-rw-rw-   0        0        0      321 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/mark_square.py
--rw-rw-rw-   0        0        0      403 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/position_sync_grid.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.390262 galvoplotter-0.1.1/galvo/
--rw-rw-rw-   0        0        0      596 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/__init__.py
--rw-rw-rw-   0        0        0     5054 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/consts.py
--rw-rw-rw-   0        0        0    49487 2023-07-13 08:00:47.000000 galvoplotter-0.1.1/galvo/controller.py
--rw-rw-rw-   0        0        0     3633 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/mock_connection.py
--rw-rw-rw-   0        0        0    10924 2023-06-28 01:39:37.000000 galvoplotter-0.1.1/galvo/usb_connection.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.408263 galvoplotter-0.1.1/galvoplotter.egg-info/
--rw-rw-rw-   0        0        0    11320 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 09:13:27.000000 galvoplotter-0.1.1/galvoplotter.egg-info/zip-safe
--rw-rw-rw-   0        0        0      962 2023-07-13 08:05:56.411263 galvoplotter-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       91 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.394262 galvoplotter-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/test/__init__.py
--rw-rw-rw-   0        0        0     5523 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/test/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:18:55.147202 galvoplotter-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-28 05:27:33.000000 galvoplotter-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    11320 2023-07-20 10:18:55.148202 galvoplotter-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10492 2023-07-13 09:16:12.000000 galvoplotter-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 10:18:55.120200 galvoplotter-0.1.2/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-28 03:52:49.000000 galvoplotter-0.1.2/examples/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-07-20 10:02:22.000000 galvoplotter-0.1.2/examples/gpio_detect.py
+-rw-rw-rw-   0        0        0     1655 2023-07-06 08:28:29.000000 galvoplotter-0.1.2/examples/joystick.py
+-rw-rw-rw-   0        0        0     1764 2023-07-06 09:12:43.000000 galvoplotter-0.1.2/examples/light_circle_abort.py
+-rw-rw-rw-   0        0        0      368 2023-07-06 08:28:29.000000 galvoplotter-0.1.2/examples/light_simple_cross.py
+-rw-rw-rw-   0        0        0      321 2023-07-06 08:28:29.000000 galvoplotter-0.1.2/examples/mark_square.py
+-rw-rw-rw-   0        0        0      403 2023-07-06 08:28:29.000000 galvoplotter-0.1.2/examples/position_sync_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:18:55.129201 galvoplotter-0.1.2/galvo/
+-rw-rw-rw-   0        0        0      617 2023-07-20 10:18:33.000000 galvoplotter-0.1.2/galvo/__init__.py
+-rw-rw-rw-   0        0        0     5054 2023-07-06 09:12:43.000000 galvoplotter-0.1.2/galvo/consts.py
+-rw-rw-rw-   0        0        0    49832 2023-07-20 10:18:33.000000 galvoplotter-0.1.2/galvo/controller.py
+-rw-rw-rw-   0        0        0     3633 2023-07-06 09:12:43.000000 galvoplotter-0.1.2/galvo/mock_connection.py
+-rw-rw-rw-   0        0        0    10924 2023-06-28 01:39:37.000000 galvoplotter-0.1.2/galvo/usb_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:18:55.146202 galvoplotter-0.1.2/galvoplotter.egg-info/
+-rw-rw-rw-   0        0        0    11320 2023-07-20 10:18:54.000000 galvoplotter-0.1.2/galvoplotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-07-20 10:18:55.000000 galvoplotter-0.1.2/galvoplotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:18:54.000000 galvoplotter-0.1.2/galvoplotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 10:18:54.000000 galvoplotter-0.1.2/galvoplotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-20 10:18:54.000000 galvoplotter-0.1.2/galvoplotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 09:13:27.000000 galvoplotter-0.1.2/galvoplotter.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      962 2023-07-20 10:18:55.150202 galvoplotter-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       91 2023-07-06 09:12:43.000000 galvoplotter-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:18:55.132201 galvoplotter-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2023-07-06 08:28:29.000000 galvoplotter-0.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0     5523 2023-07-06 09:12:43.000000 galvoplotter-0.1.2/test/test_api.py
```

### Comparing `galvoplotter-0.1.1/LICENSE` & `galvoplotter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/PKG-INFO` & `galvoplotter-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galvoplotter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Galvo Plotter
 Home-page: https://github.com/meerk40t/galvoplotter
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Keywords: ezcad2,galvo,laser
 Classifier: Development Status :: 4 - Beta
```

### Comparing `galvoplotter-0.1.1/README.md` & `galvoplotter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/examples/gpio_detect.py` & `galvoplotter-0.1.2/examples/gpio_detect.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/examples/joystick.py` & `galvoplotter-0.1.2/examples/joystick.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/examples/light_circle_abort.py` & `galvoplotter-0.1.2/examples/light_circle_abort.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/galvo/__init__.py` & `galvoplotter-0.1.2/galvo/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .consts import *
 from .controller import GalvoController
 
+VERSION = "0.1.2"
+
 
 def generate_job(generator):
     v = generator()
 
     def job(c):
         try:
             g = next(v)
```

### Comparing `galvoplotter-0.1.1/galvo/consts.py` & `galvoplotter-0.1.2/galvo/consts.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/galvo/controller.py` & `galvoplotter-0.1.2/galvo/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,20 +637,30 @@
         if override_list is not None:
             use_list = override_list
         if use_list:
             self.list_write_port()
         else:
             self.write_port()
 
-    def rotary(self, position, min_speed=100, max_speed=5000, origin_param=100, **kwgs):
+    def rotary(self, position, min_speed=100, max_speed=5000, acc_time=100, **kwgs):
         self.set_axis_motion_param(min_speed & 0xFFFF, max_speed & 0xFFFF)
-        self.set_axis_origin_param(origin_param)
-        self.move_axis_to(position & 0xFFFF)
+        self.set_axis_origin_param(acc_time)
+        pos = position if position >= 0 else -position + 0x80000000
+        p1 = (pos >> 16) & 0xFFFF
+        p0 = (pos & 0xFFFF)
+        self.move_axis_to(p0, p1)
         self.wait_axis()
 
+    def rotary_position(self):
+        pos = self.get_axis_pos(0)
+        position = pos[1] << 16 & pos[2]
+        if position >= 0x80000000:
+            return position - 0x80000000
+        return position
+
     def get_last_xy(self):
         return self._last_x, self._last_y
 
     #######################
     # WAIT STATE COMMANDS
     #######################
 
@@ -1465,16 +1475,16 @@
 
     def axis_go_origin(self, p0=0, p1=0):
         return self._command(AxisGoOrigin, p0, p1)
 
     def move_axis_to(self, p0, p1=0, p2=0, p3=0):
         return self._command(MoveAxisTo, p0, p1, p2, p3)
 
-    def get_axis_pos(self):
-        return self._command(GetAxisPos)
+    def get_axis_pos(self, index=0):
+        return self._command(GetAxisPos, index)
 
     def get_fly_wait_count(self):
         return self._command(GetFlyWaitCount)
 
     def get_mark_count(self):
         return self._command(GetMarkCount)
```

### Comparing `galvoplotter-0.1.1/galvo/mock_connection.py` & `galvoplotter-0.1.2/galvo/mock_connection.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/galvo/usb_connection.py` & `galvoplotter-0.1.2/galvo/usb_connection.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/galvoplotter.egg-info/PKG-INFO` & `galvoplotter-0.1.2/galvoplotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galvoplotter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Galvo Plotter
 Home-page: https://github.com/meerk40t/galvoplotter
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Keywords: ezcad2,galvo,laser
 Classifier: Development Status :: 4 - Beta
```

### Comparing `galvoplotter-0.1.1/galvoplotter.egg-info/SOURCES.txt` & `galvoplotter-0.1.2/galvoplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.1/setup.cfg` & `galvoplotter-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 616c 766f 706c 6f74 7465 720d   = galvoplotter.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e31  .version = 0.1.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e32  .version = 0.1.2
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 4761 6c76 6f20 506c 6f74 7465 720d 0a6c  Galvo Plotter..l
 00000050: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 00000060: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000070: 6578 742f 6d61 726b 646f 776e 0d0a 6c6f  ext/markdown..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
 00000090: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
```

### Comparing `galvoplotter-0.1.1/test/test_api.py` & `galvoplotter-0.1.2/test/test_api.py`

 * *Files identical despite different names*

