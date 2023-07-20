# Comparing `tmp/cm2py-0.2.5.tar.gz` & `tmp/cm2py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.2.5.tar", last modified: Mon Jul 10 04:24:56 2023, max compression
+gzip compressed data, was "cm2py-0.2.6.tar", last modified: Thu Jul 20 09:41:59 2023, max compression
```

## Comparing `cm2py-0.2.5.tar` & `cm2py-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 04:24:56.316286 cm2py-0.2.5/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-07-10 04:24:56.314042 cm2py-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-06-25 04:24:23.000000 cm2py-0.2.5/README.md
--rw-rw-rw-   0        0        0      675 2023-07-10 04:24:22.000000 cm2py-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 04:24:56.316286 cm2py-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 04:24:56.265292 cm2py-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 04:24:56.281039 cm2py-0.2.5/src/cm2py/
--rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.5/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6342 2023-07-10 04:24:25.000000 cm2py-0.2.5/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:24:56.307286 cm2py-0.2.5/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-07-10 04:24:56.000000 cm2py-0.2.5/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-10 04:24:56.000000 cm2py-0.2.5/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 04:24:56.000000 cm2py-0.2.5/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 04:24:56.000000 cm2py-0.2.5/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 04:24:56.000000 cm2py-0.2.5/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 04:24:56.310292 cm2py-0.2.5/tests/
--rw-rw-rw-   0        0        0     1671 2023-06-25 04:18:52.000000 cm2py-0.2.5/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.552794 cm2py-0.2.6/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-07-20 09:41:59.549787 cm2py-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.2.6/README.md
+-rw-rw-rw-   0        0        0      675 2023-07-15 07:51:08.000000 cm2py-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 09:41:59.552794 cm2py-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.393796 cm2py-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.416794 cm2py-0.2.6/src/cm2py/
+-rw-rw-rw-   0        0        0      237 2023-07-19 11:34:20.000000 cm2py-0.2.6/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6480 2023-07-20 09:40:24.000000 cm2py-0.2.6/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.532793 cm2py-0.2.6/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.537793 cm2py-0.2.6/tests/
+-rw-rw-rw-   0        0        0     2374 2023-07-19 09:48:55.000000 cm2py-0.2.6/tests/test_app.py
```

### Comparing `cm2py-0.2.5/LICENSE` & `cm2py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.5/PKG-INFO` & `cm2py-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.5
+Version: 0.2.6
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.5/README.md` & `cm2py-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.5/pyproject.toml` & `cm2py-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.2.5/src/cm2py/cm2py.py` & `cm2py-0.2.6/src/cm2py/cm2py.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 import re
 from uuid import UUID, uuid4
 import math
 
 
 class Save:
@@ -44,30 +44,29 @@
             self.connections[str(newConnection.target.uuid)].append(newConnection)
         else:
             self.connections[str(newConnection.target.uuid)] = [newConnection]
         return newConnection
 
     def exportSave(self):
         """Export the save to a Circuit Maker 2 save string."""
-        blockStrings = []
+        string = ""
         for b in self.blocks:
-            p = "+".join(str(v) for v in b.properties) if b.properties else ""
-            blockStrings.append(f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z}," + p)
-        saveString = ";".join(blockStrings) + "?"
-        connectionStrings = []
+            if b.properties:
+                p = "+".join(str(v) for v in b.properties)
+                string += f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z},{p};"
+            else:
+                string += f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z},;"
+
+        string = string[:-1] + "?"
+        blockUuids = [str(b.uuid) for b in self.blocks]
         for c in self.connections.values():
             for n in c:
