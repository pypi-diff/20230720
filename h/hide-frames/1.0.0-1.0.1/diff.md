# Comparing `tmp/hide_frames-1.0.0.tar.gz` & `tmp/hide_frames-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hide_frames-1.0.0.tar", last modified: Thu Jul 20 13:43:47 2023, max compression
+gzip compressed data, was "hide_frames-1.0.1.tar", last modified: Thu Jul 20 13:56:43 2023, max compression
```

## Comparing `hide_frames-1.0.0.tar` & `hide_frames-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 13:43:47.101313 hide_frames-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-06-13 05:21:40.000000 hide_frames-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    43243 2023-07-20 13:43:47.097535 hide_frames-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2023-07-20 13:41:14.000000 hide_frames-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 13:43:47.092903 hide_frames-1.0.0/hide_frames.egg-info/
--rw-rw-rw-   0        0        0    43243 2023-07-20 13:43:46.000000 hide_frames-1.0.0/hide_frames.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-20 13:43:46.000000 hide_frames-1.0.0/hide_frames.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 13:43:46.000000 hide_frames-1.0.0/hide_frames.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 13:43:46.000000 hide_frames-1.0.0/hide_frames.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      510 2023-07-20 13:11:49.000000 hide_frames-1.0.0/hide_frames.py
--rw-rw-rw-   0        0        0      473 2023-07-20 13:41:40.000000 hide_frames-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 13:43:47.102295 hide_frames-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 13:56:43.990595 hide_frames-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-13 05:21:40.000000 hide_frames-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    43262 2023-07-20 13:56:43.988503 hide_frames-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2023-07-20 13:41:14.000000 hide_frames-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 13:56:43.982936 hide_frames-1.0.1/hide_frames.egg-info/
+-rw-rw-rw-   0        0        0    43262 2023-07-20 13:56:43.000000 hide_frames-1.0.1/hide_frames.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-20 13:56:43.000000 hide_frames-1.0.1/hide_frames.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:56:43.000000 hide_frames-1.0.1/hide_frames.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 13:56:43.000000 hide_frames-1.0.1/hide_frames.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      560 2023-07-20 13:52:28.000000 hide_frames-1.0.1/hide_frames.py
+-rw-rw-rw-   0        0        0      492 2023-07-20 13:55:28.000000 hide_frames-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 13:56:43.990595 hide_frames-1.0.1/setup.cfg
```

### Comparing `hide_frames-1.0.0/LICENSE` & `hide_frames-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hide_frames-1.0.0/PKG-INFO` & `hide_frames-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hide_frames
-Version: 1.0.0
-Summary: Hide ugly frames in your wrappers
+Version: 1.0.1
+Summary: Hide your ugly wrapper frames: func(*args, **kwargs)
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `hide_frames-1.0.0/README.md` & `hide_frames-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hide_frames-1.0.0/hide_frames.egg-info/PKG-INFO` & `hide_frames-1.0.1/hide_frames.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hide-frames
-Version: 1.0.0
-Summary: Hide ugly frames in your wrappers
+Version: 1.0.1
+Summary: Hide your ugly wrapper frames: func(*args, **kwargs)
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

