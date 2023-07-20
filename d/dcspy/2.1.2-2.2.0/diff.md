# Comparing `tmp/dcspy-2.1.2.tar.gz` & `tmp/dcspy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcspy-2.1.2.tar", last modified: Tue Jun  6 10:58:30 2023, max compression
+gzip compressed data, was "dcspy-2.2.0.tar", last modified: Thu Jul 20 21:07:24 2023, max compression
```

## Comparing `dcspy-2.1.2.tar` & `dcspy-2.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:58:30.474811 dcspy-2.1.2/
--rw-rw-rw-   0        0        0     1092 2022-01-03 14:12:28.000000 dcspy-2.1.2/LICENSE.md
--rw-rw-rw-   0        0        0     6491 2023-06-06 10:58:30.474312 dcspy-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-06-06 10:40:46.000000 dcspy-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:58:30.445753 dcspy-2.1.2/dcspy/
--rw-rw-rw-   0        0        0     7792 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/G13.png
--rw-rw-rw-   0        0        0    11136 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/G15v1.png
--rw-rw-rw-   0        0        0    11673 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/G15v2.png
--rw-rw-rw-   0        0        0    13267 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/G19.png
--rw-rw-rw-   0        0        0    10850 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/G510.png
--rw-rw-rw-   0        0        0     4819 2023-05-24 10:21:45.000000 dcspy-2.1.2/dcspy/__init__.py
--rw-rw-rw-   0        0        0    54818 2023-05-30 20:43:20.000000 dcspy-2.1.2/dcspy/aircraft.py
--rw-rw-rw-   0        0        0      476 2023-05-06 10:14:09.000000 dcspy-2.1.2/dcspy/config.yaml
--rw-rw-rw-   0        0        0     6139 2023-05-24 10:21:45.000000 dcspy-2.1.2/dcspy/dcsbios.py
--rw-rw-rw-   0        0        0    21694 2023-05-25 17:59:50.000000 dcspy-2.1.2/dcspy/dcspy.ico
--rw-rw-rw-   0        0        0    35819 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/dcspy.png
--rw-rw-rw-   0        0        0    21614 2023-05-25 17:59:50.000000 dcspy-2.1.2/dcspy/dcspy_white.ico
--rw-rw-rw-   0        0        0    20420 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/falconded.ttf
--rw-rw-rw-   0        0        0      236 2023-04-25 15:37:52.000000 dcspy-2.1.2/dcspy/license.txt
--rw-rw-rw-   0        0        0     1235 2023-05-24 10:21:45.000000 dcspy-2.1.2/dcspy/log.py
--rw-rw-rw-   0        0        0     7447 2023-05-25 20:31:26.000000 dcspy-2.1.2/dcspy/logitech.py
--rw-rw-rw-   0        0        0        0 2022-08-25 13:36:54.000000 dcspy-2.1.2/dcspy/py.typed
--rw-rw-rw-   0        0        0     1107 2023-06-06 10:40:46.000000 dcspy-2.1.2/dcspy/run.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:58:30.460888 dcspy-2.1.2/dcspy/sdk/
--rw-rw-rw-   0        0        0     1464 2023-05-24 10:21:45.000000 dcspy-2.1.2/dcspy/sdk/__init__.py
--rw-rw-rw-   0        0        0     8507 2023-05-25 20:31:26.000000 dcspy-2.1.2/dcspy/sdk/lcd_sdk.py
--rw-rw-rw-   0        0        0     7924 2023-05-25 20:31:26.000000 dcspy-2.1.2/dcspy/sdk/led_sdk.py
--rw-rw-rw-   0        0        0    31528 2023-05-25 21:22:54.000000 dcspy-2.1.2/dcspy/splash.png
--rw-rw-rw-   0        0        0     4343 2023-06-06 10:40:46.000000 dcspy-2.1.2/dcspy/starter.py
--rw-rw-rw-   0        0        0    47677 2023-06-06 10:40:46.000000 dcspy-2.1.2/dcspy/tk_gui.py
--rw-rw-rw-   0        0        0    13282 2023-06-05 18:36:16.000000 dcspy-2.1.2/dcspy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:58:30.456918 dcspy-2.1.2/dcspy.egg-info/
--rw-rw-rw-   0        0        0     6491 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      354 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 10:58:30.000000 dcspy-2.1.2/dcspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3496 2023-06-06 10:40:17.000000 dcspy-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 10:58:30.475309 dcspy-2.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 10:58:30.472658 dcspy-2.1.2/tests/
--rw-rw-rw-   0        0        0    18375 2023-05-25 20:31:26.000000 dcspy-2.1.2/tests/test_aircraft.py
--rw-rw-rw-   0        0        0      971 2023-05-30 20:39:20.000000 dcspy-2.1.2/tests/test_bios.py
--rw-rw-rw-   0        0        0     5197 2023-05-22 00:14:36.000000 dcspy-2.1.2/tests/test_dcsbios.py
--rw-rw-rw-   0        0        0     5488 2023-06-06 10:40:17.000000 dcspy-2.1.2/tests/test_lcd_sdk.py
--rw-rw-rw-   0        0        0     3586 2023-05-22 00:14:36.000000 dcspy-2.1.2/tests/test_led_sdk.py
--rw-rw-rw-   0        0        0     7035 2023-05-22 00:14:36.000000 dcspy-2.1.2/tests/test_logitech.py
--rw-rw-rw-   0        0        0     1323 2023-05-22 00:14:36.000000 dcspy-2.1.2/tests/test_starter.py
--rw-rw-rw-   0        0        0     8585 2023-06-05 17:47:55.000000 dcspy-2.1.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:24.336664 dcspy-2.2.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-20 21:04:51.000000 dcspy-2.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     6533 2023-07-20 21:07:24.336664 dcspy-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5008 2023-07-20 21:04:51.000000 dcspy-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:24.321038 dcspy-2.2.0/dcspy/
+-rw-rw-rw-   0        0        0     7792 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/G13.png
+-rw-rw-rw-   0        0        0    11136 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/G15v1.png
+-rw-rw-rw-   0        0        0    11673 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/G15v2.png
+-rw-rw-rw-   0        0        0    13267 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/G19.png
+-rw-rw-rw-   0        0        0    10850 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/G510.png
+-rw-rw-rw-   0        0        0     4900 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/__init__.py
+-rw-rw-rw-   0        0        0    54666 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/aircraft.py
+-rw-rw-rw-   0        0        0      476 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/config.yaml
+-rw-rw-rw-   0        0        0     6139 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/dcsbios.py
+-rw-rw-rw-   0        0        0    21694 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/dcspy.ico
+-rw-rw-rw-   0        0        0    35819 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/dcspy.png
+-rw-rw-rw-   0        0        0    21614 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/dcspy_white.ico
+-rw-rw-rw-   0        0        0    20420 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/falconded.ttf
+-rw-rw-rw-   0        0        0      236 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/license.txt
+-rw-rw-rw-   0        0        0     1235 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/log.py
+-rw-rw-rw-   0        0        0     7547 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/logitech.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/py.typed
+-rw-rw-rw-   0        0        0     1107 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/run.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:24.336664 dcspy-2.2.0/dcspy/sdk/
+-rw-rw-rw-   0        0        0     1378 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/sdk/__init__.py
+-rw-rw-rw-   0        0        0     8507 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/sdk/lcd_sdk.py
+-rw-rw-rw-   0        0        0     7924 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/sdk/led_sdk.py
+-rw-rw-rw-   0        0        0    31528 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/splash.png
+-rw-rw-rw-   0        0        0     4549 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/starter.py
+-rw-rw-rw-   0        0        0    46961 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/tk_gui.py
+-rw-rw-rw-   0        0        0    14330 2023-07-20 21:04:51.000000 dcspy-2.2.0/dcspy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:24.321038 dcspy-2.2.0/dcspy.egg-info/
+-rw-rw-rw-   0        0        0     6533 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      358 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 21:07:24.000000 dcspy-2.2.0/dcspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3485 2023-07-20 21:04:51.000000 dcspy-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 21:07:24.336664 dcspy-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 21:07:24.336664 dcspy-2.2.0/tests/
+-rw-rw-rw-   0        0        0    19715 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_aircraft.py
+-rw-rw-rw-   0        0        0      979 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_bios.py
+-rw-rw-rw-   0        0        0     5169 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_dcsbios.py
+-rw-rw-rw-   0        0        0     5488 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_lcd_sdk.py
+-rw-rw-rw-   0        0        0     3586 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_led_sdk.py
+-rw-rw-rw-   0        0        0     7042 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_logitech.py
+-rw-rw-rw-   0        0        0     1323 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_starter.py
+-rw-rw-rw-   0        0        0    10135 2023-07-20 21:04:51.000000 dcspy-2.2.0/tests/test_utils.py
```

### Comparing `dcspy-2.1.2/LICENSE.md` & `dcspy-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/PKG-INFO` & `dcspy-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcspy
-Version: 2.1.2
+Version: 2.2.0
 Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
 Author: Michal Plichta
 Maintainer: Michal Plichta
 License: MIT License
 Project-URL: Homepage, https://github.com/emcek/dcspy
 Project-URL: Documentation, https://github.com/emcek/dcspy/wiki
 Project-URL: Repository, https://github.com/emcek/dcspy.git
