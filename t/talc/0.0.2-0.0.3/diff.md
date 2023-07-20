# Comparing `tmp/talc-0.0.2.tar.gz` & `tmp/talc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.0.2.tar", last modified: Tue Jul 18 01:10:25 2023, max compression
+gzip compressed data, was "talc-0.0.3.tar", last modified: Thu Jul 20 20:30:26 2023, max compression
```

## Comparing `talc-0.0.2.tar` & `talc-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-18 01:10:25.056186 talc-0.0.2/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.2/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)      628 2023-07-18 01:10:25.056068 talc-0.0.2/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      274 2023-07-10 19:53:13.000000 talc-0.0.2/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      491 2023-07-18 01:08:31.000000 talc-0.0.2/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-18 01:10:25.056228 talc-0.0.2/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-18 01:10:25.054461 talc-0.0.2/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-18 01:10:25.054979 talc-0.0.2/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.2/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)     6533 2023-07-18 00:06:05.000000 talc-0.0.2/src/talc/talc.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-18 01:10:25.055897 talc-0.0.2/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)      628 2023-07-18 01:10:25.000000 talc-0.0.2/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-18 01:10:25.000000 talc-0.0.2/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-18 01:10:25.000000 talc-0.0.2/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-18 01:10:25.000000 talc-0.0.2/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-18 01:10:25.000000 talc-0.0.2/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.310779 talc-0.0.3/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.3/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)      648 2023-07-20 20:30:26.310655 talc-0.0.3/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      274 2023-07-10 19:53:13.000000 talc-0.0.3/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      531 2023-07-20 20:29:04.000000 talc-0.0.3/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-20 20:30:26.310814 talc-0.0.3/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.308798 talc-0.0.3/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.309282 talc-0.0.3/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.3/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)     6537 2023-07-20 20:28:21.000000 talc-0.0.3/src/talc/talc.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.310480 talc-0.0.3/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)      648 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.0.2/PKG-INFO` & `talc-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logging client for Talc.
-Author-email: Max Kerr <max@joinhomey.co>
+Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `talc-0.0.2/src/talc.egg-info/PKG-INFO` & `talc-0.0.3/src/talc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logging client for Talc.
-Author-email: Max Kerr <max@joinhomey.co>
+Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

