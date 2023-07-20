# Comparing `tmp/ThermalNetwork-0.1.tar.gz` & `tmp/ThermalNetwork-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ThermalNetwork-0.1.tar", last modified: Wed Jul 19 16:57:35 2023, max compression
+gzip compressed data, was "ThermalNetwork-0.1.1.tar", last modified: Thu Jul 20 17:35:11 2023, max compression
```

## Comparing `ThermalNetwork-0.1.tar` & `ThermalNetwork-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mattmitchell   (501) staff       (20)        0 2023-07-19 16:57:35.115014 ThermalNetwork-0.1/
--rw-r--r--   0 mattmitchell   (501) staff       (20)     1500 2023-04-11 01:40:10.000000 ThermalNetwork-0.1/LICENSE
--rw-r--r--   0 mattmitchell   (501) staff       (20)      660 2023-07-19 16:57:35.115259 ThermalNetwork-0.1/PKG-INFO
--rw-r--r--   0 mattmitchell   (501) staff       (20)      121 2023-07-19 16:57:02.000000 ThermalNetwork-0.1/README.md
-drwxr-xr-x   0 mattmitchell   (501) staff       (20)        0 2023-07-19 16:57:35.103088 ThermalNetwork-0.1/ThermalNetwork.egg-info/
--rw-r--r--   0 mattmitchell   (501) staff       (20)      660 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/PKG-INFO
--rw-r--r--   0 mattmitchell   (501) staff       (20)      531 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/SOURCES.txt
--rw-r--r--   0 mattmitchell   (501) staff       (20)        1 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/dependency_links.txt
--rw-r--r--   0 mattmitchell   (501) staff       (20)       77 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/entry_points.txt
--rw-r--r--   0 mattmitchell   (501) staff       (20)       30 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/requires.txt
--rw-r--r--   0 mattmitchell   (501) staff       (20)       15 2023-07-19 16:57:35.000000 ThermalNetwork-0.1/ThermalNetwork.egg-info/top_level.txt
--rw-r--r--   0 mattmitchell   (501) staff       (20)      232 2023-07-19 16:57:35.116181 ThermalNetwork-0.1/setup.cfg
--rw-r--r--   0 mattmitchell   (501) staff       (20)     1093 2023-07-19 16:57:02.000000 ThermalNetwork-0.1/setup.py
-drwxr-xr-x   0 mattmitchell   (501) staff       (20)        0 2023-07-19 16:57:35.113917 ThermalNetwork-0.1/thermalnetwork/
--rw-r--r--   0 mattmitchell   (501) staff       (20)       16 2023-07-19 16:47:43.000000 ThermalNetwork-0.1/thermalnetwork/__init__.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)      424 2023-07-13 14:38:11.000000 ThermalNetwork-0.1/thermalnetwork/base_component.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)     1222 2023-07-19 16:57:02.000000 ThermalNetwork-0.1/thermalnetwork/energy_transfer_station.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)      260 2023-04-19 15:04:01.000000 ThermalNetwork-0.1/thermalnetwork/enums.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)      533 2023-04-19 15:01:57.000000 ThermalNetwork-0.1/thermalnetwork/fan.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)     4334 2023-07-19 16:57:02.000000 ThermalNetwork-0.1/thermalnetwork/ground_heat_exchanger.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)     1032 2023-04-19 15:01:57.000000 ThermalNetwork-0.1/thermalnetwork/heat_pump.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)    23849 2023-07-19 16:57:02.000000 ThermalNetwork-0.1/thermalnetwork/network.py
--rw-r--r--   0 mattmitchell   (501) staff       (20)      901 2023-04-19 15:04:01.000000 ThermalNetwork-0.1/thermalnetwork/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/thermalnetwork/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/base_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/energy_transfer_station.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/fan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/ground_heat_exchanger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23849 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/pump.py
```

### Comparing `ThermalNetwork-0.1/LICENSE` & `ThermalNetwork-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/PKG-INFO` & `ThermalNetwork-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.1
+Version: 0.1.1
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
+Description: # ThermalNetwork
+        
+        A library for sizing multiple ground heat exchangers distributed around a single-pipe thermal network.
+        
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ThermalNetwork
-
-A library for sizing multiple ground heat exchangers distributed around a single-pipe thermal network.
```

### Comparing `ThermalNetwork-0.1/ThermalNetwork.egg-info/PKG-INFO` & `ThermalNetwork-0.1.1/ThermalNetwork.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.1
+Version: 0.1.1
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
+Description: # ThermalNetwork
+        
+        A library for sizing multiple ground heat exchangers distributed around a single-pipe thermal network.
+        
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ThermalNetwork
-
-A library for sizing multiple ground heat exchangers distributed around a single-pipe thermal network.
```

### Comparing `ThermalNetwork-0.1/ThermalNetwork.egg-info/SOURCES.txt` & `ThermalNetwork-0.1.1/ThermalNetwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/setup.py` & `ThermalNetwork-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,14 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
     install_requires=[
         'click>=8.1.6',
-        'ghedesigner>=1.1'
+        'ghedesigner>=1.1',
+        'pandas>=2.0.3'
     ],
     entry_points={
-        'console_scripts': ['thermalnetwork=thermalnetwork.network.run_sizer_from_cli']
+        'console_scripts': ['thermalnetwork=thermalnetwork.network:run_sizer_from_cli']
     }
 )
```

### Comparing `ThermalNetwork-0.1/thermalnetwork/energy_transfer_station.py` & `ThermalNetwork-0.1.1/thermalnetwork/energy_transfer_station.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/thermalnetwork/fan.py` & `ThermalNetwork-0.1.1/thermalnetwork/fan.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/thermalnetwork/ground_heat_exchanger.py` & `ThermalNetwork-0.1.1/thermalnetwork/ground_heat_exchanger.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/thermalnetwork/heat_pump.py` & `ThermalNetwork-0.1.1/thermalnetwork/heat_pump.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/thermalnetwork/network.py` & `ThermalNetwork-0.1.1/thermalnetwork/network.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1/thermalnetwork/pump.py` & `ThermalNetwork-0.1.1/thermalnetwork/pump.py`

 * *Files identical despite different names*

