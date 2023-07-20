# Comparing `tmp/intelab_python_sdk-0.7.3.tar.gz` & `tmp/intelab_python_sdk-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelab_python_sdk-0.7.3.tar", last modified: Thu Aug 12 06:45:47 2021, max compression
+gzip compressed data, was "intelab_python_sdk-0.7.4.tar", last modified: Thu Jul 20 16:25:50 2023, max compression
```

## Comparing `intelab_python_sdk-0.7.3.tar` & `intelab_python_sdk-0.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.756034 intelab_python_sdk-0.7.3/intelab_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.756034 intelab_python_sdk-0.7.3/intelab_python_sdk/cache/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/cache/file_system_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.756034 intelab_python_sdk-0.7.3/intelab_python_sdk/dingtalk/
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/dingtalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.756034 intelab_python_sdk-0.7.3/intelab_python_sdk/email/
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/email/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_capture.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_concat.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_mp4tomp3.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_prune.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_read_frames.py
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/intelab_python_sdk/helper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/helper/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/intelab_python_sdk/logger/
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/logger/timerotaingfilehandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/intelab_python_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 06:45:47.756034 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-08-12 06:45:47.000000 intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-08-12 06:45:47.760034 intelab_python_sdk-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-08-12 06:45:38.000000 intelab_python_sdk-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-20 16:25:50.973698 intelab_python_sdk-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/cache/file_system_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/dingtalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/dingtalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/email/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/email/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_mp4tomp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_read_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/helper/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/logger/timerotaingfilehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/intelab_python_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:25:50.969697 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 16:25:50.000000 intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 16:25:50.973698 intelab_python_sdk-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-20 16:25:39.000000 intelab_python_sdk-0.7.4/setup.py
```

### Comparing `intelab_python_sdk-0.7.3/LICENSE` & `intelab_python_sdk-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/README.rst` & `intelab_python_sdk-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/cache/file_system_cache.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/cache/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/dingtalk/__init__.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/dingtalk/__init__.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/email/__init__.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/email/__init__.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/__init__.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_capture.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_capture.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_concat.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_concat.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_prune.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_prune.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_read_frames.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_read_frames.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_record.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_record.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/ffmpeg/ffmpeg_utils.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/ffmpeg/ffmpeg_utils.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/helper/cpu.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/helper/cpu.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/logger/__init__.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/logger/timerotaingfilehandler.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/logger/timerotaingfilehandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         return self.baseFilename + "." + time.strftime(self.suffix,
                                                        time.localtime())
 
     def _open(self):
         if self.encoding is None:
             stream = open(self.current_file_name, self.mode)
         else:
+            # 修复PYTHON 3.11版本报错：LookupError: unknown encoding: locale
+            self.encoding = 'utf-8' if self.encoding == 'locale' else self.encoding
             stream = codecs.open(self.current_file_name,
                                  self.mode, self.encoding)
         return stream
 
     def acquire(self):
         self.lock_file.acquire()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk/utils.py` & `intelab_python_sdk-0.7.4/intelab_python_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/intelab_python_sdk.egg-info/SOURCES.txt` & `intelab_python_sdk-0.7.4/intelab_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intelab_python_sdk-0.7.3/setup.py` & `intelab_python_sdk-0.7.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 
 with open('README.rst', 'r', 'utf-8') as f:
     readme = f.read()
 
 setup(
     name='intelab_python_sdk',
-    version='0.7.3',
+    version='0.7.4',
     url='https://github.com/zwwangoo/intelab-python-sdk',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='zwwangoo',
     author_email='w_angzhiwen@163.com',
     packages=find_packages(exclude=('tests', 'tests.*')),
     zip_safe=False,
     include_package_data=True,
     python_requires='>=3.5',
     classifiers=[
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.11',
     ],
     entry_points={
         'console_scripts': [
             'intelab_python_sdk = intelab_python_sdk.helper.cpu:run_print'
         ]
     }
```

