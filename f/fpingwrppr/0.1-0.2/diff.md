# Comparing `tmp/fpingwrppr-0.1.tar.gz` & `tmp/fpingwrppr-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpingwrppr-0.1.tar", last modified: Thu Jul 20 18:19:31 2023, max compression
+gzip compressed data, was "fpingwrppr-0.2.tar", last modified: Thu Jul 20 18:25:15 2023, max compression
```

## Comparing `fpingwrppr-0.1.tar` & `fpingwrppr-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:19:31.714362 fpingwrppr-0.1/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:19:31.714362 fpingwrppr-0.1/PKG-INFO
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:19:31.714362 fpingwrppr-0.1/fping/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      720 2023-07-20 18:14:53.000000 fpingwrppr-0.1/fping/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:19:31.714362 fpingwrppr-0.1/fping/backends/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.1/fping/backends/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.1/fping/backends/base.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1340 2023-07-20 18:11:20.000000 fpingwrppr-0.1/fping/backends/fping.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.1/fping/backends/util.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:19:31.714362 fpingwrppr-0.1/fpingwrppr.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:19:31.000000 fpingwrppr-0.1/fpingwrppr.egg-info/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      340 2023-07-20 18:19:31.000000 fpingwrppr-0.1/fpingwrppr.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:19:31.000000 fpingwrppr-0.1/fpingwrppr.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:19:31.000000 fpingwrppr-0.1/fpingwrppr.egg-info/top_level.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:19:31.000000 fpingwrppr-0.1/fpingwrppr.egg-info/zip-safe
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:19:31.714362 fpingwrppr-0.1/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:19:28.000000 fpingwrppr-0.1/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:19:31.714362 fpingwrppr-0.1/tests/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.1/tests/test_backends.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.1/tests/test_base.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:25:15.265693 fpingwrppr-0.2/PKG-INFO
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fping/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      720 2023-07-20 18:14:53.000000 fpingwrppr-0.2/fping/__init__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fping/backends/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1375 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/base.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1368 2023-07-20 18:24:27.000000 fpingwrppr-0.2/fping/backends/fping.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       86 2023-07-20 17:31:11.000000 fpingwrppr-0.2/fping/backends/util.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/fpingwrppr.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      340 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/top_level.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 18:25:15.000000 fpingwrppr-0.2/fpingwrppr.egg-info/zip-safe
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 18:25:15.265693 fpingwrppr-0.2/setup.cfg
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 18:25:11.000000 fpingwrppr-0.2/setup.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 18:25:15.265693 fpingwrppr-0.2/tests/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.2/tests/test_backends.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.2/tests/test_base.py
```

### Comparing `fpingwrppr-0.1/fping/__init__.py` & `fpingwrppr-0.2/fping/__init__.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.1/fping/backends/base.py` & `fpingwrppr-0.2/fping/backends/base.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.1/fping/backends/fping.py` & `fpingwrppr-0.2/fping/backends/fping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-import os
-import tempfile
-import subprocess
+import subprocess, os
 from fping.backends.base import BasePinger
 from fping.backends.util import os_wait
 
-
 class FpingPinger(BasePinger):
     program = "fping"
     help_return_code = 3
 
     def ping_many_updown_iter(self, hosts, fast=False):
-        """Ping a list of ips, return an iterator of state, node"""
+        """Ping a list of IPs, return an iterator of state, node"""
         cmd = [self.program_path]
         if fast:
             cmd.extend(["-r", "1", "-t", "100"])
 
-        sub = subprocess.Popen(cmd, shell=False, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, close_fds=True)
-        for ip in hosts:
-            sub.stdin.write("%s\n" % ip)
-        sub.stdin.close()
-
-        up=[]
-        down=[]
-        for line in sub.stdout:
-            line=line.strip()
-            ip = line.split(" ",1)[0]
-            if "is alive" in line:
-                yield 'up', ip
-            elif "is unreachable" in line:
-                yield 'down', ip
-            
-        sub.stdout.close()
+        with subprocess.Popen(cmd, shell=False, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, close_fds=True) as sub:
+            for ip in hosts:
+                sub.stdin.write(f"{ip}\n")
+            sub.stdin.close()
+
+            up = []
+            down = []
+            for line in sub.stdout:
+                line = line.strip()
+                ip, _, status = line.partition(" ")
+                if status == "is alive":
+                    yield 'up', ip
+                elif status == "is unreachable":
+                    yield 'down', ip
+
         os_wait()
 
     def ping_many_updown(self, hosts, fast=False):
-        """Ping a list of ips, return a tuple of (up nodes, down nodes)"""
-        up=[]
-        down=[]
-        lists = dict(up=up,down=down)
+        """Ping a list of IPs, return a tuple of (up nodes, down nodes)"""
+        up = []
+        down = []
+        lists = dict(up=up, down=down)
         for state, ip in self.ping_many_updown_iter(hosts, fast):
             lists[state].append(ip)
         return up, down
 
+
 pinger_class = FpingPinger
```

### Comparing `fpingwrppr-0.1/setup.py` & `fpingwrppr-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.1'
+version = '0.2'
 
 setup(name='fpingwrppr',
       version=version,
       description="Fping Wrapper",
       long_description="""\
 """,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `fpingwrppr-0.1/tests/test_backends.py` & `fpingwrppr-0.2/tests/test_backends.py`

 * *Files identical despite different names*

