# Comparing `tmp/etrobo_python-0.4.tar.gz` & `tmp/etrobo_python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/etrobo_python-0.4.tar", last modified: Sun Jun 18 13:12:02 2023, max compression
+gzip compressed data, was "dist/etrobo_python-0.4.1.tar", last modified: Thu Jul 20 11:38:41 2023, max compression
```

## Comparing `etrobo_python-0.4.tar` & `etrobo_python-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.232245 etrobo_python-0.4/
--rw-r--r--   0 atushi     (501) staff       (20)     1071 2022-05-05 20:12:25.000000 etrobo_python-0.4/LICENSE
--rw-r--r--   0 atushi     (501) staff       (20)      965 2023-06-18 13:12:02.231589 etrobo_python-0.4/PKG-INFO
--rw-r--r--   0 atushi     (501) staff       (20)      578 2023-06-18 12:59:11.000000 etrobo_python-0.4/README.txt
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.222167 etrobo_python-0.4/etrobo_python/
--rw-r--r--   0 atushi     (501) staff       (20)      199 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/__init__.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.225462 etrobo_python-0.4/etrobo_python/backends/
--rw-r--r--   0 atushi     (501) staff       (20)        0 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/__init__.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.226726 etrobo_python-0.4/etrobo_python/backends/pybricks/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)     4314 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     1463 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/dispatcher.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.228440 etrobo_python-0.4/etrobo_python/backends/raspike/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/raspike/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)    10152 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/raspike/connector.py
--rw-r--r--   0 atushi     (501) staff       (20)     3493 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/raspike/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     1360 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/raspike/dispatcher.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.230855 etrobo_python-0.4/etrobo_python/backends/simulator/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/simulator/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)     7337 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/simulator/connector.py
--rw-r--r--   0 atushi     (501) staff       (20)     3718 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/simulator/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     2278 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/simulator/dispatcher.py
--rw-r--r--   0 atushi     (501) staff       (20)     6003 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     5329 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/etrobo.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.224846 etrobo_python-0.4/etrobo_python.egg-info/
--rw-r--r--   0 atushi     (501) staff       (20)      965 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/PKG-INFO
--rw-r--r--   0 atushi     (501) staff       (20)      770 2023-06-18 13:12:02.000000 etrobo_python-0.4/etrobo_python.egg-info/SOURCES.txt
--rw-r--r--   0 atushi     (501) staff       (20)        1 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/dependency_links.txt
--rw-r--r--   0 atushi     (501) staff       (20)       14 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/top_level.txt
--rw-r--r--   0 atushi     (501) staff       (20)       38 2023-06-18 13:12:02.232439 etrobo_python-0.4/setup.cfg
--rw-r--r--   0 atushi     (501) staff       (20)      648 2023-06-18 12:59:11.000000 etrobo_python-0.4/setup.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.317259 etrobo_python-0.4.1/
+-rw-r--r--   0 atushi     (501) staff       (20)     1071 2022-05-05 20:12:25.000000 etrobo_python-0.4.1/LICENSE
+-rw-r--r--   0 atushi     (501) staff       (20)      967 2023-07-20 11:38:41.316897 etrobo_python-0.4.1/PKG-INFO
+-rw-r--r--   0 atushi     (501) staff       (20)      578 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/README.txt
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.306816 etrobo_python-0.4.1/etrobo_python/
+-rw-r--r--   0 atushi     (501) staff       (20)      201 2023-07-20 11:21:53.000000 etrobo_python-0.4.1/etrobo_python/__init__.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.309953 etrobo_python-0.4.1/etrobo_python/backends/
+-rw-r--r--   0 atushi     (501) staff       (20)        0 2022-05-05 20:12:25.000000 etrobo_python-0.4.1/etrobo_python/backends/__init__.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.311752 etrobo_python-0.4.1/etrobo_python/backends/pybricks/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4.1/etrobo_python/backends/pybricks/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)     4314 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/etrobo_python/backends/pybricks/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     1463 2022-05-17 10:25:33.000000 etrobo_python-0.4.1/etrobo_python/backends/pybricks/dispatcher.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.314229 etrobo_python-0.4.1/etrobo_python/backends/raspike/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-17 10:25:33.000000 etrobo_python-0.4.1/etrobo_python/backends/raspike/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)    10151 2023-07-20 11:01:48.000000 etrobo_python-0.4.1/etrobo_python/backends/raspike/connector.py
+-rw-r--r--   0 atushi     (501) staff       (20)     3493 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/etrobo_python/backends/raspike/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     1360 2023-07-20 11:11:22.000000 etrobo_python-0.4.1/etrobo_python/backends/raspike/dispatcher.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.316341 etrobo_python-0.4.1/etrobo_python/backends/simulator/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4.1/etrobo_python/backends/simulator/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)     7337 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/etrobo_python/backends/simulator/connector.py
+-rw-r--r--   0 atushi     (501) staff       (20)     3718 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/etrobo_python/backends/simulator/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     2278 2022-05-17 10:25:33.000000 etrobo_python-0.4.1/etrobo_python/backends/simulator/dispatcher.py
+-rw-r--r--   0 atushi     (501) staff       (20)     6003 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/etrobo_python/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     5329 2022-05-17 10:25:33.000000 etrobo_python-0.4.1/etrobo_python/etrobo.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-07-20 11:38:41.309450 etrobo_python-0.4.1/etrobo_python.egg-info/
+-rw-r--r--   0 atushi     (501) staff       (20)      967 2023-07-20 11:38:41.000000 etrobo_python-0.4.1/etrobo_python.egg-info/PKG-INFO
+-rw-r--r--   0 atushi     (501) staff       (20)      770 2023-07-20 11:38:41.000000 etrobo_python-0.4.1/etrobo_python.egg-info/SOURCES.txt
+-rw-r--r--   0 atushi     (501) staff       (20)        1 2023-07-20 11:38:41.000000 etrobo_python-0.4.1/etrobo_python.egg-info/dependency_links.txt
+-rw-r--r--   0 atushi     (501) staff       (20)       14 2023-07-20 11:38:41.000000 etrobo_python-0.4.1/etrobo_python.egg-info/top_level.txt
+-rw-r--r--   0 atushi     (501) staff       (20)       38 2023-07-20 11:38:41.317344 etrobo_python-0.4.1/setup.cfg
+-rw-r--r--   0 atushi     (501) staff       (20)      648 2023-06-18 12:59:11.000000 etrobo_python-0.4.1/setup.py
```

### Comparing `etrobo_python-0.4/LICENSE` & `etrobo_python-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/PKG-INFO` & `etrobo_python-0.4.1/etrobo_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: etrobo_python
-Version: 0.4
+Name: etrobo-python
+Version: 0.4.1
 Summary: Python middleware for ET-ROBOCON 2023.
 Home-page: https://github.com/takedarts/etrobo-python
 Author: Atsushi TAKEDA
 Author-email: takedarts@mail.tohoku-gakuin.ac.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etrobo_python-0.4/README.txt` & `etrobo_python-0.4.1/README.txt`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/pybricks/device.py` & `etrobo_python-0.4.1/etrobo_python/backends/pybricks/device.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/pybricks/dispatcher.py` & `etrobo_python-0.4.1/etrobo_python/backends/pybricks/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/raspike/connector.py` & `etrobo_python-0.4.1/etrobo_python/backends/raspike/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional, Tuple
 
 import serial
 
 # モーターの回転方向
 # モーターの設定値と取得値の方向を設定する
 # +1 か -1 を設定すること
-MOTOR_SIGN = -1
+MOTOR_SIGN = 1
 
 _CONNECTOR: Optional['_Connector'] = None
 
 # 受信データ
 # バッファ内の位置: 命令番号 - 意味
 # 00:  1 - カラーセンサ（ambient)
 # 01:  2 - カラーセンサ（color）
```

