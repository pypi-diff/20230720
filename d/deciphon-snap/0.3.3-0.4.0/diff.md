# Comparing `tmp/deciphon_snap-0.3.3.tar.gz` & `tmp/deciphon_snap-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.3.3.tar", max compression
+gzip compressed data, was "deciphon_snap-0.4.0.tar", max compression
```

## Comparing `deciphon_snap-0.3.3.tar` & `deciphon_snap-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/LICENSE
--rw-r--r--   0        0        0     2453 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/README.md
--rw-r--r--   0        0        0      355 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/amino.py
--rw-r--r--   0        0        0     2900 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/interval.py
--rw-r--r--   0        0        0     3054 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     1377 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/README.md
+-rw-r--r--   0        0        0      355 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2900 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     3054 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1701 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-20 15:35:19.911838 deciphon_snap-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.4.0/PKG-INFO
```

### Comparing `deciphon_snap-0.3.3/LICENSE` & `deciphon_snap-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/README.md` & `deciphon_snap-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/hit.py` & `deciphon_snap-0.4.0/deciphon_snap/hit.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/hmmer.py` & `deciphon_snap-0.4.0/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/interval.py` & `deciphon_snap-0.4.0/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/match.py` & `deciphon_snap-0.4.0/deciphon_snap/match.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/prod.py` & `deciphon_snap-0.4.0/deciphon_snap/prod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 from pydantic import BaseModel, RootModel
 
 from deciphon_snap.hit import Hit, HitList
 from deciphon_snap.hmmer import H3Result
+from deciphon_snap.match import Match
 from deciphon_snap.match import LazyMatchList
 from deciphon_snap.query_interval import QueryIntervalBuilder
 
 __all__ = ["Prod"]
 
 
 class Prod(BaseModel):
@@ -28,14 +29,25 @@
         for hit in HitList.make(self.match_list):
             hit.interval = qibuilder.make(hit.match_list_interval)
             hit.match_list = self.match_list.evaluate()
             hits.append(hit)
         return hits
 
     @property
+    def matches(self) -> list[Hit]:
+        matches = []
+        i = 0
+        for x in self.match_list:
+            match = Match.model_validate(x)
+            match.position = i
+            matches.append(match)
+            i += len(match.query)
+        return matches
+
+    @property
     def hmmer(self):
         assert self.h3result is not None
         return self.h3result
 
     @property
     def query(self):
         return self.match_list.query
```

### Comparing `deciphon_snap-0.3.3/deciphon_snap/query_interval.py` & `deciphon_snap-0.4.0/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/shorten.py` & `deciphon_snap-0.4.0/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/deciphon_snap/snap_file.py` & `deciphon_snap-0.4.0/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.3/PKG-INFO` & `deciphon_snap-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.3.3
+Version: 0.4.0
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

