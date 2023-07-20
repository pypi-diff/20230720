# Comparing `tmp/hmmer_tables-0.4.0.tar.gz` & `tmp/hmmer_tables-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.4.0.tar", max compression
+gzip compressed data, was "hmmer_tables-0.5.0.tar", max compression
```

## Comparing `hmmer_tables-0.4.0.tar` & `hmmer_tables-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/LICENSE
--rw-r--r--   0        0        0       15 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      692 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/cleanup.py
--rw-r--r--   0        0        0      367 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3432 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1966 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/interval.py
--rw-r--r--   0        0        0     1456 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/output.py
--rw-r--r--   0        0        0       72 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     7334 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/hmmer_tables/query.py
--rw-r--r--   0        0        0     2141 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      468 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 hmmer_tables-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/LICENSE
+-rw-r--r--   0        0        0       15 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/cleanup.py
+-rw-r--r--   0        0        0      367 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3432 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1966 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/interval.py
+-rw-r--r--   0        0        0     1456 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/output.py
+-rw-r--r--   0        0        0       72 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     7548 2023-07-20 12:26:22.123561 hmmer_tables-0.5.0/hmmer_tables/query.py
+-rw-r--r--   0        0        0     2141 2023-07-20 12:26:22.127561 hmmer_tables-0.5.0/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      468 2023-07-20 12:26:22.127561 hmmer_tables-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 hmmer_tables-0.5.0/PKG-INFO
```

### Comparing `hmmer_tables-0.4.0/LICENSE` & `hmmer_tables-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/hmmer_tables/cleanup.py` & `hmmer_tables-0.5.0/hmmer_tables/cleanup.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/hmmer_tables/domtbl.py` & `hmmer_tables-0.5.0/hmmer_tables/domtbl.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/hmmer_tables/interval.py` & `hmmer_tables-0.5.0/hmmer_tables/interval.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/hmmer_tables/output.py` & `hmmer_tables-0.5.0/hmmer_tables/output.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/hmmer_tables/query.py` & `hmmer_tables-0.5.0/hmmer_tables/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ]
 
 
 class Align(BaseModel):
     core_interval: RInterval
     query_interval: RInterval
     profile: str
+    query_name: str
     hmm_cs: str
     hmm_rf: str
     query_cs: str
     match: str
     query: str
     score: str
 
@@ -123,22 +124,24 @@
 
 def _parse_match(row: str, line_slice: slice):
     return row[line_slice]
 
 
 def _parse_target(row: str, line_slice: slice, last_pos: int):
     tgt = row[line_slice]
-    start = row[: line_slice.start].rstrip().split()[-1]
+    vals = row[: line_slice.start].rstrip().split()
+    start = vals[-1]
+    query_name = vals[0] if len(vals) > 1 else ""
     stop = row[line_slice.stop :].strip()
     if start == "-":
         assert stop == "-"
         start = str(last_pos)
         stop = str(last_pos - 1)
     query_interval = RInterval(start=int(start), stop=int(stop))
-    return tgt, query_interval
+    return tgt, query_name, query_interval
 
 
 def _parse_align_chunk(stream: Iterable[str], last_pos: int):
     it = iter(stream)
     hmm_cs = ""
     hmm_rf = ""
 
@@ -149,15 +152,15 @@
         elif row.endswith(" RF"):
             hmm_rf = row[: row.rfind(" ")].strip()
         else:
             break
 
     line_slice, tgt_cs, core_interval, profile = _parse_target_consensus(row)
     match = _parse_match(next(it), line_slice)
-    tgt, query_interval = _parse_target(next(it), line_slice, last_pos)
+    tgt, query_name, query_interval = _parse_target(next(it), line_slice, last_pos)
 
     row = next(it)
     assert row.endswith(" PP")
     score = row[line_slice]
 
     hmm_cs = "?" * len(tgt_cs) if len(hmm_cs) == 0 else hmm_cs
     hmm_rf = "?" * len(tgt_cs) if len(hmm_rf) == 0 else hmm_rf
@@ -165,14 +168,15 @@
     assert len(hmm_cs) == len(hmm_rf) == len(tgt_cs)
     assert len(tgt_cs) == len(match) == len(tgt) == len(score)
 
     return Align(
         core_interval=core_interval,
         query_interval=query_interval,
         profile=profile,
+        query_name=query_name,
         hmm_cs=hmm_cs,
         hmm_rf=hmm_rf,
         query_cs=tgt_cs,
         match=match,
         query=tgt,
         score=score,
     )
@@ -180,18 +184,20 @@
 
 def _merge_aligns_pair(x: Align, y: Align):
     assert x.core_interval.stop + 1 == y.core_interval.start
     assert x.query_interval.stop + 1 == y.query_interval.start
     core_interval = RInterval(start=x.core_interval.start, stop=y.core_interval.stop)
     query_interval = RInterval(start=x.query_interval.start, stop=y.query_interval.stop)
     assert x.profile == y.profile
+    assert x.query_name == y.query_name
     return Align(
         core_interval=core_interval,
         query_interval=query_interval,
         profile=x.profile,
+        query_name=x.query_name,
         hmm_cs=x.hmm_cs + y.hmm_cs,
         hmm_rf=x.hmm_rf + y.hmm_rf,
         query_cs=x.query_cs + y.query_cs,
         match=x.match + y.match,
         query=x.query + y.query,
         score=x.score + y.score,
     )
```

### Comparing `hmmer_tables-0.4.0/hmmer_tables/tbl.py` & `hmmer_tables-0.5.0/hmmer_tables/tbl.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.4.0/PKG-INFO` & `hmmer_tables-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.4.0
+Version: 0.5.0
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