@@ -23,19 +23,19 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
-[![image](https://img.shields.io/badge/pypi-v2.1.2-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
@@ -66,14 +66,15 @@
 * Ka-50 Black Shark II and III - PVI-800 and autopilot channels
 * Mi-8MTV2 Hip - autopilot channels and Radios information
 * Mi-24P Hind - Autopilot channels and modes and Radios information
 * A-10C Warthog and A-10C II Tank Killer - Radio frequency information
 * F-14A and F-14B Tomcat - basic support for RIO CAP
 * AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
 * AH-64D Apache - Enhanced Up Front Display
+* F-15E Eagle - Upfront Control Panel
 * more to come....
 
 ## Requirements
 * [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
 * [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
 * DCS World: [2.8.5.40170](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.5.40170/) Open Beta (any release 2.8.* should work)
 * (recommended) [Git](https://git-scm.com/download/win) it is necessary for using live version of DCS-BIOS, see [Live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios))
```

### Comparing `dcspy-2.1.2/README.md` & `dcspy-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![image](https://img.shields.io/badge/pypi-v2.1.2-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
@@ -33,14 +33,15 @@
 * Ka-50 Black Shark II and III - PVI-800 and autopilot channels
 * Mi-8MTV2 Hip - autopilot channels and Radios information
 * Mi-24P Hind - Autopilot channels and modes and Radios information
 * A-10C Warthog and A-10C II Tank Killer - Radio frequency information
 * F-14A and F-14B Tomcat - basic support for RIO CAP
 * AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
 * AH-64D Apache - Enhanced Up Front Display
+* F-15E Eagle - Upfront Control Panel
 * more to come....
 
 ## Requirements
 * [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
 * [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
 * DCS World: [2.8.5.40170](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.5.40170/) Open Beta (any release 2.8.* should work)
 * (recommended) [Git](https://git-scm.com/download/win) it is necessary for using live version of DCS-BIOS, see [Live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios))
```

### Comparing `dcspy-2.1.2/dcspy/G13.png` & `dcspy-2.2.0/dcspy/G13.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/G15v1.png` & `dcspy-2.2.0/dcspy/G15v1.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/G15v2.png` & `dcspy-2.2.0/dcspy/G15v2.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/G19.png` & `dcspy-2.2.0/dcspy/G19.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/G510.png` & `dcspy-2.2.0/dcspy/G510.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/__init__.py` & `dcspy-2.2.0/dcspy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 except ImportError:
     from typing_extensions import TypedDict
 
 
 SUPPORTED_CRAFTS = {
     'FA18Chornet': {'name': 'F/A-18C Hornet', 'bios': 'FA-18C_hornet'},
     'Ka50': {'name': 'Ka-50 Black Shark II', 'bios': 'Ka-50'},
-    'Ka503': {'name': 'Ka-50 Black Shark III', 'bios': 'Ka-50'},
+    'Ka503': {'name': 'Ka-50 Black Shark III', 'bios': 'Ka-50_3'},
     'Mi8MT': {'name': 'Mi-8MTV2 Magnificent Eight', 'bios': 'Mi-8MT'},
     'Mi24P': {'name': 'Mi-24P Hind', 'bios': 'Mi-24P'},
     'F16C50': {'name': 'F-16C Viper', 'bios': 'F-16C_50'},
-    'AH64DBLKII': {'name': 'AH-64D Apache', 'bios': 'AH-64D'},
+    'F15ESE': {'name': 'F-15ESE Eagle', 'bios': 'F-15ESE'},
+    'AH64DBLKII': {'name': 'AH-64D Apache', 'bios': 'AH-64D_BLK_II'},
     'A10C': {'name': 'A-10C Warthog', 'bios': 'A-10C'},
-    'A10C2': {'name': 'A-10C II Tank Killer', 'bios': 'A-10C2'},
-    'F14A135GR': {'name': 'F-14A Tomcat', 'bios': 'F14'},
-    'F14B': {'name': 'F-14B Tomcat', 'bios': 'F-14'},
+    'A10C2': {'name': 'A-10C II Tank Killer', 'bios': 'A-10C_2'},
+    'F14A135GR': {'name': 'F-14A Tomcat', 'bios': 'F-14A-135-GR'},
+    'F14B': {'name': 'F-14B Tomcat', 'bios': 'F-14B'},
     'AV8BNA': {'name': 'AV-8B N/A Harrier', 'bios': 'AV8BNA'},
 }
 SEND_ADDR = ('127.0.0.1', 7778)
 RECV_ADDR = ('', 5010)
 MULTICAST_IP = '239.255.50.10'
 LOCAL_APPDATA = True
```

### Comparing `dcspy-2.1.2/dcspy/aircraft.py` & `dcspy-2.2.0/dcspy/aircraft.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,66 +10,80 @@
 
 from PIL import Image, ImageDraw, ImageFont
 
 from dcspy import (DED_FONT, SUPPORTED_CRAFTS, BiosValue, LcdButton, LcdInfo,
                    LcdType, config)
 from dcspy.sdk import lcd_sdk
 
+try:
+    from typing import TypedDict
+except ImportError:
+    from typing_extensions import TypedDict
+
 LOG = getLogger(__name__)
 
 
+class CycleButton(TypedDict):
+    """Map BIOS key string with iterator to keep current value."""
+    bios: str
+    iter: Iterator[int]
+
+
 class Aircraft:
     """Common Aircraft."""
     def __init__(self, lcd_type: LcdInfo) -> None:
         """
         Create common aircraft.
 
         :param lcd_type: LCD type
         """
         self.lcd = lcd_type
         self.bios_data: Dict[str, BiosValue] = {}
-        self.cycle_buttons: Dict[str, Iterator[int]] = {}
+        self.cycle_buttons: Dict[LcdButton, CycleButton] = {}
         self._debug_img = cycle(chain([f'{x:02}' for x in range(10)], range(10, 99)))
+        self.button_actions: Dict[LcdButton, str] = {}
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+    def button_request(self, button: LcdButton) -> str:
         """
         Prepare aircraft specific DCS-BIOS request for button pressed.
 
         For G13/G15/G510: 1-4
         For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
 
         :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
         :return: ready to send DCS-BIOS request
         """
-        LOG.debug(f'{self.__class__.__name__} Button: {button}')
+        LOG.debug(f'{type(self).__name__} Button: {button}')
+        if button in self.cycle_buttons:
+            self.button_actions[button] = self._get_cycle_request(button)
+        request = self.button_actions.get(button, '\n')
         LOG.debug(f'Request: {request.replace(whitespace[2], " ")}')
         return request
 
     def prepare_image(self) -> Image.Image:
         """
         Prepare image to be sent to correct type of LCD.
 
         :return: image instance ready display on LCD
         """
         img = Image.new(mode=self.lcd.mode.value, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
         getattr(self, f'draw_for_lcd_{self.lcd.type.name.lower()}')(img)
         if config.get('save_lcd', False):
-            img.save(Path(gettempdir()) / f'{self.__class__.__name__}_{next(self._debug_img)}.png', 'PNG')
+            img.save(Path(gettempdir()) / f'{type(self).__name__}_{next(self._debug_img)}.png', 'PNG')
         return img
 
     def set_bios(self, selector: str, value: Union[str, int]) -> None:
         """
         Set value for DCS-BIOS selector.
 
         :param selector:
         :param value:
         """
         self.bios_data[selector]['value'] = value
-        LOG.debug(f'{self.__class__.__name__} {selector} value: "{value}"')
+        LOG.debug(f'{type(self).__name__} {selector} value: "{value}"')
         lcd_sdk.update_display(self.prepare_image())
 
     def get_bios(self, selector: str) -> Union[str, int]:
         """
         Get value for DCS-BIOS selector.
 
         :param selector:
@@ -83,28 +97,40 @@
         """Prepare image for Aircraft for Mono LCD."""
         raise NotImplementedError
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for Aircraft for Color LCD."""
         raise NotImplementedError
 
-    def get_next_value_for_button(self, btn_name: str) -> int:
+    def _get_next_value_for_button(self, button: LcdButton) -> int:
         """
         Get next int value (cycle fore and back) for button name.
 
-        :param btn_name: BIOS button name
+        :param button: LcdButton Enum
         """
-        if not isinstance(self.cycle_buttons[btn_name], cycle):
-            curr_val = int(self.get_bios(btn_name))
-            max_val = self.bios_data[btn_name]['max_value']
+        if not isinstance(self.cycle_buttons[button]['iter'], cycle):
+            bios = self.cycle_buttons[button]['bios']
+            curr_val = int(self.get_bios(bios))
+            max_val = self.bios_data[bios]['max_value']
             full_seed = list(range(max_val + 1)) + list(range(max_val - 1, 0, -1)) + list(range(max_val + 1))
             seed = full_seed[curr_val + 1:2 * max_val + curr_val + 1]
-            LOG.debug(f'{self.__class__.__name__} {btn_name} full_seed: {full_seed} seed: {seed} curr_val: {curr_val}')
-            self.cycle_buttons[btn_name] = cycle(chain(seed))
-        return next(self.cycle_buttons[btn_name])
+            LOG.debug(f'{type(self).__name__} {bios} full_seed: {full_seed} seed: {seed} curr_val: {curr_val}')
+            self.cycle_buttons[button]['iter'] = cycle(chain(seed))
+        return next(self.cycle_buttons[button]['iter'])
+
+    def _get_cycle_request(self, button: LcdButton) -> str:
+        """
+        Get request for cycle button.
+
+        :param button: LcdButton Enum
+        :return: ready to send DCS-BIOS request
+        """
+        button_bios_name = self.cycle_buttons[button]['bios']
+        settings = self._get_next_value_for_button(button)
+        return f'{button_bios_name} {settings}\n'
 
     def __repr__(self) -> str:
         """
         Show all details of Aircraft.
 
         :return: string
         """
@@ -136,16 +162,31 @@
             'UFC_OPTION_CUEING_3': {'klass': 'StringBuffer', 'args': {'address': 0x742c, 'max_length': 1}, 'value': ''},
             'UFC_OPTION_CUEING_4': {'klass': 'StringBuffer', 'args': {'address': 0x742e, 'max_length': 1}, 'value': ''},
             'UFC_OPTION_CUEING_5': {'klass': 'StringBuffer', 'args': {'address': 0x7430, 'max_length': 1}, 'value': ''},
             'IFEI_FUEL_DOWN': {'klass': 'StringBuffer', 'args': {'address': 0x748a, 'max_length': 6}, 'value': ''},
             'IFEI_FUEL_UP': {'klass': 'StringBuffer', 'args': {'address': 0x7490, 'max_length': 6}, 'value': ''},
             'HUD_ATT_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x742e, 'mask': 0x300, 'shift_by': 0x8}, 'value': int(), 'max_value': 2},
             'IFEI_DWN_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x10, 'shift_by': 0x4}, 'value': int(), 'max_value': 1},
-            'IFEI_UP_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x8, 'shift_by': 0x3}, 'value': int(), 'max_value': 1}}
-        self.cycle_buttons = {'HUD_ATT_SW': iter([0]), 'IFEI_DWN_BTN': iter([0]), 'IFEI_UP_BTN': iter([0])}
+            'IFEI_UP_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x8, 'shift_by': 0x3}, 'value': int(), 'max_value': 1},
+        }
+        self.cycle_buttons = {
+            LcdButton.OK: {'bios': 'HUD_ATT_SW', 'iter': iter([0])},
+            LcdButton.MENU: {'bios': 'IFEI_DWN_BTN', 'iter': iter([0])},
+            LcdButton.CANCEL: {'bios': 'IFEI_UP_BTN', 'iter': iter([0])},
+        }
+        self.button_actions = {
+            LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+            LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+            LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+            LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
+            LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+            LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+            LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+            LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n',
+        }
 
     def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> ImageDraw.ImageDraw:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
@@ -190,44 +231,14 @@
         :param value:
         """
         if selector in ('UFC_SCRATCHPAD_STRING_1_DISPLAY', 'UFC_SCRATCHPAD_STRING_2_DISPLAY',
                         'UFC_COMM1_DISPLAY', 'UFC_COMM2_DISPLAY'):
             value = str(value).replace('`', '1').replace('~', '2')
         super().set_bios(selector, value)
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F/A-18 Hornet specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        button_map = {LcdButton.OK: 'HUD_ATT_SW', LcdButton.CANCEL: 'IFEI_UP_BTN', LcdButton.MENU: 'IFEI_DWN_BTN'}
-        settings = 0
-        button_bios_name = ''
-        if button in button_map:
-            button_bios_name = button_map[button]
-            settings = self.get_next_value_for_button(button_bios_name)
-        action = {LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-                  LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-                  LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-                  LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
-                  LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-                  LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-                  LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-                  LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n',
-                  LcdButton.MENU: f'{button_bios_name} {settings}\n',
-                  LcdButton.CANCEL: f'{button_bios_name} {settings}\n',
-                  LcdButton.OK: f'{button_bios_name} {settings}\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
 
 class F16C50(Aircraft):
     """F-16C Viper."""
     def __init__(self, lcd_type: LcdInfo) -> None:
         """
         Create F-16C Viper.
 
@@ -243,16 +254,26 @@
             'DED_LINE_2': {'klass': 'StringBuffer', 'args': {'address': 0x4528, 'max_length': 29}, 'value': ''},
             'DED_LINE_3': {'klass': 'StringBuffer', 'args': {'address': 0x4546, 'max_length': 29}, 'value': ''},
             'DED_LINE_4': {'klass': 'StringBuffer', 'args': {'address': 0x4564, 'max_length': 29}, 'value': ''},
             'DED_LINE_5': {'klass': 'StringBuffer', 'args': {'address': 0x4582, 'max_length': 29}, 'value': ''},
             'IFF_MASTER_KNB': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1}, 'value': int(), 'max_value': 4},
             'IFF_ENABLE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x600, 'shift_by': 0x9}, 'value': int(), 'max_value': 2},
             'IFF_M4_CODE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x30, 'shift_by': 0x4}, 'value': int(), 'max_value': 2},
-            'IFF_M4_REPLY_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xc0, 'shift_by': 0x6}, 'value': int(), 'max_value': 2}}
-        self.cycle_buttons = {'IFF_MASTER_KNB': iter([0]), 'IFF_ENABLE_SW': iter([0]), 'IFF_M4_CODE_SW': iter([0]), 'IFF_M4_REPLY_SW': iter([0])}
+            'IFF_M4_REPLY_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xc0, 'shift_by': 0x6}, 'value': int(), 'max_value': 2},
+        }
+        self.cycle_buttons = {
+            LcdButton.ONE: {'bios': 'IFF_MASTER_KNB', 'iter': iter([0])},
+            LcdButton.TWO: {'bios': 'IFF_ENABLE_SW', 'iter': iter([0])},
+            LcdButton.THREE: {'bios': 'IFF_M4_CODE_SW', 'iter': iter([0])},
+            LcdButton.FOUR: {'bios': 'IFF_M4_REPLY_SW', 'iter': iter([0])},
+            LcdButton.LEFT: {'bios': 'IFF_MASTER_KNB', 'iter': iter([0])},
+            LcdButton.RIGHT: {'bios': 'IFF_ENABLE_SW', 'iter': iter([0])},
+            LcdButton.DOWN: {'bios': 'IFF_M4_CODE_SW', 'iter': iter([0])},
+            LcdButton.UP: {'bios': 'IFF_M4_REPLY_SW', 'iter': iter([0])},
+        }
 
     def _draw_common_data(self, draw: ImageDraw.ImageDraw, separation: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param separation: between lines in pixels
@@ -274,15 +295,15 @@
         Catch BIOS changes and remove garbage characters and replace with correct ones.
 
         :param selector: selector name
         :param value: value form DCS-BIOS
         """
         if 'DED_LINE_' in selector:
             value = str(value)
-            LOG.debug(f'{self.__class__.__name__} {selector} org  : "{value}"')
+            LOG.debug(f'{type(self).__name__} {selector} org  : "{value}"')
             for character in ['A\x10\x04', '\x82', '\x03', '\x02', '\x80', '\x08', '\x10', '\x07', '\x0f', '\xfe', '\xfc', '\x03', '\xff', '\xc0']:
                 value = value.replace(character, '')  # List page
             if value and value[-1] == '@':
                 value = value.replace('@', '')  # List - 6
             if self.lcd.type == LcdType.MONO:
                 value = value.replace('o', '\u00b0')  # 'o' to degree sign
                 value = value.replace('a', '\u2666')  # 'a' to up-down arrow 2195 or black diamond 2666
@@ -300,47 +321,64 @@
                 value = sub(r'(M1\s:\d+\s+)M4(\s+\(\d\).*)', r'\1mÄ\2', value)
                 value = sub(r'M1(\s:\d+\s+)M4(\s+:\s+\(\d\).*)', r'mÁ\1mÄ\2', value)
                 value = sub(r'M3(\s+:\d+\s+×\s+\d×[A-Z]+\(\d\).*)', r'mÃ\1', value)
                 value = sub(r'(\s[\s|×])HUD BLNK([×|\s]\s+)', r'\1hud blnk\2', value)
                 value = sub(r'(\s[\s|×])CKPT BLNK([×|\s]\s+)', r'\1ckpt blnk\2', value)
         super().set_bios(selector, value)
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F-16C Viper specific DCS-BIOS request for button pressed.
 
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+class F15ESE(Aircraft):
+    """F-15ESE Egle."""
 
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
+    def __init__(self, lcd_type: LcdInfo) -> None:
         """
-        button_map = {LcdButton.ONE: 'IFF_MASTER_KNB',
-                      LcdButton.TWO: 'IFF_ENABLE_SW',
-                      LcdButton.THREE: 'IFF_M4_CODE_SW',
-                      LcdButton.FOUR: 'IFF_M4_REPLY_SW',
-                      LcdButton.LEFT: 'IFF_MASTER_KNB',
-                      LcdButton.RIGHT: 'IFF_ENABLE_SW',
-                      LcdButton.DOWN: 'IFF_M4_CODE_SW',
-                      LcdButton.UP: 'IFF_M4_REPLY_SW'}
-        settings = 0
-        button_bios_name = ''
-        if button in button_map:
-            button_bios_name = button_map[button]
-            settings = self.get_next_value_for_button(button_bios_name)
-        action = {LcdButton.ONE: f'{button_bios_name} {settings}\n',
-                  LcdButton.TWO: f'{button_bios_name} {settings}\n',
-                  LcdButton.THREE: f'{button_bios_name} {settings}\n',
-                  LcdButton.FOUR: f'{button_bios_name} {settings}\n',
-                  LcdButton.LEFT: f'{button_bios_name} {settings}\n',
-                  LcdButton.RIGHT: f'{button_bios_name} {settings}\n',
-                  LcdButton.DOWN: f'{button_bios_name} {settings}\n',
-                  LcdButton.UP: f'{button_bios_name} {settings}\n'}
-        return super().button_request(button, action.get(button, '\n'))
+        Create F-15ESE Egle.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'F_UFC_Line1_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x9214, 'max_length': 0x14}, 'value': ''},
+            'F_UFC_Line2_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x9228, 'max_length': 0x14}, 'value': ''},
+            'F_UFC_Line3_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x923c, 'max_length': 0x14}, 'value': ''},
+            'F_UFC_Line4_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x9250, 'max_length': 0x14}, 'value': ''},
+            'F_UFC_Line5_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x9264, 'max_length': 0x14}, 'value': ''},
+            'F_UFC_Line6_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x9278, 'max_length': 0x14}, 'value': ''},
+        }
+        self.button_actions = {
+            LcdButton.ONE: 'F_UFC_PRE_CHAN_L_SEL -3200\n',
+            LcdButton.TWO: 'F_UFC_PRE_CHAN_L_SEL 3200\n',
+            LcdButton.THREE: 'F_UFC_PRE_CHAN_R_SEL -3200\n',
+            LcdButton.FOUR: 'F_UFC_PRE_CHAN_R_SEL 3200\n',
+            LcdButton.LEFT: 'F_UFC_PRE_CHAN_L_SEL -3200\n',
+            LcdButton.RIGHT: 'F_UFC_PRE_CHAN_L_SEL 3200\n',
+            LcdButton.DOWN: 'F_UFC_PRE_CHAN_R_SEL -3200\n',
+            LcdButton.UP: 'F_UFC_PRE_CHAN_R_SEL 3200\n',
+            LcdButton.MENU: 'F_UFC_KEY_L_GUARD 1\n|F_UFC_KEY_L_GUARD 0\n',
+            LcdButton.CANCEL: 'F_UFC_KEY_R_GUARD 1\n|F_UFC_KEY_R_GUARD 0\n',
+        }
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for F-15ESE Eagle for Mono LCD."""
+        draw = ImageDraw.Draw(img)
+        for i in range(1, 6):
+            offset = (i - 1) * 8
+            draw.text(xy=(0, offset), text=str(self.get_bios(f'F_UFC_Line{i}_DISPLAY')), fill=self.lcd.foreground, font=self.lcd.font_s)
+        mat = search(r'\s*([0-9G]{1,2})\s+([0-9GV]{1,2})\s+', str(self.get_bios('F_UFC_Line6_DISPLAY')))
+        if mat:
+            uhf, v_uhf = mat.groups()
+            draw.text(xy=(130, 30), text=f'{uhf:>2} {v_uhf:>2}', fill=self.lcd.foreground, font=self.lcd.font_s)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for F-15ESE Eagle for Color LCD."""
+        draw = ImageDraw.Draw(img)
+        for i in range(1, 7):
+            offset = (i - 1) * 24
+            # todo: fix custom font for Color LCD
+            draw.text(xy=(0, offset), text=str(self.get_bios(f'F_UFC_Line{i}_DISPLAY')), fill=self.lcd.foreground, font=ImageFont.truetype('consola.ttf', 29))
 
 
 class Ka50(Aircraft):
     """Ka-50 Black Shark."""
     def __init__(self, lcd_type: LcdInfo) -> None:
         """
         Create Ka-50 Black Shark.
@@ -359,15 +397,26 @@
             'PVI_LINE2_POINT': {'klass': 'StringBuffer', 'args': {'address': 0x1932, 'max_length': 1}, 'value': ''},
             'PVI_LINE2_SIGN': {'klass': 'StringBuffer', 'args': {'address': 0x1922, 'max_length': 1}, 'value': ''},
             'PVI_LINE2_TEXT': {'klass': 'StringBuffer', 'args': {'address': 0x192a, 'max_length': 6}, 'value': ''},
             'AP_ALT_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
             'AP_BANK_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
             'AP_FD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1938, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
             'AP_HDG_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
-            'AP_PITCH_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()}}
+            'AP_PITCH_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
+        }
+        self.button_actions = {
+            LcdButton.ONE: 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n',
+            LcdButton.TWO: 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n',
+            LcdButton.THREE: 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n',
+            LcdButton.FOUR: 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n',
+            LcdButton.LEFT: 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n',
+            LcdButton.RIGHT: 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n',
+            LcdButton.DOWN: 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n',
+            LcdButton.UP: 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n',
+        }
 
     def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
@@ -425,35 +474,14 @@
         """Prepare image for Ka-50 Black Shark for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for Ka-50 Black Shark for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare Ka-50 Black Shark specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
-                  LcdButton.TWO: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
-                  LcdButton.THREE: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
-                  LcdButton.FOUR: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n',
-                  LcdButton.LEFT: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
-                  LcdButton.RIGHT: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
-                  LcdButton.DOWN: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
-                  LcdButton.UP: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
 
 class Ka503(Ka50):
     """Ka-50 Black Shark III."""
     pass
 
 
 class Mi8MT(Aircraft):
@@ -623,14 +651,22 @@
             'PLT_EUFD_LINE7': {'klass': 'StringBuffer', 'args': {'address': 0x8212, 'max_length': 56}, 'value': ''},
             'PLT_EUFD_LINE8': {'klass': 'StringBuffer', 'args': {'address': 0x824a, 'max_length': 56}, 'value': ''},
             'PLT_EUFD_LINE9': {'klass': 'StringBuffer', 'args': {'address': 0x8282, 'max_length': 56}, 'value': ''},
             'PLT_EUFD_LINE10': {'klass': 'StringBuffer', 'args': {'address': 0x82ba, 'max_length': 56}, 'value': ''},
             'PLT_EUFD_LINE11': {'klass': 'StringBuffer', 'args': {'address': 0x82f2, 'max_length': 56}, 'value': ''},
             'PLT_EUFD_LINE12': {'klass': 'StringBuffer', 'args': {'address': 0x832a, 'max_length': 56}, 'value': ''},
         }
+        self.button_actions = {
+            LcdButton.TWO: 'PLT_EUFD_RTS 0\n|PLT_EUFD_RTS 1\n',
+            LcdButton.THREE: 'PLT_EUFD_PRESET 0\n|PLT_EUFD_PRESET 1\n',
+            LcdButton.FOUR: 'PLT_EUFD_ENT 0\n|PLT_EUFD_ENT 1\n',
+            LcdButton.RIGHT: 'PLT_EUFD_RTS 0\n|PLT_EUFD_RTS 1\n',
+            LcdButton.DOWN: 'PLT_EUFD_PRESET 0\n|PLT_EUFD_PRESET 1\n',
+            LcdButton.UP: 'PLT_EUFD_ENT 0\n|PLT_EUFD_ENT 1\n',
+        }
 
     def draw_for_lcd_mono(self, img: Image.Image) -> None:
         """Prepare image for AH-64D Apache for Mono LCD."""
         LOG.debug(f'Mode: {self.mode}')
         kwargs = {'draw': ImageDraw.Draw(img), 'scale': 1}
         mode = self.mode.name.lower()
         if mode == 'pre':
@@ -732,54 +768,47 @@
         """
         if selector == 'PLT_EUFD_LINE1':
             match = search(r'.*\|.*\|(PRESET TUNE)\s\w+', str(value))
             self.mode = ApacheEufdMode.IDM
             if match:
                 self.mode = ApacheEufdMode.PRE
         if selector in ('PLT_EUFD_LINE8', 'PLT_EUFD_LINE9', 'PLT_EUFD_LINE10', 'PLT_EUFD_LINE11', 'PLT_EUFD_LINE12'):
-            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
+            LOG.debug(f'{type(self).__name__} {selector} original: "{value}"')
             value = str(value).replace(']', '\u2666').replace('[', '\u25ca').replace('~', '\u25a0'). \
                 replace('>', '\u25b8').replace('<', '\u25c2').replace('=', '\u2219')
         if 'PLT_EUFD_LINE' in selector:
-            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
+            LOG.debug(f'{type(self).__name__} {selector} original: "{value}"')
             value = str(value).replace('!', '\u2192')  # replace ! with ->
         super().set_bios(selector, value)
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+    def button_request(self, button: LcdButton) -> str:
         """
         Prepare AH-64D Apache specific DCS-BIOS request for button pressed.
 
         For G13/G15/G510: 1-4
         For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
 
         :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
         :return: ready to send DCS-BIOS request
         """
-        wca_or_idm = 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'
+        wca_or_idm = 'PLT_EUFD_WCA 0\n|PLT_EUFD_WCA 1\n'
         if self.mode == ApacheEufdMode.IDM:
-            wca_or_idm = 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'
+            wca_or_idm = 'PLT_EUFD_IDM 0\n|PLT_EUFD_IDM 1\n'
 
         if button in (LcdButton.FOUR, LcdButton.UP) and self.mode == ApacheEufdMode.IDM:
             self.mode = ApacheEufdMode.WCA
         elif button in (LcdButton.FOUR, LcdButton.UP) and self.mode != ApacheEufdMode.IDM:
             self.mode = ApacheEufdMode.IDM
 
         if button in (LcdButton.ONE, LcdButton.LEFT) and self.mode == ApacheEufdMode.WCA:
             self.warning_line += 1
 
-        action = {LcdButton.ONE: wca_or_idm,
-                  LcdButton.TWO: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
-                  LcdButton.THREE: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
-                  LcdButton.FOUR: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n',
-                  LcdButton.LEFT: wca_or_idm,
-                  LcdButton.RIGHT: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
-                  LcdButton.DOWN: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
-                  LcdButton.UP: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'}
-        return super().button_request(button, action.get(button, '\n'))
+        self.button_actions[LcdButton.ONE] = wca_or_idm
+        self.button_actions[LcdButton.LEFT] = wca_or_idm
+        return super().button_request(button)
 
 
 class A10C(Aircraft):
     """A-10C Warthog."""
     def __init__(self, lcd_type: LcdInfo) -> None:
         """
         Create A-10C Warthog or A-10C II Tank Killer.
@@ -796,15 +825,16 @@
             'VHFFM_FREQ2': {'klass': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf, 'shift_by': 0x0}, 'value': int()},
             'VHFFM_FREQ3': {'klass': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf0, 'shift_by': 0x4}, 'value': int()},
             'VHFFM_FREQ4': {'klass': 'StringBuffer', 'args': {'address': 0x119e, 'max_length': 2}, 'value': ''},
             'UHF_100MHZ_SEL': {'klass': 'StringBuffer', 'args': {'address': 0x1178, 'max_length': 1}, 'value': ''},
             'UHF_10MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1170, 'mask': 0x3c00, 'shift_by': 0xa}, 'value': int()},
             'UHF_1MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
             'UHF_POINT1MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf000, 'shift_by': 0xc}, 'value': int()},
-            'UHF_POINT25_SEL': {'klass': 'StringBuffer', 'args': {'address': 0x117a, 'max_length': 2}, 'value': ''}}
+            'UHF_POINT25_SEL': {'klass': 'StringBuffer', 'args': {'address': 0x117a, 'max_length': 2}, 'value': ''},
+        }
 
     def _generate_freq_values(self) -> Sequence[str]:
         """
         Generate frequency for all 3 radios (VHF AM, VHF FM and UHF).
 
         :return: All 3 frequency settings as strings
         """
@@ -849,53 +879,43 @@
         :param lcd_type: LCD type
         """
         super().__init__(lcd_type)
         self.bios_data: Dict[str, BiosValue] = {
             'RIO_CAP_CLEAR': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x4000, 'shift_by': 0xe}, 'value': int()},
             'RIO_CAP_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
             'RIO_CAP_NE': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
-            'RIO_CAP_ENTER': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()}}
+            'RIO_CAP_ENTER': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
+        }
+        self.button_actions = {
+            LcdButton.ONE: 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n',
+            LcdButton.TWO: 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n',
+            LcdButton.THREE: 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n',
+            LcdButton.FOUR: 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n',
+            LcdButton.LEFT: 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n',
+            LcdButton.RIGHT: 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n',
+            LcdButton.DOWN: 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n',
+            LcdButton.UP: 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n',
+        }
 
     def _draw_common_data(self, draw: ImageDraw.ImageDraw) -> None:
         """
         Draw common part for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         """
-        draw.text(xy=(2, 3), text=f'{SUPPORTED_CRAFTS[self.__class__.__name__]["name"]}', fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(2, 3), text=f'{SUPPORTED_CRAFTS[type(self).__name__]["name"]}', fill=self.lcd.foreground, font=self.lcd.font_l)
 
     def draw_for_lcd_mono(self, img: Image.Image) -> None:
         """Prepare image for F-14B Tomcat for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img))
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for F-14B Tomcat for Color LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img))
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F-14B Tomcat specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
-                  LcdButton.TWO: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
-                  LcdButton.THREE: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
-                  LcdButton.FOUR: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n',
-                  LcdButton.LEFT: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
-                  LcdButton.RIGHT: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
-                  LcdButton.DOWN: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
-                  LcdButton.UP: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
 
 class F14A135GR(F14B):
     """F-14A-135-GR Tomcat."""
     pass
 
 
 class AV8BNA(Aircraft):
