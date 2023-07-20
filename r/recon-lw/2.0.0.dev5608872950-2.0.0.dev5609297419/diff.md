# Comparing `tmp/recon_lw-2.0.0.dev5608872950.tar.gz` & `tmp/recon_lw-2.0.0.dev5609297419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5608872950.tar", last modified: Thu Jul 20 08:48:58 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5609297419.tar", last modified: Thu Jul 20 09:31:55 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5608872950.tar` & `recon_lw-2.0.0.dev5609297419.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-20 08:48:34.000000 recon_lw-2.0.0.dev5608872950/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13891 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    18012 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 08:48:58.000000 recon_lw-2.0.0.dev5608872950/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 08:48:06.000000 recon_lw-2.0.0.dev5608872950/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-20 09:31:32.000000 recon_lw-2.0.0.dev5609297419/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13891 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:31:55.000000 recon_lw-2.0.0.dev5609297419/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 09:31:04.000000 recon_lw-2.0.0.dev5609297419/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5609297419/recon_lw/recon_oe_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         body = {"oe": match[1]["body"]}
         attached_messages.extend(match[1]['attachedMessageIds'])
         ev =  create_event("OEMDMissingMD", "OEMDMissingMD", False, body, attached_messages)
         send_events([ev])
     else:
         body = {"md": match[0]["body"]}
         attached_messages.extend(match[0]['attachedMessageIds'])
-        ev =  create_event("OEMDMissingOE", "OEMDMissingOE", ok, body, attached_messages)
+        ev =  create_event("OEMDMissingOE", "OEMDMissingOE", False, body, attached_messages)
         send_events([ev])
 
 
 def oe_ob_get_timestamp(o):
     return o["body"]["timestamp"]
```

### Comparing `recon_lw-2.0.0.dev5608872950/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5609297419/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/setup.py` & `recon_lw-2.0.0.dev5609297419/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5608872950/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5609297419/test/test_recon_ob.py`

 * *Files identical despite different names*

