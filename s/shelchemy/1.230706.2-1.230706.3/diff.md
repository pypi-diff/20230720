# Comparing `tmp/shelchemy-1.230706.2.tar.gz` & `tmp/shelchemy-1.230706.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelchemy-1.230706.2.tar", max compression
+gzip compressed data, was "shelchemy-1.230706.3.tar", max compression
```

## Comparing `shelchemy-1.230706.2.tar` & `shelchemy-1.230706.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-1.230706.2/LICENSE
--rw-r--r--   0        0        0     1410 2023-07-19 22:22:01.860318 shelchemy-1.230706.2/README.md
--rw-r--r--   0        0        0     1036 2023-07-19 22:22:03.696319 shelchemy-1.230706.2/pyproject.toml
--rw-r--r--   0        0        0      501 2023-07-06 23:38:55.083313 shelchemy-1.230706.2/src/shelchemy/__init__.py
--rw-r--r--   0        0        0     8593 2023-07-19 22:21:56.700315 shelchemy-1.230706.2/src/shelchemy/cache.py
--rw-r--r--   0        0        0     1758 2022-09-06 20:21:46.000000 shelchemy-1.230706.2/src/shelchemy/lazy.py
--rw-r--r--   0        0        0     5350 2023-04-14 21:34:25.807393 shelchemy-1.230706.2/src/shelchemy/locker.py
--rw-r--r--   0        0        0     2097 2023-01-12 19:31:50.000000 shelchemy-1.230706.2/src/shelchemy/scheduler.py
--rw-r--r--   0        0        0      333 2023-07-06 23:38:55.087313 shelchemy-1.230706.2/src/shelchemy/sqla.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 shelchemy-1.230706.2/setup.py
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 shelchemy-1.230706.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-1.230706.3/LICENSE
+-rw-r--r--   0        0        0     1410 2023-07-20 20:06:07.115439 shelchemy-1.230706.3/README.md
+-rw-r--r--   0        0        0     1036 2023-07-20 20:06:09.495440 shelchemy-1.230706.3/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-06 23:38:55.083313 shelchemy-1.230706.3/src/shelchemy/__init__.py
+-rw-r--r--   0        0        0     8626 2023-07-20 20:05:10.823409 shelchemy-1.230706.3/src/shelchemy/cache.py
+-rw-r--r--   0        0        0     1758 2022-09-06 20:21:46.000000 shelchemy-1.230706.3/src/shelchemy/lazy.py
+-rw-r--r--   0        0        0     5398 2023-07-20 20:06:04.347437 shelchemy-1.230706.3/src/shelchemy/locker.py
+-rw-r--r--   0        0        0     2097 2023-01-12 19:31:50.000000 shelchemy-1.230706.3/src/shelchemy/scheduler.py
+-rw-r--r--   0        0        0      333 2023-07-06 23:38:55.087313 shelchemy-1.230706.3/src/shelchemy/sqla.py
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 shelchemy-1.230706.3/PKG-INFO
```

### Comparing `shelchemy-1.230706.2/LICENSE` & `shelchemy-1.230706.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shelchemy-1.230706.2/README.md` & `shelchemy-1.230706.3/README.md`

 * *Files identical despite different names*

### Comparing `shelchemy-1.230706.2/pyproject.toml` & `shelchemy-1.230706.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shelchemy"
-version = "1.230706.2"
+version = "1.230706.3"
 description = "Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "shelchemy", from = "src" }
 ]
```

### Comparing `shelchemy-1.230706.2/src/shelchemy/cache.py` & `shelchemy-1.230706.3/src/shelchemy/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 def check(key):
     if not isinstance(key, str):
         try:
             dump = dumps(key, protocol=5)
         except Exception as e:
             print(e)
             raise WrongKeyType(f"Key must be string or serializable (pickable), not {type(key)}.", key)
-        key = dump
-    return md5(key.encode()).hexdigest() if len(key) not in [32, 40] else key
+        key = md5(dump).hexdigest()
+    elif len(key) not in [32, 40]:
+        key = md5(key.encode()).hexdigest()
+    return key
 
 
 class Cache:
     r"""
     Dict-like persistence based on SQLAlchemy
 
     string or serializable (pickle) keys only
```

### Comparing `shelchemy-1.230706.2/src/shelchemy/lazy.py` & `shelchemy-1.230706.3/src/shelchemy/lazy.py`

 * *Files identical despite different names*

### Comparing `shelchemy-1.230706.2/src/shelchemy/locker.py` & `shelchemy-1.230706.3/src/shelchemy/locker.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,21 +98,23 @@
     ...    print(f"{name} processed!")
     'a' already done, skipping
     'b' already done, skipping
     'c' already done, skipping
     'd' already done, skipping
     'e' already done, skipping
     """
+    from shelchemy.cache import Cache
+
     if dict__url is None:
         ctx = partial(shelve.open, "/tmp/locker.db")
     elif isinstance(dict__url, str):
         from shelchemy.cache import sopen
 
         ctx = partial(sopen, dict__url, autopack=False)
-    elif isinstance(dict__url, dict) and hasattr(dict__url, "__contains__"):
+    elif isinstance(dict__url, (dict, Cache)) and hasattr(dict__url, "__contains__"):
 
         @contextmanager
         def ctx():
             yield dict__url
 
     else:
         ctx = dict__url
```

### Comparing `shelchemy-1.230706.2/src/shelchemy/scheduler.py` & `shelchemy-1.230706.3/src/shelchemy/scheduler.py`

 * *Files identical despite different names*

### Comparing `shelchemy-1.230706.2/PKG-INFO` & `shelchemy-1.230706.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelchemy
-Version: 1.230706.2
+Version: 1.230706.3
 Summary: Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks
 License: GPL
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shelchemy Version: 1.230706.2 Summary: Shelve-like
+Metadata-Version: 2.1 Name: shelchemy Version: 1.230706.3 Summary: Shelve-like
 dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks
 License: GPL Author: davips Author-email: dpsabc@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: full
 Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0) Requires-Dist: lz4 (>=4.0.2,<5.0.0)
 ; extra == "full" Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ;
```