@@ -916,15 +936,26 @@
             'AV8BNA_ODU_2_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x796c, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_2_Text': {'klass': 'StringBuffer', 'args': {'address': 0x796e, 'max_length': 4}, 'value': ''},
             'AV8BNA_ODU_3_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7972, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_3_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7974, 'max_length': 4}, 'value': ''},
             'AV8BNA_ODU_4_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7978, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_4_Text': {'klass': 'StringBuffer', 'args': {'address': 0x797a, 'max_length': 4}, 'value': ''},
             'AV8BNA_ODU_5_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x797e, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_5_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7980, 'max_length': 4}, 'value': ''}}
+            'AV8BNA_ODU_5_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7980, 'max_length': 4}, 'value': ''},
+        }
+        self.button_actions = {
+            LcdButton.ONE: 'UFC_COM1_SEL -3200\n',
+            LcdButton.TWO: 'UFC_COM1_SEL 3200\n',
+            LcdButton.THREE: 'UFC_COM2_SEL -3200\n',
+            LcdButton.FOUR: 'UFC_COM2_SEL 3200\n',
+            LcdButton.LEFT: 'UFC_COM1_SEL -3200\n',
+            LcdButton.RIGHT: 'UFC_COM1_SEL 3200\n',
+            LcdButton.DOWN: 'UFC_COM2_SEL -3200\n',
+            LcdButton.UP: 'UFC_COM2_SEL 3200\n',
+        }
 
     def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> ImageDraw.ImageDraw:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
