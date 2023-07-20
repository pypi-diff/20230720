# Comparing `tmp/ephys_link-0.9.1.tar.gz` & `tmp/ephys_link-0.9.2.tar.gz`

## Comparing `ephys_link-0.9.1.tar` & `ephys_link-0.9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ephys_link-0.9.1/Dockerfile
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-0.9.1/MANIFEST.in
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ephys_link-0.9.1/docker-compose.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ephys_link-0.9.1/requirements.txt
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/auto-formatters.txt
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/dependabot.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/workflows/autoformat-and-lint.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/.gitignore
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/ephys-link.iml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/misc.xml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/modules.xml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/other.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/vcs.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/__main__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/common.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/gui.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platform_handler.py
--rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/server.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/__init__.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/new_scale_handler.py
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/new_scale_manipulator.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/new_scale_pathway_handler.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/sensapex_handler.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/platforms/sensapex_manipulator.py
--rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/resources/CP210xManufacturing.dll
--rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/resources/NstMotorCtrl.dll
--rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/resources/SiUSBXp.dll
--rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 ephys_link-0.9.1/ephys_link/resources/libum.dll
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ephys_link-0.9.1/scripts/draw_demo.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ephys_link-0.9.1/scripts/new_scale_move.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ephys_link-0.9.1/scripts/probe_crash_test.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ephys_link-0.9.1/scripts/read_to_file.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/calibration_test.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/can_write_test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/drive_to_depth_test.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/get_manipulators_test.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/get_pos_test.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/inside_brain_test.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/move_test.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/register_manipulator_test.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ephys_link-0.9.1/tests/stop_test.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 ephys_link-0.9.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-0.9.1/LICENSE
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 ephys_link-0.9.1/README.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 ephys_link-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 ephys_link-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ephys_link-0.9.2/Dockerfile
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-0.9.2/MANIFEST.in
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ephys_link-0.9.2/docker-compose.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ephys_link-0.9.2/requirements.txt
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/auto-formatters.txt
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/workflows/autoformat-and-lint.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/.gitignore
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/ephys-link.iml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/misc.xml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/modules.xml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/other.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/vcs.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/__main__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/common.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/gui.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platform_handler.py
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/server.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/__init__.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/new_scale_handler.py
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/new_scale_manipulator.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/new_scale_pathway_handler.py
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/sensapex_handler.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/platforms/sensapex_manipulator.py
+-rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/resources/CP210xManufacturing.dll
+-rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/resources/NstMotorCtrl.dll
+-rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/resources/SiUSBXp.dll
+-rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 ephys_link-0.9.2/ephys_link/resources/libum.dll
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ephys_link-0.9.2/scripts/draw_demo.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ephys_link-0.9.2/scripts/new_scale_move.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ephys_link-0.9.2/scripts/probe_crash_test.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ephys_link-0.9.2/scripts/read_to_file.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/calibration_test.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/can_write_test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/drive_to_depth_test.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/get_manipulators_test.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/get_pos_test.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/inside_brain_test.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/move_test.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/register_manipulator_test.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ephys_link-0.9.2/tests/stop_test.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 ephys_link-0.9.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 ephys_link-0.9.2/README.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 ephys_link-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 ephys_link-0.9.2/PKG-INFO
```

### Comparing `ephys_link-0.9.1/.github/CODE_OF_CONDUCT.md` & `ephys_link-0.9.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.github/CONTRIBUTING.md` & `ephys_link-0.9.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.github/dependabot.yml` & `ephys_link-0.9.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `ephys_link-0.9.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.github/workflows/autoformat-and-lint.yml` & `ephys_link-0.9.2/.github/workflows/autoformat-and-lint.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.github/workflows/codeql-analysis.yml` & `ephys_link-0.9.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/common.py` & `ephys_link-0.9.2/ephys_link/common.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/gui.py` & `ephys_link-0.9.2/ephys_link/gui.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/platform_handler.py` & `ephys_link-0.9.2/ephys_link/platform_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/server.py` & `ephys_link-0.9.2/ephys_link/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 """
 
 import argparse
 import importlib
 import signal
 import time
 from threading import Event, Thread
-from tkinter import Tk
 from typing import Any
 
 import common as com
 
 # noinspection PyPackageRequirements
 import socketio
 from aiohttp import web
 from aiohttp.web_runner import GracefulExit
-from gui import GUI
 from platform_handler import PlatformHandler
 from pythonnet import load
 from serial import Serial
 from serial.tools.list_ports import comports
 
 # Setup server
 load("netfx")
@@ -48,15 +46,16 @@
 # parser.add_argument("-g", "--gui", dest="gui", action="store_true", help="Launches GUI")
 parser.add_argument(
     "-t",
     "--type",
     type=str,
     dest="type",
     default="sensapex",
-    help='Manipulator type (i.e. "sensapex", "new_scale", or "new_scale_pathway"). Default: "sensapex"',
+    help='Manipulator type (i.e. "sensapex", "new_scale", or "new_scale_pathway").'
+    ' Default: "sensapex"',
 )
 parser.add_argument(
     "-d", "--debug", dest="debug", action="store_true", help="Enable debug mode"
 )
 parser.add_argument(
     "-p",
     "--port",
@@ -66,15 +65,15 @@
     help="Port to serve on. Default: 8081 (avoids conflict with other HTTP servers)",
 )
 parser.add_argument(
     "--pathway_port",
     type=int,
     default=8080,
     dest="pathway_port",
-    help="Port New Scale Pathway's server is on. Default: 8080"
+    help="Port New Scale Pathway's server is on. Default: 8080",
 )
 parser.add_argument(
     "-s",
     "--serial",
     type=str,
     default="no-e-stop",
     dest="serial",
@@ -493,42 +492,40 @@
 def start() -> None:
     """Starts everything"""
 
     # Parse arguments
     args = parser.parse_args()
     com.set_debug(args.debug)
 
-    if args.gui:
-        # Start GUI (doesn't launch server yet)
-        # Will not run, option is removed
-        root = Tk()
-        GUI(root, launch_server, stop, poll_serial, args)
-        root.mainloop()
+    # if args.gui:
+    #     # Start GUI (doesn't launch server yet)
+    #     root = Tk()
+    #     GUI(root, launch_server, stop, poll_serial, args)
+    #     root.mainloop()
+
+    if args.serial != "no-e-stop":
+        # Register serial exit
+        signal.signal(signal.SIGTERM, close_serial)
+        signal.signal(signal.SIGINT, close_serial)
+
+        # Start emergency stop system if serial is provided
+        global poll_serial_thread
+        poll_serial_thread = Thread(
+            target=poll_serial,
+            args=(
+                kill_serial_event,
+                args.serial,
+            ),
+            daemon=True,
+        )
+        poll_serial_thread.start()
 
-    else:
-        if args.serial != "no-e-stop":
-            # Register serial exit
-            signal.signal(signal.SIGTERM, close_serial)
-            signal.signal(signal.SIGINT, close_serial)
-
-            # Start emergency stop system if serial is provided
-            global poll_serial_thread
-            poll_serial_thread = Thread(
-                target=poll_serial,
-                args=(
-                    kill_serial_event,
-                    args.serial,
-                ),
-                daemon=True,
-            )
-            poll_serial_thread.start()
-
-        # Register server exit
-        signal.signal(signal.SIGTERM, close_server)
-        signal.signal(signal.SIGINT, close_server)
+    # Register server exit
+    signal.signal(signal.SIGTERM, close_server)
+    signal.signal(signal.SIGINT, close_server)
 
-        # Launch with parsed arguments on main thread
-        launch_server(args.type, args.port, args.pathway_port)
+    # Launch with parsed arguments on main thread
+    launch_server(args.type, args.port, args.pathway_port)
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `ephys_link-0.9.1/ephys_link/platforms/new_scale_handler.py` & `ephys_link-0.9.2/ephys_link/platforms/new_scale_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/platforms/new_scale_manipulator.py` & `ephys_link-0.9.2/ephys_link/platforms/new_scale_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/platforms/new_scale_pathway_handler.py` & `ephys_link-0.9.2/ephys_link/platforms/new_scale_pathway_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Handle communications with New Scale API
 
 Implements New Scale specific API calls.
 
 This is a subclass of :class:`ephys_link.platform_handler.PlatformHandler`.
 """
 
-import time
 from json import loads
 from urllib import request
 
 # noinspection PyPackageRequirements
 import socketio
 
 from ephys_link import common as com
@@ -164,35 +163,35 @@
                 manipulator_data["Stage_Z"],
                 manipulator_data["Stage_Z"],
             ],
             "",
         )
 
     async def _goto_pos(
-            self, manipulator_id: str, position: list[float], speed: int
+        self, manipulator_id: str, position: list[float], speed: int
     ) -> com.PositionalOutputData:
         pass
 
     async def _drive_to_depth(
-            self, manipulator_id: str, depth: float, speed: int
+        self, manipulator_id: str, depth: float, speed: int
     ) -> com.DriveToDepthOutputData:
         pass
 
     def _set_inside_brain(
-            self, manipulator_id: str, inside: bool
+        self, manipulator_id: str, inside: bool
     ) -> com.StateOutputData:
         pass
 
     async def _calibrate(self, manipulator_id: str, sio: socketio.AsyncServer) -> str:
         pass
 
     def _bypass_calibration(self, manipulator_id: str) -> str:
         return ""
 
     def _set_can_write(
-            self,
-            manipulator_id: str,
-            can_write: bool,
-            hours: float,
-            sio: socketio.AsyncServer,
+        self,
+        manipulator_id: str,
+        can_write: bool,
+        hours: float,
+        sio: socketio.AsyncServer,
     ) -> com.StateOutputData:
         pass
```

### Comparing `ephys_link-0.9.1/ephys_link/platforms/sensapex_handler.py` & `ephys_link-0.9.2/ephys_link/platforms/sensapex_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/platforms/sensapex_manipulator.py` & `ephys_link-0.9.2/ephys_link/platforms/sensapex_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/resources/CP210xManufacturing.dll` & `ephys_link-0.9.2/ephys_link/resources/CP210xManufacturing.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/resources/NstMotorCtrl.dll` & `ephys_link-0.9.2/ephys_link/resources/NstMotorCtrl.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/resources/SiUSBXp.dll` & `ephys_link-0.9.2/ephys_link/resources/SiUSBXp.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/ephys_link/resources/libum.dll` & `ephys_link-0.9.2/ephys_link/resources/libum.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/scripts/draw_demo.py` & `ephys_link-0.9.2/scripts/draw_demo.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/scripts/new_scale_move.py` & `ephys_link-0.9.2/scripts/new_scale_move.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/scripts/probe_crash_test.py` & `ephys_link-0.9.2/scripts/probe_crash_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/scripts/read_to_file.py` & `ephys_link-0.9.2/scripts/read_to_file.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/calibration_test.py` & `ephys_link-0.9.2/tests/calibration_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/can_write_test.py` & `ephys_link-0.9.2/tests/can_write_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/drive_to_depth_test.py` & `ephys_link-0.9.2/tests/drive_to_depth_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/get_manipulators_test.py` & `ephys_link-0.9.2/tests/get_manipulators_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/get_pos_test.py` & `ephys_link-0.9.2/tests/get_pos_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/inside_brain_test.py` & `ephys_link-0.9.2/tests/inside_brain_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/move_test.py` & `ephys_link-0.9.2/tests/move_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/register_manipulator_test.py` & `ephys_link-0.9.2/tests/register_manipulator_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/tests/stop_test.py` & `ephys_link-0.9.2/tests/stop_test.py`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/.gitignore` & `ephys_link-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/LICENSE` & `ephys_link-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/README.md` & `ephys_link-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ephys_link-0.9.1/pyproject.toml` & `ephys_link-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ephys-link"
-version = "0.9.1"
+version = "0.9.2"
 authors = [{ name = "Kenneth Yang", email = "kjy5@uw.edu" }]
 description = "A Python WebSocket server that allows any WebSocket compliant application to communicate with manipulators used in electrophysiology experiments."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["websocket", "manipulator", "electrophysiology", "ephys", "sensapex", "neuroscience", "vbl", "brain"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ephys_link-0.9.1/PKG-INFO` & `ephys_link-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephys-link
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python WebSocket server that allows any WebSocket compliant application to communicate with manipulators used in electrophysiology experiments.
 Project-URL: GitHub, https://github.com/VirtualBrainLab/ephys-link
 Project-URL: Documentation, https://virtualbrainlab.org/05_misc/03_ephys_link.html
 Project-URL: Issue Tracker, https://github.com/VirtualBrainLab/ephys-link/issues
 Author-email: Kenneth Yang <kjy5@uw.edu>
 License-File: LICENSE
 Keywords: brain,electrophysiology,ephys,manipulator,neuroscience,sensapex,vbl,websocket
```

