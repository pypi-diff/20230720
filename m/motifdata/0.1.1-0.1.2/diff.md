# Comparing `tmp/motifdata-0.1.1.tar.gz` & `tmp/motifdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motifdata-0.1.1.tar", max compression
+gzip compressed data, was "motifdata-0.1.2.tar", max compression
```

## Comparing `motifdata-0.1.1.tar` & `motifdata-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-01-31 23:19:36.000000 motifdata-0.1.1/LICENSE
--rw-r--r--   0        0        0      479 2023-05-23 17:49:32.000000 motifdata-0.1.1/README.md
--rw-r--r--   0        0        0     4914 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/_Motif.py
--rw-r--r--   0        0        0      550 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/__init__.py
--rw-r--r--   0        0        0     7957 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/_convert.py
--rw-r--r--   0        0        0    12831 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/_io.py
--rw-r--r--   0        0        0     1919 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/_transform.py
--rw-r--r--   0        0        0     7139 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/_utils.py
--rw-r--r--   0        0        0   111006 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/filters_out.meme
--rw-r--r--   0        0        0  1632317 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/jaspar_out.meme
--rw-r--r--   0        0        0     2857 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample.meme
--rw-r--r--   0        0        0     4392 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample.motifs
--rw-r--r--   0        0        0      424 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample.pfm
--rw-r--r--   0        0        0      189 2023-02-02 22:17:57.000000 motifdata-0.1.1/motifdata/resources/sample.sites
--rw-r--r--   0        0        0      269 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample_filter.meme
--rw-r--r--   0        0        0    21084 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample_filters.meme
--rw-r--r--   0        0        0     2194 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample_out.meme
--rw-r--r--   0        0        0     3482 2023-07-20 18:22:43.000000 motifdata-0.1.1/motifdata/resources/sample_out.motifs
--rw-r--r--   0        0        0      532 2023-07-20 19:51:01.000000 motifdata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 motifdata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-01-31 23:19:36.000000 motifdata-0.1.2/LICENSE
+-rw-r--r--   0        0        0      479 2023-05-23 17:49:32.000000 motifdata-0.1.2/README.md
+-rw-r--r--   0        0        0     4914 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/_Motif.py
+-rw-r--r--   0        0        0      550 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/__init__.py
+-rw-r--r--   0        0        0     7957 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/_convert.py
+-rw-r--r--   0        0        0    12831 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/_io.py
+-rw-r--r--   0        0        0     1919 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/_transform.py
+-rw-r--r--   0        0        0     7139 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/_utils.py
+-rw-r--r--   0        0        0   111006 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/filters_out.meme
+-rw-r--r--   0        0        0  1632317 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/jaspar_out.meme
+-rw-r--r--   0        0        0     2857 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample.meme
+-rw-r--r--   0        0        0     4392 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample.motifs
+-rw-r--r--   0        0        0      424 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample.pfm
+-rw-r--r--   0        0        0      189 2023-02-02 22:17:57.000000 motifdata-0.1.2/motifdata/resources/sample.sites
+-rw-r--r--   0        0        0      269 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample_filter.meme
+-rw-r--r--   0        0        0    21084 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample_filters.meme
+-rw-r--r--   0        0        0     2194 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample_out.meme
+-rw-r--r--   0        0        0     3482 2023-07-20 18:22:43.000000 motifdata-0.1.2/motifdata/resources/sample_out.motifs
+-rw-r--r--   0        0        0      532 2023-07-20 19:53:58.000000 motifdata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 motifdata-0.1.2/PKG-INFO
```

### Comparing `motifdata-0.1.1/LICENSE` & `motifdata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/_Motif.py` & `motifdata-0.1.2/motifdata/_Motif.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/__init__.py` & `motifdata-0.1.2/motifdata/__init__.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/_convert.py` & `motifdata-0.1.2/motifdata/_convert.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/_io.py` & `motifdata-0.1.2/motifdata/_io.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/_transform.py` & `motifdata-0.1.2/motifdata/_transform.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/_utils.py` & `motifdata-0.1.2/motifdata/_utils.py`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/filters_out.meme` & `motifdata-0.1.2/motifdata/resources/filters_out.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/jaspar_out.meme` & `motifdata-0.1.2/motifdata/resources/jaspar_out.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/sample.meme` & `motifdata-0.1.2/motifdata/resources/sample.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/sample.motifs` & `motifdata-0.1.2/motifdata/resources/sample.motifs`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/sample_filters.meme` & `motifdata-0.1.2/motifdata/resources/sample_filters.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/sample_out.meme` & `motifdata-0.1.2/motifdata/resources/sample_out.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/motifdata/resources/sample_out.motifs` & `motifdata-0.1.2/motifdata/resources/sample_out.motifs`

 * *Files identical despite different names*

### Comparing `motifdata-0.1.1/pyproject.toml` & `motifdata-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motifdata"
-version = "0.1.1"
+version = "0.1.2"
 description = "Motif representation and analysis toolkit"
 authors = ["adamklie <aklie@ucsd.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "^1.23.2"
```

### Comparing `motifdata-0.1.1/PKG-INFO` & `motifdata-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motifdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Motif representation and analysis toolkit
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