-                connectionStrings.append(
-                    (
-                        f"{[str(b.uuid) for b in self.blocks].index(str(n.source.uuid))+1},"
-                        f"{[str(b.uuid) for b in self.blocks].index(str(n.target.uuid))+1}"
-                    )
-                )
-        saveString += ";".join(connectionStrings) + "?"
-        return saveString
+                string += f"{blockUuids.index(str(n.source.uuid))+1},{blockUuids.index(str(n.target.uuid))+1};"
+        string = string[:-1] + "??"  # TODO: Custom build support & sign data support
+        return string
 
     def deleteBlock(self, blockRef):
         """Delete a block from the save."""
         assert isinstance(blockRef, Block), "blockRef must be a Block object"
         assert blockRef in self.blocks, "block does not exist in save"
         for c in self.connections.values():
             for n in c:
@@ -85,24 +84,24 @@
             for n in c:
                 if connectionRef == n:
                     del self.connections[str(n.target.uuid)][self.connections[str(n.target.uuid)].index(n)]
 
 
 class Block:
     def __init__(self, blockId, pos, state=False, properties=None):
-        assert isinstance(blockId, int) and 0 <= blockId <= 11, "blockId must be an integer between 0 and 11"
+        assert isinstance(blockId, int) and 0 <= blockId <= 13, "blockId must be an integer between 0 and 11"
         assert (
             isinstance(pos, tuple)
             and len(pos) == 3
             and (isinstance(pos[0], float) or isinstance(pos[0], int))
             and (isinstance(pos[1], float) or isinstance(pos[1], int))
             and (isinstance(pos[2], float) or isinstance(pos[2], int))
         ), "pos must be a 3d tuple of integers"
         assert isinstance(state, bool), "state must be a boolean"
-        assert isinstance(properties, list) or properties == None, "properties must be a list of numbers, or None"
+        assert isinstance(properties, list) or properties == None, "properties must be a list of numbers, or None."
         self.blockId = blockId
         self.pos = pos
         self.x = self.pos[0]
         self.y = self.pos[1]
         self.z = self.pos[2]
         self.state = state
         self.properties = properties
@@ -117,15 +116,15 @@
         self.target = target
 
 
 def importSave(string, snapToGrid=True):
     """Import a Circuit Maker 2 save string as a save."""
     regex = (
         # Match all blocks
-        r"^((\d+,){2}(-?\d+(\.\d+)?,){3}(((\d+(\.\d+)?\+)*(\d+(\.\d+)?)))?;)+"
+        r"^((\d+,){2}(-?\d+(\.\d+)?,){3}(((\d+(\.\d+)?\+)*(\d+(\.\d+)?)))?;)*"
         r"((\d+,){2}(-?\d+(\.\d+)?,){3}(((\d+(\.\d+)?\+)*(\d+(\.\d+)?)))?\?)"
         # Match all connections
         r"((([1-9][0-9]*),([1-9][0-9]*)|((([1-9][0-9]*),([1-9][0-9]*);)+"
         r"([1-9][0-9]*),([1-9][0-9]*)))?\?)"
         # Match custom build syntax
         r"((\w+(,(-?\d+(\.\d+)?(\+-?\d+(\.\d+)?)*)*)+)(;(\w+(,(-?\d+(\.\d+)?(\+-?\d+(\.\d+)?)*)*)+))*)*\?"
         # Match sign data
@@ -133,15 +132,24 @@
     )
 
     assert re.match(regex, string), "invalid save string"
 
     newSave = Save()
 
     blocks = [
-        [[int(a) for a in v] if "+" in v else int(v) if v else None for v in i.split(",")]
+        [
+            None
+            if not v
+            else [float(a) for a in v.split("+")]
+            if "+" in v or p == 5
+            else float(v)
+            if (v and p != 0)
+            else int(v)
+            for p, v in enumerate(i.split(","))
+        ]
         for i in "".join(string.split("?")[0]).split(";")
     ]
     connections = [
         [int(v) for v in i.split(",")]
         for i in "".join(string.split("?")[1]).split(";")
         if len("".join(string.split("?")[1]).split(";")) > 1
         and isinstance("".join(string.split("?")[1]).split(";")[0], int)
```

### Comparing `cm2py-0.2.5/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.6/src/cm2py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.5
+Version: 0.2.6
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

