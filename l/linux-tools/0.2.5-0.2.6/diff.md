# Comparing `tmp/linux-tools-0.2.5.tar.gz` & `tmp/linux-tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linux-tools-0.2.5.tar", last modified: Thu May 11 15:23:37 2023, max compression
+gzip compressed data, was "linux-tools-0.2.6.tar", last modified: Thu Jul 20 16:28:51 2023, max compression
```

## Comparing `linux-tools-0.2.5.tar` & `linux-tools-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/
--rw-r--r--   0 build     (1000) build     (1000)     1558 2023-05-11 15:22:48.000000 linux-tools-0.2.5/LICENSE
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-05-11 15:23:37.069933 linux-tools-0.2.5/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)    19849 2023-05-11 15:22:48.000000 linux-tools-0.2.5/README.md
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/linux_tools/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     3214 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/bits.py
--rw-r--r--   0 build     (1000) build     (1000)     8312 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/irqstat.py
--rw-r--r--   0 build     (1000) build     (1000)    11038 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/netgraph.py
--rw-r--r--   0 build     (1000) build     (1000)     1697 2023-05-11 15:22:48.000000 linux-tools-0.2.5/linux_tools/table.py
-drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-05-11 15:23:37.069933 linux-tools-0.2.5/linux_tools.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)    20173 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)      341 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)      119 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)       12 2023-05-11 15:23:37.000000 linux-tools-0.2.5/linux_tools.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)      235 2023-05-11 15:22:48.000000 linux-tools-0.2.5/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1000)      352 2023-05-11 15:23:37.069933 linux-tools-0.2.5/setup.cfg
--rw-r--r--   0 build     (1000) build     (1000)      779 2023-05-11 15:22:48.000000 linux-tools-0.2.5/setup.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/
+-rw-r--r--   0 build     (1000) build     (1000)     1558 2023-07-20 16:28:24.000000 linux-tools-0.2.6/LICENSE
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 16:28:51.000521 linux-tools-0.2.6/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)    19849 2023-07-20 16:28:24.000000 linux-tools-0.2.6/README.md
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/linux_tools/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     3214 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/bits.py
+-rw-r--r--   0 build     (1000) build     (1000)     8312 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/irqstat.py
+-rw-r--r--   0 build     (1000) build     (1000)    11906 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/netgraph.py
+-rw-r--r--   0 build     (1000) build     (1000)     1787 2023-07-20 16:28:24.000000 linux-tools-0.2.6/linux_tools/table.py
+drwxr-sr-x   0 build     (1000) build     (1000)        0 2023-07-20 16:28:51.000521 linux-tools-0.2.6/linux_tools.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)    20173 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)      341 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)      119 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)       12 2023-07-20 16:28:50.000000 linux-tools-0.2.6/linux_tools.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)      235 2023-07-20 16:28:24.000000 linux-tools-0.2.6/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1000)      352 2023-07-20 16:28:51.000521 linux-tools-0.2.6/setup.cfg
+-rw-r--r--   0 build     (1000) build     (1000)      779 2023-07-20 16:28:24.000000 linux-tools-0.2.6/setup.py
```

### Comparing `linux-tools-0.2.5/LICENSE` & `linux-tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.5/PKG-INFO` & `linux-tools-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.5/README.md` & `linux-tools-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.5/linux_tools/bits.py` & `linux-tools-0.2.6/linux_tools/bits.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         dest="mode",
         const=bit_list,
         help="""
         Print the combined args as a list of bit IDs. Consecutive IDs are
         compressed as ranges.
         """,
     )
-    parser.set_defaults(mode=bit_mask)
+    parser.set_defaults(mode=hex_mask)
     args = parser.parse_args()
     bit_ids = set()
     for a in args.args:
         bit_ids.update(a)
     print(args.mode(bit_ids))
