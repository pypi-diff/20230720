# Comparing `tmp/fpingwrppr-0.2.tar.gz` & `tmp/fpingwrppr-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpingwrppr-0.2.tar", last modified: Thu Jul 20 18:25:15 2023, max compression
+gzip compressed data, was "fpingwrppr-0.3.tar", last modified: Thu Jul 20 18:30:15 2023, max compression
```

## Comparing `fpingwrppr-0.2.tar` & `fpingwrppr-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:25:15.265693 fpingwrppr-0.2/PKG-INFO
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fping/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      720 2023-07-20 18:14:53.000000 fpingwrppr-0.2/fping/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fping/backends/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/base.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1368 2023-07-20 18:24:27.000000 fpingwrppr-0.2/fping/backends/fping.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/util.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fpingwrppr.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      340 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/top_level.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/zip-safe
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:25:15.265693 fpingwrppr-0.2/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:25:11.000000 fpingwrppr-0.2/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/tests/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.2/tests/test_backends.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.2/tests/test_base.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:30:15.265680 fpingwrppr-0.3/PKG-INFO
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fping/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      720 2023-07-20 18:29:31.000000 fpingwrppr-0.3/fping/__init__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fping/backends/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/base.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1368 2023-07-20 18:24:27.000000 fpingwrppr-0.3/fping/backends/fping.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/util.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fpingwrppr.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      340 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/top_level.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/zip-safe
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:30:15.265680 fpingwrppr-0.3/setup.cfg
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:30:12.000000 fpingwrppr-0.3/setup.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/tests/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.3/tests/test_backends.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.3/tests/test_base.py
```

### Comparing `fpingwrppr-0.2/fping/__init__.py` & `fpingwrppr-0.3/fping/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from fping.backends import fping
 
 backends = {
     "fping": fping.pinger_class,
 }
 
-def get_backend(priority="fping", **kwargs):
-
+def get_backend(priority=["fping"], **kwargs):
     for name in priority:
         b = backends.get(name)
         if b:
             inst = b(**kwargs)
             if inst.is_available():
                 return inst
 
-    #raise RuntimeError("No pinger backends Available")
+    raise RuntimeError("No pinger backends Available")
 
 def ping_one(host):
     return get_backend().ping_one(host)
 
 def ping_many_updown(hosts):
     return get_backend().ping_many_updown(hosts)
```

### Comparing `fpingwrppr-0.2/fping/backends/base.py` & `fpingwrppr-0.3/fping/backends/base.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.2/fping/backends/fping.py` & `fpingwrppr-0.3/fping/backends/fping.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.2/setup.py` & `fpingwrppr-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.2'
+version = '0.3'
 
 setup(name='fpingwrppr',
       version=version,
       description="Fping Wrapper",
       long_description="""\
 """,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `fpingwrppr-0.2/tests/test_backends.py` & `fpingwrppr-0.3/tests/test_backends.py`

 * *Files identical despite different names*

