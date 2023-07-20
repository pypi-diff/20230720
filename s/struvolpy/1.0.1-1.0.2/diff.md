# Comparing `tmp/struvolpy-1.0.1.tar.gz` & `tmp/struvolpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struvolpy-1.0.1.tar", last modified: Wed Jul 19 12:48:15 2023, max compression
+gzip compressed data, was "struvolpy-1.0.2.tar", last modified: Thu Jul 20 11:46:48 2023, max compression
```

## Comparing `struvolpy-1.0.1.tar` & `struvolpy-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-19 12:48:15.953201 struvolpy-1.0.1/
--rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-18 08:40:59.000000 struvolpy-1.0.1/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-19 12:48:15.953201 struvolpy-1.0.1/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 08:46:27.000000 struvolpy-1.0.1/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      958 2023-07-19 12:48:15.957201 struvolpy-1.0.1/setup.cfg
--rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-18 08:40:59.000000 struvolpy-1.0.1/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-19 12:48:15.953201 struvolpy-1.0.1/struvolpy/
--rw-rw-r--   0 luc       (1000) luc       (1000)    20325 2023-07-19 08:41:35.000000 struvolpy-1.0.1/struvolpy/Structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)    22154 2023-07-19 08:41:39.000000 struvolpy-1.0.1/struvolpy/Volume.py
--rw-rw-r--   0 luc       (1000) luc       (1000)       83 2023-07-18 14:24:23.000000 struvolpy-1.0.1/struvolpy/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-19 12:48:15.953201 struvolpy-1.0.1/struvolpy/wrappers/
--rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-18 14:24:41.000000 struvolpy-1.0.1/struvolpy/wrappers/__init__.py
--rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-18 15:44:06.000000 struvolpy-1.0.1/struvolpy/wrappers/wrappers.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-19 12:48:15.953201 struvolpy-1.0.1/struvolpy.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-19 12:48:15.000000 struvolpy-1.0.1/struvolpy.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-19 12:48:15.000000 struvolpy-1.0.1/struvolpy.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-19 12:48:15.000000 struvolpy-1.0.1/struvolpy.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-19 12:48:15.000000 struvolpy-1.0.1/struvolpy.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-19 12:48:15.000000 struvolpy-1.0.1/struvolpy.egg-info/top_level.txt
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-19 12:48:15.953201 struvolpy-1.0.1/tests/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-18 15:14:19.000000 struvolpy-1.0.1/tests/test_structure.py
--rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-18 15:43:50.000000 struvolpy-1.0.1/tests/test_volume.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    34523 2023-07-19 13:31:13.000000 struvolpy-1.0.2/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-20 11:46:48.192202 struvolpy-1.0.2/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      903 2023-07-19 13:31:13.000000 struvolpy-1.0.2/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      958 2023-07-20 11:46:48.192202 struvolpy-1.0.2/setup.cfg
+-rw-rw-r--   0 luc       (1000) luc       (1000)       38 2023-07-19 13:31:13.000000 struvolpy-1.0.2/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.188202 struvolpy-1.0.2/struvolpy/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    20325 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/Structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)    22154 2023-07-20 11:13:06.000000 struvolpy-1.0.2/struvolpy/Volume.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)       83 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/struvolpy/wrappers/
+-rw-rw-r--   0 luc       (1000) luc       (1000)       36 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/wrappers/__init__.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)      827 2023-07-19 13:31:13.000000 struvolpy-1.0.2/struvolpy/wrappers/wrappers.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.188202 struvolpy-1.0.2/struvolpy.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1586 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      384 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       60 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       10 2023-07-20 11:46:48.000000 struvolpy-1.0.2/struvolpy.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-20 11:46:48.192202 struvolpy-1.0.2/tests/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1797 2023-07-19 13:31:13.000000 struvolpy-1.0.2/tests/test_structure.py
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1215 2023-07-19 13:31:13.000000 struvolpy-1.0.2/tests/test_volume.py
```

### Comparing `struvolpy-1.0.1/LICENSE` & `struvolpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.1/PKG-INFO` & `struvolpy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.1/README.md` & `struvolpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.1/setup.cfg` & `struvolpy-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = struvolpy
-version = 1.0.1
+version = 1.0.2
 author = Luc Elliott
 author_email = hllelli2@liverpool.ac.uk
 description = "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 long_description = file: ./README.md
 long_description_content_type = text/markdown
 Home-page = https://github.com/hllelli2/struvolpy/
 license = "GPLv3"
```

### Comparing `struvolpy-1.0.1/struvolpy/Structure.py` & `struvolpy-1.0.2/struvolpy/Structure.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.1/struvolpy/Volume.py` & `struvolpy-1.0.2/struvolpy/Volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,15 +602,15 @@
         Raises:
             ValueError: If no resolution is specified.
 
         Returns:
             None
         """
         if self.__tempy_map is None:
-            self.create_tempy_object()
+            self.create_TEMPy_object()
 
         if simulated:
             if not self.__resolution:
                 raise ValueError("No resolution specified")
 
             if self.__resolution > 10.0:
                 t = 2.5
```

### Comparing `struvolpy-1.0.1/struvolpy/wrappers/wrappers.py` & `struvolpy-1.0.2/struvolpy/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.1/struvolpy.egg-info/PKG-INFO` & `struvolpy-1.0.2/struvolpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struvolpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: "A python package for parsing atomic coordinates files (pdb, mmcif) and electron density files (map, mrc, ccp4)"
 Home-page: https://github.com/hllelli2/struvolpy/
 Author: Luc Elliott
 Author-email: hllelli2@liverpool.ac.uk
 License: "GPLv3"
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `struvolpy-1.0.1/tests/test_structure.py` & `struvolpy-1.0.2/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `struvolpy-1.0.1/tests/test_volume.py` & `struvolpy-1.0.2/tests/test_volume.py`

 * *Files identical despite different names*

