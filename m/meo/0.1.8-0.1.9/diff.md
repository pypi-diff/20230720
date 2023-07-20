# Comparing `tmp/meo-0.1.8.tar.gz` & `tmp/meo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.8.tar", last modified: Thu Jul  6 12:02:41 2023, max compression
+gzip compressed data, was "meo-0.1.9.tar", last modified: Wed Jul 12 01:45:37 2023, max compression
```

## Comparing `meo-0.1.8.tar` & `meo-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 12:02:41.504425 meo-0.1.8/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-07-01 13:29:07.000000 meo-0.1.8/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-06 12:02:41.504425 meo-0.1.8/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-07-01 13:29:07.000000 meo-0.1.8/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 12:02:41.501092 meo-0.1.8/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      134 2023-07-01 13:29:07.000000 meo-0.1.8/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-07-06 12:02:37.000000 meo-0.1.8/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 12:02:41.504425 meo-0.1.8/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-07-01 13:29:07.000000 meo-0.1.8/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5317 2023-07-01 13:29:07.000000 meo-0.1.8/meo/crack/cracker.py
--rw-r--r--   0 meo       (1000) meo       (1000)      725 2023-07-01 13:29:07.000000 meo-0.1.8/meo/crack/pdf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-07-01 13:29:07.000000 meo-0.1.8/meo/crack/utils.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1046 2023-07-01 13:29:07.000000 meo-0.1.8/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-07-01 13:29:07.000000 meo-0.1.8/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2671 2023-07-01 13:29:07.000000 meo-0.1.8/meo/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-07-01 13:29:07.000000 meo-0.1.8/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-07-01 13:29:07.000000 meo-0.1.8/meo/screen.py
--rw-r--r--   0 meo       (1000) meo       (1000)      434 2023-07-06 12:02:30.000000 meo-0.1.8/meo/utils.py
--rw-r--r--   0 meo       (1000) meo       (1000)      332 2023-07-01 13:29:07.000000 meo-0.1.8/meo/wapper.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 12:02:41.501092 meo-0.1.8/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-06 12:02:41.000000 meo-0.1.8/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      415 2023-07-06 12:02:41.000000 meo-0.1.8/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-06 12:02:41.000000 meo-0.1.8/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-07-06 12:02:41.000000 meo-0.1.8/meo.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-07-06 12:02:41.000000 meo-0.1.8/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-06 12:02:41.504425 meo-0.1.8/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-07-01 13:29:07.000000 meo-0.1.8/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 12:02:41.504425 meo-0.1.8/test/
--rw-r--r--   0 meo       (1000) meo       (1000)      435 2023-07-01 13:29:07.000000 meo-0.1.8/test/test.py
--rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-07-01 13:29:07.000000 meo-0.1.8/test/test_crack.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-07-01 13:29:07.000000 meo-0.1.8/test/test_imp.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-12 01:45:37.587274 meo-0.1.9/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-07-01 13:29:07.000000 meo-0.1.9/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-12 01:45:37.587274 meo-0.1.9/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-07-01 13:29:07.000000 meo-0.1.9/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-12 01:45:37.587274 meo-0.1.9/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      134 2023-07-01 13:29:07.000000 meo-0.1.9/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-07-12 01:45:35.000000 meo-0.1.9/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-12 01:45:37.587274 meo-0.1.9/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-07-01 13:29:07.000000 meo-0.1.9/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5200 2023-07-12 01:43:54.000000 meo-0.1.9/meo/crack/cracker.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      725 2023-07-01 13:29:07.000000 meo-0.1.9/meo/crack/pdf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-07-01 13:29:07.000000 meo-0.1.9/meo/crack/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1001 2023-07-12 01:44:51.000000 meo-0.1.9/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-07-01 13:29:07.000000 meo-0.1.9/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2671 2023-07-01 13:29:07.000000 meo-0.1.9/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-07-01 13:29:07.000000 meo-0.1.9/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-07-01 13:29:07.000000 meo-0.1.9/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      813 2023-07-12 01:40:58.000000 meo-0.1.9/meo/thread.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      434 2023-07-06 12:02:30.000000 meo-0.1.9/meo/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      332 2023-07-01 13:29:07.000000 meo-0.1.9/meo/wapper.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-12 01:45:37.587274 meo-0.1.9/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-12 01:45:37.000000 meo-0.1.9/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      429 2023-07-12 01:45:37.000000 meo-0.1.9/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-12 01:45:37.000000 meo-0.1.9/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-07-12 01:45:37.000000 meo-0.1.9/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-07-12 01:45:37.000000 meo-0.1.9/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-12 01:45:37.587274 meo-0.1.9/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-07-01 13:29:07.000000 meo-0.1.9/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-12 01:45:37.587274 meo-0.1.9/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)      435 2023-07-01 13:29:07.000000 meo-0.1.9/test/test.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-07-01 13:29:07.000000 meo-0.1.9/test/test_crack.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-07-01 13:29:07.000000 meo-0.1.9/test/test_imp.py
```

### Comparing `meo-0.1.8/LICENSE` & `meo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/PKG-INFO` & `meo-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.8
+Version: 0.1.9
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.8/meo/crack/cracker.py` & `meo-0.1.9/meo/crack/cracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
             if re:
                 info['key'] = re
                 pool.terminate()
         def create_gc_timer():
             gc_timer = threading.Timer(gc_interval, create_gc_timer)
             gc_timer.start()
             gc.collect()
