# Comparing `tmp/fspy-0.3.1-py2.py3-none-any.whl.zip` & `tmp/fspy-0.3.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 29870 bytes, number of entries: 9
+Zip file size: 29869 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       33 b- defN 23-Jun-12 11:01 fspy/__init__.py
 -rw-rw-r--  2.0 unx     2067 b- defN 23-Jun-11 16:35 fspy/response_models.py
 -rw-rw-r--  2.0 unx     9604 b- defN 23-Jun-12 10:39 fspy/solver.py
 -rw-rw-r--  2.0 unx      441 b- defN 23-Jun-11 16:35 fspy/solver_exceptions.py
--rw-rw-r--  2.0 unx    35128 b- defN 23-Jul-20 13:20 fspy-0.3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    42729 b- defN 23-Jul-20 13:20 fspy-0.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-20 13:20 fspy-0.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-20 13:20 fspy-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 23-Jul-20 13:20 fspy-0.3.1.dist-info/RECORD
-9 files, 90793 bytes uncompressed, 28720 bytes compressed:  68.4%
+-rw-rw-r--  2.0 unx    35128 b- defN 23-Jul-20 13:23 fspy-0.3.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    42729 b- defN 23-Jul-20 13:23 fspy-0.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-20 13:23 fspy-0.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-20 13:23 fspy-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jul-20 13:23 fspy-0.3.2.dist-info/RECORD
+9 files, 90793 bytes uncompressed, 28719 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fspy/solver.py
 Comment: 
 
 Filename: fspy/solver_exceptions.py
 Comment: 
 
-Filename: fspy-0.3.1.dist-info/LICENSE
+Filename: fspy-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: fspy-0.3.1.dist-info/METADATA
+Filename: fspy-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: fspy-0.3.1.dist-info/WHEEL
+Filename: fspy-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: fspy-0.3.1.dist-info/top_level.txt
+Filename: fspy-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fspy-0.3.1.dist-info/RECORD
+Filename: fspy-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fspy-0.3.1.dist-info/LICENSE` & `fspy-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fspy-0.3.1.dist-info/METADATA` & `fspy-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fspy
-Version: 0.3.1
+Version: 0.3.2
 Summary: A FlareSolverr wrapper for Python.
 Author: NandeMD
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi (>=2017.4.17)
 Requires-Dist: charset-normalizer (<4,>=2)
 Requires-Dist: idna (<4,>=2.5)
 Requires-Dist: urllib3 (<3,>=1.21.1)
 Requires-Dist: requests (>=2.9.2)
-Requires-Dist: orjson (==3.9.0)
+Requires-Dist: orjson (>=3.8.0)
 
 # FSPy
 An easy to use FlareSolverr wrapper for Python.
 
 ## Usage
 ```python
 from fspy import FlareSolverr
```

