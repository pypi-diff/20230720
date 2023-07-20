# Comparing `tmp/kappe-0.8.1.tar.gz` & `tmp/kappe-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappe-0.8.1.tar", last modified: Thu Jul 20 14:50:39 2023, max compression
+gzip compressed data, was "kappe-0.8.2.tar", last modified: Thu Jul 20 15:27:06 2023, max compression
```

## Comparing `kappe-0.8.1.tar` & `kappe-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:50:30.000000 kappe-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 14:50:39.818515 kappe-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 14:50:30.000000 kappe-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 14:50:30.000000 kappe-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:50:39.818515 kappe-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.814515 kappe-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/kappe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/qos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/module/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/msg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/pointcloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 14:50:30.000000 kappe-0.8.1/src/kappe/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:39.818515 kappe-0.8.1/src/kappe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 14:50:39.000000 kappe-0.8.1/src/kappe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:26:53.000000 kappe-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 15:27:06.506395 kappe-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 15:26:53.000000 kappe-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 15:26:53.000000 kappe-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:27:06.506395 kappe-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.502395 kappe-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/kappe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/msg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/top_level.txt
```

### Comparing `kappe-0.8.1/PKG-INFO` & `kappe-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.8.1
+Version: 0.8.2
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `kappe-0.8.1/README.md` & `kappe-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/pyproject.toml` & `kappe-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/convert.py` & `kappe-0.8.2/src/kappe/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import logging
 import time
 from collections.abc import Iterable, Iterator
 from datetime import datetime, timezone
 from pathlib import Path
 
 import strictyaml
-from mcap.reader import make_reader
+from mcap.reader import DecodedMessageTuple, make_reader
 from mcap.records import Schema, Statistics
 from mcap.summary import Summary
 from mcap.well_known import Profile, SchemaEncoding
-from mcap_ros1.reader import read_ros1_messages
-from mcap_ros2.reader import read_ros2_messages
+from mcap_ros1.decoder import DecoderFactory as Ros1DecoderFactory
+from mcap_ros2.decoder import DecoderFactory as Ros2DecoderFactory
 from mcap_ros2.writer import Writer as McapWriter
 from tqdm import tqdm
 
 from kappe import __version__
 from kappe.module.pointcloud import point_cloud
-from kappe.module.tf import tf_remove
+from kappe.module.tf import tf_remove, tf_static_insert
 from kappe.module.timing import fix_ros1_time, time_offset
 from kappe.plugin import ConverterPlugin, load_plugin
 from kappe.settings import Settings
 from kappe.utils.msg_def import get_message_definition
-from kappe.utils.types import McapROSMessage
 
 logger = logging.getLogger(__name__)
 
 
 def generate_qos(config: dict) -> str:
     qos_default = {
         'history': 3,
@@ -56,14 +55,16 @@
         self.config = config
         self.input_path = input_path
         self.output_path = output_path
         self.raw_config = raw_config
 
         self.drop_msg_count: dict[str, int] = {}
 
+        self.tf_inserted = False
+
         # maps input topic to list of plugins
         self.plugin_conv: dict[str, list[tuple[ConverterPlugin, str]]] = {}
 
         # load plugins
         for conv in config.plugins:
             lst = self.plugin_conv.get(conv.input_topic, [])
             cls = load_plugin(self.config.plugin_folder, conv.name)
@@ -217,56 +218,63 @@
                 keep = True
 
             if keep:
                 filtered_channels.add(channel.topic)
 
         return filtered_channels
 
-    def read_ros_messaged(self,
-                          topics: Iterable[str] | None = None,
-                          start_time: datetime | None = None,
-                          end_time: datetime | None = None,
-                          ) -> Iterator[McapROSMessage]:
+    def read_ros_messaged(
+        self,
+        topics: Iterable[str] | None = None,
+        start_time: datetime | None = None,
+        end_time: datetime | None = None,
+    ) -> Iterator[DecodedMessageTuple]:
         self.f_reader.seek(0)
         if self.mcap_header.profile == Profile.ROS1:
-            msg_iter = read_ros1_messages(
-                self.f_reader,
+            self.reader = make_reader(
+                self.f_reader, decoder_factories=[Ros1DecoderFactory()],
+            )
+
+            msg_iter = self.reader.iter_decoded_messages(
                 topics=topics,
                 start_time=start_time,
                 end_time=end_time,
             )
         elif self.mcap_header.profile == Profile.ROS2:
-            msg_iter = read_ros2_messages(
-                self.f_reader,
+            self.reader = make_reader(
+                self.f_reader, decoder_factories=[Ros2DecoderFactory()],
+            )
+
+            msg_iter = self.reader.iter_decoded_messages(
                 topics=topics,
                 start_time=start_time,
                 end_time=end_time,
             )
         else:
             raise ValueError(f'Unsupported profile {self.mcap_header.profile}')
 
         return msg_iter
 
-    def process_message(self, msg: McapROSMessage):
-        ros_msg = msg.ros_msg
-        schema_name = msg.schema.name
-        topic = msg.channel.topic
+    def process_message(self, msg: DecodedMessageTuple):
+        schema, channel, message, ros_msg = msg
+        schema_name = schema.name
+        topic = channel.topic
 
         # handling of converters
         conv_list = self.plugin_conv.get(topic, [])
         for conv, output_topic in conv_list:
             if conv_msg := conv.convert(ros_msg):
                 # TODO: pass this to process_message?
                 self.writer.write_message(
                     topic=output_topic,
                     schema=self.schema_list[conv.output_schema],
                     message=conv_msg,
-                    log_time=msg.log_time_ns,
-                    publish_time=msg.publish_time_ns,
-                    sequence=msg.sequence_count,
+                    log_time=message.log_time,
+                    publish_time=message.publish_time,
+                    sequence=message.sequence,
                 )
 
         # late remove topics which are required by a plugin
         if topic in self.config.topic.remove:
             return
 
         # drop every n-th message
@@ -275,40 +283,43 @@
             self.drop_msg_count[topic] = drop_count + 1
 
             drop_cfg = self.config.topic.drop[topic]
             if drop_count % drop_cfg == 0:
                 return
 
         if self.mcap_header.profile == Profile.ROS1:
-            fix_ros1_time(msg.ros_msg)
+            fix_ros1_time(ros_msg)
 
         # drop messages that are not in the schema list
         msg_schema = self.schema_list.get(schema_name)
         if msg_schema is None:
             return
 
         if topic in ['/tf', '/tf_static']:
             tf_remove(self.config.tf_static, msg)
 
+        if topic in ['/tf_static'] and not self.tf_inserted:
+            self.tf_inserted = tf_static_insert(self.config.tf_static, msg)
+
         if topic in self.config.time_offset:
             time_offset(self.config.time_offset[topic], msg)
 
         if schema_name in [
             'sensor_msgs/msg/PointCloud2',
                 'sensor_msgs/PointCloud2',
         ] and topic in self.config.point_cloud:
             point_cloud(self.config.point_cloud[topic], msg)
 
         self.writer.write_message(
             topic=self.config.topic.mapping.get(topic, topic),
             schema=self.schema_list[schema_name],
             message=ros_msg,
-            log_time=msg.log_time_ns,
-            publish_time=msg.publish_time_ns,
-            sequence=msg.sequence_count,
+            log_time=message.log_time,
+            publish_time=message.publish_time,
+            sequence=message.sequence,
         )
 
     def process_file(self, tqdm_idx: int = 0):
 
         start_time = self.statistics.message_start_time / 1e9
         if self.config.time_start is not None:
             start_time = max(start_time, self.config.time_start.timestamp())
@@ -383,15 +394,16 @@
         with tqdm(
             total=duration,
             position=tqdm_idx,
             desc=f'{self.input_path.name}',
             unit='secs',
         ) as pbar:
             for msg in msg_iter:
-                pbar.update((msg.log_time_ns // 1e6 - start_time) - pbar.n)
+                message = msg[2]
+                pbar.update((message.log_time // 1e6 - start_time) - pbar.n)
                 self.process_message(msg)
 
     def finish(self):
         # save used convert config
         self.writer._writer.add_attachment(  # noqa: SLF001
             create_time=time.time_ns(),
             log_time=time.time_ns(),
```