@@ -949,35 +980,14 @@
         """Prepare image for AV-8B N/A for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for AV-8B N/A for Color LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
 
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare AV-8B N/A specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'UFC_COM1_SEL -3200\n',
-                  LcdButton.TWO: 'UFC_COM1_SEL 3200\n',
-                  LcdButton.THREE: 'UFC_COM2_SEL -3200\n',
-                  LcdButton.FOUR: 'UFC_COM2_SEL 3200\n',
-                  LcdButton.LEFT: 'UFC_COM1_SEL -3200\n',
-                  LcdButton.RIGHT: 'UFC_COM1_SEL 3200\n',
-                  LcdButton.DOWN: 'UFC_COM2_SEL -3200\n',
-                  LcdButton.UP: 'UFC_COM2_SEL 3200\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
 
 def draw_autopilot_channels(lcd: LcdInfo,
                             ap_channel: str,
                             c_rect: Tuple[float, float, float, float],
                             c_text: Tuple[float, float],
                             draw_obj: ImageDraw.ImageDraw,
                             turn_on: Union[str, int]) -> None:
```

### Comparing `dcspy-2.1.2/dcspy/dcsbios.py` & `dcspy-2.2.0/dcspy/dcsbios.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/dcspy.ico` & `dcspy-2.2.0/dcspy/dcspy.ico`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/dcspy.png` & `dcspy-2.2.0/dcspy/dcspy.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/dcspy_white.ico` & `dcspy-2.2.0/dcspy/dcspy_white.ico`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/falconded.ttf` & `dcspy-2.2.0/dcspy/falconded.ttf`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/log.py` & `dcspy-2.2.0/dcspy/log.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/logitech.py` & `dcspy-2.2.0/dcspy/logitech.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import partial
 from importlib import import_module
 from logging import getLogger
 from pprint import pformat
 from socket import socket
+from time import sleep
 from typing import List
 
 from PIL import Image, ImageDraw
 
 from dcspy import SEND_ADDR, SUPPORTED_CRAFTS, LcdButton, LcdColor, LcdMono
 from dcspy.aircraft import Aircraft
 from dcspy.dcsbios import ProtocolParser
@@ -132,15 +133,17 @@
         * detect if button was pressed
         * fetch DCS-BIOS request from current plane
         * sent action to DCS-BIOS via. network socket
         :param sock: network socket
         """
         button = self.check_buttons()
         if button.value:
