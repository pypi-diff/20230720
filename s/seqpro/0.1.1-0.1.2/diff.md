# Comparing `tmp/seqpro-0.1.1.tar.gz` & `tmp/seqpro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqpro-0.1.1.tar", max compression
+gzip compressed data, was "seqpro-0.1.2.tar", max compression
```

## Comparing `seqpro-0.1.1.tar` & `seqpro-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      543 2023-06-23 19:52:39.000000 seqpro-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      977 2023-06-23 19:48:20.000000 seqpro-0.1.1/seqpro/__init__.py
--rw-r--r--   0        0        0     5455 2023-06-11 21:58:41.000000 seqpro-0.1.1/seqpro/_analyzers.py
--rw-r--r--   0        0        0     1276 2023-06-01 00:42:03.000000 seqpro-0.1.1/seqpro/_cleaners.py
--rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.1/seqpro/_comparisons.py
--rw-r--r--   0        0        0     5098 2023-06-23 16:45:31.000000 seqpro-0.1.1/seqpro/_encoders.py
--rw-r--r--   0        0        0     6926 2023-06-23 19:49:15.000000 seqpro-0.1.1/seqpro/_modifiers.py
--rw-r--r--   0        0        0     3535 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/_numba.py
--rw-r--r--   0        0        0     3810 2023-06-23 16:04:56.000000 seqpro-0.1.1/seqpro/_utils.py
--rw-r--r--   0        0        0     1458 2023-06-11 21:58:41.000000 seqpro-0.1.1/seqpro/alphabets/__init__.py
--rw-r--r--   0        0        0     8278 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/alphabets/_alphabets.py
--rw-r--r--   0        0        0     2504 2023-06-23 17:05:29.000000 seqpro-0.1.1/seqpro/deprecated/_analyzers.py
--rw-r--r--   0        0        0     1358 2023-06-23 17:05:27.000000 seqpro-0.1.1/seqpro/deprecated/_cleaners.py
--rw-r--r--   0        0        0     4364 2023-06-23 17:05:11.000000 seqpro-0.1.1/seqpro/deprecated/_encoders.py
--rw-r--r--   0        0        0     9481 2023-06-23 16:48:35.000000 seqpro-0.1.1/seqpro/deprecated/_helpers.py
--rw-r--r--   0        0        0     6113 2023-06-23 17:05:21.000000 seqpro-0.1.1/seqpro/deprecated/_modifiers.py
--rw-r--r--   0        0        0     1419 2023-06-23 17:05:25.000000 seqpro-0.1.1/seqpro/deprecated/_utils.py
--rw-r--r--   0        0        0     2162 2023-06-23 17:05:59.000000 seqpro-0.1.1/seqpro/experimental/_experimental.py
--rw-r--r--   0        0        0      773 2023-06-23 17:05:39.000000 seqpro-0.1.1/seqpro/experimental/_visualizers.py
--rw-r--r--   0        0        0     6198 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/xr/__init__.py
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 seqpro-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-20 18:52:35.000000 seqpro-0.1.2/LICENSE
+-rw-r--r--   0        0        0      543 2023-07-20 19:49:51.000000 seqpro-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      977 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/__init__.py
+-rw-r--r--   0        0        0     5455 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_analyzers.py
+-rw-r--r--   0        0        0     1276 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_cleaners.py
+-rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.2/seqpro/_comparisons.py
+-rw-r--r--   0        0        0     5098 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_encoders.py
+-rw-r--r--   0        0        0     6926 2023-07-20 18:32:36.000000 seqpro-0.1.2/seqpro/_modifiers.py
+-rw-r--r--   0        0        0     3535 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_numba.py
+-rw-r--r--   0        0        0     3810 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_utils.py
+-rw-r--r--   0        0        0     1458 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/alphabets/__init__.py
+-rw-r--r--   0        0        0     8278 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/alphabets/_alphabets.py
+-rw-r--r--   0        0        0     2504 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_analyzers.py
+-rw-r--r--   0        0        0     1358 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_cleaners.py
+-rw-r--r--   0        0        0     4364 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_encoders.py
+-rw-r--r--   0        0        0     9481 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/deprecated/_helpers.py
+-rw-r--r--   0        0        0     6113 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_modifiers.py
+-rw-r--r--   0        0        0     1419 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_utils.py
+-rw-r--r--   0        0        0     2914 2023-07-20 18:52:06.000000 seqpro-0.1.2/seqpro/experimental/_experimental.py
+-rw-r--r--   0        0        0      773 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/experimental/_visualizers.py
+-rw-r--r--   0        0        0     6198 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/xr/__init__.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 seqpro-0.1.2/PKG-INFO
```

### Comparing `seqpro-0.1.1/pyproject.toml` & `seqpro-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqpro"
-version = "0.1.1"
+version = "0.1.2"
 description = "Sequence processing toolkit"
 authors = ["Adam Klie <aklie@ucsd.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numba = "^0.57.0"
 numpy = "~1.23.5"
```

### Comparing `seqpro-0.1.1/seqpro/__init__.py` & `seqpro-0.1.2/seqpro/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_analyzers.py` & `seqpro-0.1.2/seqpro/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_cleaners.py` & `seqpro-0.1.2/seqpro/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_encoders.py` & `seqpro-0.1.2/seqpro/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_modifiers.py` & `seqpro-0.1.2/seqpro/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_numba.py` & `seqpro-0.1.2/seqpro/_numba.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/_utils.py` & `seqpro-0.1.2/seqpro/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/alphabets/__init__.py` & `seqpro-0.1.2/seqpro/alphabets/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/alphabets/_alphabets.py` & `seqpro-0.1.2/seqpro/alphabets/_alphabets.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_analyzers.py` & `seqpro-0.1.2/seqpro/deprecated/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_cleaners.py` & `seqpro-0.1.2/seqpro/deprecated/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_encoders.py` & `seqpro-0.1.2/seqpro/deprecated/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_helpers.py` & `seqpro-0.1.2/seqpro/deprecated/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_modifiers.py` & `seqpro-0.1.2/seqpro/deprecated/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/deprecated/_utils.py` & `seqpro-0.1.2/seqpro/deprecated/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/experimental/_experimental.py` & `seqpro-0.1.2/seqpro/experimental/_experimental.py`

 * *Files 22% similar despite different names*

```diff
@@ -128,7 +128,42 @@
 ]
 STOP_CODONS = ["TAG", "TAA", "TGA"]
 
 # want to one-hot encode AA sequence and codons
 # https://github.com/gagneurlab/concise/blob/master/concise/preprocessing/sequence.py
 
 # Performing motif anal
