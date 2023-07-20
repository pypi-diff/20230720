# Comparing `tmp/lammpsio-0.4.0.tar.gz` & `tmp/lammpsio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammpsio-0.4.0.tar", last modified: Fri Mar 31 14:01:21 2023, max compression
+gzip compressed data, was "lammpsio-0.4.1.tar", last modified: Thu Jul 20 21:14:16 2023, max compression
```

## Comparing `lammpsio-0.4.0.tar` & `lammpsio-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:01:21.178858 lammpsio-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-31 14:01:09.000000 lammpsio-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-03-31 14:01:21.178858 lammpsio-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-31 14:01:09.000000 lammpsio-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 14:01:09.000000 lammpsio-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-31 14:01:21.178858 lammpsio-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 14:01:09.000000 lammpsio-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:01:21.170858 lammpsio-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:01:21.174857 lammpsio-0.4.0/src/lammpsio/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 14:01:09.000000 lammpsio-0.4.0/src/lammpsio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-31 14:01:09.000000 lammpsio-0.4.0/src/lammpsio/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-03-31 14:01:09.000000 lammpsio-0.4.0/src/lammpsio/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-03-31 14:01:09.000000 lammpsio-0.4.0/src/lammpsio/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-03-31 14:01:09.000000 lammpsio-0.4.0/src/lammpsio/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:01:21.178858 lammpsio-0.4.0/src/lammpsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-03-31 14:01:21.000000 lammpsio-0.4.0/src/lammpsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-31 14:01:21.000000 lammpsio-0.4.0/src/lammpsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:01:21.000000 lammpsio-0.4.0/src/lammpsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 14:01:21.000000 lammpsio-0.4.0/src/lammpsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 14:01:21.000000 lammpsio-0.4.0/src/lammpsio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:01:21.178858 lammpsio-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-31 14:01:09.000000 lammpsio-0.4.0/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-31 14:01:09.000000 lammpsio-0.4.0/tests/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-31 14:01:09.000000 lammpsio-0.4.0/tests/test_dump_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-03-31 14:01:09.000000 lammpsio-0.4.0/tests/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-20 21:14:05.000000 lammpsio-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 21:14:16.950640 lammpsio-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-20 21:14:05.000000 lammpsio-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 21:14:05.000000 lammpsio-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-20 21:14:16.950640 lammpsio-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:14:05.000000 lammpsio-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/lammpsio/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/lammpsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_dump_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_snapshot.py
```

### Comparing `lammpsio-0.4.0/LICENSE` & `lammpsio-0.4.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2022, Auburn University
+Copyright (c) 2021-2023, Auburn University
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `lammpsio-0.4.0/PKG-INFO` & `lammpsio-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
@@ -18,21 +18,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lammpsio
 
 [![PyPI version](https://img.shields.io/pypi/v/lammpsio.svg)](https://pypi.org/project/lammpsio)
+[![PyPI downloads](https://img.shields.io/pypi/dm/lammpsio)](https://pypi.org/project/lammpsio)
+[![Conda](https://img.shields.io/conda/dn/conda-forge/lammpsio)](https://anaconda.org/conda-forge/lammpsio)
 
 Tools for working with LAMMPS data and dump files.
 
 `lammpsio` is a pure Python package that can be installed using `pip`:
 
     pip install lammpsio
 
+or `conda`:
+
+    conda install -c conda-forge lammpsio
+
 ## Snapshot
 
 The particle configuration is stored in a `Snapshot`. A `Snapshot` holds the
 data for *N* particles, the simulation `Box`, and the timestep. The `Box` follows
 the LAMMPS conventions for its shape and bounds. Here is a 3-particle
 configuration in an orthorhombic box centered at the origin at step 100:
```