-            sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), SEND_ADDR)
+            for request in self.plane.button_request(button).split('|'):
+                sock.sendto(bytes(request, 'utf-8'), SEND_ADDR)
+                sleep(0.1)
 
     def clear(self, true_clear=False) -> None:
         """
         Clear LCD.
 
         :param true_clear:
         """
@@ -163,15 +166,15 @@
 
     def __str__(self) -> str:
         """
         Show basic info of LCD.
 
         :return: string
         """
-        return f'{self.__class__.__name__}: {self.lcd.width}x{self.lcd.height}'
+        return f'{type(self).__name__}: {self.lcd.width}x{self.lcd.height}'
 
     def __repr__(self) -> str:
         """
         Show all details of LCD.
 
         :return: string
         """
```

### Comparing `dcspy-2.1.2/dcspy/run.py` & `dcspy-2.2.0/dcspy/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import customtkinter
 
 from dcspy import config
 from dcspy.tk_gui import DcspyGui
 from dcspy.utils import check_dcs_ver
 
 LOG = getLogger(__name__)
-__version__ = '2.1.2'
+__version__ = '2.2.0'
 
 
 def run() -> None:
     """Start DCSpy GUI."""
     customtkinter.set_appearance_mode(config['theme_mode'])
     customtkinter.set_default_color_theme(config['theme_color'])
     LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
```

### Comparing `dcspy-2.1.2/dcspy/sdk/__init__.py` & `dcspy-2.2.0/dcspy/sdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,12 @@
     :param lib_type: library to load: LCD or LED
     :return: C DLL instance
     """
     try:
         dll = _init_dll(lib_type)
         LOG.info(f'Loading of {lib_type} SDK success')
         return dll
-    except (KeyError, FileNotFoundError) as err:
+    except (KeyError, OSError) as err:
         header = '*' * 44
-        error_string = 'ERROR!!!'
-        LOG.error(f'\n{header}\n*{error_string:^42}*\n{header}\n'
-                  f'Loading of {lib_type} SDK failed: {err.__class__.__name__}', exc_info=True)
+        LOG.error(f'\n{header}\n*{type(err).__name__:^42}*\n{header}\nLoading of {lib_type} SDK failed !', exc_info=True)
         LOG.error(f'{header}')
         return None
```

### Comparing `dcspy-2.1.2/dcspy/sdk/lcd_sdk.py` & `dcspy-2.2.0/dcspy/sdk/lcd_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/sdk/led_sdk.py` & `dcspy-2.2.0/dcspy/sdk/led_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/splash.png` & `dcspy-2.2.0/dcspy/splash.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/dcspy/starter.py` & `dcspy-2.2.0/dcspy/starter.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from threading import Event
 from time import gmtime, time
 from typing import Iterator
 
 from dcspy import MULTICAST_IP, RECV_ADDR, config
 from dcspy.dcsbios import ProtocolParser
 from dcspy.logitech import LogitechKeyboard
-from dcspy.utils import get_version_string
+from dcspy.utils import check_bios_ver, get_version_string
 
 LOG = getLogger(__name__)
 LOOP_FLAG = True
-__version__ = '2.1.2'
+__version__ = '2.2.0'
 
 
-def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, event: Event) -> None:
+def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, ver_string: str, event: Event) -> None:
     """
     Handle main loop where all the magic is happened.
 
     :param logi_keyboard: type of Logitech keyboard with LCD
     :param parser: DCS protocol parser
     :param sock: multi-cast UDP socket
+    :param ver_string: current version to show
     :param event: stop event for main loop
     """
     start_time = time()
-    ver_string = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=config['check_ver'])
     LOG.info('Waiting for DCS connection...')
     support_banner = _supporters(text='Huge thanks to: Alexander Leschanz, Sireyn, Nick Thain, BrotherBloat and others! For support and help! ', width=26)
     while not event.is_set():
         try:
             dcs_bios_resp = sock.recv(2048)
             for int_byte in dcs_bios_resp:
                 parser.process_byte(int_byte)
@@ -107,15 +107,16 @@
     """
     Real starting point of DCSpy.
 
     :param lcd_type: LCD handling class as string
     :param event: stop event for main loop
     """
     parser = ProtocolParser()
-    logi_keyboard = getattr(import_module('dcspy.logitech'), lcd_type)(parser)
+    logi_keyboard: LogitechKeyboard = getattr(import_module('dcspy.logitech'), lcd_type)(parser)
     LOG.info(f'Loading: {str(logi_keyboard)}')
     LOG.debug(f'Loading: {repr(logi_keyboard)}')
     dcs_sock = _prepare_socket()
-    _handle_connection(logi_keyboard, parser, dcs_sock, event)
+    dcspy_ver = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=config['check_ver'])
+    _handle_connection(logi_keyboard=logi_keyboard, parser=parser, sock=dcs_sock, ver_string=dcspy_ver, event=event)
     dcs_sock.close()
     LOG.info('DCSpy stopped.')
-    logi_keyboard.display = ['Logitech LCD OK', 'DCSpy stopped', '', f'v{__version__}']
+    logi_keyboard.display = ['DCSpy stopped', '', f'DCSpy: {dcspy_ver}', f'DCS-BIOS: {check_bios_ver(bios_path=str(config["dcsbios"])).ver}']
```

### Comparing `dcspy-2.1.2/dcspy/tk_gui.py` & `dcspy-2.2.0/dcspy/tk_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import tkinter as tk
 from functools import partial
 from logging import getLogger
 from pathlib import Path
 from platform import architecture, python_implementation, python_version, uname
-from re import search
 from shutil import copy, copytree, rmtree, unpack_archive
 from tempfile import gettempdir
 from threading import Event, Thread
-from typing import Optional, Union
+from typing import Optional
 from webbrowser import open_new
 
 import customtkinter
 from CTkMessagebox import CTkMessagebox
 from CTkToolTip import CTkToolTip
 from packaging import version
 from PIL import Image
 from pystray import Icon, MenuItem
 
 from dcspy import LCD_TYPES, LOCAL_APPDATA, config
 from dcspy.starter import dcspy_run
-from dcspy.utils import (ReleaseInfo, check_dcs_bios_entry, check_dcs_ver,
-                         check_github_repo, check_ver_at_github, defaults_cfg,
-                         download_file, get_default_yaml, get_version_string,
-                         is_git_exec_present, proc_is_running, save_cfg)
+from dcspy.utils import (ReleaseInfo, check_bios_ver, check_dcs_bios_entry,
+                         check_dcs_ver, check_github_repo, check_ver_at_github,
+                         defaults_cfg, download_file, get_default_yaml,
+                         get_version_string, is_git_exec_present,
+                         proc_is_running, save_cfg)
 
-__version__ = '2.1.2'
+__version__ = '2.2.0'
 LOG = getLogger(__name__)
 
 
 class DcspyGui(tk.Frame):
     """Tkinter GUI."""
     def __init__(self, master: tk.Tk) -> None:
         """
         Create basic GUI for dcspy application.
 
         :param master: Top level widget
         """
         super().__init__(master)
         self.master: tk.Tk = master
         self.cfg_file = get_default_yaml(local_appdata=LOCAL_APPDATA)
-        self.l_bios: Union[version.Version, version.LegacyVersion] = version.LegacyVersion('Not checked')
-        self.r_bios: Union[version.Version, version.LegacyVersion] = version.LegacyVersion('Not checked')
+        self.l_bios = version.Version('0.0.0')
+        self.r_bios = version.Version('0.0.0')
         self.event = Event()
 
         self.status_txt = tk.StringVar()
         self.lcd_type = tk.StringVar()
         self.bios_path = tk.StringVar()
         self.dcs_path = tk.StringVar()
         self.autostart_switch = customtkinter.BooleanVar()
@@ -705,26 +705,16 @@
 
     def _check_local_bios(self) -> ReleaseInfo:
         """
         Check version of local BIOS.
 
         :return: release description info
         """
-        self.l_bios = version.parse('not installed')
-        result = ReleaseInfo(False, self.l_bios, '', '', '', '')
-        try:
-            with open(file=Path(self.bios_path.get()) / 'lib' / 'CommonData.lua', encoding='utf-8') as cd_lua:
-                cd_lua_data = cd_lua.read()
-        except FileNotFoundError as err:
-            LOG.debug(f'While checking DCS-BIOS version {err.__class__.__name__}: {err.filename}')
-        else:
-            bios_re = search(r'function getVersion\(\)\s*return\s*\"([\d.]*)\"', cd_lua_data)
-            if bios_re:
-                self.l_bios = version.parse(bios_re.group(1))
-                result = ReleaseInfo(False, self.l_bios, '', '', '', '')
+        result = check_bios_ver(bios_path=self.bios_path.get())
+        self.l_bios = result.ver
         return result
 
     def _check_remote_bios(self) -> ReleaseInfo:
         """
         Check version of remote BIOS.
 
         :return: release description info
@@ -792,15 +782,15 @@
         result = 'Installation Success. Done.'
         lua_dst_path = Path(self.bios_path.get()).parent
         lua = 'Export.lua'
         try:
             with open(file=lua_dst_path / lua, encoding='utf-8') as lua_dst:
                 lua_dst_data = lua_dst.read()
         except FileNotFoundError as err:
-            LOG.debug(f'{err.__class__.__name__}: {err.filename}')
+            LOG.debug(f'{type(err).__name__}: {err.filename}')
             copy(src=temp_dir / lua, dst=lua_dst_path)
             LOG.debug(f'Copy Export.lua from: {temp_dir} to {lua_dst_path} ')
         else:
             result += check_dcs_bios_entry(lua_dst_data, lua_dst_path, temp_dir)
         return result
 
     def _show_gui(self) -> None:
```

### Comparing `dcspy-2.1.2/dcspy/utils.py` & `dcspy-2.2.0/dcspy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             save_cfg(cfg_dict=defaults_cfg, filename=cfg_ful_path)
     return cfg_ful_path
 
 
 class ReleaseInfo(NamedTuple):
     """Tuple to store release related information."""
     latest: bool
-    ver: Union[version.Version, version.LegacyVersion]
+    ver: version.Version
     dl_url: str
     published: str
     release_type: str
     archive_file: str
 
 
 def load_cfg(filename: Path) -> ConfigDict:
@@ -84,15 +84,15 @@
         with open(file=filename, encoding='utf-8') as yaml_file:
             cfg_dict = load(yaml_file, Loader=FullLoader)
             if not isinstance(cfg_dict, dict):
                 cfg_dict, old_dict = {}, cfg_dict
                 raise AttributeError(f'Config is not a dict {type(old_dict)} value: **{old_dict}**')
     except (FileNotFoundError, parser.ParserError, AttributeError) as err:
         makedirs(name=filename.parent, exist_ok=True)
