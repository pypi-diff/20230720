# Comparing `tmp/tortoise_api_model-0.0.1.tar.gz` & `tmp/tortoise_api_model-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.0.1.tar", last modified: Thu Jul 20 18:14:57 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.0.2.tar", last modified: Thu Jul 20 18:30:17 2023, max compression
```

## Comparing `tortoise_api_model-0.0.1.tar` & `tortoise_api_model-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:14:57.222445 tortoise_api_model-0.0.1/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-20 18:14:57.222272 tortoise_api_model-0.0.1/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:14:57.222492 tortoise_api_model-0.0.1/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-20 18:09:21.000000 tortoise_api_model-0.0.1/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:14:57.221032 tortoise_api_model-0.0.1/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       24 2023-07-20 18:11:48.000000 tortoise_api_model-0.0.1/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)      232 2023-07-20 17:58:24.000000 tortoise_api_model-0.0.1/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:14:57.221994 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-20 18:14:57.000000 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-20 18:14:57.000000 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:14:57.000000 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 18:14:57.000000 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 18:14:57.000000 tortoise_api_model-0.0.1/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:30:17.554339 tortoise_api_model-0.0.2/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-20 18:30:17.554120 tortoise_api_model-0.0.2/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:30:17.554402 tortoise_api_model-0.0.2/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-20 18:30:08.000000 tortoise_api_model-0.0.2/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:30:17.551787 tortoise_api_model-0.0.2/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)       25 2023-07-20 18:29:19.000000 tortoise_api_model-0.0.2/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)      232 2023-07-20 17:58:24.000000 tortoise_api_model-0.0.2/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:30:17.553762 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-20 18:30:17.000000 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-20 18:30:17.000000 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:30:17.000000 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 18:30:17.000000 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 18:30:17.000000 tortoise_api_model-0.0.2/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.0.1/setup.py` & `tortoise_api_model-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