-        # create_gc_timer()
-        gc_cnt = 1
+        create_gc_timer()
+        # gc_cnt = 1
         while True:
             try:
                 pwds_slice = itertools.islice(it, 0, slice_size)
                 if pwds_list := list(pwds_slice):
                     pwds, char_sizes = list(zip(*pwds_list))
                     char_size = char_sizes[-1]
                     pool.apply_async(self.step_some, (*pwds, ), callback=cb, error_callback=print)
@@ -59,19 +59,15 @@
                     return info['key']
                 else:
                     raise e
             if progressbar:
                 bar.set_postfix({
                     "char": char_size
                 }, refresh=False)
-            if gc_cnt % gc_interval == 0:
-                gc.collect()
-                gc_cnt = 1
-            else:
-                gc_cnt += 1
+            # gc.collect()
 
     def in_multiprocess_by_book(self, book:list, n_processes=None, chunksize=1000):
         pool = multiprocessing.Pool(n_processes)
         manager = multiprocessing.Manager()
         info = manager.dict()
         info['key'] = None
         def cb(pwds):
```

### Comparing `meo-0.1.8/meo/crack/pdf.py` & `meo-0.1.9/meo/crack/pdf.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo/crack/utils.py` & `meo-0.1.9/meo/crack/utils.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo/crack/zip.py` & `meo-0.1.9/meo/crack/zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,19 @@
         except:
             return False
 
     def step_once(self, pwd: bytes) -> bytes | None:
         zfile = ZipFile(self.path)
         mem = zfile.filelist[0].filename
         if self.test(zfile, pwd, mem):
-            del pwd
             return pwd
         del pwd
         return None
     
     def step_some(self, *pwds: bytes) -> bytes | None:
         zfile = ZipFile(self.path)
         mem = zfile.filelist[0].filename
         for pwd in pwds:
             if self.test(zfile, pwd, mem):
-                del pwds
                 return pwd
         del pwds
         return None
```

### Comparing `meo-0.1.8/meo/flask.py` & `meo-0.1.9/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo/io.py` & `meo-0.1.9/meo/io.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo/net.py` & `meo-0.1.9/meo/net.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo/screen.py` & `meo-0.1.9/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.8/meo.egg-info/PKG-INFO` & `meo-0.1.9/meo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.8
+Version: 0.1.9
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.8/setup.py` & `meo-0.1.9/setup.py`

 * *Files identical despite different names*

