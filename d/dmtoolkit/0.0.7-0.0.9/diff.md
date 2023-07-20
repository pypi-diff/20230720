# Comparing `tmp/dmtoolkit-0.0.7.tar.gz` & `tmp/dmtoolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolkit-0.0.7.tar", last modified: Tue Jul 18 15:53:30 2023, max compression
+gzip compressed data, was "dmtoolkit-0.0.9.tar", last modified: Tue Jul 18 17:27:13 2023, max compression
```

## Comparing `dmtoolkit-0.0.7.tar` & `dmtoolkit-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.877596 dmtoolkit-0.0.7/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.7/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 15:53:30.876596 dmtoolkit-0.0.7/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.7/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.7/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.7/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-18 15:53:30.877596 dmtoolkit-0.0.7/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.7/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.864596 dmtoolkit-0.0.7/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.869596 dmtoolkit-0.0.7/src/dmtoolkit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-18 15:53:15.000000 dmtoolkit-0.0.7/src/dmtoolkit/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.872596 dmtoolkit-0.0.7/src/dmtoolkit/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      176 2023-07-13 19:03:53.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/dndbeyondapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/foundryapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     6051 2023-07-18 15:47:28.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/open5eapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/wikijsapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.7/src/dmtoolkit/dmtools.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.875596 dmtoolkit-0.0.7/src/dmtoolkit/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1794 2023-07-18 14:56:37.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndcharacter.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      927 2023-07-18 15:06:01.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dnditem.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1803 2023-07-18 15:05:51.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndmonster.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1421 2023-07-18 15:26:03.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndobject.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndshop.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1030 2023-07-18 15:05:41.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndspell.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.871596 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.272178 dmtoolkit-0.0.9/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.9/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 17:27:13.271178 dmtoolkit-0.0.9/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.9/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.9/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.9/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-18 17:27:13.272178 dmtoolkit-0.0.9/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.9/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.261178 dmtoolkit-0.0.9/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.264178 dmtoolkit-0.0.9/src/dmtoolkit/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-18 17:26:54.000000 dmtoolkit-0.0.9/src/dmtoolkit/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.267178 dmtoolkit-0.0.9/src/dmtoolkit/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      176 2023-07-13 19:03:53.000000 dmtoolkit-0.0.9/src/dmtoolkit/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.9/src/dmtoolkit/apis/dndbeyondapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.9/src/dmtoolkit/apis/foundryapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     6051 2023-07-18 15:47:28.000000 dmtoolkit-0.0.9/src/dmtoolkit/apis/open5eapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.9/src/dmtoolkit/apis/wikijsapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.9/src/dmtoolkit/dmtools.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.270178 dmtoolkit-0.0.9/src/dmtoolkit/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1794 2023-07-18 14:56:37.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dndcharacter.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      927 2023-07-18 15:06:01.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dnditem.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1803 2023-07-18 15:05:51.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dndmonster.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1544 2023-07-18 17:07:19.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dndobject.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dndshop.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1030 2023-07-18 15:05:41.000000 dmtoolkit-0.0.9/src/dmtoolkit/models/dndspell.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 17:27:13.265178 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 17:27:13.000000 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-18 17:27:13.000000 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-18 17:27:13.000000 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-18 17:27:13.000000 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-18 17:27:13.000000 dmtoolkit-0.0.9/src/dmtoolkit.egg-info/top_level.txt
```

### Comparing `dmtoolkit-0.0.7/LICENSE` & `dmtoolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/PKG-INFO` & `dmtoolkit-0.0.9/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.7
+Version: 0.0.9
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.7/README.md` & `dmtoolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/pyproject.toml` & `dmtoolkit-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/setup.py` & `dmtoolkit-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/apis/dndbeyondapi.py` & `dmtoolkit-0.0.9/src/dmtoolkit/apis/dndbeyondapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/apis/open5eapi.py` & `dmtoolkit-0.0.9/src/dmtoolkit/apis/open5eapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/apis/wikijsapi.py` & `dmtoolkit-0.0.9/src/dmtoolkit/apis/wikijsapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/dmtools.py` & `dmtoolkit-0.0.9/src/dmtoolkit/dmtools.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dndcharacter.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dndcharacter.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dnditem.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dnditem.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dndmonster.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dndmonster.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dndobject.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dndobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,22 @@
             self.image = self._storage.save(self.image["raw"], folder=folder)
         return super().save()
 
     @classmethod
     def search(cls, **kwargs):
         results = super().search(**kwargs)
         if cls.search_api:
-            names = {obj.name for obj in results}
+            names = [obj.name for obj in results]
             api_results = cls.search_api.search(list(kwargs.values()))
-            results = [obj for obj in api_results if obj["name"] not in names and cls(**obj).save()]
+            for obj in api_results:
+                if obj["name"] not in names:
+                    o = cls(**obj)
+                    o.save()
+                    results.append(o)
+                    names.append(o.name)
         return results
 
     def generate_image(self):
         resp = OpenAI().generate_image(
             self.get_image_prompt(),
             n=1,
         )
```

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dndshop.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dndshop.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit/models/dndspell.py` & `dmtoolkit-0.0.9/src/dmtoolkit/models/dndspell.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit.egg-info/PKG-INFO` & `dmtoolkit-0.0.9/src/dmtoolkit.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.7
+Version: 0.0.9
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.7/src/dmtoolkit.egg-info/SOURCES.txt` & `dmtoolkit-0.0.9/src/dmtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

