# Comparing `tmp/MediaLib-3.0.1.8.tar.gz` & `tmp/MediaLib-3.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MediaLib-3.0.1.8.tar", last modified: Thu Jul 20 14:24:28 2023, max compression
+gzip compressed data, was "MediaLib-3.0.1.9.tar", last modified: Thu Jul 20 14:30:54 2023, max compression
```

## Comparing `MediaLib-3.0.1.8.tar` & `MediaLib-3.0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:24:28.862409 MediaLib-3.0.1.8/
--rw-r--r--   0 adamwynn   (501) staff       (20)      292 2023-07-20 14:24:28.862470 MediaLib-3.0.1.8/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.8/README.rst
--rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-07-20 14:24:28.862670 MediaLib-3.0.1.8/setup.cfg
--rw-r--r--   0 adamwynn   (501) staff       (20)      465 2023-07-20 14:24:13.000000 MediaLib-3.0.1.8/setup.py
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:24:28.860734 MediaLib-3.0.1.8/src/
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:24:28.861787 MediaLib-3.0.1.8/src/MediaLib.egg-info/
--rw-r--r--   0 adamwynn   (501) staff       (20)      292 2023-07-20 14:24:28.000000 MediaLib-3.0.1.8/src/MediaLib.egg-info/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)      258 2023-07-20 14:24:28.000000 MediaLib-3.0.1.8/src/MediaLib.egg-info/SOURCES.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-07-20 14:24:28.000000 MediaLib-3.0.1.8/src/MediaLib.egg-info/dependency_links.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-07-20 14:24:28.000000 MediaLib-3.0.1.8/src/MediaLib.egg-info/requires.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        9 2023-07-20 14:24:28.000000 MediaLib-3.0.1.8/src/MediaLib.egg-info/top_level.txt
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:24:28.862157 MediaLib-3.0.1.8/src/medialib/
--rw-r--r--   0 adamwynn   (501) staff       (20)       23 2023-05-02 15:49:43.000000 MediaLib-3.0.1.8/src/medialib/__init__.py
--rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.8/src/medialib/medialib.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:30:54.225313 MediaLib-3.0.1.9/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      357 2023-07-20 14:30:54.225363 MediaLib-3.0.1.9/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.9/README.rst
+-rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-07-20 14:30:54.225549 MediaLib-3.0.1.9/setup.cfg
+-rw-r--r--   0 adamwynn   (501) staff       (20)      557 2023-07-20 14:30:49.000000 MediaLib-3.0.1.9/setup.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:30:54.223771 MediaLib-3.0.1.9/src/
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:30:54.224770 MediaLib-3.0.1.9/src/MediaLib.egg-info/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      357 2023-07-20 14:30:54.000000 MediaLib-3.0.1.9/src/MediaLib.egg-info/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)      258 2023-07-20 14:30:54.000000 MediaLib-3.0.1.9/src/MediaLib.egg-info/SOURCES.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-07-20 14:30:54.000000 MediaLib-3.0.1.9/src/MediaLib.egg-info/dependency_links.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-07-20 14:30:54.000000 MediaLib-3.0.1.9/src/MediaLib.egg-info/requires.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        9 2023-07-20 14:30:54.000000 MediaLib-3.0.1.9/src/MediaLib.egg-info/top_level.txt
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-07-20 14:30:54.225092 MediaLib-3.0.1.9/src/medialib/
+-rw-r--r--   0 adamwynn   (501) staff       (20)       23 2023-05-02 15:49:43.000000 MediaLib-3.0.1.9/src/medialib/__init__.py
+-rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.9/src/medialib/medialib.py
```

### Comparing `MediaLib-3.0.1.8/src/medialib/medialib.py` & `MediaLib-3.0.1.9/src/medialib/medialib.py`

 * *Files identical despite different names*

