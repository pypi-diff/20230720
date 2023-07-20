# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.7.4.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.7.4.tar", last modified: Thu Jul 20 05:44:29 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.7.5.tar", last modified: Thu Jul 20 08:10:04 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4.tar` & `hyutils-hyutil-hoyun-lab-0.0.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 05:44:29.879775 hyutils-hyutil-hoyun-lab-0.0.7.4/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-07-20 05:44:29.879202 hyutils-hyutil-hoyun-lab-0.0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 05:44:29.879922 hyutils-hyutil-hoyun-lab-0.0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-20 05:41:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:44:29.857020 hyutils-hyutil-hoyun-lab-0.0.7.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 05:44:29.872519 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      449 2023-07-20 05:41:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/augmentjob.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    15946 2023-07-20 05:41:44.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0    11383 2023-07-20 05:28:52.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:44:29.877519 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-07-20 05:44:29.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-07-20 05:44:29.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 05:44:29.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 05:44:29.000000 hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 08:10:04.053267 hyutils-hyutil-hoyun-lab-0.0.7.5/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-07-20 08:10:04.052518 hyutils-hyutil-hoyun-lab-0.0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:10:04.053516 hyutils-hyutil-hoyun-lab-0.0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-20 08:09:43.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:10:04.027515 hyutils-hyutil-hoyun-lab-0.0.7.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:10:04.046016 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      449 2023-07-20 08:09:43.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/augmentjob.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    16576 2023-07-20 08:09:20.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0    11383 2023-07-20 05:28:52.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:10:04.051017 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-07-20 08:10:04.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-20 08:10:04.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:10:04.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 08:10:04.000000 hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.7.4",
+    version="0.0.7.5",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/augmentjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/augmentjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,41 @@
 from object_detection.utils import dataset_util
 from collections import namedtuple
 import glob
 import shutil
 import cv2
 
 
-def xml_to_dataframe(path, include_string):
+def xml_to_dataframe(xml_path, include_string, special_action=None):
     classes_names = []
-
-    classes_names.clear()
-    if not os.path.exists(path) or len(include_string) == 0:
-        print(f'invalid parameters: {path} {include_string}')
-        return
+    file_list = []
     xml_list = []
-    xml_target = os.path.join(path, include_string)
-    file_list = glob.glob(xml_target)
+
+    # classes_names.clear()
+
+    if special_action is not None and special_action == 'multi-annotation':
+        for item in xml_path:
+            if not os.path.exists(item) or len(include_string) == 0:
+                print(f'invalid parameters: {item} {include_string}')
+                continue
+            xml_target = os.path.join(xml_path, include_string)
+            temp_list = glob.glob(xml_target)
+            file_list += temp_list
+        random.shuffle(file_list)
+        random.shuffle(file_list)
+
+    else:
+        if not os.path.exists(xml_path) or len(include_string) == 0:
+            print(f'invalid parameters: {xml_path} {include_string}')
+            return
+
+        xml_target = os.path.join(xml_path, include_string)
+        file_list = glob.glob(xml_target)
+
+
     for xml_file in tqdm(file_list, desc=include_string):
         # sprint('---> ', xml_file)
         tree = Et.parse(xml_file)
         root = tree.getroot()
         for member in root.findall('object'):
             classes_names.append(member.find('name').text)
             bndbox = member.find('bndbox')
@@ -58,17 +75,17 @@
     --xml_path=D:\python_work\tf-train-data\faces\new_face_train_label 
     --include_string=01*.xml 
     --output_file=D:\python_work\tf-train-data\faces\new_face_train_label01.csv 
     --labelmap_name=new_face_labelmap_01.pbtxt 
 """
 
 
-def convert_to_csv(xml_path, include_string, output_file, labelmap_path):
+def convert_to_csv(xml_path, include_string, output_file, labelmap_path, special_action=None):
 
-    xml_df, classes_names = xml_to_dataframe(xml_path, include_string)
+    xml_df, classes_names = xml_to_dataframe(xml_path, include_string, special_action)
 
     # label map 생성
     # labelmap_dir = os.path.dirname(output_file)
     # label_map_path = os.path.join(labelmap_dir, labelmap_name)
     print(f'label_map_path > {labelmap_path}')
     pbtxt_content = ""
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.7.5/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