```

### Comparing `linux-tools-0.2.5/linux_tools/irqstat.py` & `linux-tools-0.2.6/linux_tools/irqstat.py`

 * *Files identical despite different names*

### Comparing `linux-tools-0.2.5/linux_tools/netgraph.py` & `linux-tools-0.2.6/linux_tools/netgraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     %(prog)s | dot -Tsvg > net.svg
 
 System dependencies: iproute2, ethtool
 """
 
 import argparse
 import json
+import os
 import re
 import subprocess
 import sys
 
 from . import bits
 
 
@@ -69,15 +70,15 @@
     print("  edge [fontsize=11 fontname=monospace margin=0];")
     print("  graph [fontsize=11 fontname=monospace compound=true style=dotted];")
 
     for ns, links in namespaces.items():
         print()
         if ns:
             print(f"  subgraph {safe(ns)} {{")
-            print(f'    label="netns {ns}";')
+            print(f'    label="{ns}";')
             print("    cluster=true;")
             print()
             indent = "  "
         else:
             indent = ""
         for link in links:
             print(f"{indent}  {link['id']} [{node_attrs(link)}];")
@@ -188,33 +189,63 @@
     return iproute2_cmd("ip", ns, *cmd)
 
 
 def bridge(ns, *cmd):
     return iproute2_cmd("bridge", ns, *cmd)
 
 
+def get_nsids(netns):
+    missing_nsid = set(os.listdir("/run/netns"))
+    nsids = {}
+    for ns in ip(netns, "netns", "list-id"):
+        nsid = ns["nsid"]
+        if "name" in ns:
+            missing_nsid.discard(ns["name"])
+            nsids[nsid] = ns["name"]
+        elif nsid == 0:
+            # XXX: hack: there is absolutely no guarantee that 0 is a special
+            # number that will always point to the netns of PID 1. However,
+            # this workaround seems to work most of the time.
+            nsids[nsid] = ""
+    for name in missing_nsid:
+        cmd = ["ip"]
+        if netns != "":
+            cmd += ["-n", netns]
+        subprocess.call(
+            cmd + ["netns", "set", name, "auto"],
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+
+    if missing_nsid:
+        for ns in ip(netns, "netns", "list-id"):
+            nsid = ns["nsid"]
+            if nsid not in nsids and "name" in ns:
+                nsids[nsid] = ns["name"]
+
+    return nsids
+
+
 def get_running():
     addrs = ip("", "addr", "show")
-    nsids = ip("", "netns", "list-id")
     running = {
         "": {
             "addr_names": {a["ifname"]: a for a in addrs},
             "addr_ids": {a["ifindex"]: a for a in addrs},
-            "nsids": {n["nsid"]: n["name"] for n in nsids if "name" in n},
+            "nsids": get_nsids(""),
         },
     }
     for ns in running[""]["nsids"].values():
         if ns == "":
             continue
         addrs = ip(ns, "addr", "show")
-        nsids = ip(ns, "netns", "list-id")
         running[ns] = {
             "addr_names": {a["ifname"]: a for a in addrs},
             "addr_ids": {a["ifindex"]: a for a in addrs},
-            "nsids": {n["nsid"]: n.get("name", "") for n in nsids},
+            "nsids": get_nsids(ns),
         }
 
     return running
 
 
 def preprocess(conf, args):
     out = {}
```

### Comparing `linux-tools-0.2.5/linux_tools/table.py` & `linux-tools-0.2.6/linux_tools/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,11 +44,13 @@
                 if len(col.name) > col.width:
                     col.width = len(col.name)
         if self.columns[-1].align == ALIGN_LEFT:
             self.columns[-1].width = 0
         if with_headers:
             names = [c.name for c in self.columns]
             headers = [c.align(n) for c, n in zip(self.columns, names)]
+            headers[-1] = headers[-1].rstrip()
             fileobj.write(self.separator.join(headers) + "\n")
         for row in self.rows:
             cells = [c.align(r) for c, r in zip(self.columns, row)]
+            cells[-1] = cells[-1].rstrip()
             fileobj.write(self.separator.join(cells) + "\n")
```

### Comparing `linux-tools-0.2.5/linux_tools.egg-info/PKG-INFO` & `linux-tools-0.2.6/linux_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linux-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: Various command line utilities for Linux written in python
 Home-page: https://git.sr.ht/~rjarry/linux-tools
 Author: Robin Jarry
 Author-email: ~rjarry/public-inbox@lists.sr.ht
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `linux-tools-0.2.5/setup.py` & `linux-tools-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setuptools.setup(
     name="linux-tools",
     description="Various command line utilities for Linux written in python",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text("utf-8"),
     long_description_content_type="text/markdown",
     license="BSD-3-Clause",
-    version="0.2.5",
+    version="0.2.6",
     author="Robin Jarry",
     author_email="~rjarry/public-inbox@lists.sr.ht",
     url="https://git.sr.ht/~rjarry/linux-tools",
     packages=setuptools.find_packages("."),
     entry_points="""
     [console_scripts]
     bits = linux_tools.bits:main
```

