# Comparing `tmp/recon_lw-2.0.0.dev5585671861.tar.gz` & `tmp/recon_lw-2.0.0.dev5608740227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5585671861.tar", last modified: Tue Jul 18 09:25:28 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5608740227.tar", last modified: Thu Jul 20 08:34:49 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5585671861.tar` & `recon_lw-2.0.0.dev5608740227.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-18 09:25:09.000000 recon_lw-2.0.0.dev5585671861/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:25:28.000000 recon_lw-2.0.0.dev5585671861/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-18 09:24:47.000000 recon_lw-2.0.0.dev5585671861/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-20 08:34:29.000000 recon_lw-2.0.0.dev5608740227/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13891 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18012 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:34:49.000000 recon_lw-2.0.0.dev5608740227/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 08:34:05.000000 recon_lw-2.0.0.dev5608740227/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/EventsSaver.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,24 +26,25 @@
             scope = e["scope"] if "scope" in e else "default"
             if scope not in self._scopes_buffers:
                 self._scopes_buffers[scope] = []
             self._scopes_buffers[scope].append(e)
             if len(self._scopes_buffers[scope]) > 50000:
                 self.flush_scope(scope)
 
-    def create_event(self, name, type, ok=True, body=None, parentId=None):
+    def create_event(self, name, type, ok=True, body=None, parentId=None, attached_messages=None):
+        attached_messages = attached_messages or []
         ts = datetime.now()
         e = {"eventId": self._create_event_id(),
              "successful": ok,
              "eventName": name,
              "eventType": type,
              "body": body,
              "parentEventId": parentId,
              "startTimestamp": {"epochSecond": int(ts.timestamp()), "nano": ts.microsecond * 1000},
-             "attachedMessageIds": []}
+             "attachedMessageIds": attached_messages}
         return e
 
     def _create_event_id(self):
         self._event_sequence["n"] += 1
         return "{0}_{1}-{2}".format(self._event_sequence["name"],
                                     self._event_sequence["stamp"],
                                     self._event_sequence["n"])
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/StateSequenceGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     if ts_key not in arranged:
                         arranged[ts_key] = {}
                     chained_key = key
                     if key in chains:
                         chained_key = chains[key]                        
                     if new_key is not None and new_key != key:
                         chains[new_key] = chained_key
-                    if key not in arranged[ts_key]:
+                    if chained_key not in arranged[ts_key]:
                         arranged[ts_key][chained_key] = [(o, key, new_key)]
                     else:
                         arranged[ts_key][chained_key].append((o, key, new_key))
                 processed += 1
 
             tss = list(arranged.keys())
             tss.sort()
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/recon_lw.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     if len(m["body"]) == 0:
         return "error"
     if "protocol" not in m["body"]["metadata"]:
         return "not_defined"
     return m["body"]["metadata"]["protocol"]
 
 
-def open_scoped_events_streams(streams_path, name_filter=None):
+def open_scoped_events_streams(streams_path, name_filter=None, data_filter=None):
     streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
     files = listdir(streams_path)
     files.sort()
     scopes_streams = {}
     for f in files:
         if ".pickle" not in f:
             continue
@@ -315,14 +315,16 @@
             continue
         scope = f[:f.index("_scope_")]
         if scope not in scopes_streams:
             scopes_streams[scope] = Data.from_cache_file(path.join(streams_path, f))
         else:
             scopes_streams[scope] += Data.from_cache_file(path.join(streams_path, f))
     for strm in scopes_streams.values():
+        if data_filter:
+            strm = strm.filter(data_filter)
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(strm), None))
     return streams
 
 
 def open_streams(streams_path, name_filter=None, expanded_messages=False):
     streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob_cross_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 continue
             else:
                 continue
         if k not in book2 or book2[k] is None:
             problems.append({"mismatch_key": k, "1": book1[k], "2": None})
             continue
         if book1[k] != book2[k]:
-            problems.append({"mismatch_key": k, "1": book1[k], "2": None})
+            problems.append({"mismatch_key": k, "1": book1[k], "2": book2[k]})
     return problems
 
 
 def compare_full_vs_aggr(full_book: dict, aggr_book: dict) -> list:
     problems = []
     for side in ["ask", "bid"]:
         full_levels = list(full_book[side].keys())
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5608740227/recon_lw/recon_oe_ob.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pathlib
 from datetime import datetime
 from itertools import islice
+import string
 
 from recon_lw import recon_lw
 from recon_lw.EventsSaver import EventsSaver
 from recon_lw import recon_ob_cross_stream
 from recon_lw.TimeCacheMatcher import TimeCacheMatcher
 from th2_data_services.utils.message_utils import message_utils
 from recon_lw.StateSequenceGenerator import StateSequenceGenerator
