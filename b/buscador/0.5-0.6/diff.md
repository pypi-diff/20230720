# Comparing `tmp/buscador-0.5.tar.gz` & `tmp/buscador-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.5.tar", last modified: Thu Jul 20 13:51:12 2023, max compression
+gzip compressed data, was "buscador-0.6.tar", last modified: Thu Jul 20 14:41:39 2023, max compression
```

## Comparing `buscador-0.5.tar` & `buscador-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:51:12.767804 buscador-0.5/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.5/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:51:12.768006 buscador-0.5/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      697 2023-07-20 13:47:30.000000 buscador-0.5/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:51:12.763746 buscador-0.5/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.5/buscador/__init__.py
--rw-r--r--   0 samcook    (501) staff       (20)      450 2023-07-19 20:53:58.000000 buscador-0.5/buscador/classFindValue.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:51:12.767323 buscador-0.5/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:51:12.000000 buscador-0.5/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 13:51:12.000000 buscador-0.5/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 13:51:12.000000 buscador-0.5/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       13 2023-07-20 13:51:12.000000 buscador-0.5/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 13:51:12.000000 buscador-0.5/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 13:51:12.768703 buscador-0.5/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)     1018 2023-07-20 13:51:08.000000 buscador-0.5/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.845123 buscador-0.6/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.6/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 14:41:39.845371 buscador-0.6/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      697 2023-07-20 13:47:30.000000 buscador-0.6/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.841645 buscador-0.6/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.6/buscador/__init__.py
+-rw-r--r--   0 samcook    (501) staff       (20)      485 2023-07-20 14:41:31.000000 buscador-0.6/buscador/classFindValue.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.844658 buscador-0.6/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       13 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 14:41:39.845971 buscador-0.6/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)      964 2023-07-20 14:41:31.000000 buscador-0.6/setup.py
```

### Comparing `buscador-0.5/LICENSE.txt` & `buscador-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buscador-0.5/PKG-INFO` & `buscador-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.5
+Version: 0.6
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.5.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.6.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.5/README.md` & `buscador-0.6/README.md`

 * *Files identical despite different names*

### Comparing `buscador-0.5/buscador.egg-info/PKG-INFO` & `buscador-0.6/buscador.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.5
+Version: 0.6
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.5.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.6.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

