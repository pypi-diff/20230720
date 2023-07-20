# Comparing `tmp/deciphon_snap-0.4.0.tar.gz` & `tmp/deciphon_snap-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.4.0.tar", max compression
+gzip compressed data, was "deciphon_snap-0.5.0.tar", max compression
```

## Comparing `deciphon_snap-0.4.0.tar` & `deciphon_snap-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/LICENSE
--rw-r--r--   0        0        0     2453 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/README.md
--rw-r--r--   0        0        0      355 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/amino.py
--rw-r--r--   0        0        0     2900 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/interval.py
--rw-r--r--   0        0        0     3054 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     1701 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 16:10:55.755236 deciphon_snap-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-20 16:10:55.755236 deciphon_snap-0.5.0/README.md
+-rw-r--r--   0        0        0      355 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2900 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     3054 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1701 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0     6735 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/deciphon_snap/view.py
+-rw-r--r--   0        0        0      541 2023-07-20 16:10:55.759236 deciphon_snap-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.5.0/PKG-INFO
```

### Comparing `deciphon_snap-0.4.0/LICENSE` & `deciphon_snap-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/README.md` & `deciphon_snap-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/hit.py` & `deciphon_snap-0.5.0/deciphon_snap/hit.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/hmmer.py` & `deciphon_snap-0.5.0/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/interval.py` & `deciphon_snap-0.5.0/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/match.py` & `deciphon_snap-0.5.0/deciphon_snap/match.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/prod.py` & `deciphon_snap-0.5.0/deciphon_snap/prod.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/query_interval.py` & `deciphon_snap-0.5.0/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/shorten.py` & `deciphon_snap-0.5.0/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/deciphon_snap/snap_file.py` & `deciphon_snap-0.5.0/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.4.0/pyproject.toml` & `deciphon_snap-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.4.0"
+version = "0.5.0"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphon_snap-0.4.0/PKG-INFO` & `deciphon_snap-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.4.0
+Version: 0.5.0
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

