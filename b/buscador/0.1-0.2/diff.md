# Comparing `tmp/buscador-0.1.tar.gz` & `tmp/buscador-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.1.tar", last modified: Wed Jul 19 21:15:57 2023, max compression
+gzip compressed data, was "buscador-0.2.tar", last modified: Thu Jul 20 13:34:21 2023, max compression
```

## Comparing `buscador-0.1.tar` & `buscador-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-19 21:15:57.584357 buscador-0.1/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.1/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      587 2023-07-19 21:15:57.584693 buscador-0.1/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      370 2023-07-19 21:10:54.000000 buscador-0.1/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-19 21:15:57.579106 buscador-0.1/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.1/buscador/__init__.py
--rw-r--r--   0 samcook    (501) staff       (20)      450 2023-07-19 20:53:58.000000 buscador-0.1/buscador/classFindValue.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-19 21:15:57.583752 buscador-0.1/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      587 2023-07-19 21:15:57.000000 buscador-0.1/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-19 21:15:57.000000 buscador-0.1/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-19 21:15:57.000000 buscador-0.1/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       23 2023-07-19 21:15:57.000000 buscador-0.1/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-19 21:15:57.000000 buscador-0.1/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-19 21:15:57.585509 buscador-0.1/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)      969 2023-07-19 21:12:12.000000 buscador-0.1/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.533546 buscador-0.2/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.2/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:34:21.533777 buscador-0.2/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      696 2023-07-20 13:25:10.000000 buscador-0.2/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.528159 buscador-0.2/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.2/buscador/__init__.py
+-rw-r--r--   0 samcook    (501) staff       (20)      450 2023-07-19 20:53:58.000000 buscador-0.2/buscador/classFindValue.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.532905 buscador-0.2/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       23 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 13:34:21.534563 buscador-0.2/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)     1053 2023-07-20 13:33:23.000000 buscador-0.2/setup.py
```

### Comparing `buscador-0.1/LICENSE.txt` & `buscador-0.2/LICENSE.txt`

 * *Files identical despite different names*

