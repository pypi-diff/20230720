# Comparing `tmp/kappe-0.7.3.tar.gz` & `tmp/kappe-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappe-0.7.3.tar", last modified: Wed Apr 26 09:47:42 2023, max compression
+gzip compressed data, was "kappe-0.8.0.tar", last modified: Thu Jul 20 13:41:54 2023, max compression
```

## Comparing `kappe-0.7.3.tar` & `kappe-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.110287 kappe-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 09:47:29.000000 kappe-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-26 09:47:42.110287 kappe-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-26 09:47:29.000000 kappe-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-26 09:47:29.000000 kappe-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:47:42.110287 kappe-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.098287 kappe-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.102287 kappe-0.7.3/src/kappe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/kappe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/qos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.110287 kappe-0.7.3/src/kappe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/msg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/pointcloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.199529 kappe-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 13:41:44.000000 kappe-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 13:41:54.195529 kappe-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 13:41:44.000000 kappe-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-20 13:41:44.000000 kappe-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:41:54.199529 kappe-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.191529 kappe-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/kappe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/module/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/msg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 13:41:44.000000 kappe-0.8.0/src/kappe/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:41:54.195529 kappe-0.8.0/src/kappe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 13:41:54.000000 kappe-0.8.0/src/kappe.egg-info/top_level.txt
```

### Comparing `kappe-0.7.3/PKG-INFO` & `kappe-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.7.3
+Version: 0.8.0
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -23,8 +23,8 @@
 git clone --depth=1 --branch=humble https://github.com/ros2/example_interfaces.git msgs/example_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/rcl_interfaces.git msgs/rcl_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/geometry2.git msgs/geometry2
 ```
 
 ## Licenses
 
-- [kappe/utils/pointcloud2.py](./kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
+- [pointcloud2.py](./src/kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
```

### Comparing `kappe-0.7.3/README.md` & `kappe-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 git clone --depth=1 --branch=humble https://github.com/ros2/example_interfaces.git msgs/example_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/rcl_interfaces.git msgs/rcl_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/geometry2.git msgs/geometry2
 ```
 
 ## Licenses
 
-- [kappe/utils/pointcloud2.py](./kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
+- [pointcloud2.py](./src/kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
```

### Comparing `kappe-0.7.3/src/kappe/convert.py` & `kappe-0.8.0/src/kappe/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,25 @@
         return filtered_channels
 
     def read_ros_messaged(self,
                           topics: Iterable[str] | None = None,
                           start_time: datetime | None = None,
                           end_time: datetime | None = None,
                           ) -> Iterator[McapROSMessage]:
+        self.f_reader.seek(0)
         if self.mcap_header.profile == Profile.ROS1:
             msg_iter = read_ros1_messages(
-                self.reader,
+                self.f_reader,
                 topics=topics,
                 start_time=start_time,
                 end_time=end_time,
             )
         elif self.mcap_header.profile == Profile.ROS2:
             msg_iter = read_ros2_messages(
-                self.reader,
+                self.f_reader,
                 topics=topics,
                 start_time=start_time,
                 end_time=end_time,
             )
         else:
             raise ValueError(f'Unsupported profile {self.mcap_header.profile}')
 
@@ -249,16 +250,15 @@
         ros_msg = msg.ros_msg
         schema_name = msg.schema.name
         topic = msg.channel.topic
 
         # handling of converters
         conv_list = self.plugin_conv.get(topic, [])
         for conv, output_topic in conv_list:
-            conv_msg = conv.convert(ros_msg)
-            if conv_msg is not None:
+            if conv_msg := conv.convert(ros_msg):
                 # TODO: pass this to process_message?
                 self.writer.write_message(
                     topic=output_topic,
                     schema=self.schema_list[conv.output_schema],
                     message=conv_msg,
                     log_time=msg.log_time_ns,
                     publish_time=msg.publish_time_ns,
```

### Comparing `kappe-0.7.3/src/kappe/cut.py` & `kappe-0.8.0/src/kappe/cut.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/kappe.py` & `kappe-0.8.0/src/kappe/kappe.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/module/pointcloud.py` & `kappe-0.8.0/src/kappe/module/pointcloud.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/module/qos.py` & `kappe-0.8.0/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/module/tf.py` & `kappe-0.8.0/src/kappe/module/tf.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/module/timing.py` & `kappe-0.8.0/src/kappe/module/timing.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/plugin.py` & `kappe-0.8.0/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/plugins/image.py` & `kappe-0.8.0/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/settings.py` & `kappe-0.8.0/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/utils/msg_def.py` & `kappe-0.8.0/src/kappe/utils/msg_def.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/utils/pointcloud2.py` & `kappe-0.8.0/src/kappe/utils/pointcloud2.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe/utils/settings.py` & `kappe-0.8.0/src/kappe/utils/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.3/src/kappe.egg-info/PKG-INFO` & `kappe-0.8.0/src/kappe.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.7.3
+Version: 0.8.0
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -23,8 +23,8 @@
 git clone --depth=1 --branch=humble https://github.com/ros2/example_interfaces.git msgs/example_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/rcl_interfaces.git msgs/rcl_interfaces
 git clone --depth=1 --branch=humble https://github.com/ros2/geometry2.git msgs/geometry2
 ```
 
 ## Licenses
 
-- [kappe/utils/pointcloud2.py](./kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
+- [pointcloud2.py](./src/kappe/utils/pointcloud2.py) based on [sensor_msgs_py/point_cloud2.py](https://github.com/ros2/common_interfaces/blob/rolling/sensor_msgs_py/sensor_msgs_py/point_cloud2.py) licensed [Apache License 2.0](https://raw.githubusercontent.com/ros2/common_interfaces/rolling/LICENSE)
```

### Comparing `kappe-0.7.3/src/kappe.egg-info/SOURCES.txt` & `kappe-0.8.0/src/kappe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