### Comparing `kappe-0.8.1/src/kappe/cut.py` & `kappe-0.8.2/src/kappe/cut.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/kappe.py` & `kappe-0.8.2/src/kappe/kappe.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/module/pointcloud.py` & `kappe-0.8.2/src/kappe/module/pointcloud.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
+from mcap.reader import DecodedMessageTuple
 from pydantic import BaseModel, Extra
 from scipy.spatial.transform import Rotation
 
 from kappe.utils.pointcloud2 import create_cloud, read_points
 from kappe.utils.settings import SettingRotation
-from kappe.utils.types import McapROSMessage
 
 
 class SettingPointCloud(BaseModel, extra=Extra.forbid):
     """
     Point cloud settings.
 
     :ivar remove_zero: Remove points with all zero coordinates (x, y, z).
@@ -17,23 +17,25 @@
     """
 
     remove_zero: bool = False
     rotation: SettingRotation = SettingRotation()
     field_mapping: dict[str, str] | None
 
 
-def point_cloud(cfg: SettingPointCloud, msg: McapROSMessage):
+def point_cloud(cfg: SettingPointCloud, msg: DecodedMessageTuple):
+    schema, channel, message, ros_msg = msg
+
     if cfg.field_mapping is not None:
-        for pc_field in msg.ros_msg.fields:
+        for pc_field in ros_msg.fields:
             pc_field.name = cfg.field_mapping.get(
                 pc_field.name, pc_field.name)
 
