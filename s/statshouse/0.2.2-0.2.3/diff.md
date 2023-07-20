# Comparing `tmp/statshouse-0.2.2.tar.gz` & `tmp/statshouse-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statshouse-0.2.2.tar", last modified: Mon Jun  5 13:27:34 2023, max compression
+gzip compressed data, was "statshouse-0.2.3.tar", last modified: Thu Jul 20 09:17:16 2023, max compression
```

## Comparing `statshouse-0.2.2.tar` & `statshouse-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.2/LICENSE
--rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.2/README.md
--rw-r--r--   0        0        0     1083 2023-06-05 13:27:34.788701 statshouse-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      138 2023-06-05 13:22:06.791909 statshouse-0.2.2/src/statshouse/__init__.py
--rw-r--r--   0        0        0     3840 2023-06-05 13:22:06.787909 statshouse-0.2.2/src/statshouse/_statshouse.py
--rw-r--r--   0        0        0      191 2023-06-05 13:22:06.783909 statshouse-0.2.2/tests/test_statshouse.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    16727 2022-11-28 20:50:24.714223 statshouse-0.2.3/LICENSE
+-rw-r--r--   0        0        0      943 2023-05-25 16:09:41.327601 statshouse-0.2.3/README.md
+-rw-r--r--   0        0        0     1083 2023-07-20 09:17:16.590885 statshouse-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      138 2023-06-05 13:22:06.791909 statshouse-0.2.3/src/statshouse/__init__.py
+-rw-r--r--   0        0        0     3832 2023-07-20 09:14:33.703591 statshouse-0.2.3/src/statshouse/_statshouse.py
+-rw-r--r--   0        0        0      191 2023-06-05 13:22:06.783909 statshouse-0.2.3/tests/test_statshouse.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 statshouse-0.2.3/PKG-INFO
```

### Comparing `statshouse-0.2.2/LICENSE` & `statshouse-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.2/README.md` & `statshouse-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `statshouse-0.2.2/pyproject.toml` & `statshouse-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "statshouse"
-version = "0.2.2"
+version = "0.2.3"
 description = "StatsHouse client library for Python"
 authors = [
     { name = "Gregory Petrosyan", email = "pgregory@pgregory.net" },
 ]
 dependencies = [
     "msgpack>=1.0.5",
 ]
```

### Comparing `statshouse-0.2.2/src/statshouse/_statshouse.py` & `statshouse-0.2.3/src/statshouse/_statshouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         type=str,
         default=os.getenv("STATSHOUSE_ADDR", DEFAULT_STATSHOUSE_ADDR),
     )
     p.add_argument(
         "--statshouse-env", type=str, default=os.getenv("STATSHOUSE_ENV", "")
     )
 
-    args, left = p.parse_known_args(sys.argv)
+    args, left = p.parse_known_args()
     sys.argv = sys.argv[:1] + left
 
     return Client(addr=args.statshouse_addr, env=args.statshouse_env)
 
 
 __sh = _init_global()
```

### Comparing `statshouse-0.2.2/PKG-INFO` & `statshouse-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statshouse
-Version: 0.2.2
+Version: 0.2.3
 Summary: StatsHouse client library for Python
 Author-Email: Gregory Petrosyan <pgregory@pgregory.net>
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

