# Comparing `tmp/pymazda-0.3.8.tar.gz` & `tmp/pymazda-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymazda-0.3.8.tar", max compression
+gzip compressed data, was "pymazda-0.3.9.tar", max compression
```

## Comparing `pymazda-0.3.8.tar` & `pymazda-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1075 2022-11-27 04:00:04.480300 pymazda-0.3.8/LICENSE
--rw-r--r--   0        0        0    14288 2023-03-08 16:52:07.828813 pymazda-0.3.8/README.md
--rw-r--r--   0        0        0      250 2022-11-27 04:00:04.480300 pymazda-0.3.8/pymazda/__init__.py
--rw-r--r--   0        0        0    14145 2023-03-08 16:52:48.536233 pymazda-0.3.8/pymazda/client.py
--rw-r--r--   0        0        0    14605 2023-03-08 16:40:29.577906 pymazda-0.3.8/pymazda/connection.py
--rw-r--r--   0        0        0    11171 2023-03-08 16:47:06.369198 pymazda-0.3.8/pymazda/controller.py
--rw-r--r--   0        0        0     1582 2022-11-27 04:00:04.480300 pymazda-0.3.8/pymazda/crypto_utils.py
--rw-r--r--   0        0        0     2227 2022-11-27 04:00:04.480300 pymazda-0.3.8/pymazda/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/__init__.py
--rw-r--r--   0        0        0    23773 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/android_builds.py
--rw-r--r--   0        0        0     1280 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/background_event_list.py
--rw-r--r--   0        0        0     1502 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/key_event_list.py
--rw-r--r--   0        0        0     1260 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/performance_test_results.py
--rw-r--r--   0        0        0     6031 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/sensor_data_builder.py
--rw-r--r--   0        0        0     2129 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/sensor_data_encryptor.py
--rw-r--r--   0        0        0     1266 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/sensor_data_util.py
--rw-r--r--   0        0        0     3836 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/system_info.py
--rw-r--r--   0        0        0     3052 2022-11-27 04:00:04.484300 pymazda-0.3.8/pymazda/sensordata/touch_event_list.py
--rw-r--r--   0        0        0      746 2023-03-08 16:54:04.023170 pymazda-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    15556 1970-01-01 00:00:00.000000 pymazda-0.3.8/setup.py
--rw-r--r--   0        0        0    15208 1970-01-01 00:00:00.000000 pymazda-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-01 03:26:40.128349 pymazda-0.3.9/LICENSE
+-rw-r--r--   0        0        0    14288 2023-07-01 03:26:40.128349 pymazda-0.3.9/README.md
+-rw-r--r--   0        0        0      250 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/__init__.py
+-rw-r--r--   0        0        0    14145 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/client.py
+-rw-r--r--   0        0        0    14605 2023-07-01 03:30:34.716345 pymazda-0.3.9/pymazda/connection.py
+-rw-r--r--   0        0        0    11171 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/controller.py
+-rw-r--r--   0        0        0     1582 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/crypto_utils.py
+-rw-r--r--   0        0        0     2227 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/__init__.py
+-rw-r--r--   0        0        0    23773 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/android_builds.py
+-rw-r--r--   0        0        0     1280 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/background_event_list.py
+-rw-r--r--   0        0        0     1502 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/key_event_list.py
+-rw-r--r--   0        0        0     1260 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/performance_test_results.py
+-rw-r--r--   0        0        0     6031 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/sensor_data_builder.py
+-rw-r--r--   0        0        0     2129 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/sensor_data_encryptor.py
+-rw-r--r--   0        0        0     1266 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/sensor_data_util.py
+-rw-r--r--   0        0        0     3836 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/system_info.py
+-rw-r--r--   0        0        0     3052 2023-07-01 03:26:40.128349 pymazda-0.3.9/pymazda/sensordata/touch_event_list.py
+-rw-r--r--   0        0        0      746 2023-07-01 03:31:34.468026 pymazda-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    15160 1970-01-01 00:00:00.000000 pymazda-0.3.9/PKG-INFO
```

### Comparing `pymazda-0.3.8/LICENSE` & `pymazda-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/README.md` & `pymazda-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/client.py` & `pymazda-0.3.9/pymazda/client.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/connection.py` & `pymazda-0.3.9/pymazda/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         "usher_url": "https://c5ulfwxr.mazda.com/appapi/v1/"
     }
 }
 
 IV = "0102030405060708"
 SIGNATURE_MD5 = "C383D8C4D279B78130AD52DC71D95CAA"
 APP_PACKAGE_ID = "com.interrait.mymazda"
-USER_AGENT_BASE_API = "MyMazda-Android/8.4.2"
-USER_AGENT_USHER_API = "MyMazda/8.4.2 (Google Pixel 3a; Android 11)"
+USER_AGENT_BASE_API = "MyMazda-Android/8.5.0"
+USER_AGENT_USHER_API = "MyMazda/8.5.0 (Google Pixel 3a; Android 11)"
 APP_OS = "Android"
-APP_VERSION = "8.4.2"
+APP_VERSION = "8.5.0"
 USHER_SDK_VERSION = "11.3.0700.001"
 
 MAX_RETRIES = 4
 
 class Connection:
     """Main class for handling MyMazda API connection"""
```

### Comparing `pymazda-0.3.8/pymazda/controller.py` & `pymazda-0.3.9/pymazda/controller.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/crypto_utils.py` & `pymazda-0.3.9/pymazda/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/exceptions.py` & `pymazda-0.3.9/pymazda/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/android_builds.py` & `pymazda-0.3.9/pymazda/sensordata/android_builds.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/background_event_list.py` & `pymazda-0.3.9/pymazda/sensordata/background_event_list.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/key_event_list.py` & `pymazda-0.3.9/pymazda/sensordata/key_event_list.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/performance_test_results.py` & `pymazda-0.3.9/pymazda/sensordata/performance_test_results.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/sensor_data_builder.py` & `pymazda-0.3.9/pymazda/sensordata/sensor_data_builder.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/sensor_data_encryptor.py` & `pymazda-0.3.9/pymazda/sensordata/sensor_data_encryptor.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/sensor_data_util.py` & `pymazda-0.3.9/pymazda/sensordata/sensor_data_util.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/system_info.py` & `pymazda-0.3.9/pymazda/sensordata/system_info.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pymazda/sensordata/touch_event_list.py` & `pymazda-0.3.9/pymazda/sensordata/touch_event_list.py`

 * *Files identical despite different names*

### Comparing `pymazda-0.3.8/pyproject.toml` & `pymazda-0.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymazda"
-version = "0.3.8"
+version = "0.3.9"
 description = "An API client for interacting with the MyMazda (Mazda Connected Services) API"
 authors = ["Brandon Rothweiler <brandonrothweiler@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdr99/pymazda"
 repository = "https://github.com/bdr99/pymazda"
 documentation = "https://github.com/bdr99/pymazda"
```

### Comparing `pymazda-0.3.8/PKG-INFO` & `pymazda-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pymazda
-Version: 0.3.8
+Version: 0.3.9
 Summary: An API client for interacting with the MyMazda (Mazda Connected Services) API
 Home-page: https://github.com/bdr99/pymazda
 License: MIT
 Author: Brandon Rothweiler
 Author-email: brandonrothweiler@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: cryptography (>=36.0.2)
 Project-URL: Documentation, https://github.com/bdr99/pymazda
 Project-URL: Repository, https://github.com/bdr99/pymazda
 Description-Content-Type: text/markdown
 
 # pymazda
```