-    fields = [x.name for x in msg.ros_msg.fields]
+    fields = [x.name for x in ros_msg.fields]
     if 'x' in fields and 'y' in fields and 'z' in fields:
-        cloud = np.array(read_points(msg.ros_msg))
+        cloud = np.array(read_points(ros_msg))
         org_len = len(cloud)
 
         if cfg.remove_zero:
             cloud = cloud[np.logical_and(
                 cloud['x'] != 0.0, cloud['y'] != 0.0,
                 cloud['z'] != 0.0)]
 
@@ -46,20 +48,20 @@
 
             cloud['x'] = r_cloud[:, 0]
             cloud['y'] = r_cloud[:, 1]
             cloud['z'] = r_cloud[:, 2]
 
         if quat is not None or len(cloud) != org_len:
             msg_cloud = create_cloud(
-                msg.ros_msg.header,
-                msg.ros_msg.fields,
+                ros_msg.header,
+                ros_msg.fields,
                 cloud,
-                msg.ros_msg.point_step,
+                ros_msg.point_step,
             )
-            msg.ros_msg.data = msg_cloud['data']
+            ros_msg.data = msg_cloud['data']
 
-            msg.ros_msg.height = msg_cloud['height']
-            msg.ros_msg.width = msg_cloud['width']
-            msg.ros_msg.is_dense = msg_cloud['is_dense']
-            msg.ros_msg.is_bigendian = msg_cloud['is_bigendian']
-            msg.ros_msg.point_step = msg_cloud['point_step']
-            msg.ros_msg.row_step = msg_cloud['row_step']
+            ros_msg.height = msg_cloud['height']
+            ros_msg.width = msg_cloud['width']
+            ros_msg.is_dense = msg_cloud['is_dense']
+            ros_msg.is_bigendian = msg_cloud['is_bigendian']
+            ros_msg.point_step = msg_cloud['point_step']
+            ros_msg.row_step = msg_cloud['row_step']
```

### Comparing `kappe-0.8.1/src/kappe/module/qos.py` & `kappe-0.8.2/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/module/tf.py` & `kappe-0.8.2/src/kappe/module/tf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 
+from mcap.reader import DecodedMessageTuple
 from pydantic import BaseModel, Extra
 
 from kappe.utils.settings import SettingRotation, SettingTranslation
-from kappe.utils.types import ClassDict, McapROSMessage
+from kappe.utils.types import ClassDict
 
 
 class SettingTFInsert(BaseModel, extra=Extra.forbid):
     """
     TF insert settings.
 
     :ivar frame_id: Frame ID of the new transform.
@@ -29,54 +30,59 @@
     :ivar remove: List of child frame IDs to remove.
     :ivar insert: List of transforms to insert.
     """
 
     remove: list[str] | None = None
     insert: list[SettingTFInsert] | None = None
 
-    _inserted: bool = False
 
+def tf_static_insert(cfg: SettingTF, msg: DecodedMessageTuple) -> bool:
+    schema, channel, message, ros_msg = msg
 
-def tf_static_insert(cfg: SettingTF, msg: McapROSMessage):
-    ros_msg = msg.ros_msg
+    if cfg.insert is None:
+        return True
 