-        LOG.warning(f'{err.__class__.__name__}: {filename}. Default configuration will be used.')
+        LOG.warning(f'{type(err).__name__}: {filename}. Default configuration will be used.')
         LOG.debug(f'{err}')
     return cfg_dict
 
 
 def save_cfg(cfg_dict: ConfigDict, filename: Path) -> None:
     """
     Update yaml file with dict.
@@ -125,25 +125,25 @@
 
 def check_ver_at_github(repo: str, current_ver: str) -> ReleaseInfo:
     """
     Check version of <organization>/<package> at GitHub.
 
     Return tuple with:
     - result (bool) - if local version is latest
-    - online version (version.Version, version.LegacyVersion) - the latest version
+    - online version (version.Version) - the latest version
     - download url (str) - ready to download
     - published date (str) - format DD MMMM YYYY
     - release type (str) - Regular or Pre-release
     - archive file (str) - file name of archive
 
     :param repo: format '<organization or user>/<package>'
     :param current_ver: current local version
     :return: ReleaseInfo NamedTuple with information
     """
-    latest, online_version, asset_url, published, pre_release = False, 'unknown', '', '', False
+    latest, online_version, asset_url, published, pre_release = False, '0.0.0', '', '', False
     package = repo.split('/')[1]
     try:
         response = get(url=f'https://api.github.com/repos/{repo}/releases/latest', timeout=5)
         if response.ok:
             dict_json = response.json()
             online_version = dict_json['tag_name']
             pre_release = dict_json['prerelease']
@@ -151,15 +151,20 @@
             asset_url = dict_json['assets'][0]['browser_download_url']
             LOG.debug(f'Latest GitHub version:{online_version} pre:{pre_release} date:{published} url:{asset_url}')
             latest = _compare_versions(package, current_ver, online_version)
         else:
             LOG.warning(f'Unable to check {package} version online. Try again later. Status={response.status_code}')
     except Exception as exc:
         LOG.warning(f'Unable to check {package} version online: {exc}')
-    return ReleaseInfo(latest, version.parse(online_version), asset_url, published, 'Pre-release' if pre_release else 'Regular', asset_url.split('/')[-1])
+    return ReleaseInfo(latest=latest,
+                       ver=version.parse(online_version),
+                       dl_url=asset_url,
+                       published=published,
+                       release_type='Pre-release' if pre_release else 'Regular',
+                       archive_file=asset_url.split('/')[-1])
 
 
 def _compare_versions(package: str, current_ver: str, remote_ver: str) -> bool:
     """
     Compare two version of package and return result.
 
     :param package: package name
@@ -187,17 +192,17 @@
     """
     ver_string = f'v{current_ver}'
     if check:
         result = check_ver_at_github(repo=repo, current_ver=current_ver)
         details = ''
         if result.latest:
             details = ' (latest)'
-        elif str(result.ver) != 'unknown':
-            details = ' (please update!)'
-        elif str(result.ver) == 'unknown':
+        elif str(result.ver) != '0.0.0':
+            details = ' (update!)'
+        elif str(result.ver) == '0.0.0':
             details = ' (failed)'
         ver_string = f'v{current_ver}{details}'
     return ver_string
 
 
 def download_file(url: str, save_path: Path) -> bool:
     """
@@ -241,26 +246,47 @@
     :return: dcs type and version as strings
     """
     result_type, result_ver = 'Unknown', 'Unknown'
     try:
         with open(file=dcs_path / 'autoupdate.cfg', encoding='utf-8') as autoupdate_cfg:
             autoupdate_data = autoupdate_cfg.read()
     except (FileNotFoundError, PermissionError) as err:
-        LOG.debug(f'{err.__class__.__name__}: {err.filename}')
+        LOG.debug(f'{type(err).__name__}: {err.filename}')
     else:
         result_type = 'stable'
         dcs_type = search(r'"branch":\s"([\w.]*)"', autoupdate_data)
         if dcs_type:
             result_type = str(dcs_type.group(1))
         dcs_ver = search(r'"version":\s"([\d.]*)"', autoupdate_data)
         if dcs_ver:
             result_ver = str(dcs_ver.group(1))
     return result_type, result_ver
 
 
+def check_bios_ver(bios_path: Union[Path, str]) -> ReleaseInfo:
+    """
+    Check DSC-BIOS release version.
+
+    :param bios_path: path to DCS-BIOS directory in Saved Games folder
+    :return: ReleaseInfo named tuple
+    """
+    result = ReleaseInfo(latest=False, ver=version.parse('0.0.0'), dl_url='', published='', release_type='', archive_file='')
+    try:
+        with open(file=Path(bios_path) / 'lib' / 'CommonData.lua', encoding='utf-8') as cd_lua:
+            cd_lua_data = cd_lua.read()
+    except FileNotFoundError as err:
+        LOG.debug(f'While checking DCS-BIOS version {type(err).__name__}: {err.filename}')
+    else:
+        bios_re = search(r'function getVersion\(\)\s*return\s*\"([\d.]*)\"', cd_lua_data)
+        if bios_re:
+            bios = version.parse(bios_re.group(1))
+            result = ReleaseInfo(latest=False, ver=bios, dl_url='', published='', release_type='', archive_file='')
+    return result
+
+
 def is_git_repo(dir_path: str) -> bool:
     """
     Check if dir_path ios Git repository.
 
     :param dir_path: path as string
     :return: true if dir is git repo
     """
@@ -358,9 +384,9 @@
 
     :return: True if git.exe is available
     """
     try:
         import git
         return bool(git.GIT_OK)
     except ImportError as err:
-        LOG.debug(err.__class__.__name__, exc_info=True)
+        LOG.debug(type(err).__name__, exc_info=True)
         return False
```

### Comparing `dcspy-2.1.2/dcspy.egg-info/PKG-INFO` & `dcspy-2.2.0/dcspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcspy
-Version: 2.1.2
+Version: 2.2.0
 Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
 Author: Michal Plichta
 Maintainer: Michal Plichta
 License: MIT License
 Project-URL: Homepage, https://github.com/emcek/dcspy
 Project-URL: Documentation, https://github.com/emcek/dcspy/wiki
 Project-URL: Repository, https://github.com/emcek/dcspy.git
