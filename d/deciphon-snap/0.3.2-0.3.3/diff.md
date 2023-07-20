# Comparing `tmp/deciphon_snap-0.3.2.tar.gz` & `tmp/deciphon_snap-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.3.2.tar", max compression
+gzip compressed data, was "deciphon_snap-0.3.3.tar", max compression
```

## Comparing `deciphon_snap-0.3.2.tar` & `deciphon_snap-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/LICENSE
--rw-r--r--   0        0        0     2453 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/README.md
--rw-r--r--   0        0        0      355 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/amino.py
--rw-r--r--   0        0        0     2706 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/interval.py
--rw-r--r--   0        0        0     3054 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     1377 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-19 15:48:35.697927 deciphon_snap-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/README.md
+-rw-r--r--   0        0        0      355 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2900 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     3054 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1377 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-20 12:33:42.018346 deciphon_snap-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.3/PKG-INFO
```

### Comparing `deciphon_snap-0.3.2/LICENSE` & `deciphon_snap-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/README.md` & `deciphon_snap-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/hit.py` & `deciphon_snap-0.3.3/deciphon_snap/hit.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import List, Type, TypeVar
 
 from pydantic import BaseModel, RootModel
 
 from deciphon_snap.match import MatchList, MatchListInterval
 from deciphon_snap.query_interval import QueryInterval
+from deciphon_snap.match import Match
 
 __all__ = ["Hit", "HitList"]
 
 
 class Hit(BaseModel):
     id: int
     match_list_interval: MatchListInterval
@@ -34,15 +35,15 @@
     def match_list(self, x: MatchList):
         self._match_list = x
 
     @property
     def matches(self):
         assert self._interval is not None
         assert self._match_list is not None
-        matches = []
+        matches: list[Match] = []
         offset = self._interval.pyinterval.start
         for x in self._match_list[self.match_list_interval.slice]:
             x.position = offset
             if x.state.startswith("I"):
                 offset += len(x.query)
             if x.state.startswith("M"):
                 offset += len(x.query)
@@ -56,15 +57,19 @@
 class HitList(RootModel):
     root: List[Hit]
 
     def __len__(self):
         return len(self.root)
 
     def __getitem__(self, i):
-        return self.root[i]
+        if isinstance(i, slice):
+            return HitList.model_validate(self.root[i])
+        hit = self.root[i]
+        assert isinstance(hit, Hit)
+        return hit
 
     def __iter__(self):
         return iter(self.root)
 
     def __str__(self):
         return " ".join(str(i) for i in self.root)
```

### Comparing `deciphon_snap-0.3.2/deciphon_snap/hmmer.py` & `deciphon_snap-0.3.3/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/interval.py` & `deciphon_snap-0.3.3/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/match.py` & `deciphon_snap-0.3.3/deciphon_snap/match.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/prod.py` & `deciphon_snap-0.3.3/deciphon_snap/prod.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/query_interval.py` & `deciphon_snap-0.3.3/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/shorten.py` & `deciphon_snap-0.3.3/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/deciphon_snap/snap_file.py` & `deciphon_snap-0.3.3/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.3.2/PKG-INFO` & `deciphon_snap-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.6.0)
 Requires-Dist: h3result (>=0.3.0)
-Requires-Dist: hmmer-tables (>=0.4.0)
+Requires-Dist: hmmer-tables (>=0.5.0)
 Requires-Dist: prettytable (>=3.8.0)
 Requires-Dist: pydantic (>=2.0.3)
 Description-Content-Type: text/markdown
 
 # deciphon-snap
 
 ## Example
```