### Comparing `lammpsio-0.4.0/README.md` & `lammpsio-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # lammpsio
 
 [![PyPI version](https://img.shields.io/pypi/v/lammpsio.svg)](https://pypi.org/project/lammpsio)
+[![PyPI downloads](https://img.shields.io/pypi/dm/lammpsio)](https://pypi.org/project/lammpsio)
+[![Conda](https://img.shields.io/conda/dn/conda-forge/lammpsio)](https://anaconda.org/conda-forge/lammpsio)
 
 Tools for working with LAMMPS data and dump files.
 
 `lammpsio` is a pure Python package that can be installed using `pip`:
 
     pip install lammpsio
 
+or `conda`:
+
+    conda install -c conda-forge lammpsio
+
 ## Snapshot
 
 The particle configuration is stored in a `Snapshot`. A `Snapshot` holds the
 data for *N* particles, the simulation `Box`, and the timestep. The `Box` follows
 the LAMMPS conventions for its shape and bounds. Here is a 3-particle
 configuration in an orthorhombic box centered at the origin at step 100:
```

### Comparing `lammpsio-0.4.0/setup.cfg` & `lammpsio-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/src/lammpsio/box.py` & `lammpsio-0.4.1/src/lammpsio/box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/src/lammpsio/data.py` & `lammpsio-0.4.1/src/lammpsio/data.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/src/lammpsio/dump.py` & `lammpsio-0.4.1/src/lammpsio/dump.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/src/lammpsio/snapshot.py` & `lammpsio-0.4.1/src/lammpsio/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,19 @@
             Converted HOOMD GSD frame.
 
         """
         if "gsd" not in _optional_imports:
             raise ImportError("GSD package not found")
 
         # make Frame/Snapshot without deprecation warnings
-        gsd_version = packaging.version.Version(gsd.__version__)
-        if gsd_version >= packaging.version.Version("2.8.0"):
+        try:
+            gsd_version = gsd.version.version
+        except AttributeError:
+            gsd_version = gsd.__version__
+        if packaging.version.Version(gsd_version) >= packaging.version.Version("2.8.0"):
             frame = gsd.hoomd.Frame()
         else:
             frame = gsd.hoomd.Snapshot()
 
         if self.step is not None:
             frame.configuration.step = int(self.step)
```

### Comparing `lammpsio-0.4.0/src/lammpsio.egg-info/PKG-INFO` & `lammpsio-0.4.1/src/lammpsio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
@@ -18,21 +18,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lammpsio
 
 [![PyPI version](https://img.shields.io/pypi/v/lammpsio.svg)](https://pypi.org/project/lammpsio)
+[![PyPI downloads](https://img.shields.io/pypi/dm/lammpsio)](https://pypi.org/project/lammpsio)
+[![Conda](https://img.shields.io/conda/dn/conda-forge/lammpsio)](https://anaconda.org/conda-forge/lammpsio)
 
 Tools for working with LAMMPS data and dump files.
 
 `lammpsio` is a pure Python package that can be installed using `pip`:
 
     pip install lammpsio
 
+or `conda`:
+
+    conda install -c conda-forge lammpsio
+
 ## Snapshot
 
 The particle configuration is stored in a `Snapshot`. A `Snapshot` holds the
 data for *N* particles, the simulation `Box`, and the timestep. The `Box` follows
 the LAMMPS conventions for its shape and bounds. Here is a 3-particle
 configuration in an orthorhombic box centered at the origin at step 100:
```

### Comparing `lammpsio-0.4.0/tests/test_box.py` & `lammpsio-0.4.1/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/tests/test_data_file.py` & `lammpsio-0.4.1/tests/test_data_file.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/tests/test_dump_file.py` & `lammpsio-0.4.1/tests/test_dump_file.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.0/tests/test_snapshot.py` & `lammpsio-0.4.1/tests/test_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,19 @@
     assert snap.N == 3
     assert isinstance(snap.box, lammpsio.Box)
     assert snap.step == 10
 
 
 def test_gsd_conversion():
     # make a GSD frame
-    if version.Version(gsd.__version__) >= version.Version("2.8.0"):
+    try:
+        gsd_version = gsd.version.version
+    except AttributeError:
+        gsd_version = gsd.__version__
+    if version.Version(gsd_version) >= version.Version("2.8.0"):
         frame = gsd.hoomd.Frame()
     else:
         frame = gsd.hoomd.Snapshot()
     frame.configuration.step = 3
     frame.configuration.box = [4, 5, 6, 0.1, 0.2, 0.3]
     frame.particles.N = 2
     frame.particles.position = [[0.1, 0.2, 0.3], [-0.1, -0.2, -0.3]]
```

