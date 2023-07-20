# Comparing `tmp/fpingwrppr-0.3.tar.gz` & `tmp/fpingwrppr-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpingwrppr-0.3.tar", last modified: Thu Jul 20 18:30:15 2023, max compression
+gzip compressed data, was "fpingwrppr-0.4.tar", last modified: Thu Jul 20 18:38:57 2023, max compression
```

## Comparing `fpingwrppr-0.3.tar` & `fpingwrppr-0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:30:15.265680 fpingwrppr-0.3/PKG-INFO
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fping/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      720 2023-07-20 18:29:31.000000 fpingwrppr-0.3/fping/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fping/backends/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/base.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1368 2023-07-20 18:24:27.000000 fpingwrppr-0.3/fping/backends/fping.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.3/fping/backends/util.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/fpingwrppr.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      340 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/top_level.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:30:15.000000 fpingwrppr-0.3/fpingwrppr.egg-info/zip-safe
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:30:15.265680 fpingwrppr-0.3/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:30:12.000000 fpingwrppr-0.3/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:30:15.265680 fpingwrppr-0.3/tests/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.3/tests/test_backends.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.3/tests/test_base.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:38:57.774050 fpingwrppr-0.4/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:38:57.774050 fpingwrppr-0.4/PKG-INFO
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:38:57.764050 fpingwrppr-0.4/fping/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1268 2023-07-20 18:38:11.000000 fpingwrppr-0.4/fping/__init__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:38:57.764050 fpingwrppr-0.4/fping/backends/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.4/fping/backends/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.4/fping/backends/base.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1368 2023-07-20 18:24:27.000000 fpingwrppr-0.4/fping/backends/fping.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1794 2023-07-20 18:37:52.000000 fpingwrppr-0.4/fping/backends/nmap.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      581 2023-07-20 18:37:26.000000 fpingwrppr-0.4/fping/backends/ping.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.4/fping/backends/util.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:38:57.774050 fpingwrppr-0.4/fpingwrppr.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:38:57.000000 fpingwrppr-0.4/fpingwrppr.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      386 2023-07-20 18:38:57.000000 fpingwrppr-0.4/fpingwrppr.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:38:57.000000 fpingwrppr-0.4/fpingwrppr.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:38:57.000000 fpingwrppr-0.4/fpingwrppr.egg-info/top_level.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:38:57.000000 fpingwrppr-0.4/fpingwrppr.egg-info/zip-safe
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:38:57.774050 fpingwrppr-0.4/setup.cfg
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:38:53.000000 fpingwrppr-0.4/setup.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:38:57.774050 fpingwrppr-0.4/tests/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.4/tests/test_backends.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.4/tests/test_base.py
```

### Comparing `fpingwrppr-0.3/fping/__init__.py` & `fpingwrppr-0.4/fping/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,31 @@
+from fping.backends import nmap
 from fping.backends import fping
+from fping.backends import ping
+
+backends = {
+    "nmap":   nmap.pinger_class,
+    "fping": fping.pinger_class,
+    "ping":   ping.pinger_class,
+}
+
+default_priority = ["fping", "nmap", "ping"]
+
+def get_backend(priority=None, **kwargs):
+    if not priority:
+        priority = default_priority
+
+    for name in priority:
+        b = backends.get(name)
+        if b:
+            inst = b(**kwargs)
+            if inst.is_available():
+                return inst
+
+    raise RuntimeError("No pinger backends Available")
 
 backends = {
     "fping": fping.pinger_class,
 }
 
 def get_backend(priority=["fping"], **kwargs):
     for name in priority:
```

### Comparing `fpingwrppr-0.3/fping/backends/base.py` & `fpingwrppr-0.4/fping/backends/base.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.3/fping/backends/fping.py` & `fpingwrppr-0.4/fping/backends/fping.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.3/setup.py` & `fpingwrppr-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.3'
+version = '0.4'
 
 setup(name='fpingwrppr',
       version=version,
       description="Fping Wrapper",
       long_description="""\
 """,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `fpingwrppr-0.3/tests/test_backends.py` & `fpingwrppr-0.4/tests/test_backends.py`

 * *Files identical despite different names*

