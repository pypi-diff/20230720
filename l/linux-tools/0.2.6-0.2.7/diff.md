# Comparing `tmp/linux-tools-0.2.6.tar.gz` & `tmp/linux-tools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linux-tools-0.2.6.tar", last modified: Thu Jul 20 16:28:51 2023, max compression
+gzip compressed data, was "linux-tools-0.2.7.tar", last modified: Thu Jul 20 18:31:42 2023, max compression
```

## Comparing `linux-tools-0.2.6.tar` & `linux-tools-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/
--rw-r--r--   0 build     (1000) build     (1000)     1558 2023-07-20 16:28:24.000000 linux-tools-0.2.6/LICENSE
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 16:28:51.000521 linux-tools-0.2.6/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)    19849 2023-07-20 16:28:24.000000 linux-tools-0.2.6/README.md
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/linux_tools/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     3214 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/bits.py
--rw-r--r--   0 build     (1000) build     (1000)     8312 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/irqstat.py
--rw-r--r--   0 build     (1000) build     (1000)    11906 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/netgraph.py
--rw-r--r--   0 build     (1000) build     (1000)     1787 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/table.py
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/linux_tools.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)      341 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)      119 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)       12 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)      235 2023-07-20 16:28:24.000000 linux-tools-0.2.6/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1000)      352 2023-07-20 16:28:51.000521 linux-tools-0.2.6/setup.cfg
--rw-r--r--   0 build     (1000) build     (1000)      779 2023-07-20 16:28:24.000000 linux-tools-0.2.6/setup.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 18:31:42.937463 linux-tools-0.2.7/
+-rw-r--r--   0 build     (1000) build     (1000)     1558 2023-07-20 18:31:15.000000 linux-tools-0.2.7/LICENSE
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 18:31:42.937463 linux-tools-0.2.7/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)    19849 2023-07-20 18:31:15.000000 linux-tools-0.2.7/README.md
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 18:31:42.934118 linux-tools-0.2.7/linux_tools/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-20 18:31:15.000000 linux-tools-0.2.7/linux_tools/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     3214 2023-07-20 18:31:15.000000 linux-tools-0.2.7/linux_tools/bits.py
+-rw-r--r--   0 build     (1000) build     (1000)     8312 2023-07-20 18:31:15.000000 linux-tools-0.2.7/linux_tools/irqstat.py
+-rw-r--r--   0 build     (1000) build     (1000)    11968 2023-07-20 18:31:15.000000 linux-tools-0.2.7/linux_tools/netgraph.py
+-rw-r--r--   0 build     (1000) build     (1000)     1787 2023-07-20 18:31:15.000000 linux-tools-0.2.7/linux_tools/table.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 18:31:42.937463 linux-tools-0.2.7/linux_tools.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 18:31:42.000000 linux-tools-0.2.7/linux_tools.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)      341 2023-07-20 18:31:42.000000 linux-tools-0.2.7/linux_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-20 18:31:42.000000 linux-tools-0.2.7/linux_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)      119 2023-07-20 18:31:42.000000 linux-tools-0.2.7/linux_tools.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)       12 2023-07-20 18:31:42.000000 linux-tools-0.2.7/linux_tools.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)      235 2023-07-20 18:31:15.000000 linux-tools-0.2.7/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1000)      352 2023-07-20 18:31:42.937463 linux-tools-0.2.7/setup.cfg
+-rw-r--r--   0 build     (1000) build     (1000)      779 2023-07-20 18:31:15.000000 linux-tools-0.2.7/setup.py
```

### Comparing `linux-tools-0.2.6/LICENSE` & `linux-tools-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.6/PKG-INFO` & `linux-tools-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.6
+Version: 0.2.7
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.6/README.md` & `linux-tools-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.6/linux_tools/bits.py` & `linux-tools-0.2.7/linux_tools/bits.py`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.6/linux_tools/irqstat.py` & `linux-tools-0.2.7/linux_tools/irqstat.py`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.6/linux_tools/netgraph.py` & `linux-tools-0.2.7/linux_tools/netgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,18 @@
 
 
 def bridge(ns, *cmd):
     return iproute2_cmd("bridge", ns, *cmd)
 
 
 def get_nsids(netns):
-    missing_nsid = set(os.listdir("/run/netns"))
+    try:
+        missing_nsid = set(os.listdir("/run/netns"))
+    except OSError:
+        missing_nsid = set()
     nsids = {}
     for ns in ip(netns, "netns", "list-id"):
         nsid = ns["nsid"]
         if "name" in ns:
             missing_nsid.discard(ns["name"])
             nsids[nsid] = ns["name"]
         elif nsid == 0:
```

### Comparing `linux-tools-0.2.6/linux_tools/table.py` & `linux-tools-0.2.7/linux_tools/table.py`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.6/linux_tools.egg-info/PKG-INFO` & `linux-tools-0.2.7/linux_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.6
+Version: 0.2.7
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.6/setup.py` & `linux-tools-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setuptools.setup(
     name="linux-tools",
     description="Various command line utilities for Linux written in python",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text("utf-8"),
     long_description_content_type="text/markdown",
     license="BSD-3-Clause",
-    version="0.2.6",
+    version="0.2.7",
     author="Robin Jarry",
     author_email="~rjarry/public-inbox@lists.sr.ht",
     url="https://git.sr.ht/~rjarry/linux-tools",
     packages=setuptools.find_packages("."),
     entry_points="""
     [console_scripts]
     bits = linux_tools.bits:main
```