@@ -53,25 +54,29 @@
 
 def process_oe_md_comparison(ob_events_path, oe_images_events_path, md_sessions_list, result_events_path,
                               horizon_delay_seconds, is_book_open):
     events_saver = EventsSaver(result_events_path)
     root_event = events_saver.create_event("recon_lw_oe_ob_compare" + datetime.now().isoformat(), "Microservice")
     events_saver.save_events([root_event])
     
-    create_event = lambda n, t, ok, b: events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"])
+    def create_event(n, t, ok, b, am=None):
+        return events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"], attached_messages=am)
+
+    #create_event = lambda n, t, ok, b: events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"])
     save_events = lambda ev_batch: events_saver.save_events(ev_batch)
     processor = TimeCacheMatcher(horizon_delay_seconds,
                                  oe_ob_get_timestamp_key1_key2,
                                  oe_ob_interpret_func,
                                  {"is_book_open": is_book_open},
                                  create_event,
                                  save_events)
     
+    data_filter = lambda e: e['body'] and e['body'].get("timestamp", -1) != -1
     streams = recon_lw.open_scoped_events_streams(ob_events_path, lambda n: any(s in n for s in md_sessions_list))
-    streams2 = recon_lw.open_scoped_events_streams(oe_images_events_path)
+    streams2 = recon_lw.open_scoped_events_streams(oe_images_events_path, data_filter=data_filter)
     for elem in streams2:
         streams.add(elem)
 
     message_buffer = [None] * 100
     buffer_len = 100
     while len(streams) > 0:
         next_batch_len = recon_lw.get_next_batch(streams, message_buffer, buffer_len, oe_ob_get_timestamp)
@@ -98,17 +103,25 @@
         ts = recon_lw.epoch_nano_str_to_ts(str_toe)
         if not is_book_open(o["body"]["operation_params"]["instr"],ts):
             return None, None, None
         return ts, None, f'{str_toe}.{o["body"]["operation_params"]["order_id"]}.{o["body"]["otv"]}'
     else:
         return None, None, None
 
+def clear_bookid(book_id):
+    book_id = book_id.split("(", maxsplit=1)[0]
+    return book_id
+
 def oe_ob_interpret_func(match, custom_settings, create_event, send_events):
+    attached_messages = []
     if match[0] is not None and match[1] is not None:
         operation_problem = None
+        book_id = clear_bookid(match[0]['body']['book_id'])
+        match[0]['body']['book_id'] = book_id
+        match[0]['body']['operation_params']['instr'] = book_id
         if match[0]["body"]["operation"] != match[1]["body"]["operation"]:
             operation_problem = f'{match[0]["body"]["operation"]} != {match[1]["body"]["operation"]}'
         comparison = recon_ob_cross_stream.compare_keys(match[1]["body"]["operation_params"].keys(),
                                                         match[0]["body"]["operation_params"],
                                                         match[1]["body"]["operation_params"])
         instr_problem = None
         if match[0]["body"]["book_id"] != match[1]["body"]["operation_params"]["instr"]:
@@ -121,23 +134,27 @@
         if len(comparison) > 0:
             problems["comparison"] = comparison
         
         ok = len(problems) == 0
         body = {"md": match[0]["body"], "oe": match[1]["body"]}
         if not ok:
             body["problems"] = problems
-        ev =  create_event("OEMDMatch", "OEMDMatch", ok, body)
+        attached_messages.extend(match[0]['attachedMessageIds'])
+        attached_messages.extend(match[1]['attachedMessageIds'])
+        ev =  create_event("OEMDMatch", "OEMDMatch", ok, body, attached_messages)
         send_events([ev])
     elif match[0] is None:
         body = {"oe": match[1]["body"]}
-        ev =  create_event("OEMDMissingMD", "OEMDMissingMD", False, body)
+        attached_messages.extend(match[1]['attachedMessageIds'])
+        ev =  create_event("OEMDMissingMD", "OEMDMissingMD", False, body, attached_messages)
         send_events([ev])
     else:
         body = {"md": match[0]["body"]}
-        ev =  create_event("OEMDMissingOE", "OEMDMissingOE", ok, body)
+        attached_messages.extend(match[0]['attachedMessageIds'])
+        ev =  create_event("OEMDMissingOE", "OEMDMissingOE", ok, body, attached_messages)
         send_events([ev])
 
 
 def oe_ob_get_timestamp(o):
     return o["body"]["timestamp"]
```

### Comparing `recon_lw-2.0.0.dev5585671861/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5608740227/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/setup.py` & `recon_lw-2.0.0.dev5608740227/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5585671861/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5608740227/test/test_recon_ob.py`

 * *Files identical despite different names*

