# Comparing `tmp/streamlit_clickable_card-0.0.3.tar.gz` & `tmp/streamlit_clickable_card-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_clickable_card-0.0.3.tar", last modified: Thu Jul 20 18:53:06 2023, max compression
+gzip compressed data, was "streamlit_clickable_card-0.0.4.tar", last modified: Thu Jul 20 19:00:04 2023, max compression
```

## Comparing `streamlit_clickable_card-0.0.3.tar` & `streamlit_clickable_card-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.983309 streamlit_clickable_card-0.0.3/
--rw-r--r--   0 hbrown     (501) staff       (20)     1063 2023-07-11 17:26:51.000000 streamlit_clickable_card-0.0.3/LICENSE
--rw-r--r--   0 hbrown     (501) staff       (20)       50 2023-07-12 17:55:42.000000 streamlit_clickable_card-0.0.3/MANIFEST.in
--rw-r--r--   0 hbrown     (501) staff       (20)      297 2023-07-20 18:53:06.983110 streamlit_clickable_card-0.0.3/PKG-INFO
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.978229 streamlit_clickable_card-0.0.3/clickable_card/
--rw-r--r--   0 hbrown     (501) staff       (20)     5105 2023-07-20 18:31:26.000000 streamlit_clickable_card-0.0.3/clickable_card/__init__.py
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.976398 streamlit_clickable_card-0.0.3/clickable_card/frontend/
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.979287 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/
--rw-r--r--   0 hbrown     (501) staff       (20)      221 2023-07-20 18:52:19.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/asset-manifest.json
--rw-r--r--   0 hbrown     (501) staff       (20)   197459 2023-07-20 18:52:15.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/bootstrap.min.css
--rw-r--r--   0 hbrown     (501) staff       (20)      492 2023-07-20 18:52:19.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/index.html
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.976724 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.980461 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/
--rw-r--r--   0 hbrown     (501) staff       (20)   379839 2023-07-20 18:52:19.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js
--rw-r--r--   0 hbrown     (501) staff       (20)     1443 2023-07-20 18:52:19.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js.LICENSE.txt
--rw-r--r--   0 hbrown     (501) staff       (20)  1355487 2023-07-20 18:52:19.000000 streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js.map
--rw-r--r--   0 hbrown     (501) staff       (20)       38 2023-07-20 18:53:06.983368 streamlit_clickable_card-0.0.3/setup.cfg
--rw-r--r--   0 hbrown     (501) staff       (20)      625 2023-07-20 17:40:46.000000 streamlit_clickable_card-0.0.3/setup.py
-drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 18:53:06.982825 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/
--rw-r--r--   0 hbrown     (501) staff       (20)      297 2023-07-20 18:53:06.000000 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/PKG-INFO
--rw-r--r--   0 hbrown     (501) staff       (20)      620 2023-07-20 18:53:06.000000 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/SOURCES.txt
--rw-r--r--   0 hbrown     (501) staff       (20)        1 2023-07-20 18:53:06.000000 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/dependency_links.txt
--rw-r--r--   0 hbrown     (501) staff       (20)       16 2023-07-20 18:53:06.000000 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/requires.txt
--rw-r--r--   0 hbrown     (501) staff       (20)       15 2023-07-20 18:53:06.000000 streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/top_level.txt
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.375418 streamlit_clickable_card-0.0.4/
+-rw-r--r--   0 hbrown     (501) staff       (20)     1063 2023-07-11 17:26:51.000000 streamlit_clickable_card-0.0.4/LICENSE
+-rw-r--r--   0 hbrown     (501) staff       (20)       50 2023-07-12 17:55:42.000000 streamlit_clickable_card-0.0.4/MANIFEST.in
+-rw-r--r--   0 hbrown     (501) staff       (20)      297 2023-07-20 19:00:04.375211 streamlit_clickable_card-0.0.4/PKG-INFO
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.370369 streamlit_clickable_card-0.0.4/clickable_card/
+-rw-r--r--   0 hbrown     (501) staff       (20)     5104 2023-07-20 18:57:03.000000 streamlit_clickable_card-0.0.4/clickable_card/__init__.py
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.368434 streamlit_clickable_card-0.0.4/clickable_card/frontend/
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.371498 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/
+-rw-r--r--   0 hbrown     (501) staff       (20)      221 2023-07-20 18:59:45.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/asset-manifest.json
+-rw-r--r--   0 hbrown     (501) staff       (20)   197459 2023-07-20 18:59:42.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/bootstrap.min.css
+-rw-r--r--   0 hbrown     (501) staff       (20)      492 2023-07-20 18:59:45.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/index.html
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.368811 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.372680 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/
+-rw-r--r--   0 hbrown     (501) staff       (20)   379839 2023-07-20 18:59:45.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js
+-rw-r--r--   0 hbrown     (501) staff       (20)     1443 2023-07-20 18:59:45.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js.LICENSE.txt
+-rw-r--r--   0 hbrown     (501) staff       (20)  1355487 2023-07-20 18:59:45.000000 streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js.map
+-rw-r--r--   0 hbrown     (501) staff       (20)       38 2023-07-20 19:00:04.375477 streamlit_clickable_card-0.0.4/setup.cfg
+-rw-r--r--   0 hbrown     (501) staff       (20)      625 2023-07-20 18:59:20.000000 streamlit_clickable_card-0.0.4/setup.py
+drwxr-xr-x   0 hbrown     (501) staff       (20)        0 2023-07-20 19:00:04.374921 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/
+-rw-r--r--   0 hbrown     (501) staff       (20)      297 2023-07-20 19:00:03.000000 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/PKG-INFO
+-rw-r--r--   0 hbrown     (501) staff       (20)      620 2023-07-20 19:00:04.000000 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/SOURCES.txt
+-rw-r--r--   0 hbrown     (501) staff       (20)        1 2023-07-20 19:00:03.000000 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/dependency_links.txt
+-rw-r--r--   0 hbrown     (501) staff       (20)       16 2023-07-20 19:00:04.000000 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/requires.txt
+-rw-r--r--   0 hbrown     (501) staff       (20)       15 2023-07-20 19:00:04.000000 streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/top_level.txt
```

### Comparing `streamlit_clickable_card-0.0.3/LICENSE` & `streamlit_clickable_card-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_clickable_card-0.0.3/clickable_card/__init__.py` & `streamlit_clickable_card-0.0.4/clickable_card/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import streamlit.components.v1 as components
 import base64
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `streamlit_clickable_card-0.0.3/clickable_card/frontend/build/bootstrap.min.css` & `streamlit_clickable_card-0.0.4/clickable_card/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js` & `streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js`

 * *Files identical despite different names*

### Comparing `streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js.LICENSE.txt` & `streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_clickable_card-0.0.3/clickable_card/frontend/build/static/js/main.c978769c.js.map` & `streamlit_clickable_card-0.0.4/clickable_card/frontend/build/static/js/main.c978769c.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_clickable_card-0.0.3/setup.py` & `streamlit_clickable_card-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_clickable_card",
-    version="0.0.3",
+    version="0.0.4",
     author="Hartland Brown",
     author_email="hartland.brown@snowflake.com",
     description="Clickable Card",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_clickable_card-0.0.3/streamlit_clickable_card.egg-info/SOURCES.txt` & `streamlit_clickable_card-0.0.4/streamlit_clickable_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

