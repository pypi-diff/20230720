# Comparing `tmp/fusion-engine-0.2.3.1.tar.gz` & `tmp/fusion-engine-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.2.3.1.tar", last modified: Thu Jul 20 12:20:59 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.4.tar", last modified: Thu Jul 20 12:22:11 2023, max compression
```

## Comparing `fusion-engine-0.2.3.1.tar` & `fusion-engine-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:20:59.082911 fusion-engine-0.2.3.1/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.3.1/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5101 2023-07-20 12:20:59.082140 fusion-engine-0.2.3.1/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3856 2023-07-20 10:41:07.000000 fusion-engine-0.2.3.1/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1673 2023-07-20 12:19:42.000000 fusion-engine-0.2.3.1/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.3.1/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-20 12:20:59.083160 fusion-engine-0.2.3.1/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-12 18:18:50.000000 fusion-engine-0.2.3.1/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:20:59.049229 fusion-engine-0.2.3.1/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:20:59.059873 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5101 2023-07-20 12:20:59.000000 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      846 2023-07-20 12:20:59.000000 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-20 12:20:59.000000 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-20 12:20:59.000000 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-20 12:20:59.000000 fusion-engine-0.2.3.1/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:20:59.061149 fusion-engine-0.2.3.1/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      896 2023-07-20 12:20:53.000000 fusion-engine-0.2.3.1/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:20:59.080748 fusion-engine-0.2.3.1/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3439 2023-07-10 21:29:12.000000 fusion-engine-0.2.3.1/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1372 2023-07-14 21:16:17.000000 fusion-engine-0.2.3.1/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.3.1/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      105 2023-07-20 10:28:33.000000 fusion-engine-0.2.3.1/src/fusionengine/files/debug.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2409 2023-07-09 21:02:50.000000 fusion-engine-0.2.3.1/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-16 22:38:57.000000 fusion-engine-0.2.3.1/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.3.1/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.3.1/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      113 2023-07-16 22:46:12.000000 fusion-engine-0.2.3.1/src/fusionengine/files/fonts.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      904 2023-07-09 20:56:06.000000 fusion-engine-0.2.3.1/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.3.1/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.3.1/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.3.1/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.3.1/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.3.1/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3234 2023-07-19 08:46:10.000000 fusion-engine-0.2.3.1/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1867 2023-07-14 21:27:23.000000 fusion-engine-0.2.3.1/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.505118 fusion-engine-0.2.4/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.4/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5099 2023-07-20 12:22:11.503915 fusion-engine-0.2.4/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3856 2023-07-20 10:41:07.000000 fusion-engine-0.2.4/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1647 2023-07-20 12:21:59.000000 fusion-engine-0.2.4/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.4/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-20 12:22:11.505366 fusion-engine-0.2.4/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-12 18:18:50.000000 fusion-engine-0.2.4/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.465794 fusion-engine-0.2.4/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.474852 fusion-engine-0.2.4/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5099 2023-07-20 12:22:11.000000 fusion-engine-0.2.4/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      881 2023-07-20 12:22:11.000000 fusion-engine-0.2.4/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-20 12:22:11.000000 fusion-engine-0.2.4/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-20 12:22:11.000000 fusion-engine-0.2.4/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-20 12:22:11.000000 fusion-engine-0.2.4/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.475921 fusion-engine-0.2.4/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      894 2023-07-20 12:21:48.000000 fusion-engine-0.2.4/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.477067 fusion-engine-0.2.4/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.4/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-20 12:22:11.501858 fusion-engine-0.2.4/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3439 2023-07-10 21:29:12.000000 fusion-engine-0.2.4/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1372 2023-07-14 21:16:17.000000 fusion-engine-0.2.4/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.4/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      105 2023-07-20 10:28:33.000000 fusion-engine-0.2.4/src/fusionengine/files/debug.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2409 2023-07-09 21:02:50.000000 fusion-engine-0.2.4/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-16 22:38:57.000000 fusion-engine-0.2.4/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.4/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.4/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      113 2023-07-16 22:46:12.000000 fusion-engine-0.2.4/src/fusionengine/files/fonts.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      904 2023-07-09 20:56:06.000000 fusion-engine-0.2.4/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.4/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.4/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.4/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.4/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.4/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3234 2023-07-19 08:46:10.000000 fusion-engine-0.2.4/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1867 2023-07-14 21:27:23.000000 fusion-engine-0.2.4/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.3.1/LICENCE.md` & `fusion-engine-0.2.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/PKG-INFO` & `fusion-engine-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.3.1
+Version: 0.2.4
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.2.3.1/README.md` & `fusion-engine-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/pyproject.toml` & `fusion-engine-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,12 +34,12 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "fusionengine.__version__"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools.package-data]
-fusionengine = ["src/fusionengine/debugfiles/fe.png"]
+fusionengine = ["**/*.png"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 exclude = ["old_gui"]
```

### Comparing `fusion-engine-0.2.3.1/setup.py` & `fusion-engine-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.4/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.3.1
+Version: 0.2.4
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.2.3.1/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.4/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 src/fusion_engine.egg-info/PKG-INFO
 src/fusion_engine.egg-info/SOURCES.txt
 src/fusion_engine.egg-info/dependency_links.txt
 src/fusion_engine.egg-info/requires.txt
 src/fusion_engine.egg-info/top_level.txt
 src/fusionengine/__init__.py
+src/fusionengine/debugfiles/fe.png
 src/fusionengine/files/body.py
 src/fusionengine/files/color.py
 src/fusionengine/files/data.py
 src/fusionengine/files/debug.py
 src/fusionengine/files/draw.py
 src/fusionengine/files/enums.py
 src/fusionengine/files/event.py
```

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/__init__.py` & `fusion-engine-0.2.4/src/fusionengine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Dimkauzh"
-__version__ = "0.2.3.1"
+__version__ = "0.2.4"
 
 import fusionengine.files.data as data
 import fusionengine.files.systems as sysconfig
 
 from fusionengine.files.imports import *
 
 class Main:
```

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/body.py` & `fusion-engine-0.2.4/src/fusionengine/files/body.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/color.py` & `fusion-engine-0.2.4/src/fusionengine/files/color.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/draw.py` & `fusion-engine-0.2.4/src/fusionengine/files/draw.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/event.py` & `fusion-engine-0.2.4/src/fusionengine/files/event.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/image.py` & `fusion-engine-0.2.4/src/fusionengine/files/image.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/imports.py` & `fusion-engine-0.2.4/src/fusionengine/files/imports.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/shape.py` & `fusion-engine-0.2.4/src/fusionengine/files/shape.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/storage.py` & `fusion-engine-0.2.4/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/systems.py` & `fusion-engine-0.2.4/src/fusionengine/files/systems.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/ui.py` & `fusion-engine-0.2.4/src/fusionengine/files/ui.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.3.1/src/fusionengine/files/window.py` & `fusion-engine-0.2.4/src/fusionengine/files/window.py`

 * *Files identical despite different names*

