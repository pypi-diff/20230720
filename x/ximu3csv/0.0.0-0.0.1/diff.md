# Comparing `tmp/ximu3csv-0.0.0.tar.gz` & `tmp/ximu3csv-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ximu3csv-0.0.0.tar", last modified: Mon Jun 12 13:23:08 2023, max compression
+gzip compressed data, was "ximu3csv-0.0.1.tar", last modified: Thu Jul 20 19:17:24 2023, max compression
```

## Comparing `ximu3csv-0.0.0.tar` & `ximu3csv-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:23:08.057556 ximu3csv-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 13:22:54.000000 ximu3csv-0.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-12 13:23:08.057556 ximu3csv-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 13:22:54.000000 ximu3csv-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:23:08.057556 ximu3csv-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-12 13:22:54.000000 ximu3csv-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:23:08.057556 ximu3csv-0.0.0/ximu3csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-12 13:23:08.000000 ximu3csv-0.0.0/ximu3csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 13:23:08.000000 ximu3csv-0.0.0/ximu3csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:23:08.000000 ximu3csv-0.0.0/ximu3csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 13:23:08.000000 ximu3csv-0.0.0/ximu3csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-12 13:22:54.000000 ximu3csv-0.0.0/ximu3csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:17:24.809592 ximu3csv-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-20 19:17:08.000000 ximu3csv-0.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 19:17:24.809592 ximu3csv-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-20 19:17:08.000000 ximu3csv-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:17:24.809592 ximu3csv-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 19:17:08.000000 ximu3csv-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:17:24.809592 ximu3csv-0.0.1/ximu3csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 19:17:24.000000 ximu3csv-0.0.1/ximu3csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 19:17:24.000000 ximu3csv-0.0.1/ximu3csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:17:24.000000 ximu3csv-0.0.1/ximu3csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 19:17:24.000000 ximu3csv-0.0.1/ximu3csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-20 19:17:08.000000 ximu3csv-0.0.1/ximu3csv.py
```

### Comparing `ximu3csv-0.0.0/LICENSE.md` & `ximu3csv-0.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ximu3csv-0.0.0/PKG-INFO` & `ximu3csv-0.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ximu3csv
-Version: 0.0.0
+Version: 0.0.1
 Summary: x-IMU3 CSV
 Home-page: https://github.com/xioTechnologies/ximu3csv
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ximu3csv-0.0.0/README.md` & `ximu3csv-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ximu3csv-0.0.0/setup.py` & `ximu3csv-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if len(sys.argv) == 1:  # if this script was called without arguments
     sys.argv.append("install")
     sys.argv.append("--user")
 
 github_url = "https://github.com/xioTechnologies/ximu3csv"
 
 setup(name="ximu3csv",
-      version="0.0.0",
+      version="0.0.1",
       description="x-IMU3 CSV",
       long_description="See [github](" + github_url + ") for documentation and examples.",
       long_description_content_type='text/markdown',
       url=github_url,
       author="x-io Technologies Limited",
       author_email="info@x-io.co.uk",
       license="MIT",
```

### Comparing `ximu3csv-0.0.0/ximu3csv.egg-info/PKG-INFO` & `ximu3csv-0.0.1/ximu3csv.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ximu3csv
-Version: 0.0.0
+Version: 0.0.1
 Summary: x-IMU3 CSV
 Home-page: https://github.com/xioTechnologies/ximu3csv
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ximu3csv-0.0.0/ximu3csv.py` & `ximu3csv-0.0.1/ximu3csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         file_path = os.path.join(directory, message_type.file_name)
 
         if not os.path.isfile(file_path):
             return
 
         self._numerical = numpy.genfromtxt(file_path, delimiter=",", skip_header=1)
 
-        if message_type in (MessageType.SERIAL_ACCESSORY, MessageType.NOTIFICATION, MessageType.ERROR):
+        if message_type in (MessageType.NOTIFICATION, MessageType.ERROR):
             self._string = numpy.genfromtxt(file_path, delimiter=",", skip_header=1, usecols=1, dtype=None, encoding=None)  # TODO: Handle strings that contain commas
 
     @property
     def timestamp(self):
         return self._numerical[:, 0]
 
 
@@ -299,16 +299,16 @@
 
 
 class SerialAccessory(__Message):
     def __init__(self, directory, message_types):
         super().__init__(directory, message_types, MessageType.SERIAL_ACCESSORY)
 
     @property
-    def string(self):
-        return self._string
+    def csv(self):
+        return self._numerical[:, 1:]
 
 
 class Notification(__Message):
     def __init__(self, directory, message_types):
         super().__init__(directory, message_types, MessageType.NOTIFICATION)
 
     @property
```