+
+
+def kmer2seq(kmers):
+    """
+    Convert kmers to original sequence
+    
+    Arguments:
+    kmers -- str, kmers separated by space.
+    
+    Returns:
+    seq -- str, original sequence.
+
+    """
+    kmers_list = kmers.split(" ")
+    bases = [kmer[0] for kmer in kmers_list[0:-1]]
+    bases.append(kmers_list[-1])
+    seq = "".join(bases)
+    assert len(seq) == len(kmers_list) + len(kmers_list[0]) - 1
+    return seq
+
+def seq2kmer(seq, k):
+    """
+    Convert original sequence to kmers
+    
+    Arguments:
+    seq -- str, original sequence.
+    k -- int, kmer of length k specified.
+    
+    Returns:
+    kmers -- str, kmers separated by space
+
+    """
+    kmer = [seq[x:x+k] for x in range(len(seq)+1-k)]
+    kmers = " ".join(kmer)
+    return kmers
```

### Comparing `seqpro-0.1.1/seqpro/experimental/_visualizers.py` & `seqpro-0.1.2/seqpro/experimental/_visualizers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/seqpro/xr/__init__.py` & `seqpro-0.1.2/seqpro/xr/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.1/PKG-INFO` & `seqpro-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqpro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sequence processing toolkit
 Author: Adam Klie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