-    if not cfg._inserted and cfg.insert is not None and len(  # noqa: SLF001
-            ros_msg.transforms) > 0:
-        header = ros_msg.transforms[0].header
-        cfg._inserted = True  # noqa: SLF001
-        for insert in cfg.insert:
-            tf_msg = ClassDict(
-                header=copy.deepcopy(header),
-                child_frame_id=insert.child_frame_id,
-            )
-
-            tf_msg.header.frame_id = insert.frame_id
-
-            trans = {}
-            translation = insert.translation
-            if translation is not None:
-                trans['translation'] = {
-                    'x': translation.x,
-                    'y': translation.y,
-                    'z': translation.z,
-                }
-
-            rot_quat = insert.rotation.to_quaternion()
-            if rot_quat is not None:
-                trans['rotation'] = {
-                    'x': rot_quat[0],
-                    'y': rot_quat[1],
-                    'z': rot_quat[2],
-                    'w': rot_quat[3],
-                }
+    # One transform needed as reference
+    if len(ros_msg.transforms) == 0:
+        return False
+
+    header = ros_msg.transforms[0].header
+
+    for insert in cfg.insert:
+        tf_msg = ClassDict(
+            header=copy.deepcopy(header),
+            child_frame_id=insert.child_frame_id,
+        )
+
+        tf_msg.header.frame_id = insert.frame_id
+
+        trans = {}
+        translation = insert.translation
+        if translation is not None:
+            trans['translation'] = {
+                'x': translation.x,
+                'y': translation.y,
+                'z': translation.z,
+            }
+
+        rot_quat = insert.rotation.to_quaternion()
+        if rot_quat is not None:
+            trans['rotation'] = {
+                'x': rot_quat[0],
+                'y': rot_quat[1],
+                'z': rot_quat[2],
+                'w': rot_quat[3],
+            }
 
-            tf_msg['transform'] = trans
-            ros_msg.transforms.append(tf_msg)
+        tf_msg['transform'] = trans
+        ros_msg.transforms.append(tf_msg)
 
+    return True
 
-def tf_remove(cfg: SettingTF, msg: McapROSMessage):
-    ros_msg = msg.ros_msg
+
+def tf_remove(cfg: SettingTF, msg: DecodedMessageTuple):
+    schema, channel, message, ros_msg = msg
 
     if cfg.remove:
         for transform in ros_msg.transforms:
             if transform.child_frame_id in cfg.remove:
                 ros_msg.transforms.remove(transform)
```

### Comparing `kappe-0.8.1/src/kappe/module/timing.py` & `kappe-0.8.2/src/kappe/module/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 from types import SimpleNamespace
 from typing import Any
 
+from mcap.reader import DecodedMessageTuple
 from mcap_ros1._vendor.genpy.rostime import Duration as ROS1Duration
 from mcap_ros1._vendor.genpy.rostime import Time as ROS1Time
 from pydantic import BaseModel, Extra
 
-from kappe.utils.types import McapROSMessage
-
 logger = logging.getLogger(__name__)
 
 # TODO: move to utils, make more generic
 TimeMsg = type(
     'builtin_interfaces/Time',
     (SimpleNamespace,),
     {
@@ -75,19 +74,20 @@
 
         if 'mcap_ros2._dynamic.Time' in str(type(attr)):
             time_offset_stamp(cfg, publish_time_ns, attr)
         else:
             time_offset_rec(cfg, publish_time_ns, attr)
 
 
-def time_offset(cfg: SettingTimeOffset, msg: McapROSMessage):
+def time_offset(cfg: SettingTimeOffset, msg: DecodedMessageTuple):
     """Apply time offset to the message."""
+    schema, channel, message, ros_msg = msg
     if not hasattr(msg, '__slots__'):
         return
-    time_offset_rec(cfg, msg.publish_time_ns, msg.ros_msg)
+    time_offset_rec(cfg, message.publish_time_ns, ros_msg)
 
 
 def fix_ros1_time(msg: Any):
     """
     Fix ROS1 time and duration types, recursively inplace.
 
     secs -> sec
```

### Comparing `kappe-0.8.1/src/kappe/plugin.py` & `kappe-0.8.2/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/plugins/image.py` & `kappe-0.8.2/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/settings.py` & `kappe-0.8.2/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/utils/msg_def.py` & `kappe-0.8.2/src/kappe/utils/msg_def.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/utils/pointcloud2.py` & `kappe-0.8.2/src/kappe/utils/pointcloud2.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe/utils/settings.py` & `kappe-0.8.2/src/kappe/utils/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.1/src/kappe.egg-info/PKG-INFO` & `kappe-0.8.2/src/kappe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.8.1
+Version: 0.8.2
 Summary: Converts ROS MCAPs
 Author: Marko Bausch
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `kappe-0.8.1/src/kappe.egg-info/SOURCES.txt` & `kappe-0.8.2/src/kappe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

