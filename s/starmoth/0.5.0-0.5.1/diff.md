# Comparing `tmp/starmoth-0.5.0.tar.gz` & `tmp/starmoth-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.5.0.tar", last modified: Thu Jun 15 20:18:41 2023, max compression
+gzip compressed data, was "starmoth-0.5.1.tar", last modified: Thu Jul 20 19:42:11 2023, max compression
```

## Comparing `starmoth-0.5.0.tar` & `starmoth-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     2384 2023-06-15 20:18:41.716005 starmoth-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-06-15 20:13:10.000000 starmoth-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/
--rw-rw-rw-   0 root         (0) root         (0)     4428 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.5.0/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.5.0/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     7379 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.5.0/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 20:18:41.716005 starmoth-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2384 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.153070 starmoth-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-07-20 19:42:11.153070 starmoth-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2023-07-20 18:39:06.000000 starmoth-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.145069 starmoth-0.5.1/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-07-20 18:39:06.000000 starmoth-0.5.1/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.145069 starmoth-0.5.1/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.5.1/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.145069 starmoth-0.5.1/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.5.1/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.149070 starmoth-0.5.1/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2023-07-20 18:39:06.000000 starmoth-0.5.1/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.5.1/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.149070 starmoth-0.5.1/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-06-15 20:13:10.000000 starmoth-0.5.1/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 19:42:11.153070 starmoth-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 19:42:11.149070 starmoth-0.5.1/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-20 19:42:11.000000 starmoth-0.5.1/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.5.0/PKG-INFO` & `starmoth-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.5.0
+Version: 0.5.1
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `starmoth-0.5.0/README.md` & `starmoth-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/moth/__init__.py` & `starmoth-0.5.1/moth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,18 +65,22 @@
         last_heartbeat = None
         last_heartbeat_sent = time.time()
         result_queue = queue.Queue()
         prompt_queue = queue.Queue()
 
         # Workers to handle prompts
         def prompt_loop():
-            while not self.stop:
-                func = self._PROMPT_FUNCTIONS[0]
-                message = prompt_queue.get()
-                result_queue.put(func(message))
+            try:
+                while not self.stop:
+                    func = self._PROMPT_FUNCTIONS[0]
+                    message = prompt_queue.get()
+                    result_queue.put(func(message))
+            except Exception as err:
+                print("Failed to handle prompt: ", err)
+                self.stop = True
 
         threading.Thread(target=prompt_loop, daemon=True).start()
 
         while not self.stop:
             try:
                 events = dict(pool.poll(1000))
```

### Comparing `starmoth-0.5.0/moth/cli/__init__.py` & `starmoth-0.5.1/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/moth/driver/__init__.py` & `starmoth-0.5.1/moth/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/moth/message/__init__.py` & `starmoth-0.5.1/moth/message/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/moth/server/__init__.py` & `starmoth-0.5.1/moth/server/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/setup.py` & `starmoth-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.5.0/starmoth.egg-info/PKG-INFO` & `starmoth-0.5.1/starmoth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.5.0
+Version: 0.5.1
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