@@ -23,19 +23,19 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
-[![image](https://img.shields.io/badge/pypi-v2.1.2-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
@@ -66,14 +66,15 @@
 * Ka-50 Black Shark II and III - PVI-800 and autopilot channels
 * Mi-8MTV2 Hip - autopilot channels and Radios information
 * Mi-24P Hind - Autopilot channels and modes and Radios information
 * A-10C Warthog and A-10C II Tank Killer - Radio frequency information
 * F-14A and F-14B Tomcat - basic support for RIO CAP
 * AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
 * AH-64D Apache - Enhanced Up Front Display
+* F-15E Eagle - Upfront Control Panel
 * more to come....
 
 ## Requirements
 * [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
 * [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
 * DCS World: [2.8.5.40170](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.5.40170/) Open Beta (any release 2.8.* should work)
 * (recommended) [Git](https://git-scm.com/download/win) it is necessary for using live version of DCS-BIOS, see [Live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios))
```

### Comparing `dcspy-2.1.2/dcspy.egg-info/SOURCES.txt` & `dcspy-2.2.0/dcspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/pyproject.toml` & `dcspy-2.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [project]
 name = 'dcspy'
 authors = [{name = 'Michal Plichta'}]
 maintainers = [{name = 'Michal Plichta'}]
 description = 'Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD'
 license = {text = 'MIT License'}
 requires-python = '>=3.7'
+readme = 'README.md'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Environment :: Win32 (MS Windows)',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
@@ -24,21 +25,21 @@
     'Topic :: Games/Entertainment',
     'Topic :: Games/Entertainment :: Simulation',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: System :: Hardware',
     'Topic :: Utilities',
 ]
 keywords = ['logitech', 'logitech sdk', 'logitech keyboards', 'logitech gaming', 'logitech gaming keyboard', 'dcsworld', 'dcs', 'g13', 'g15', 'g510', 'g19']
-dynamic = ['version', 'readme']
+dynamic = ['version']
 dependencies = [
     'CTkMessagebox',
     'CTkToolTip',
     'customtkinter >= 5.0.3',
     'GitPython',
-    'packaging <= 21.3',
+    'packaging',
     'Pillow >= 9.3.0',
     'psutil',
     'pystray',
     'PyYAML',
     'requests>=2.31.0',
     'typing-extensions; python_version < "3.11"',
 ]
@@ -59,29 +60,29 @@
 test = [
     'codacy-coverage',
     'coveralls',
     'flake8',
     'interrogate',
     'lxml',
     'mypy',
+    'pip-audit',
     'pycodestyle',
     'pydocstyle[toml]',
     'pytest',
     'pytest-cov',
     'pytest-random',
     'ruff',
     'types-Pillow',
     'types-psutil',
     'types-PyYAML',
     'types-requests',
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = 'dcspy.run.__version__'}
-readme = {file = ['README.md']}
 
 [tool.setuptools.packages.find]
 include = ['dcspy*']
 exclude = ['dcspy.tests*']
 
 [tool.setuptools.package-data]
 dcspy = [
```

### Comparing `dcspy-2.1.2/tests/test_aircraft.py` & `dcspy-2.2.0/tests/test_aircraft.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 resources = Path(__file__).resolve().with_name('resources')
 
 
 # <=><=><=><=><=> Base Class <=><=><=><=><=>
 @mark.parametrize('model', all_plane_list, ids=[
     'FA-18 Hornet',
     'F-16C Viper',
+    'F-15ESE Eagle',
     'Ka-50 Black Shark II',
     'Ka-50 Black Shark III',
     'Mi-8MT Hip',
     'Mi-24P Hind',
     'AH-64D Apache',
     'A-10C Warthog',
     'A-10C II Tank Killer',
@@ -88,63 +89,76 @@
     ('harrier_color', LcdButton.LEFT, 'UFC_COM1_SEL -3200\n'),
     ('harrier_color', LcdButton.RIGHT, 'UFC_COM1_SEL 3200\n'),
     ('harrier_color', LcdButton.DOWN, 'UFC_COM2_SEL -3200\n'),
     ('harrier_color', LcdButton.UP, 'UFC_COM2_SEL 3200\n'),
     ('harrier_color', LcdButton.MENU, '\n'),
     ('harrier_color', LcdButton.CANCEL, '\n'),
     ('harrier_color', LcdButton.OK, '\n'),
+    ('eagle_mono', LcdButton.NONE, '\n'),
+    ('eagle_mono', LcdButton.ONE, 'F_UFC_PRE_CHAN_L_SEL -3200\n'),
+    ('eagle_mono', LcdButton.TWO, 'F_UFC_PRE_CHAN_L_SEL 3200\n'),
+    ('eagle_mono', LcdButton.THREE, 'F_UFC_PRE_CHAN_R_SEL -3200\n'),
+    ('eagle_mono', LcdButton.FOUR, 'F_UFC_PRE_CHAN_R_SEL 3200\n'),
+    ('eagle_color', LcdButton.NONE, '\n'),
+    ('eagle_color', LcdButton.LEFT, 'F_UFC_PRE_CHAN_L_SEL -3200\n'),
+    ('eagle_color', LcdButton.RIGHT, 'F_UFC_PRE_CHAN_L_SEL 3200\n'),
+    ('eagle_color', LcdButton.DOWN, 'F_UFC_PRE_CHAN_R_SEL -3200\n'),
+    ('eagle_color', LcdButton.UP, 'F_UFC_PRE_CHAN_R_SEL 3200\n'),
+    ('eagle_color', LcdButton.MENU, 'F_UFC_KEY_L_GUARD 1\n|F_UFC_KEY_L_GUARD 0\n'),
+    ('eagle_color', LcdButton.CANCEL, 'F_UFC_KEY_R_GUARD 1\n|F_UFC_KEY_R_GUARD 0\n'),
+    ('eagle_color', LcdButton.OK, '\n'),
     ('shark_mono', LcdButton.NONE, '\n'),
-    ('shark_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n'),
+    ('shark_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n'),
+    ('shark_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n'),
+    ('shark_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n'),
     ('shark_color', LcdButton.NONE, '\n'),
-    ('shark_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n'),
+    ('shark_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n'),
+    ('shark_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n'),
+    ('shark_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n'),
     ('shark_color', LcdButton.MENU, '\n'),
     ('shark_color', LcdButton.CANCEL, '\n'),
     ('shark_color', LcdButton.OK, '\n'),
     ('shark3_mono', LcdButton.NONE, '\n'),
-    ('shark3_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark3_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark3_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark3_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark3_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n'),
+    ('shark3_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n'),
+    ('shark3_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n'),
+    ('shark3_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n'),
     ('shark3_color', LcdButton.NONE, '\n'),
-    ('shark3_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark3_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark3_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark3_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark3_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\n|PVI_WAYPOINTS_BTN 0\n'),
+    ('shark3_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\n|PVI_FIXPOINTS_BTN 0\n'),
+    ('shark3_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\n|PVI_AIRFIELDS_BTN 0\n'),
+    ('shark3_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\n|PVI_TARGETS_BTN 0\n'),
     ('shark3_color', LcdButton.MENU, '\n'),
     ('shark3_color', LcdButton.CANCEL, '\n'),
     ('shark3_color', LcdButton.OK, '\n'),
     ('tomcata_mono', LcdButton.NONE, '\n'),
-    ('tomcata_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcata_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcata_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcata_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcata_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n'),
+    ('tomcata_mono', LcdButton.TWO, 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n'),
+    ('tomcata_mono', LcdButton.THREE, 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n'),
+    ('tomcata_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n'),
     ('tomcata_color', LcdButton.NONE, '\n'),
-    ('tomcata_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcata_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcata_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcata_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcata_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n'),
+    ('tomcata_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n'),
+    ('tomcata_color', LcdButton.DOWN, 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n'),
+    ('tomcata_color', LcdButton.UP, 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n'),
     ('tomcata_color', LcdButton.MENU, '\n'),
     ('tomcata_color', LcdButton.CANCEL, '\n'),
     ('tomcata_color', LcdButton.OK, '\n'),
     ('tomcatb_mono', LcdButton.NONE, '\n'),
-    ('tomcatb_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcatb_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcatb_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcatb_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcatb_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n'),
+    ('tomcatb_mono', LcdButton.TWO, 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n'),
+    ('tomcatb_mono', LcdButton.THREE, 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n'),
+    ('tomcatb_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n'),
     ('tomcatb_color', LcdButton.NONE, '\n'),
-    ('tomcatb_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcatb_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcatb_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcatb_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcatb_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\n|RIO_CAP_CLEAR 0\n'),
+    ('tomcatb_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\n|RIO_CAP_SW 0\n'),
+    ('tomcatb_color', LcdButton.DOWN, 'RIO_CAP_NE 1\n|RIO_CAP_NE 0\n'),
+    ('tomcatb_color', LcdButton.UP, 'RIO_CAP_ENTER 1\n|RIO_CAP_ENTER 0\n'),
     ('tomcatb_color', LcdButton.MENU, '\n'),
     ('tomcatb_color', LcdButton.CANCEL, '\n'),
     ('tomcatb_color', LcdButton.OK, '\n'),
     ('viper_mono', LcdButton.NONE, '\n'),
     ('viper_mono', LcdButton.ONE, 'IFF_MASTER_KNB 1\n'),
     ('viper_mono', LcdButton.TWO, 'IFF_ENABLE_SW 1\n'),
     ('viper_mono', LcdButton.THREE, 'IFF_M4_CODE_SW 1\n'),
@@ -154,30 +168,30 @@
     ('viper_color', LcdButton.RIGHT, 'IFF_ENABLE_SW 1\n'),
     ('viper_color', LcdButton.DOWN, 'IFF_M4_CODE_SW 1\n'),
     ('viper_color', LcdButton.UP, 'IFF_M4_REPLY_SW 1\n'),
     ('viper_color', LcdButton.MENU, '\n'),
     ('viper_color', LcdButton.CANCEL, '\n'),
     ('viper_color', LcdButton.OK, '\n'),
     ('apache_mono', LcdButton.NONE, '\n'),
-    ('apache_mono', LcdButton.ONE, 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'),
-    ('apache_mono', LcdButton.TWO, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
-    ('apache_mono', LcdButton.THREE, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
-    ('apache_mono', LcdButton.FOUR, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
+    ('apache_mono', LcdButton.ONE, 'PLT_EUFD_IDM 0\n|PLT_EUFD_IDM 1\n'),
+    ('apache_mono', LcdButton.TWO, 'PLT_EUFD_RTS 0\n|PLT_EUFD_RTS 1\n'),
+    ('apache_mono', LcdButton.THREE, 'PLT_EUFD_PRESET 0\n|PLT_EUFD_PRESET 1\n'),
+    ('apache_mono', LcdButton.FOUR, 'PLT_EUFD_ENT 0\n|PLT_EUFD_ENT 1\n'),
 ])
 def test_button_pressed_for_planes(plane, button, result, request):
     plane = request.getfixturevalue(plane)
     assert plane.button_request(button) == result
 
 
 @mark.parametrize('button, result', [
     (LcdButton.NONE, '\n'),
-    (LcdButton.LEFT, 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'),
-    (LcdButton.RIGHT, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
-    (LcdButton.DOWN, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
-    (LcdButton.UP, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
+    (LcdButton.LEFT, 'PLT_EUFD_WCA 0\n|PLT_EUFD_WCA 1\n'),
+    (LcdButton.RIGHT, 'PLT_EUFD_RTS 0\n|PLT_EUFD_RTS 1\n'),
+    (LcdButton.DOWN, 'PLT_EUFD_PRESET 0\n|PLT_EUFD_PRESET 1\n'),
+    (LcdButton.UP, 'PLT_EUFD_ENT 0\n|PLT_EUFD_ENT 1\n'),
     (LcdButton.MENU, '\n'),
     (LcdButton.CANCEL, '\n'),
     (LcdButton.OK, '\n'),
 ], ids=['NONE', 'LEFT', 'RIGHT', 'DOWN', 'UP', 'MENU', 'CANCEL', 'OK'])
 def test_button_pressed_for_apache_color(button, result, apache_color):
     from dcspy.aircraft import ApacheEufdMode
     apache_color.mode = ApacheEufdMode.WCA
@@ -211,15 +225,15 @@
 ])
 def test_get_next_value_for_cycle_buttons(plane, btn_name, btn, values, request):
     from itertools import cycle
     plane = request.getfixturevalue(plane)
     assert not all([isinstance(cyc_btn, cycle) for cyc_btn in plane.cycle_buttons.values()])
     for val in values:
         assert plane.button_request(btn) == f'{btn_name} {val}\n'
-    assert isinstance(plane.cycle_buttons[btn_name], cycle)
+    assert isinstance(plane.cycle_buttons[btn]['iter'], cycle)
 
 
 # <=><=><=><=><=> Set BIOS <=><=><=><=><=>
 @mark.parametrize('plane, bios_pairs, result', [
     ('hornet_mono', [('UFC_SCRATCHPAD_STRING_2_DISPLAY', '~~')], '22'),
     ('hornet_mono', [('UFC_COMM1_DISPLAY', '``')], '11'),
     ('hornet_mono', [('IFEI_FUEL_UP', '104T')], '104T'),
@@ -270,37 +284,47 @@
     set_bios_during_test(plane, bios_pairs)
     assert plane.mode.name == mode
 
 
 # <=><=><=><=><=> Prepare Image <=><=><=><=><=>
 
 @mark.parametrize('lcd', ['mono', 'color'])
-@mark.parametrize('model', ['hornet', 'viper', 'shark', 'shark3', 'hip', 'hind', 'apache', 'warthog', 'warthog2', 'tomcata', 'tomcatb', 'harrier'])
+@mark.parametrize('model', ['hornet', 'viper', 'eagle', 'shark', 'shark3', 'hip', 'hind', 'apache', 'warthog', 'warthog2', 'tomcata', 'tomcatb', 'harrier'])
 def test_prepare_image_for_all_planes(model, lcd, img_precision, request):
     aircraft_model = request.getfixturevalue(f'{model}_{lcd}')
     bios_pairs = request.getfixturevalue(f'{model}_{lcd}_bios')
     set_bios_during_test(aircraft_model, bios_pairs)
     img = aircraft_model.prepare_image()
-    assert compare_images(img=img, file_path=resources / platform / f'{model}_{lcd}_{aircraft_model.__class__.__name__}.png', precision=img_precision)
+    # if 'eagle' in model:
+    #     img.save(resources / platform / f'{platform}_{model}_{lcd}_{type(aircraft_model).__name__}.png')
+    # else:
+    assert compare_images(img=img, file_path=resources / platform / f'{model}_{lcd}_{type(aircraft_model).__name__}.png', precision=img_precision)
 
 
 @mark.parametrize('model', ['apache_mono', 'apache_color'], ids=['Mono LCD', 'Color LCD'])
 def test_prepare_image_for_apache_wca_mode(model, img_precision, request):
+    from itertools import repeat
+    from tempfile import gettempdir
+
     from dcspy.aircraft import ApacheEufdMode
+
     apache = request.getfixturevalue(model)
+    apache._debug_img = repeat(999)
     bios_pairs = [
         ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
         ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
         ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  '),
         ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  |                  '),
         ('PLT_EUFD_LINE5', '                  |                  |                  ')
     ]
     set_bios_during_test(apache, bios_pairs)
     apache.mode = ApacheEufdMode.WCA
-    img = apache.prepare_image()
+    with patch('dcspy.aircraft.config', return_value={'save_lcd': True}):
+        img = apache.prepare_image()
+    assert (Path(gettempdir()) / f'{type(apache).__name__}_999.png').exists()
     assert compare_images(img=img, file_path=resources / platform / f'{model}_wca_mode.png', precision=img_precision)
 
 
 # <=><=><=><=><=> Apache special <=><=><=><=><=>
 @mark.parametrize('model', ['apache_mono', 'apache_color'], ids=['Mono LCD', 'Color LCD'])
 def test_apache_wca_more_then_one_screen_scrolled(model, img_precision, request):
     from dcspy.aircraft import ApacheEufdMode
```

### Comparing `dcspy-2.1.2/tests/test_bios.py` & `dcspy-2.2.0/tests/test_bios.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from pytest import mark
 
 from dcspy import SUPPORTED_CRAFTS
 from tests.helpers import check_dcsbios_data, generate_bios_data_for_plane
 
 
 @mark.dcsbios
-@mark.parametrize('plane', ['hornet_mono', 'viper_mono', 'shark_mono', 'hip_mono', 'hind_mono', 'warthog_mono', 'tomcatb_mono', 'harrier_mono', 'apache_mono'])
+@mark.parametrize('plane', [
+    'hornet_mono', 'viper_mono', 'eagle_mono', 'shark_mono', 'hip_mono', 'hind_mono', 'warthog_mono', 'tomcatb_mono', 'harrier_mono', 'apache_mono'
+])
 def test_bios_values_all_planes(plane, request):
     plane = request.getfixturevalue(plane)
-    name = SUPPORTED_CRAFTS[plane.__class__.__name__]['bios']
-    results, dcsbios_ver = check_dcsbios_data(plane_bios=plane.bios_data, plane_json=f'{name}.json', git_bios=True)
+    name = SUPPORTED_CRAFTS[type(plane).__name__]['bios']
+    results, dcsbios_ver = check_dcsbios_data(plane_bios=plane.bios_data, plane_name=f'{name}', git_bios=True)
     print(f'\n{name} BIOS {dcsbios_ver}\n{"-" * (len(name) + 13)}')
     pprint(results if results else 'No issues found', width=100)
     if results:
         print('----- Full BIOS entry -----')
-        pprint(generate_bios_data_for_plane(plane_bios=plane.bios_data, plane_json=f'{name}.json', git_bios=True), width=160)
+        pprint(generate_bios_data_for_plane(plane_bios=plane.bios_data, plane_name=f'{name}', git_bios=True), width=160)
     assert not results
```

### Comparing `dcspy-2.1.2/tests/test_dcsbios.py` & `dcspy-2.2.0/tests/test_dcsbios.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,16 +100,18 @@
         assert kwargs == dict()
 
     protocol_parser.frame_sync_callbacks.add(partial(_callback))
     protocol_parser.sync_byte_count = 3
     protocol_parser.process_byte(bytes([0x55]))
 
 
-@mark.parametrize('class_name, params', [('StringBuffer', {'address': 0x192a, 'max_length': 6}),
-                                         ('IntegerBuffer', {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf})])
+@mark.parametrize('class_name, params', [
+    ('StringBuffer', {'address': 0x192a, 'max_length': 6}),
+    ('IntegerBuffer', {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf}),
+])
 def test_simple_instance_of_buffers(class_name, params, protocol_parser):
     from dcspy import dcsbios
 
     buff = getattr(dcsbios, class_name)(parser=protocol_parser, callback=lambda x: x, **params)
     assert 'on_dcsbios_write' in dir(buff)
```

### Comparing `dcspy-2.1.2/tests/test_lcd_sdk.py` & `dcspy-2.2.0/tests/test_lcd_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/tests/test_led_sdk.py` & `dcspy-2.2.0/tests/test_led_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/tests/test_logitech.py` & `dcspy-2.2.0/tests/test_logitech.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     ('keyboard_mono', False, [False] * 3 + [True], LcdButton.FOUR, [call(1), call(2), call(4), call(8)], True),
     ('keyboard_color', False, [False] * 4 + [True] + [False] * 2, LcdButton.OK, [call(256), call(512), call(4096), call(8192), call(1024)], True),
     ('keyboard_mono', True, [True, False, False, False], LcdButton.NONE, [call(1)], True),
     ('keyboard_color', True, [True] + [False] * 6, LcdButton.NONE, [call(256)], True),
     ('keyboard_mono', False, [False] * 4, LcdButton.NONE, [call(1), call(2), call(4), call(8)], False),
     ('keyboard_color', False, [False] * 8, LcdButton.NONE, [call(256), call(512), call(4096), call(8192), call(1024), call(2048), call(16384)], False),
 ], ids=['Mono 4 Button', 'Color Ok Button', 'Mono None already_pressed', 'Color None already_pressed', 'Mono None Button', 'Color None Button'])
-def test_keyboard_mono_check_buttons(keyboard, pressed1, effect, chk_btn, calls, pressed2, request):
+def test_keyboard_check_buttons(keyboard, pressed1, effect, chk_btn, calls, pressed2, request):
     from dcspy.sdk import lcd_sdk
     keyboard = request.getfixturevalue(keyboard)
     keyboard.already_pressed = pressed1
     with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=effect) as lcd_btn_pressed:
         assert keyboard.check_buttons() == chk_btn
     lcd_btn_pressed.assert_has_calls(calls)
     assert keyboard.already_pressed is pressed2
 
 
 @mark.parametrize('keyboard', ['keyboard_mono', 'keyboard_color'], ids=['Mono Keyboard', 'Color Keyboard'])
-def test_keyboard_color_button_handle(keyboard, sock, request):
+def test_keyboard_button_handle(keyboard, sock, request):
     from dcspy.sdk import lcd_sdk
     keyboard = request.getfixturevalue(keyboard)
     with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=[True]):
         keyboard.button_handle(sock)
     sock.sendto.assert_called_once_with(b'\n', ('127.0.0.1', 7778))
 
 
@@ -123,14 +123,15 @@
         keyboard.text(['1', '2'])
         upd_txt.assert_called()
 
 
 @mark.parametrize('model', all_plane_list, ids=[
     'FA-18 Hornet',
     'F-16C Viper',
+    'F-15ESE Eagle',
     'Ka-50 Black Shark II',
     'Ka-50 Black Shark III',
     'Mi-8MT Hip',
     'Mi-24P Hind',
     'AH-64D Apache',
     'A-10C Warthog',
     'A-10C II Tank Killer',
@@ -142,8 +143,8 @@
     from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         keyboard_mono.plane_name = model
         keyboard_mono.load_new_plane()
     assert isinstance(keyboard_mono.plane, Aircraft)
-    assert model in keyboard_mono.plane.__class__.__name__
+    assert model in type(keyboard_mono.plane).__name__
```

### Comparing `dcspy-2.1.2/tests/test_starter.py` & `dcspy-2.2.0/tests/test_starter.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.2/tests/test_utils.py` & `dcspy-2.2.0/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,54 @@
+from os import makedirs
 from pathlib import Path
 from unittest.mock import MagicMock, PropertyMock, mock_open, patch
 
 from packaging import version
 from pytest import mark
 
 from dcspy import utils
 
 
 @mark.parametrize('online_tag, result', [
-    ('1.1.1', utils.ReleaseInfo(True, version.parse('1.1.1'), 'github.com/fake.tgz', '09 August 2021', 'Pre-release', 'fake.tgz')),
-    ('3.2.1', utils.ReleaseInfo(False, version.parse('3.2.1'), 'github.com/fake.tgz', '09 August 2021', 'Pre-release', 'fake.tgz'))
+    ('1.1.1', utils.ReleaseInfo(latest=True,
+                                ver=version.parse('1.1.1'),
+                                dl_url='github.com/fake.tgz',
+                                published='09 August 2021',
+                                release_type='Pre-release',
+                                archive_file='fake.tgz')),
+    ('3.2.1', utils.ReleaseInfo(latest=False,
+                                ver=version.parse('3.2.1'),
+                                dl_url='github.com/fake.tgz',
+                                published='09 August 2021',
+                                release_type='Pre-release',
+                                archive_file='fake.tgz'))
 ], ids=['No update', 'New version'])
 def test_check_ver_is_possible(online_tag, result):
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=True)
         type(response_get.return_value).json = MagicMock(return_value={'tag_name': online_tag, 'prerelease': True,
                                                                        'assets': [{'browser_download_url': 'github.com/fake.tgz'}],
                                                                        'published_at': '2021-08-09T16:41:51Z'})
         assert utils.check_ver_at_github(repo='fake1/package1', current_ver='1.1.1') == result
 
 
 def test_check_ver_can_not_check():
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=False)
-        assert utils.check_ver_at_github(repo='fake2/package2', current_ver='2.2.2') == utils.ReleaseInfo(False, version.parse('unknown'), '', '', 'Regular', '')
+        assert utils.check_ver_at_github(repo='fake2/package2', current_ver='2.2.2') == utils.ReleaseInfo(False, version.parse('0.0.0'), '', '', 'Regular', '')
 
 
 def test_check_ver_exception():
     with patch.object(utils, 'get', side_effect=Exception('Connection error')):
-        assert utils.check_ver_at_github(repo='fake3/package3', current_ver='3.3.3') == utils.ReleaseInfo(False, version.parse('unknown'), '', '', 'Regular', '')
+        assert utils.check_ver_at_github(repo='fake3/package3', current_ver='3.3.3') == utils.ReleaseInfo(False, version.parse('0.0.0'), '', '', 'Regular', '')
 
 
 @mark.parametrize('online_tag, result', [
     ('1.1.1', 'v1.1.1 (latest)'),
-    ('3.2.1', 'v1.1.1 (please update!)')
+    ('3.2.1', 'v1.1.1 (update!)')
 ], ids=['No update', 'New version'])
 def test_get_version_string_is_possible(online_tag, result):
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=True)
         type(response_get.return_value).json = MagicMock(return_value={'tag_name': online_tag, 'prerelease': True,
                                                                        'assets': [{'browser_download_url': 'github.com/fake.tgz'}],
                                                                        'published_at': '2021-08-09T16:41:51Z'})
@@ -123,14 +134,35 @@
 @mark.parametrize('side_effect', [FileNotFoundError, PermissionError])
 def test_check_dcs_ver_file_not_exists(side_effect):
     with patch('dcspy.utils.open', side_effect=side_effect):
         dcs_ver = utils.check_dcs_ver(Path(''))
         assert dcs_ver == ('Unknown', 'Unknown')
 
 
+def test_check_bios_ver(tmpdir):
+    makedirs(Path(tmpdir) / 'lib')
+    with open(file=Path(tmpdir) / 'lib' / 'CommonData.lua', encoding='utf-8', mode='w+') as cd_lua:
+        cd_lua.write('local function getVersion()\n\treturn "1.2.3"\nend')
+    result = utils.check_bios_ver(bios_path=tmpdir)
+    assert result == utils.ReleaseInfo(latest=False, ver=version.parse('1.2.3'), dl_url='', published='', release_type='', archive_file='')
+
+
+def test_check_bios_ver_empty_lua(tmpdir):
+    makedirs(Path(tmpdir) / 'lib')
+    with open(file=Path(tmpdir) / 'lib' / 'CommonData.lua', encoding='utf-8', mode='w+') as cd_lua:
+        cd_lua.write('')
+    result = utils.check_bios_ver(bios_path=tmpdir)
+    assert result == utils.ReleaseInfo(latest=False, ver=version.parse('0.0.0'), dl_url='', published='', release_type='', archive_file='')
+
+
+def test_check_bios_ver_raise_exception(tmpdir):
+    result = utils.check_bios_ver(bios_path=tmpdir)
+    assert result == utils.ReleaseInfo(latest=False, ver=version.parse('0.0.0'), dl_url='', published='', release_type='', archive_file='')
+
+
 def test_is_git_repo(tmpdir):
     from git import Repo
     assert utils.is_git_repo(tmpdir) is False
     Repo.init(tmpdir)
     assert utils.is_git_repo(tmpdir) is True
```