### Comparing `etrobo_python-0.4/etrobo_python/backends/raspike/device.py` & `etrobo_python-0.4.1/etrobo_python/backends/raspike/device.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/raspike/dispatcher.py` & `etrobo_python-0.4.1/etrobo_python/backends/raspike/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/simulator/connector.py` & `etrobo_python-0.4.1/etrobo_python/backends/simulator/connector.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/simulator/device.py` & `etrobo_python-0.4.1/etrobo_python/backends/simulator/device.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/backends/simulator/dispatcher.py` & `etrobo_python-0.4.1/etrobo_python/backends/simulator/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/device.py` & `etrobo_python-0.4.1/etrobo_python/device.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python/etrobo.py` & `etrobo_python-0.4.1/etrobo_python/etrobo.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/etrobo_python.egg-info/PKG-INFO` & `etrobo_python-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: etrobo-python
-Version: 0.4
+Name: etrobo_python
+Version: 0.4.1
 Summary: Python middleware for ET-ROBOCON 2023.
 Home-page: https://github.com/takedarts/etrobo-python
 Author: Atsushi TAKEDA
 Author-email: takedarts@mail.tohoku-gakuin.ac.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etrobo_python-0.4/etrobo_python.egg-info/SOURCES.txt` & `etrobo_python-0.4.1/etrobo_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.4/setup.py` & `etrobo_python-0.4.1/setup.py`

 * *Files identical despite different names*

