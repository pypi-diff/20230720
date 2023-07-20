# Comparing `tmp/chorde-1.0.8.tar.gz` & `tmp/chorde-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chorde-1.0.8.tar", last modified: Wed Jul 12 18:53:17 2023, max compression
+gzip compressed data, was "chorde-1.0.9.tar", last modified: Thu Jul 20 18:46:27 2023, max compression
```

## Comparing `chorde-1.0.8.tar` & `chorde-1.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.687903 chorde-1.0.8/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     8607 2023-07-12 18:52:32.000000 chorde-1.0.8/CHANGELOG
--rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.8/MANIFEST.in
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-07-12 18:53:17.687903 chorde-1.0.8/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.8/README.rst
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.675903 chorde-1.0.8/lib/
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.679903 chorde-1.0.8/lib/chorde/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.8/lib/chorde/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-07-12 18:52:28.000000 chorde-1.0.8/lib/chorde/_version.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.687903 chorde-1.0.8/lib/chorde/clients/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   727274 2023-07-12 18:52:48.000000 chorde-1.0.8/lib/chorde/clients/_async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.8/lib/chorde/clients/_async.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    16229 2023-07-12 18:52:28.000000 chorde-1.0.8/lib/chorde/clients/_async.pyx
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.8/lib/chorde/clients/async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2750357 2023-07-12 18:52:49.000000 chorde-1.0.8/lib/chorde/clients/asyncache.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    65512 2023-07-12 18:52:28.000000 chorde-1.0.8/lib/chorde/clients/asyncache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.8/lib/chorde/clients/base.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/coherent.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/elasticache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/files.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.8/lib/chorde/clients/inproc.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/inproc.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.8/lib/chorde/clients/memcached.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.8/lib/chorde/clients/tiered.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/clients/tiered.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.8/lib/chorde/decorators.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.8/lib/chorde/decorators.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/decorators.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/dnsutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/external_integration.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.687903 chorde-1.0.8/lib/chorde/mq/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.8/lib/chorde/mq/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/mq/coherence.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.8/lib/chorde/mq/compat.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.687903 chorde-1.0.8/lib/chorde/mq/ipsub/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.8/lib/chorde/mq/ipsub/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/mq/ipsub/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/mq/ipsub/ipsub_zmq.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4668 2023-06-27 18:15:41.000000 chorde-1.0.8/lib/chorde/sPickle.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.8/lib/chorde/serialize.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/shmemutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/threadpool.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.8/lib/chorde/worker.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-12 18:53:17.679903 chorde-1.0.8/lib/chorde.egg-info/
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-07-12 18:53:17.000000 chorde-1.0.8/lib/chorde.egg-info/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-07-12 18:53:17.000000 chorde-1.0.8/lib/chorde.egg-info/SOURCES.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-07-12 18:53:17.000000 chorde-1.0.8/lib/chorde.egg-info/dependency_links.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.8/lib/chorde.egg-info/not-zip-safe
--rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-07-12 18:53:17.000000 chorde-1.0.8/lib/chorde.egg-info/requires.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-07-12 18:53:17.000000 chorde-1.0.8/lib/chorde.egg-info/top_level.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.8/requirements.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-07-12 18:53:17.687903 chorde-1.0.8/setup.cfg
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-07-12 18:52:28.000000 chorde-1.0.8/setup.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.132484 chorde-1.0.9/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     8708 2023-07-20 18:45:03.000000 chorde-1.0.9/CHANGELOG
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.9/MANIFEST.in
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-07-20 18:46:27.132484 chorde-1.0.9/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.9/README.rst
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:26.920483 chorde-1.0.9/lib/
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.000484 chorde-1.0.9/lib/chorde/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.9/lib/chorde/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-07-20 18:44:45.000000 chorde-1.0.9/lib/chorde/_version.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.128484 chorde-1.0.9/lib/chorde/clients/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   747693 2023-07-20 18:46:20.000000 chorde-1.0.9/lib/chorde/clients/_async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      379 2023-07-20 18:44:45.000000 chorde-1.0.9/lib/chorde/clients/_async.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    16471 2023-07-20 18:44:45.000000 chorde-1.0.9/lib/chorde/clients/_async.pyx
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.9/lib/chorde/clients/async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2750357 2023-07-12 18:52:49.000000 chorde-1.0.9/lib/chorde/clients/asyncache.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    65512 2023-07-12 18:52:28.000000 chorde-1.0.9/lib/chorde/clients/asyncache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.9/lib/chorde/clients/base.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/coherent.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/elasticache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/files.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.9/lib/chorde/clients/inproc.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/inproc.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.9/lib/chorde/clients/memcached.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.9/lib/chorde/clients/tiered.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/clients/tiered.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.9/lib/chorde/decorators.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.9/lib/chorde/decorators.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/decorators.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/dnsutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/external_integration.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.132484 chorde-1.0.9/lib/chorde/mq/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.9/lib/chorde/mq/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/mq/coherence.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.9/lib/chorde/mq/compat.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.132484 chorde-1.0.9/lib/chorde/mq/ipsub/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.9/lib/chorde/mq/ipsub/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/mq/ipsub/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/mq/ipsub/ipsub_zmq.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4668 2023-06-27 18:15:41.000000 chorde-1.0.9/lib/chorde/sPickle.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.9/lib/chorde/serialize.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/shmemutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/threadpool.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.9/lib/chorde/worker.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-07-20 18:46:27.000484 chorde-1.0.9/lib/chorde.egg-info/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-07-20 18:46:26.000000 chorde-1.0.9/lib/chorde.egg-info/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-07-20 18:46:26.000000 chorde-1.0.9/lib/chorde.egg-info/SOURCES.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-07-20 18:46:26.000000 chorde-1.0.9/lib/chorde.egg-info/dependency_links.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.9/lib/chorde.egg-info/not-zip-safe
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-07-20 18:46:26.000000 chorde-1.0.9/lib/chorde.egg-info/requires.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-07-20 18:46:26.000000 chorde-1.0.9/lib/chorde.egg-info/top_level.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.9/requirements.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-07-20 18:46:27.136484 chorde-1.0.9/setup.cfg
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-07-20 18:44:45.000000 chorde-1.0.9/setup.py
```

### Comparing `chorde-1.0.8/CHANGELOG` & `chorde-1.0.9/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Change Log
 
 All notable changes to this project will be documented here.
 
+## [1.0.9] - 2023-07-20
+### Added
+- Fix Future's await implementation to be compatible with asyncio
+
 ## [1.0.8] - 2023-07-12
 ### Added
 - chorde.client.asyncache.Future is now awaitable
 
 ## [1.0.7] - 2023-06-29
 ### Bugfixes
 - Prevent memory leaks by clearing non-running traceback
```

### Comparing `chorde-1.0.8/PKG-INFO` & `chorde-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.8
+Version: 1.0.9
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.8/README.rst` & `chorde-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/__init__.py` & `chorde-1.0.9/lib/chorde/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/_async.c` & `chorde-1.0.9/lib/chorde/clients/_async.c`

 * *Files 0% similar despite different names*

```diff
@@ -970,14 +970,15 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "lib/chorde/clients/_async.pyx",
   "stringsource",
+  "lib/chorde/clients/_async.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6chorde_7clients_6_async_Future;
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper;
 struct __pyx_obj_6chorde_7clients_6_async_WeakCallback;
 struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback;
@@ -986,15 +987,15 @@
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback;
 struct __pyx_obj_6chorde_7clients_6_async_AnyCallback;
 struct __pyx_obj_6chorde_7clients_6_async_DoneCallback;
 struct __pyx_obj_6chorde_7clients_6_async_NONE;
 struct __pyx_obj_6chorde_7clients_6_async___pyx_scope_struct____await__;
 struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise;
 
-/* "chorde/clients/_async.pyx":50
+/* "chorde/clients/_async.pyx":51
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise {
@@ -1014,104 +1015,105 @@
   PyObject *_value;
   PyObject *_logger;
   PyObject *_done_event;
   PyObject *__weakref__;
   int _running;
   int _cancel_pending;
   int _cancelled;
+  int _asyncio_future_blocking;
 };
 
 
-/* "chorde/clients/_async.pyx":42
+/* "chorde/clients/_async.pyx":43
  * 
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:             # <<<<<<<<<<<<<<
  *     cdef public object value
  *     cdef object __weakref__
  */
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper {
   PyObject_HEAD
   struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *__pyx_vtab;
   PyObject *value;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":92
+/* "chorde/clients/_async.pyx":93
  * 
  * @cython.freelist(100)
  * cdef class WeakCallback:             # <<<<<<<<<<<<<<
  *     cdef object me, callback, __weakref__
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_WeakCallback {
   PyObject_HEAD
   PyObject *me;
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":106
+/* "chorde/clients/_async.pyx":107
  * 
  * @cython.freelist(100)
  * cdef class DeferExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback {
   PyObject_HEAD
   PyObject *defer;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":114
+/* "chorde/clients/_async.pyx":115
  * 
  * @cython.freelist(100)
  * cdef class ValueCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ValueCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":123
+/* "chorde/clients/_async.pyx":124
  * 
  * @cython.freelist(100)
  * cdef class MissCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_MissCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":132
+/* "chorde/clients/_async.pyx":133
  * 
  * @cython.freelist(100)
  * cdef class ExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":141
+/* "chorde/clients/_async.pyx":142
  * 
  * @cython.freelist(100)
  * cdef class AnyCallback:             # <<<<<<<<<<<<<<
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  */
 struct __pyx_obj_6chorde_7clients_6_async_AnyCallback {
@@ -1119,55 +1121,55 @@
   PyObject *on_value;
   PyObject *on_miss;
   PyObject *on_exc;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":159
+/* "chorde/clients/_async.pyx":160
  * 
  * @cython.freelist(100)
  * cdef class DoneCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DoneCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":166
+/* "chorde/clients/_async.pyx":167
  *         return self.callback()
  * 
  * cdef class NONE:             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_NONE {
   PyObject_HEAD
 };
 
 
-/* "chorde/clients/_async.pyx":227
+/* "chorde/clients/_async.pyx":229
  *             self._done_event.set()
  * 
  *     def __await__(self):             # <<<<<<<<<<<<<<
  *         if not self.c_done():
- *             return (yield self)
+ *             yield self
  */
 struct __pyx_obj_6chorde_7clients_6_async___pyx_scope_struct____await__ {
   PyObject_HEAD
   struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self;
 };
 
 
 
-/* "chorde/clients/_async.pyx":170
+/* "chorde/clients/_async.pyx":171
  * 
  * @cython.freelist(100)
  * cdef class Future:             # <<<<<<<<<<<<<<
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  */
 
@@ -1177,15 +1179,15 @@
   PyObject *(*_set_nothreads)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*set)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*_on_stuff)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *__pyx_vtabptr_6chorde_7clients_6_async_Future;
 
 
-/* "chorde/clients/_async.pyx":42
+/* "chorde/clients/_async.pyx":43
  * 
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:             # <<<<<<<<<<<<<<
  *     cdef public object value
  *     cdef object __weakref__
  */
 
@@ -1580,14 +1582,23 @@
 
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
+/* PatchModuleWithCoroutine.proto */
+static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
+
+/* PatchInspect.proto */
+static PyObject* __Pyx_patch_inspect(PyObject* module);
+
+/* PatchAsyncIO.proto */
+static PyObject* __Pyx_patch_asyncio(PyObject* module);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1706,17 +1717,14 @@
 #else
 #define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
     __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, pvalue)
 #endif
 static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *tstate, PyObject **pvalue);
 static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state);
 
-/* PatchModuleWithCoroutine.proto */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
-
 /* PatchGeneratorABC.proto */
 static int __Pyx_patch_abc(void);
 
 /* Generator.proto */
 #define __Pyx_Generator_USED
 static PyTypeObject *__pyx_GeneratorType = 0;
 #define __Pyx_Generator_CheckExact(obj) (Py_TYPE(obj) == __pyx_GeneratorType)
@@ -1767,14 +1775,15 @@
 /* Implementation of 'chorde.clients._async' */
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_TypeError;
 static const char __pyx_k_me[] = "me";
 static const char __pyx_k_exc[] = "exc";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_ref[] = "ref";
+static const char __pyx_k_run[] = "run";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_NONE[] = "NONE";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1795,14 +1804,17 @@
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_on_any[] = "on_any";
 static const char __pyx_k_on_exc[] = "on_exc";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reason[] = "reason";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
+static const char __pyx_k_asyncio[] = "asyncio";
+static const char __pyx_k_context[] = "context";
+static const char __pyx_k_inspect[] = "inspect";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_on_miss[] = "on_miss";
 static const char __pyx_k_partial[] = "partial";
 static const char __pyx_k_reraise[] = "reraise";
 static const char __pyx_k_tb_next[] = "tb_next";
 static const char __pyx_k_timeout[] = "timeout";
 static const char __pyx_k_weakref[] = "weakref";
@@ -1832,27 +1844,30 @@
 static const char __pyx_k_DoneCallback[] = "DoneCallback";
 static const char __pyx_k_MissCallback[] = "MissCallback";
 static const char __pyx_k_TimeoutError[] = "TimeoutError";
 static const char __pyx_k_WeakCallback[] = "WeakCallback";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_ValueCallback[] = "ValueCallback";
+static const char __pyx_k_asyncio_tasks[] = "asyncio.tasks";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_set_exception[] = "set_exception";
 static const char __pyx_k_set_nothreads[] = "_set_nothreads";
 static const char __pyx_k_CacheMissError[] = "CacheMissError";
 static const char __pyx_k_CancelledError[] = "CancelledError";
 static const char __pyx_k_Future___await[] = "Future.__await__";
 static const char __pyx_k_chorde_clients[] = "chorde.clients";
 static const char __pyx_k_with_traceback[] = "with_traceback";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_ExceptionWrapper[] = "ExceptionWrapper";
+static const char __pyx_k_get_running_loop[] = "get_running_loop";
 static const char __pyx_k_ExceptionCallback[] = "ExceptionCallback";
 static const char __pyx_k_pyx_unpickle_NONE[] = "__pyx_unpickle_NONE";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_set_strip_tracebacks[] = "set_strip_tracebacks";
 static const char __pyx_k_chorde_clients__async[] = "chorde.clients._async";
 static const char __pyx_k_DeferExceptionCallback[] = "DeferExceptionCallback";
 static const char __pyx_k_Error_in_async_callback[] = "Error in async callback";
 static const char __pyx_k_lib_chorde_clients__async_pyx[] = "lib/chorde/clients/_async.pyx";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())";
@@ -1875,30 +1890,36 @@
 static PyObject *__pyx_n_s_NONE;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TimeoutError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueCallback;
 static PyObject *__pyx_n_s_WeakCallback;
 static PyObject *__pyx_n_s_args;
+static PyObject *__pyx_n_s_asyncio;
+static PyObject *__pyx_n_s_asyncio_coroutines;
+static PyObject *__pyx_n_s_asyncio_tasks;
 static PyObject *__pyx_n_s_await;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_callback;
 static PyObject *__pyx_n_s_chorde_clients;
 static PyObject *__pyx_n_s_chorde_clients__async;
 static PyObject *__pyx_n_s_clear;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
+static PyObject *__pyx_n_s_context;
 static PyObject *__pyx_n_s_defer;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_exc;
 static PyObject *__pyx_n_s_exc_info;
 static PyObject *__pyx_n_s_functools;
+static PyObject *__pyx_n_s_get_running_loop;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_inspect;
 static PyObject *__pyx_kp_s_lib_chorde_clients__async_pyx;
 static PyObject *__pyx_n_s_logger;
 static PyObject *__pyx_n_s_logging;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_me;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
@@ -1920,14 +1941,15 @@
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_reason;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_ref;
 static PyObject *__pyx_n_s_reraise;
+static PyObject *__pyx_n_s_run;
 static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_set_exception;
 static PyObject *__pyx_n_s_set_nothreads;
 static PyObject *__pyx_n_s_set_result;
 static PyObject *__pyx_n_s_set_strip_tracebacks;
 static PyObject *__pyx_n_s_setstate;
@@ -1985,14 +2007,15 @@
 static PyObject *__pyx_pf_6chorde_7clients_6_async_12DoneCallback_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_4NONE___reduce_cython__(struct __pyx_obj_6chorde_7clients_6_async_NONE *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_4NONE_2__setstate_cython__(struct __pyx_obj_6chorde_7clients_6_async_NONE *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_logger); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_2_set_nothreads(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_4set(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_6__await__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_5_loop___get__(CYTHON_UNUSED struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_9set_result(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_11miss(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_13_miss_nothreads(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_15exc(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_exc_info); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_17_exc_nothreads(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_exc_info); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_19set_exception(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_exception); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_21on_value(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback); /* proto */
@@ -2000,23 +2023,25 @@
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_25on_exc(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_27on_any(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_on_value, PyObject *__pyx_v_on_miss, PyObject *__pyx_v_on_exc); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_29on_any_once(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_on_value, PyObject *__pyx_v_on_miss, PyObject *__pyx_v_on_exc); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_31on_done(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_33chain(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_defer); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_35chain_std(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_defer); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_37_on_stuff(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback); /* proto */
-static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback); /* proto */
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback, PyObject *__pyx_v_context); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_41done(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_43running(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_45cancelled(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_47cancel_pending(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_49cancel(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_51set_running_or_notify_cancelled(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_53result(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_timeout, PyObject *__pyx_v_norecurse); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_55exception(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_timeout); /* proto */
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking___get__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
+static int __pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_2__set__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_57__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_59__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_6chorde_7clients_6_async_2__pyx_unpickle_NONE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_6chorde_7clients_6_async_Future(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -2053,15 +2078,15 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_codeobj__22;
 static PyObject *__pyx_codeobj__24;
 /* Late includes */
 
-/* "chorde/clients/_async.pyx":29
+/* "chorde/clients/_async.pyx":30
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
 
@@ -2074,15 +2099,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_strip_tracebacks (wrapper)", 0);
   assert(__pyx_arg_strip); {
-    __pyx_v_strip = __Pyx_PyObject_IsTrue(__pyx_arg_strip); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
+    __pyx_v_strip = __Pyx_PyObject_IsTrue(__pyx_arg_strip); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.set_strip_tracebacks", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -2094,39 +2119,39 @@
 }
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_set_strip_tracebacks(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_strip) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_strip_tracebacks", 0);
 
-  /* "chorde/clients/_async.pyx":38
+  /* "chorde/clients/_async.pyx":39
  *     """
  *     global strip_tracebacks
  *     strip_tracebacks = strip             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_6chorde_7clients_6_async_strip_tracebacks = __pyx_v_strip;
 
-  /* "chorde/clients/_async.pyx":29
+  /* "chorde/clients/_async.pyx":30
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":46
+/* "chorde/clients/_async.pyx":47
  *     cdef object __weakref__
  * 
  *     def __cinit__(self, value):             # <<<<<<<<<<<<<<
  *         self.value = value
  * 
  */
 
@@ -2155,26 +2180,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 47, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 47, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_self), __pyx_v_value);
 
@@ -2184,42 +2209,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":47
+  /* "chorde/clients/_async.pyx":48
  * 
  *     def __cinit__(self, value):
  *         self.value = value             # <<<<<<<<<<<<<<
  * 
  *     @cython.ccall
  */
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   __Pyx_GOTREF(__pyx_v_self->value);
   __Pyx_DECREF(__pyx_v_self->value);
   __pyx_v_self->value = __pyx_v_value;
 
-  /* "chorde/clients/_async.pyx":46
+  /* "chorde/clients/_async.pyx":47
  *     cdef object __weakref__
  * 
  *     def __cinit__(self, value):             # <<<<<<<<<<<<<<
  *         self.value = value
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":50
+/* "chorde/clients/_async.pyx":51
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 
@@ -2267,19 +2292,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reraise); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reraise); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_16ExceptionWrapper_3reraise)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2287,15 +2312,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2308,77 +2333,77 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":51
+  /* "chorde/clients/_async.pyx":52
  *     @cython.ccall
  *     def reraise(self, bint strip=True):
  *         exc = self.value             # <<<<<<<<<<<<<<
  *         if strip:
  *             del self.value
  */
   __pyx_t_1 = __pyx_v_self->value;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_exc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":52
+  /* "chorde/clients/_async.pyx":53
  *     def reraise(self, bint strip=True):
  *         exc = self.value
  *         if strip:             # <<<<<<<<<<<<<<
  *             del self.value
  *         try:
  */
   __pyx_t_6 = (__pyx_v_strip != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":53
+    /* "chorde/clients/_async.pyx":54
  *         exc = self.value
  *         if strip:
  *             del self.value             # <<<<<<<<<<<<<<
  *         try:
  *             exc_typ, exc_obj, exc_tb = exc
  */
-    if (__Pyx_PyObject_DelAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    if (__Pyx_PyObject_DelAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_value) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":52
+    /* "chorde/clients/_async.pyx":53
  *     def reraise(self, bint strip=True):
  *         exc = self.value
  *         if strip:             # <<<<<<<<<<<<<<
  *             del self.value
  *         try:
  */
   }
 
-  /* "chorde/clients/_async.pyx":54
+  /* "chorde/clients/_async.pyx":55
  *         if strip:
  *             del self.value
  *         try:             # <<<<<<<<<<<<<<
  *             exc_typ, exc_obj, exc_tb = exc
  *         finally:
  */
   /*try:*/ {
 
-    /* "chorde/clients/_async.pyx":55
+    /* "chorde/clients/_async.pyx":56
  *             del self.value
  *         try:
  *             exc_typ, exc_obj, exc_tb = exc             # <<<<<<<<<<<<<<
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  */
     if ((likely(PyTuple_CheckExact(__pyx_v_exc))) || (PyList_CheckExact(__pyx_v_exc))) {
       PyObject* sequence = __pyx_v_exc;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 55, __pyx_L5_error)
+        __PYX_ERR(0, 56, __pyx_L5_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
@@ -2386,52 +2411,52 @@
         __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
         __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
       }
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_3 = PyObject_GetIter(__pyx_v_exc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L5_error)
+      __pyx_t_3 = PyObject_GetIter(__pyx_v_exc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext;
       index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_1);
       index = 1; __pyx_t_2 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_2)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
       index = 2; __pyx_t_4 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_4)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 3) < 0) __PYX_ERR(0, 55, __pyx_L5_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 3) < 0) __PYX_ERR(0, 56, __pyx_L5_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       goto __pyx_L8_unpacking_done;
       __pyx_L7_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 55, __pyx_L5_error)
+      __PYX_ERR(0, 56, __pyx_L5_error)
       __pyx_L8_unpacking_done:;
     }
     __pyx_v_exc_typ = __pyx_t_1;
     __pyx_t_1 = 0;
     __pyx_v_exc_obj = __pyx_t_2;
     __pyx_t_2 = 0;
     __pyx_v_exc_tb = __pyx_t_4;
     __pyx_t_4 = 0;
   }
 
-  /* "chorde/clients/_async.pyx":58
+  /* "chorde/clients/_async.pyx":59
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  *             del exc             # <<<<<<<<<<<<<<
  *         try:
  *             if not strip:
  */
   /*finally:*/ {
@@ -2476,46 +2501,46 @@
       __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
       __pyx_lineno = __pyx_t_8; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
       goto __pyx_L1_error;
     }
     __pyx_L6:;
   }
 
-  /* "chorde/clients/_async.pyx":59
+  /* "chorde/clients/_async.pyx":60
  *             # Don't leave references to the exc/tb in the frame
  *             del exc
  *         try:             # <<<<<<<<<<<<<<
  *             if not strip:
  *                 kwargs = {}
  */
   /*try:*/ {
 
-    /* "chorde/clients/_async.pyx":60
+    /* "chorde/clients/_async.pyx":61
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
  *                 kwargs = {}
  *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  */
     __pyx_t_6 = ((!(__pyx_v_strip != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "chorde/clients/_async.pyx":61
+      /* "chorde/clients/_async.pyx":62
  *         try:
  *             if not strip:
  *                 kwargs = {}             # <<<<<<<<<<<<<<
  *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  *                     # Workaround for tornado's HTTPError which does not function
  */
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L12_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_v_kwargs = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "chorde/clients/_async.pyx":62
+      /* "chorde/clients/_async.pyx":63
  *             if not strip:
  *                 kwargs = {}
  *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  */
       __pyx_t_17 = (__pyx_v_6chorde_7clients_6_async__HTTPError != Py_None);
@@ -2523,107 +2548,107 @@
       if (__pyx_t_18) {
       } else {
         __pyx_t_6 = __pyx_t_18;
         goto __pyx_L16_bool_binop_done;
       }
       __pyx_t_4 = __pyx_v_6chorde_7clients_6_async__HTTPError;
       __Pyx_INCREF(__pyx_t_4);
-      __pyx_t_18 = PyObject_IsInstance(__pyx_v_exc_obj, __pyx_t_4); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L12_error)
+      __pyx_t_18 = PyObject_IsInstance(__pyx_v_exc_obj, __pyx_t_4); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 63, __pyx_L12_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_17 = (__pyx_t_18 != 0);
       __pyx_t_6 = __pyx_t_17;
       __pyx_L16_bool_binop_done:;
       if (__pyx_t_6) {
 
-        /* "chorde/clients/_async.pyx":65
+        /* "chorde/clients/_async.pyx":66
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  *                     kwargs["reason"] = exc_obj.reason             # <<<<<<<<<<<<<<
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_reason); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L12_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_reason); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_4);
-        if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_reason, __pyx_t_4) < 0)) __PYX_ERR(0, 65, __pyx_L12_error)
+        if (unlikely(PyDict_SetItem(__pyx_v_kwargs, __pyx_n_s_reason, __pyx_t_4) < 0)) __PYX_ERR(0, 66, __pyx_L12_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "chorde/clients/_async.pyx":62
+        /* "chorde/clients/_async.pyx":63
  *             if not strip:
  *                 kwargs = {}
  *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):             # <<<<<<<<<<<<<<
  *                     # Workaround for tornado's HTTPError which does not function
  *                     # correctly without a reason, and reason is given only as kwarg
  */
       }
 
-      /* "chorde/clients/_async.pyx":66
+      /* "chorde/clients/_async.pyx":67
  *                     # correctly without a reason, and reason is given only as kwarg
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj             # <<<<<<<<<<<<<<
  *             elif exc_tb is not None:
  *                 # clear any non-running traceback's frames to avoid leaking locals
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_args); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_args); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L12_error)
+      __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
+      __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_v_exc_typ, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L12_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_v_exc_typ, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, __pyx_v_exc_obj);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 66, __pyx_L12_error)
+      __PYX_ERR(0, 67, __pyx_L12_error)
 
-      /* "chorde/clients/_async.pyx":60
+      /* "chorde/clients/_async.pyx":61
  *             del exc
  *         try:
  *             if not strip:             # <<<<<<<<<<<<<<
  *                 kwargs = {}
  *                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
  */
     }
 
-    /* "chorde/clients/_async.pyx":67
+    /* "chorde/clients/_async.pyx":68
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
  *                 # clear any non-running traceback's frames to avoid leaking locals
  *                 tb = exc_tb
  */
     __pyx_t_6 = (__pyx_v_exc_tb != Py_None);
     __pyx_t_17 = (__pyx_t_6 != 0);
     if (__pyx_t_17) {
 
-      /* "chorde/clients/_async.pyx":69
+      /* "chorde/clients/_async.pyx":70
  *             elif exc_tb is not None:
  *                 # clear any non-running traceback's frames to avoid leaking locals
  *                 tb = exc_tb             # <<<<<<<<<<<<<<
  *                 while tb is not None:
  *                     try:
  */
       __Pyx_INCREF(__pyx_v_exc_tb);
       __pyx_v_tb = __pyx_v_exc_tb;
 
-      /* "chorde/clients/_async.pyx":70
+      /* "chorde/clients/_async.pyx":71
  *                 # clear any non-running traceback's frames to avoid leaking locals
  *                 tb = exc_tb
  *                 while tb is not None:             # <<<<<<<<<<<<<<
  *                     try:
  *                         tb.tb_frame.clear()
  */
       while (1) {
         __pyx_t_17 = (__pyx_v_tb != Py_None);
         __pyx_t_6 = (__pyx_t_17 != 0);
         if (!__pyx_t_6) break;
 
-        /* "chorde/clients/_async.pyx":71
+        /* "chorde/clients/_async.pyx":72
  *                 tb = exc_tb
  *                 while tb is not None:
  *                     try:             # <<<<<<<<<<<<<<
  *                         tb.tb_frame.clear()
  *                     except:
  */
         {
@@ -2631,44 +2656,44 @@
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_16);
           __Pyx_XGOTREF(__pyx_t_15);
           __Pyx_XGOTREF(__pyx_t_14);
           /*try:*/ {
 
-            /* "chorde/clients/_async.pyx":72
+            /* "chorde/clients/_async.pyx":73
  *                 while tb is not None:
  *                     try:
  *                         tb.tb_frame.clear()             # <<<<<<<<<<<<<<
  *                     except:
  *                         pass
  */
-            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_frame); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L20_error)
+            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_frame); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L20_error)
+            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __pyx_t_4 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
               __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
               if (likely(__pyx_t_4)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
                 __Pyx_INCREF(__pyx_t_4);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_2, function);
               }
             }
             __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L20_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-            /* "chorde/clients/_async.pyx":71
+            /* "chorde/clients/_async.pyx":72
  *                 tb = exc_tb
  *                 while tb is not None:
  *                     try:             # <<<<<<<<<<<<<<
  *                         tb.tb_frame.clear()
  *                     except:
  */
           }
@@ -2679,15 +2704,15 @@
           __pyx_L20_error:;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          /* "chorde/clients/_async.pyx":73
+          /* "chorde/clients/_async.pyx":74
  *                     try:
  *                         tb.tb_frame.clear()
  *                     except:             # <<<<<<<<<<<<<<
  *                         pass
  *                     tb = tb.tb_next
  */
           /*except:*/ {
@@ -2698,108 +2723,108 @@
           __Pyx_XGIVEREF(__pyx_t_16);
           __Pyx_XGIVEREF(__pyx_t_15);
           __Pyx_XGIVEREF(__pyx_t_14);
           __Pyx_ExceptionReset(__pyx_t_16, __pyx_t_15, __pyx_t_14);
           __pyx_L27_try_end:;
         }
 
-        /* "chorde/clients/_async.pyx":75
+        /* "chorde/clients/_async.pyx":76
  *                     except:
  *                         pass
  *                     tb = tb.tb_next             # <<<<<<<<<<<<<<
  * 
  *                 if exc_obj is not None:
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_next); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L12_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_next); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF_SET(__pyx_v_tb, __pyx_t_1);
         __pyx_t_1 = 0;
       }
 
-      /* "chorde/clients/_async.pyx":77
+      /* "chorde/clients/_async.pyx":78
  *                     tb = tb.tb_next
  * 
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
       __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
       __pyx_t_17 = (__pyx_t_6 != 0);
       if (likely(__pyx_t_17)) {
 
-        /* "chorde/clients/_async.pyx":78
+        /* "chorde/clients/_async.pyx":79
  * 
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
-        __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L12_error)
+        __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_17 = (__pyx_t_1 != __pyx_v_exc_tb);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_6 = (__pyx_t_17 != 0);
         if (__pyx_t_6) {
 
-          /* "chorde/clients/_async.pyx":79
+          /* "chorde/clients/_async.pyx":80
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *                     raise exc_obj
  *                 else:
  */
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L12_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_4 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_4)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
               __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_2, function);
             }
           }
           __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exc_tb);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L12_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF_SET(__pyx_v_exc_obj, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          /* "chorde/clients/_async.pyx":78
+          /* "chorde/clients/_async.pyx":79
  * 
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
         }
 
-        /* "chorde/clients/_async.pyx":80
+        /* "chorde/clients/_async.pyx":81
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  */
         __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-        __PYX_ERR(0, 80, __pyx_L12_error)
+        __PYX_ERR(0, 81, __pyx_L12_error)
 
-        /* "chorde/clients/_async.pyx":77
+        /* "chorde/clients/_async.pyx":78
  *                     tb = tb.tb_next
  * 
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
       }
 
-      /* "chorde/clients/_async.pyx":82
+      /* "chorde/clients/_async.pyx":83
  *                     raise exc_obj
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *             elif exc_obj is not None:
  *                 raise exc_obj
  */
       /*else*/ {
@@ -2812,80 +2837,80 @@
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L12_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L12_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_exc_tb);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L12_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __PYX_ERR(0, 82, __pyx_L12_error)
+        __PYX_ERR(0, 83, __pyx_L12_error)
       }
 
-      /* "chorde/clients/_async.pyx":67
+      /* "chorde/clients/_async.pyx":68
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
  *                 # clear any non-running traceback's frames to avoid leaking locals
  *                 tb = exc_tb
  */
     }
 
-    /* "chorde/clients/_async.pyx":83
+    /* "chorde/clients/_async.pyx":84
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
     __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
     __pyx_t_17 = (__pyx_t_6 != 0);
     if (unlikely(__pyx_t_17)) {
 
-      /* "chorde/clients/_async.pyx":84
+      /* "chorde/clients/_async.pyx":85
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:
  *                 raise exc_obj             # <<<<<<<<<<<<<<
  *             else:
  *                 raise exc_typ()
  */
       __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-      __PYX_ERR(0, 84, __pyx_L12_error)
+      __PYX_ERR(0, 85, __pyx_L12_error)
 
-      /* "chorde/clients/_async.pyx":83
+      /* "chorde/clients/_async.pyx":84
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":86
+    /* "chorde/clients/_async.pyx":87
  *                 raise exc_obj
  *             else:
  *                 raise exc_typ()             # <<<<<<<<<<<<<<
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  */
     /*else*/ {
@@ -2898,24 +2923,24 @@
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L12_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 86, __pyx_L12_error)
+      __PYX_ERR(0, 87, __pyx_L12_error)
     }
   }
 
-  /* "chorde/clients/_async.pyx":89
+  /* "chorde/clients/_async.pyx":90
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  *             del exc_typ, exc_obj, exc_tb             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
   /*finally:*/ {
@@ -2958,15 +2983,15 @@
       __Pyx_ErrRestore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
       __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_9; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_19;
       goto __pyx_L1_error;
     }
   }
 
-  /* "chorde/clients/_async.pyx":50
+  /* "chorde/clients/_async.pyx":51
  * 
  *     @cython.ccall
  *     def reraise(self, bint strip=True):             # <<<<<<<<<<<<<<
  *         exc = self.value
  *         if strip:
  */
 
@@ -3018,33 +3043,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_strip);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reraise") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reraise") < 0)) __PYX_ERR(0, 51, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_strip = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
+      __pyx_v_strip = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_strip == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
     } else {
       __pyx_v_strip = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("reraise", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("reraise", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 51, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.reraise", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_16ExceptionWrapper_2reraise(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_self), __pyx_v_strip);
 
@@ -3061,15 +3086,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reraise", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.strip = __pyx_v_strip;
-  __pyx_t_1 = __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper->reraise(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper->reraise(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3078,15 +3103,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":43
+/* "chorde/clients/_async.pyx":44
  * @cython.freelist(100)
  * cdef class ExceptionWrapper:
  *     cdef public object value             # <<<<<<<<<<<<<<
  *     cdef object __weakref__
  * 
  */
 
@@ -3286,15 +3311,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":95
+/* "chorde/clients/_async.pyx":96
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3328,32 +3353,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_me)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 95, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 96, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 95, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 96, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_me = values[0];
     __pyx_v_callback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 95, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 96, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_me, __pyx_v_callback);
 
@@ -3369,15 +3394,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":96
+  /* "chorde/clients/_async.pyx":97
  * 
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)             # <<<<<<<<<<<<<<
  *         self.callback = callback
  * 
  */
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_wref);
@@ -3389,37 +3414,37 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->me);
   __Pyx_DECREF(__pyx_v_self->me);
   __pyx_v_self->me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":97
+  /* "chorde/clients/_async.pyx":98
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)
  *         self.callback = callback             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":95
+  /* "chorde/clients/_async.pyx":96
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3433,15 +3458,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":99
+/* "chorde/clients/_async.pyx":100
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3470,26 +3495,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 100, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 99, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 100, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3508,15 +3533,15 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":101
+  /* "chorde/clients/_async.pyx":102
  *     def __call__(self, value):
  *         cdef object me
  *         me = self.me()             # <<<<<<<<<<<<<<
  *         if me is not None:
  *             return self.callback(me)
  */
   __Pyx_INCREF(__pyx_v_self->me);
@@ -3528,32 +3553,32 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":102
+  /* "chorde/clients/_async.pyx":103
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   __pyx_t_4 = (__pyx_v_me != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":103
+    /* "chorde/clients/_async.pyx":104
  *         me = self.me()
  *         if me is not None:
  *             return self.callback(me)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -3566,31 +3591,31 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":102
+    /* "chorde/clients/_async.pyx":103
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":99
+  /* "chorde/clients/_async.pyx":100
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3719,15 +3744,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":108
+/* "chorde/clients/_async.pyx":109
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
@@ -3756,26 +3781,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defer)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 108, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_defer = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 108, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 109, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_defer);
 
@@ -3785,42 +3810,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *__pyx_v_self, PyObject *__pyx_v_defer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":109
+  /* "chorde/clients/_async.pyx":110
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  *         self.defer = defer             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])
  */
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   __Pyx_GOTREF(__pyx_v_self->defer);
   __Pyx_DECREF(__pyx_v_self->defer);
   __pyx_v_self->defer = __pyx_v_defer;
 
-  /* "chorde/clients/_async.pyx":108
+  /* "chorde/clients/_async.pyx":109
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":110
+/* "chorde/clients/_async.pyx":111
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -3849,26 +3874,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 111, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 111, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3886,35 +3911,35 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":111
+  /* "chorde/clients/_async.pyx":112
  *         self.defer = defer
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 112, __pyx_L1_error)
   if (!__pyx_t_5) {
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
@@ -3925,20 +3950,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":110
+  /* "chorde/clients/_async.pyx":111
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -4067,15 +4092,15 @@
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":116
+/* "chorde/clients/_async.pyx":117
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4104,26 +4129,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4133,42 +4158,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":117
+  /* "chorde/clients/_async.pyx":118
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":116
+  /* "chorde/clients/_async.pyx":117
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":118
+/* "chorde/clients/_async.pyx":119
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4197,26 +4222,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4235,15 +4260,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":119
+  /* "chorde/clients/_async.pyx":120
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_2 = (__pyx_v_value != __pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -4255,15 +4280,15 @@
   }
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":120
+    /* "chorde/clients/_async.pyx":121
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4276,31 +4301,31 @@
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":119
+    /* "chorde/clients/_async.pyx":120
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":118
+  /* "chorde/clients/_async.pyx":119
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4428,15 +4453,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":125
+/* "chorde/clients/_async.pyx":126
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4465,26 +4490,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 126, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 126, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4494,42 +4519,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_MissCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":126
+  /* "chorde/clients/_async.pyx":127
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":125
+  /* "chorde/clients/_async.pyx":126
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":127
+/* "chorde/clients/_async.pyx":128
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4558,26 +4583,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 128, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 128, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4595,26 +4620,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":128
+  /* "chorde/clients/_async.pyx":129
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":129
+    /* "chorde/clients/_async.pyx":130
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4627,31 +4652,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":128
+    /* "chorde/clients/_async.pyx":129
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":127
+  /* "chorde/clients/_async.pyx":128
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4779,15 +4804,15 @@
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":134
+/* "chorde/clients/_async.pyx":135
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4816,26 +4841,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4845,42 +4870,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":135
+  /* "chorde/clients/_async.pyx":136
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":134
+  /* "chorde/clients/_async.pyx":135
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":136
+/* "chorde/clients/_async.pyx":137
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4909,26 +4934,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 137, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 136, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 137, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4946,26 +4971,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":137
+  /* "chorde/clients/_async.pyx":138
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":138
+    /* "chorde/clients/_async.pyx":139
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4978,31 +5003,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":137
+    /* "chorde/clients/_async.pyx":138
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":136
+  /* "chorde/clients/_async.pyx":137
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -5130,15 +5155,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":143
+/* "chorde/clients/_async.pyx":144
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
@@ -5175,40 +5200,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_miss)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 143, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 143, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 144, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 143, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 143, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -5218,68 +5243,68 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *__pyx_v_self, PyObject *__pyx_v_on_value, PyObject *__pyx_v_on_miss, PyObject *__pyx_v_on_exc) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":144
+  /* "chorde/clients/_async.pyx":145
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value             # <<<<<<<<<<<<<<
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  */
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   __Pyx_GOTREF(__pyx_v_self->on_value);
   __Pyx_DECREF(__pyx_v_self->on_value);
   __pyx_v_self->on_value = __pyx_v_on_value;
 
-  /* "chorde/clients/_async.pyx":145
+  /* "chorde/clients/_async.pyx":146
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value
  *         self.on_miss = on_miss             # <<<<<<<<<<<<<<
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   __Pyx_GOTREF(__pyx_v_self->on_miss);
   __Pyx_DECREF(__pyx_v_self->on_miss);
   __pyx_v_self->on_miss = __pyx_v_on_miss;
 
-  /* "chorde/clients/_async.pyx":146
+  /* "chorde/clients/_async.pyx":147
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   __Pyx_GOTREF(__pyx_v_self->on_exc);
   __Pyx_DECREF(__pyx_v_self->on_exc);
   __pyx_v_self->on_exc = __pyx_v_on_exc;
 
-  /* "chorde/clients/_async.pyx":143
+  /* "chorde/clients/_async.pyx":144
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":147
+/* "chorde/clients/_async.pyx":148
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -5308,26 +5333,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 147, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 147, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5345,37 +5370,37 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":148
+  /* "chorde/clients/_async.pyx":149
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":149
+    /* "chorde/clients/_async.pyx":150
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     __pyx_t_2 = (__pyx_v_self->on_miss != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":150
+      /* "chorde/clients/_async.pyx":151
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  *                 return self.on_miss()             # <<<<<<<<<<<<<<
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5388,63 +5413,63 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":149
+      /* "chorde/clients/_async.pyx":150
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     }
 
-    /* "chorde/clients/_async.pyx":148
+    /* "chorde/clients/_async.pyx":149
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":151
+  /* "chorde/clients/_async.pyx":152
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":152
+    /* "chorde/clients/_async.pyx":153
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     __pyx_t_2 = (__pyx_v_self->on_exc != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":153
+      /* "chorde/clients/_async.pyx":154
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)             # <<<<<<<<<<<<<<
  *         else:
  *             if self.on_value is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5457,53 +5482,53 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":152
+      /* "chorde/clients/_async.pyx":153
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":151
+    /* "chorde/clients/_async.pyx":152
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":155
+  /* "chorde/clients/_async.pyx":156
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_self->on_value != Py_None);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":156
+      /* "chorde/clients/_async.pyx":157
  *         else:
  *             if self.on_value is not None:
  *                 return self.on_value(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5516,33 +5541,33 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":155
+      /* "chorde/clients/_async.pyx":156
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":147
+  /* "chorde/clients/_async.pyx":148
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -5670,15 +5695,15 @@
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":161
+/* "chorde/clients/_async.pyx":162
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -5707,26 +5732,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 162, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -5736,42 +5761,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":162
+  /* "chorde/clients/_async.pyx":163
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         return self.callback()
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":161
+  /* "chorde/clients/_async.pyx":162
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":163
+/* "chorde/clients/_async.pyx":164
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -5800,26 +5825,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 163, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 163, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 164, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5835,15 +5860,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":164
+  /* "chorde/clients/_async.pyx":165
  *         self.callback = callback
  *     def __call__(self, value):
  *         return self.callback()             # <<<<<<<<<<<<<<
  * 
  * cdef class NONE:
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5856,22 +5881,22 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":163
+  /* "chorde/clients/_async.pyx":164
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -6284,15 +6309,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":171
+/* "chorde/clients/_async.pyx":172
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
@@ -6324,29 +6349,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_logger);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 171, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 172, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_logger = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 171, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 172, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_logger);
 
@@ -6356,109 +6381,118 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_logger) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":172
+  /* "chorde/clients/_async.pyx":173
  * cdef class Future:
  *     def __cinit__(self, logger = None):
  *         self._cb = None             # <<<<<<<<<<<<<<
  *         self._value = NONE
  *         self._logger = logger
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_cb);
   __Pyx_DECREF(__pyx_v_self->_cb);
   __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-  /* "chorde/clients/_async.pyx":173
+  /* "chorde/clients/_async.pyx":174
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  *         self._value = NONE             # <<<<<<<<<<<<<<
  *         self._logger = logger
  *         self._done_event = None
  */
   __Pyx_INCREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GOTREF(__pyx_v_self->_value);
   __Pyx_DECREF(__pyx_v_self->_value);
   __pyx_v_self->_value = ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE);
 
-  /* "chorde/clients/_async.pyx":174
+  /* "chorde/clients/_async.pyx":175
  *         self._cb = None
  *         self._value = NONE
  *         self._logger = logger             # <<<<<<<<<<<<<<
  *         self._done_event = None
  *         self._running = 0
  */
   __Pyx_INCREF(__pyx_v_logger);
   __Pyx_GIVEREF(__pyx_v_logger);
   __Pyx_GOTREF(__pyx_v_self->_logger);
   __Pyx_DECREF(__pyx_v_self->_logger);
   __pyx_v_self->_logger = __pyx_v_logger;
 
-  /* "chorde/clients/_async.pyx":175
+  /* "chorde/clients/_async.pyx":176
  *         self._value = NONE
  *         self._logger = logger
  *         self._done_event = None             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         self._cancel_pending = 0
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_done_event);
   __Pyx_DECREF(__pyx_v_self->_done_event);
   __pyx_v_self->_done_event = Py_None;
 
-  /* "chorde/clients/_async.pyx":176
+  /* "chorde/clients/_async.pyx":177
  *         self._logger = logger
  *         self._done_event = None
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         self._cancel_pending = 0
  *         self._cancelled = 0
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":177
+  /* "chorde/clients/_async.pyx":178
  *         self._done_event = None
  *         self._running = 0
  *         self._cancel_pending = 0             # <<<<<<<<<<<<<<
  *         self._cancelled = 0
- * 
+ *         self._asyncio_future_blocking = True
  */
   __pyx_v_self->_cancel_pending = 0;
 
-  /* "chorde/clients/_async.pyx":178
+  /* "chorde/clients/_async.pyx":179
  *         self._running = 0
  *         self._cancel_pending = 0
  *         self._cancelled = 0             # <<<<<<<<<<<<<<
+ *         self._asyncio_future_blocking = True
  * 
- *     cpdef _set_nothreads(self, value):
  */
   __pyx_v_self->_cancelled = 0;
 
-  /* "chorde/clients/_async.pyx":171
+  /* "chorde/clients/_async.pyx":180
+ *         self._cancel_pending = 0
+ *         self._cancelled = 0
+ *         self._asyncio_future_blocking = True             # <<<<<<<<<<<<<<
+ * 
+ *     cpdef _set_nothreads(self, value):
+ */
+  __pyx_v_self->_asyncio_future_blocking = 1;
+
+  /* "chorde/clients/_async.pyx":172
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":180
- *         self._cancelled = 0
+/* "chorde/clients/_async.pyx":182
+ *         self._asyncio_future_blocking = True
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
 static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_3_set_nothreads(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
@@ -6492,15 +6526,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_3_set_nothreads)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6509,15 +6543,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6530,236 +6564,236 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":188
+  /* "chorde/clients/_async.pyx":190
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   __pyx_t_5 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":190
+    /* "chorde/clients/_async.pyx":192
  *         if self._value is not NONE:
  *             # No setting twice
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # start atomic op
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":188
+    /* "chorde/clients/_async.pyx":190
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   }
 
-  /* "chorde/clients/_async.pyx":193
+  /* "chorde/clients/_async.pyx":195
  * 
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers             # <<<<<<<<<<<<<<
  *         _cb = self._cb
  *         if _cb is not None:
  */
   __pyx_t_1 = __pyx_v_self->_value;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_old = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":194
+  /* "chorde/clients/_async.pyx":196
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb             # <<<<<<<<<<<<<<
  *         if _cb is not None:
  *             self._cb = None
  */
   __pyx_t_1 = __pyx_v_self->_cb;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v__cb = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":195
+  /* "chorde/clients/_async.pyx":197
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
   __pyx_t_6 = (__pyx_v__cb != Py_None);
   __pyx_t_5 = (__pyx_t_6 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":196
+    /* "chorde/clients/_async.pyx":198
  *         _cb = self._cb
  *         if _cb is not None:
  *             self._cb = None             # <<<<<<<<<<<<<<
  *             self._value = value
  *             cbs = list(_cb) # end atomic op
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_cb);
     __Pyx_DECREF(__pyx_v_self->_cb);
     __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-    /* "chorde/clients/_async.pyx":197
+    /* "chorde/clients/_async.pyx":199
  *         if _cb is not None:
  *             self._cb = None
  *             self._value = value             # <<<<<<<<<<<<<<
  *             cbs = list(_cb) # end atomic op
  *         else:
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
 
-    /* "chorde/clients/_async.pyx":198
+    /* "chorde/clients/_async.pyx":200
  *             self._cb = None
  *             self._value = value
  *             cbs = list(_cb) # end atomic op             # <<<<<<<<<<<<<<
  *         else:
  *             cbs = None
  */
-    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_cbs = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":195
+    /* "chorde/clients/_async.pyx":197
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
     goto __pyx_L4;
   }
 
-  /* "chorde/clients/_async.pyx":200
+  /* "chorde/clients/_async.pyx":202
  *             cbs = list(_cb) # end atomic op
  *         else:
  *             cbs = None             # <<<<<<<<<<<<<<
  *             self._value = value # end atomic op
  *         self._running = 0
  */
   /*else*/ {
     __Pyx_INCREF(Py_None);
     __pyx_v_cbs = Py_None;
 
-    /* "chorde/clients/_async.pyx":201
+    /* "chorde/clients/_async.pyx":203
  *         else:
  *             cbs = None
  *             self._value = value # end atomic op             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         del old, _cb
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
   }
   __pyx_L4:;
 
-  /* "chorde/clients/_async.pyx":202
+  /* "chorde/clients/_async.pyx":204
  *             cbs = None
  *             self._value = value # end atomic op
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         del old, _cb
  * 
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":203
+  /* "chorde/clients/_async.pyx":205
  *             self._value = value # end atomic op
  *         self._running = 0
  *         del old, _cb             # <<<<<<<<<<<<<<
  * 
  *         if cbs is not None:
  */
   __Pyx_DECREF(__pyx_v_old);
   __pyx_v_old = NULL;
   __Pyx_DECREF(__pyx_v__cb);
   __pyx_v__cb = NULL;
 
-  /* "chorde/clients/_async.pyx":205
+  /* "chorde/clients/_async.pyx":207
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   __pyx_t_5 = (__pyx_v_cbs != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":206
+    /* "chorde/clients/_async.pyx":208
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     if (likely(PyList_CheckExact(__pyx_v_cbs)) || PyTuple_CheckExact(__pyx_v_cbs)) {
       __pyx_t_1 = __pyx_v_cbs; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 208, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 208, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 208, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_8(__pyx_t_1);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 206, __pyx_L1_error)
+            else __PYX_ERR(0, 208, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_v_cb, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "chorde/clients/_async.pyx":207
+      /* "chorde/clients/_async.pyx":209
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
       {
@@ -6767,15 +6801,15 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":208
+          /* "chorde/clients/_async.pyx":210
  *             for cb in cbs:
  *                 try:
  *                     cb(value)             # <<<<<<<<<<<<<<
  *                 except:
  *                     if self._logger is not None:
  */
           __Pyx_INCREF(__pyx_v_cb);
@@ -6787,20 +6821,20 @@
               __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L8_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "chorde/clients/_async.pyx":207
+          /* "chorde/clients/_async.pyx":209
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         }
@@ -6809,101 +6843,101 @@
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L15_try_end;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "chorde/clients/_async.pyx":209
+        /* "chorde/clients/_async.pyx":211
  *                 try:
  *                     cb(value)
  *                 except:             # <<<<<<<<<<<<<<
  *                     if self._logger is not None:
  *                         error = self._logger
  */
         /*except:*/ {
           __Pyx_AddTraceback("chorde.clients._async.Future._set_nothreads", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 209, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 211, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
 
-          /* "chorde/clients/_async.pyx":210
+          /* "chorde/clients/_async.pyx":212
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
           __pyx_t_6 = (__pyx_v_self->_logger != Py_None);
           __pyx_t_5 = (__pyx_t_6 != 0);
           if (__pyx_t_5) {
 
-            /* "chorde/clients/_async.pyx":211
+            /* "chorde/clients/_async.pyx":213
  *                 except:
  *                     if self._logger is not None:
  *                         error = self._logger             # <<<<<<<<<<<<<<
  *                     else:
  *                         error = logging.error
  */
             __pyx_t_12 = __pyx_v_self->_logger;
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_12);
             __pyx_t_12 = 0;
 
-            /* "chorde/clients/_async.pyx":210
+            /* "chorde/clients/_async.pyx":212
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
             goto __pyx_L18;
           }
 
-          /* "chorde/clients/_async.pyx":213
+          /* "chorde/clients/_async.pyx":215
  *                         error = self._logger
  *                     else:
  *                         error = logging.error             # <<<<<<<<<<<<<<
  *                     error("Error in async callback", exc_info = True)
  * 
  */
           /*else*/ {
-            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 213, __pyx_L10_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 215, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 213, __pyx_L10_except_error)
+            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 215, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_13);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_13);
             __pyx_t_13 = 0;
           }
           __pyx_L18:;
 
-          /* "chorde/clients/_async.pyx":214
+          /* "chorde/clients/_async.pyx":216
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 214, __pyx_L10_except_error)
+          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 216, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(0, 214, __pyx_L10_except_error)
-          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 214, __pyx_L10_except_error)
+          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(0, 216, __pyx_L10_except_error)
+          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 216, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
 
-        /* "chorde/clients/_async.pyx":207
+        /* "chorde/clients/_async.pyx":209
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         __Pyx_XGIVEREF(__pyx_t_9);
@@ -6915,35 +6949,35 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
         __pyx_L15_try_end:;
       }
 
-      /* "chorde/clients/_async.pyx":206
+      /* "chorde/clients/_async.pyx":208
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":205
+    /* "chorde/clients/_async.pyx":207
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   }
 
-  /* "chorde/clients/_async.pyx":180
- *         self._cancelled = 0
+  /* "chorde/clients/_async.pyx":182
+ *         self._asyncio_future_blocking = True
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
   /* function exit code */
@@ -6988,15 +7022,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_nothreads", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7005,15 +7039,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":216
+/* "chorde/clients/_async.pyx":218
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -7036,15 +7070,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_5set)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -7053,15 +7087,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -7074,72 +7108,72 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":221
+  /* "chorde/clients/_async.pyx":223
  *         a cache miss if given CacheMissError (the class itself)
  *         """
  *         self._set_nothreads(value)             # <<<<<<<<<<<<<<
  * 
  *         if self._done_event is not None:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":223
+  /* "chorde/clients/_async.pyx":225
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   __pyx_t_5 = (__pyx_v_self->_done_event != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":225
+    /* "chorde/clients/_async.pyx":227
  *         if self._done_event is not None:
  *             # wake up waiting threads
  *             self._done_event.set()             # <<<<<<<<<<<<<<
  * 
  *     def __await__(self):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":223
+    /* "chorde/clients/_async.pyx":225
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   }
 
-  /* "chorde/clients/_async.pyx":216
+  /* "chorde/clients/_async.pyx":218
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -7178,15 +7212,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7196,20 +7230,20 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6chorde_7clients_6_async_6Future_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "chorde/clients/_async.pyx":227
+/* "chorde/clients/_async.pyx":229
  *             self._done_event.set()
  * 
  *     def __await__(self):             # <<<<<<<<<<<<<<
  *         if not self.c_done():
- *             return (yield self)
+ *             yield self
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_7__await__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_7__await__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7229,23 +7263,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__await__", 0);
   __pyx_cur_scope = (struct __pyx_obj_6chorde_7clients_6_async___pyx_scope_struct____await__ *)__pyx_tp_new_6chorde_7clients_6_async___pyx_scope_struct____await__(__pyx_ptype_6chorde_7clients_6_async___pyx_scope_struct____await__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6chorde_7clients_6_async___pyx_scope_struct____await__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 227, __pyx_L1_error)
+    __PYX_ERR(0, 229, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6chorde_7clients_6_async_6Future_8generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_await, __pyx_n_s_Future___await, __pyx_n_s_chorde_clients__async); if (unlikely(!gen)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6chorde_7clients_6_async_6Future_8generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_await, __pyx_n_s_Future___await, __pyx_n_s_chorde_clients__async); if (unlikely(!gen)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7273,80 +7307,75 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L5_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 229, __pyx_L1_error)
 
-  /* "chorde/clients/_async.pyx":228
+  /* "chorde/clients/_async.pyx":230
  * 
  *     def __await__(self):
  *         if not self.c_done():             # <<<<<<<<<<<<<<
- *             return (yield self)
+ *             yield self
  *         return self.c_result(0, 1)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->c_done(__pyx_cur_scope->__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->c_done(__pyx_cur_scope->__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 230, __pyx_L1_error)
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":229
+    /* "chorde/clients/_async.pyx":231
  *     def __await__(self):
  *         if not self.c_done():
- *             return (yield self)             # <<<<<<<<<<<<<<
+ *             yield self             # <<<<<<<<<<<<<<
  *         return self.c_result(0, 1)
  * 
  */
-    __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_cur_scope->__pyx_v_self);
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L5_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __pyx_t_3 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_3);
-    __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L0;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 231, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":228
+    /* "chorde/clients/_async.pyx":230
  * 
  *     def __await__(self):
  *         if not self.c_done():             # <<<<<<<<<<<<<<
- *             return (yield self)
+ *             yield self
  *         return self.c_result(0, 1)
  */
   }
 
-  /* "chorde/clients/_async.pyx":230
+  /* "chorde/clients/_async.pyx":232
  *         if not self.c_done():
- *             return (yield self)
+ *             yield self
  *         return self.c_result(0, 1)             # <<<<<<<<<<<<<<
  * 
- *     def set_result(self, value):
+ *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->c_result(__pyx_cur_scope->__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->c_result(__pyx_cur_scope->__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "chorde/clients/_async.pyx":227
+  /* "chorde/clients/_async.pyx":229
  *             self._done_event.set()
  * 
  *     def __await__(self):             # <<<<<<<<<<<<<<
  *         if not self.c_done():
- *             return (yield self)
+ *             yield self
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("__await__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
@@ -7356,16 +7385,101 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":232
- *         return self.c_result(0, 1)
+/* "chorde/clients/_async.pyx":235
+ * 
+ *     @property
+ *     def _loop(self):             # <<<<<<<<<<<<<<
+ *         return asyncio.get_running_loop()
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_5_loop_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_5_loop_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_5_loop___get__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_5_loop___get__(CYTHON_UNUSED struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "chorde/clients/_async.pyx":236
+ *     @property
+ *     def _loop(self):
+ *         return asyncio.get_running_loop()             # <<<<<<<<<<<<<<
+ * 
+ *     def set_result(self, value):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_asyncio); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_running_loop); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "chorde/clients/_async.pyx":235
+ * 
+ *     @property
+ *     def _loop(self):             # <<<<<<<<<<<<<<
+ *         return asyncio.get_running_loop()
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("chorde.clients._async.Future._loop.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "chorde/clients/_async.pyx":238
+ *         return asyncio.get_running_loop()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
 /* Python wrapper */
@@ -7386,27 +7500,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_result", 0);
 
-  /* "chorde/clients/_async.pyx":233
+  /* "chorde/clients/_async.pyx":239
  * 
  *     def set_result(self, value):
  *         self.set(value)             # <<<<<<<<<<<<<<
  * 
  *     def miss(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":232
- *         return self.c_result(0, 1)
+  /* "chorde/clients/_async.pyx":238
+ *         return asyncio.get_running_loop()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
   /* function exit code */
@@ -7418,15 +7532,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":235
+/* "chorde/clients/_async.pyx":241
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -7450,29 +7564,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("miss", 0);
 
-  /* "chorde/clients/_async.pyx":239
+  /* "chorde/clients/_async.pyx":245
  *         Shorthand for setting a cache miss result
  *         """
  *         self.set(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def _miss_nothreads(self):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":235
+  /* "chorde/clients/_async.pyx":241
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -7486,15 +7600,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":241
+/* "chorde/clients/_async.pyx":247
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7518,29 +7632,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_miss_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":246
+  /* "chorde/clients/_async.pyx":252
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def exc(self, exc_info):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":241
+  /* "chorde/clients/_async.pyx":247
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7554,15 +7668,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":248
+/* "chorde/clients/_async.pyx":254
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7586,35 +7700,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exc", 0);
 
-  /* "chorde/clients/_async.pyx":253
+  /* "chorde/clients/_async.pyx":259
  *         as returned by sys.exc_info()
  *         """
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def _exc_nothreads(self, exc_info):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":248
+  /* "chorde/clients/_async.pyx":254
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7628,15 +7742,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":255
+/* "chorde/clients/_async.pyx":261
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7660,35 +7774,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_exc_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":261
+  /* "chorde/clients/_async.pyx":267
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def set_exception(self, exception):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":255
+  /* "chorde/clients/_async.pyx":261
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7702,15 +7816,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":263
+/* "chorde/clients/_async.pyx":269
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7740,82 +7854,82 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_exception", 0);
   __Pyx_INCREF(__pyx_v_exception);
 
-  /* "chorde/clients/_async.pyx":267
+  /* "chorde/clients/_async.pyx":273
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   __pyx_t_2 = (__pyx_v_6chorde_7clients_6_async_strip_tracebacks != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = (__pyx_t_3 != Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":268
+    /* "chorde/clients/_async.pyx":274
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)             # <<<<<<<<<<<<<<
  *         self.exc((type(exception),exception,None))
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_5, Py_None);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_exception, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":267
+    /* "chorde/clients/_async.pyx":273
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   }
 
-  /* "chorde/clients/_async.pyx":269
+  /* "chorde/clients/_async.pyx":275
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))             # <<<<<<<<<<<<<<
  * 
  *     def on_value(self, callback):
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_INCREF(__pyx_v_exception);
   __Pyx_GIVEREF(__pyx_v_exception);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_exception);
@@ -7831,20 +7945,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "chorde/clients/_async.pyx":263
+  /* "chorde/clients/_async.pyx":269
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7861,15 +7975,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exception);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":271
+/* "chorde/clients/_async.pyx":277
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7893,38 +8007,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_value", 0);
 
-  /* "chorde/clients/_async.pyx":276
+  /* "chorde/clients/_async.pyx":282
  *         will be invoked with its result.
  *         """
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_miss(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":271
+  /* "chorde/clients/_async.pyx":277
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7936,15 +8050,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":278
+/* "chorde/clients/_async.pyx":284
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -7968,38 +8082,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_miss", 0);
 
-  /* "chorde/clients/_async.pyx":283
+  /* "chorde/clients/_async.pyx":289
  *         without arugments.
  *         """
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_exc(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":278
+  /* "chorde/clients/_async.pyx":284
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -8011,15 +8125,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":285
+/* "chorde/clients/_async.pyx":291
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -8043,38 +8157,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_exc", 0);
 
-  /* "chorde/clients/_async.pyx":290
+  /* "chorde/clients/_async.pyx":296
  *         with an exc_info tuple as returned by sys.exc_info.
  *         """
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":285
+  /* "chorde/clients/_async.pyx":291
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -8086,15 +8200,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":292
+/* "chorde/clients/_async.pyx":298
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -8147,15 +8261,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(0, 292, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(0, 298, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -8167,15 +8281,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 292, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 298, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_27on_any(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -8190,44 +8304,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any", 0);
 
-  /* "chorde/clients/_async.pyx":297
+  /* "chorde/clients/_async.pyx":303
  *         faster than calling on_X repeatedly. None callbacks will be ignored.
  *         """
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_on_value);
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_on_miss);
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_on_exc);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":292
+  /* "chorde/clients/_async.pyx":298
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -8239,15 +8353,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":299
+/* "chorde/clients/_async.pyx":305
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -8300,15 +8414,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(0, 305, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -8320,15 +8434,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 299, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 305, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_29on_any_once(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -8345,64 +8459,64 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any_once", 0);
 
-  /* "chorde/clients/_async.pyx":303
+  /* "chorde/clients/_async.pyx":309
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":304
+    /* "chorde/clients/_async.pyx":310
  *         """
  *         if self._cb is None:
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_done(self, callback):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_on_value);
     __Pyx_GIVEREF(__pyx_v_on_value);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_on_value);
     __Pyx_INCREF(__pyx_v_on_miss);
     __Pyx_GIVEREF(__pyx_v_on_miss);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_on_miss);
     __Pyx_INCREF(__pyx_v_on_exc);
     __Pyx_GIVEREF(__pyx_v_on_exc);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_on_exc);
-    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(((PyObject *)__pyx_t_4));
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(((PyObject *)__pyx_t_4)); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":303
+    /* "chorde/clients/_async.pyx":309
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":299
+  /* "chorde/clients/_async.pyx":305
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -8416,15 +8530,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":306
+/* "chorde/clients/_async.pyx":312
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -8448,38 +8562,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_done", 0);
 
-  /* "chorde/clients/_async.pyx":311
+  /* "chorde/clients/_async.pyx":317
  *         regardless of the outcome. If the operation is cancelled, it won't be invoked.
  *         """
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def chain(self, defer):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":306
+  /* "chorde/clients/_async.pyx":312
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -8491,15 +8605,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":313
+/* "chorde/clients/_async.pyx":319
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8523,29 +8637,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain", 0);
 
-  /* "chorde/clients/_async.pyx":317
+  /* "chorde/clients/_async.pyx":323
  *         Invoke all the callbacks of the other defer
  *         """
  *         self._on_stuff(defer.set)             # <<<<<<<<<<<<<<
  * 
  *     def chain_std(self, defer):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":313
+  /* "chorde/clients/_async.pyx":319
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8559,15 +8673,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":319
+/* "chorde/clients/_async.pyx":325
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8599,58 +8713,58 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain_std", 0);
 
-  /* "chorde/clients/_async.pyx":324
+  /* "chorde/clients/_async.pyx":330
  *         defer follows our non-standard interface.
  *         """
  *         return self.on_any(             # <<<<<<<<<<<<<<
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "chorde/clients/_async.pyx":325
+  /* "chorde/clients/_async.pyx":331
  *         """
  *         return self.on_any(
  *             defer.set_result,             # <<<<<<<<<<<<<<
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "chorde/clients/_async.pyx":326
+  /* "chorde/clients/_async.pyx":332
  *         return self.on_any(
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),             # <<<<<<<<<<<<<<
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  *         )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_CacheMissError; __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_functools_partial; __pyx_t_8 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
@@ -8661,62 +8775,62 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 332, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "chorde/clients/_async.pyx":327
+  /* "chorde/clients/_async.pyx":333
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_defer);
-  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_10));
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -8726,58 +8840,58 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_9, __pyx_t_4);
     __Pyx_GIVEREF(((PyObject *)__pyx_t_10));
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_9, ((PyObject *)__pyx_t_10));
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":319
+  /* "chorde/clients/_async.pyx":325
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8796,15 +8910,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":330
+/* "chorde/clients/_async.pyx":336
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -8828,15 +8942,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_38_on_stuff)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8845,15 +8959,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_callback) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_callback);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -8866,84 +8980,84 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":331
+  /* "chorde/clients/_async.pyx":337
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
   __pyx_t_5 = (__pyx_v_self->_value == ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":332
+    /* "chorde/clients/_async.pyx":338
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     __pyx_t_6 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
     __pyx_t_5 = (__pyx_t_6 != 0);
     if (__pyx_t_5) {
 
-      /* "chorde/clients/_async.pyx":333
+      /* "chorde/clients/_async.pyx":339
  *         if self._value is NONE:
  *             if self._cb is None:
  *                 self._cb = list()             # <<<<<<<<<<<<<<
  *             self._cb.append(callback)
  *         else:
  */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_v_self->_cb);
       __Pyx_DECREF(__pyx_v_self->_cb);
       __pyx_v_self->_cb = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "chorde/clients/_async.pyx":332
+      /* "chorde/clients/_async.pyx":338
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     }
 
-    /* "chorde/clients/_async.pyx":334
+    /* "chorde/clients/_async.pyx":340
  *             if self._cb is None:
  *                 self._cb = list()
  *             self._cb.append(callback)             # <<<<<<<<<<<<<<
  *         else:
  *             callback(self._value)
  */
     if (unlikely(__pyx_v_self->_cb == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(0, 334, __pyx_L1_error)
+      __PYX_ERR(0, 340, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 334, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 340, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":331
+    /* "chorde/clients/_async.pyx":337
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":336
+  /* "chorde/clients/_async.pyx":342
  *             self._cb.append(callback)
  *         else:
  *             callback(self._value)             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   /*else*/ {
@@ -8956,34 +9070,34 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_value) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_value);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":337
+  /* "chorde/clients/_async.pyx":343
  *         else:
  *             callback(self._value)
  *         return self             # <<<<<<<<<<<<<<
  * 
- *     def add_done_callback(self, callback):
+ *     def add_done_callback(self, callback, *, context=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":330
+  /* "chorde/clients/_async.pyx":336
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -9019,15 +9133,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_on_stuff", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9036,93 +9150,232 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":339
+/* "chorde/clients/_async.pyx":345
  *         return self
  * 
- *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
+ *     def add_done_callback(self, callback, *, context=None):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback(PyObject *__pyx_v_self, PyObject *__pyx_v_callback); /*proto*/
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6chorde_7clients_6_async_6Future_39add_done_callback[] = "\n        When the operatio is done, the callback will be invoked with the\n        future object as argument.\n        ";
-static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback(PyObject *__pyx_v_self, PyObject *__pyx_v_callback) {
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_callback = 0;
+  PyObject *__pyx_v_context = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_done_callback (wrapper)", 0);
-  __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), ((PyObject *)__pyx_v_callback));
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_callback,&__pyx_n_s_context,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)Py_None);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (kw_args == 1) {
+        const Py_ssize_t index = 1;
+        PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
+        if (value) { values[index] = value; kw_args--; }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_done_callback") < 0)) __PYX_ERR(0, 345, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+    }
+    __pyx_v_callback = values[0];
+    __pyx_v_context = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("add_done_callback", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 345, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("chorde.clients._async.Future.add_done_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_callback, __pyx_v_context);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback) {
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_39add_done_callback(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_callback, PyObject *__pyx_v_context) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_done_callback", 0);
+  __Pyx_INCREF(__pyx_v_callback);
 
-  /* "chorde/clients/_async.pyx":344
+  /* "chorde/clients/_async.pyx":350
  *         future object as argument.
  *         """
+ *         if context is not None:             # <<<<<<<<<<<<<<
+ *             callback = functools_partial(context.run, callback)
+ *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
+ */
+  __pyx_t_1 = (__pyx_v_context != Py_None);
+  __pyx_t_2 = (__pyx_t_1 != 0);
+  if (__pyx_t_2) {
+
+    /* "chorde/clients/_async.pyx":351
+ *         """
+ *         if context is not None:
+ *             callback = functools_partial(context.run, callback)             # <<<<<<<<<<<<<<
+ *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_context, __pyx_n_s_run); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 351, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
+    __pyx_t_5 = __pyx_v_6chorde_7clients_6_async_functools_partial; __pyx_t_6 = NULL;
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_5)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_v_callback};
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_v_callback};
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      if (__pyx_t_6) {
+        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+      }
+      __Pyx_GIVEREF(__pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_4);
+      __Pyx_INCREF(__pyx_v_callback);
+      __Pyx_GIVEREF(__pyx_v_callback);
+      PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_callback);
+      __pyx_t_4 = 0;
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF_SET(__pyx_v_callback, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "chorde/clients/_async.pyx":350
+ *         future object as argument.
+ *         """
+ *         if context is not None:             # <<<<<<<<<<<<<<
+ *             callback = functools_partial(context.run, callback)
+ *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
+ */
+  }
+
+  /* "chorde/clients/_async.pyx":352
+ *         if context is not None:
+ *             callback = functools_partial(context.run, callback)
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))             # <<<<<<<<<<<<<<
  * 
  *     cdef int c_done(self) except -1:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self));
+  PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
-  __Pyx_GOTREF(((PyObject *)__pyx_t_2));
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_callback);
+  __pyx_t_5 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __Pyx_GOTREF(((PyObject *)__pyx_t_5));
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_5), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(((PyObject *)__pyx_t_5)); __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":339
+  /* "chorde/clients/_async.pyx":345
  *         return self
  * 
- *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
+ *     def add_done_callback(self, callback, *, context=None):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("chorde.clients._async.Future.add_done_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_callback);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":346
+/* "chorde/clients/_async.pyx":354
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -9130,15 +9383,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("c_done", 0);
 
-  /* "chorde/clients/_async.pyx":350
+  /* "chorde/clients/_async.pyx":358
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
@@ -9149,60 +9402,60 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = (__pyx_v_self->_cancelled != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":351
+    /* "chorde/clients/_async.pyx":359
  *         """
  *         if self._value is not NONE or self._cancelled:
  *             return 1             # <<<<<<<<<<<<<<
  *         else:
  *             return 0
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":350
+    /* "chorde/clients/_async.pyx":358
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":353
+  /* "chorde/clients/_async.pyx":361
  *             return 1
  *         else:
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     def done(self):
  */
   /*else*/ {
     __pyx_r = 0;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":346
+  /* "chorde/clients/_async.pyx":354
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":355
+/* "chorde/clients/_async.pyx":363
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -9226,61 +9479,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("done", 0);
 
-  /* "chorde/clients/_async.pyx":359
+  /* "chorde/clients/_async.pyx":367
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 367, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":360
+    /* "chorde/clients/_async.pyx":368
  *         """
  *         if self.c_done():
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":359
+    /* "chorde/clients/_async.pyx":367
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":362
+  /* "chorde/clients/_async.pyx":370
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def running(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":355
+  /* "chorde/clients/_async.pyx":363
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -9290,15 +9543,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":364
+/* "chorde/clients/_async.pyx":372
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
@@ -9318,75 +9571,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_43running(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("running", 0);
 
-  /* "chorde/clients/_async.pyx":369
+  /* "chorde/clients/_async.pyx":377
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_running != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":370
+    /* "chorde/clients/_async.pyx":378
  *         """
  *         if self._running:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":369
+    /* "chorde/clients/_async.pyx":377
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":372
+  /* "chorde/clients/_async.pyx":380
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancelled(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":364
+  /* "chorde/clients/_async.pyx":372
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":374
+/* "chorde/clients/_async.pyx":382
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
@@ -9406,75 +9659,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_45cancelled(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":378
+  /* "chorde/clients/_async.pyx":386
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":379
+    /* "chorde/clients/_async.pyx":387
  *         """
  *         if self._cancelled:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":378
+    /* "chorde/clients/_async.pyx":386
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":381
+  /* "chorde/clients/_async.pyx":389
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel_pending(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":374
+  /* "chorde/clients/_async.pyx":382
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":383
+/* "chorde/clients/_async.pyx":391
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
@@ -9494,75 +9747,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_47cancel_pending(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel_pending", 0);
 
-  /* "chorde/clients/_async.pyx":387
+  /* "chorde/clients/_async.pyx":395
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":388
+    /* "chorde/clients/_async.pyx":396
  *         """
  *         if self._cancel_pending:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":387
+    /* "chorde/clients/_async.pyx":395
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":390
+  /* "chorde/clients/_async.pyx":398
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":383
+  /* "chorde/clients/_async.pyx":391
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":392
+/* "chorde/clients/_async.pyx":400
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
@@ -9582,84 +9835,84 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_49cancel(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel", 0);
 
-  /* "chorde/clients/_async.pyx":397
+  /* "chorde/clients/_async.pyx":405
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":398
+    /* "chorde/clients/_async.pyx":406
  *         """
  *         if self._cancelled:
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._cancel_pending = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":397
+    /* "chorde/clients/_async.pyx":405
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":400
+  /* "chorde/clients/_async.pyx":408
  *             return False
  *         else:
  *             self._cancel_pending = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_cancel_pending = 1;
 
-    /* "chorde/clients/_async.pyx":401
+    /* "chorde/clients/_async.pyx":409
  *         else:
  *             self._cancel_pending = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     def set_running_or_notify_cancelled(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":392
+  /* "chorde/clients/_async.pyx":400
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":403
+/* "chorde/clients/_async.pyx":411
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9687,65 +9940,65 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_running_or_notify_cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":410
+  /* "chorde/clients/_async.pyx":418
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":411
+    /* "chorde/clients/_async.pyx":419
  *         """
  *         if self._cancel_pending:
  *             self._cancelled = 1             # <<<<<<<<<<<<<<
  *             self._running = 0
  * 
  */
     __pyx_v_self->_cancelled = 1;
 
-    /* "chorde/clients/_async.pyx":412
+    /* "chorde/clients/_async.pyx":420
  *         if self._cancel_pending:
  *             self._cancelled = 1
  *             self._running = 0             # <<<<<<<<<<<<<<
  * 
  *             # Notify waiters and callbacks
  */
     __pyx_v_self->_running = 0;
 
-    /* "chorde/clients/_async.pyx":415
+    /* "chorde/clients/_async.pyx":423
  * 
  *             # Notify waiters and callbacks
  *             self.set_exception(CancelledError())             # <<<<<<<<<<<<<<
  * 
  *             return False
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
     __pyx_t_5 = __pyx_v_6chorde_7clients_6_async_CancelledError; __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9753,64 +10006,64 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "chorde/clients/_async.pyx":417
+    /* "chorde/clients/_async.pyx":425
  *             self.set_exception(CancelledError())
  * 
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._running = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":410
+    /* "chorde/clients/_async.pyx":418
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   }
 
-  /* "chorde/clients/_async.pyx":419
+  /* "chorde/clients/_async.pyx":427
  *             return False
  *         else:
  *             self._running = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_running = 1;
 
-    /* "chorde/clients/_async.pyx":420
+    /* "chorde/clients/_async.pyx":428
  *         else:
  *             self._running = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     cdef c_result(self, timeout, int norecurse):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":403
+  /* "chorde/clients/_async.pyx":411
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9825,15 +10078,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":422
+/* "chorde/clients/_async.pyx":430
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9859,84 +10112,84 @@
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("c_result", 0);
 
-  /* "chorde/clients/_async.pyx":431
+  /* "chorde/clients/_async.pyx":439
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":432
+    /* "chorde/clients/_async.pyx":440
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":433
+    /* "chorde/clients/_async.pyx":441
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":434
+      /* "chorde/clients/_async.pyx":442
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 try:
  *                     exc_value.reraise(False)
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":435
+      /* "chorde/clients/_async.pyx":443
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 try:             # <<<<<<<<<<<<<<
  *                     exc_value.reraise(False)
  *                 finally:
  */
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":436
+        /* "chorde/clients/_async.pyx":444
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  *                     exc_value.reraise(False)             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del exc_value, value
  */
         __pyx_t_4.__pyx_n = 1;
         __pyx_t_4.strip = 0;
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L6_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
 
-      /* "chorde/clients/_async.pyx":438
+      /* "chorde/clients/_async.pyx":446
  *                     exc_value.reraise(False)
  *                 finally:
  *                     del exc_value, value             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 raise CacheMissError()
  */
       /*finally:*/ {
@@ -9981,36 +10234,36 @@
           __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_6; __pyx_filename = __pyx_t_7;
           goto __pyx_L1_error;
         }
         __pyx_L7:;
       }
 
-      /* "chorde/clients/_async.pyx":433
+      /* "chorde/clients/_async.pyx":441
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
       goto __pyx_L4;
     }
 
-    /* "chorde/clients/_async.pyx":439
+    /* "chorde/clients/_async.pyx":447
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":440
+      /* "chorde/clients/_async.pyx":448
  *                     del exc_value, value
  *             elif value is CacheMissError:
  *                 raise CacheMissError()             # <<<<<<<<<<<<<<
  *             else:
  *                 return value
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -10022,66 +10275,66 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 440, __pyx_L1_error)
+      __PYX_ERR(0, 448, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":439
+      /* "chorde/clients/_async.pyx":447
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":442
+    /* "chorde/clients/_async.pyx":450
  *                 raise CacheMissError()
  *             else:
  *                 return value             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_value);
       __pyx_r = __pyx_v_value;
       goto __pyx_L0;
     }
     __pyx_L4:;
 
-    /* "chorde/clients/_async.pyx":431
+    /* "chorde/clients/_async.pyx":439
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":443
+  /* "chorde/clients/_async.pyx":451
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":444
+    /* "chorde/clients/_async.pyx":452
  *                 return value
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             if timeout is not None and timeout == 0:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -10093,54 +10346,54 @@
         __Pyx_INCREF(__pyx_t_15);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_14, function);
       }
     }
     __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
     __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 444, __pyx_L1_error)
+    __PYX_ERR(0, 452, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":443
+    /* "chorde/clients/_async.pyx":451
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":446
+  /* "chorde/clients/_async.pyx":454
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_timeout != Py_None);
     __pyx_t_16 = (__pyx_t_1 != 0);
     if (__pyx_t_16) {
     } else {
       __pyx_t_2 = __pyx_t_16;
       goto __pyx_L11_bool_binop_done;
     }
-    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = __pyx_t_16;
     __pyx_L11_bool_binop_done:;
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":447
+      /* "chorde/clients/_async.pyx":455
  *         else:
  *             if timeout is not None and timeout == 0:
  *                 raise TimeoutError()             # <<<<<<<<<<<<<<
  *             else:
  *                 # Wait for it
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_TimeoutError);
@@ -10152,85 +10405,85 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 447, __pyx_L1_error)
+      __PYX_ERR(0, 455, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":446
+      /* "chorde/clients/_async.pyx":454
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":450
+    /* "chorde/clients/_async.pyx":458
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_self->_done_event == Py_None);
       __pyx_t_16 = (__pyx_t_2 != 0);
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":451
+        /* "chorde/clients/_async.pyx":459
  *                 # Wait for it
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()             # <<<<<<<<<<<<<<
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 451, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 459, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 451, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 459, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_14 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_v_self->_done_event);
         __Pyx_DECREF(__pyx_v_self->_done_event);
         __pyx_v_self->_done_event = __pyx_t_3;
         __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":450
+        /* "chorde/clients/_async.pyx":458
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
       }
 
-      /* "chorde/clients/_async.pyx":452
+      /* "chorde/clients/_async.pyx":460
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       __pyx_t_2 = ((!(__pyx_v_norecurse != 0)) != 0);
@@ -10242,71 +10495,71 @@
       __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
       __pyx_t_1 = (__pyx_t_2 != 0);
       if (!__pyx_t_1) {
       } else {
         __pyx_t_16 = __pyx_t_1;
         goto __pyx_L15_bool_binop_done;
       }
-      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 460, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_14 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
         if (likely(__pyx_t_14)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
           __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_15, function);
         }
       }
       __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_14, __pyx_v_timeout) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_timeout);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 460, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 460, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_16 = __pyx_t_1;
       __pyx_L15_bool_binop_done:;
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":453
+        /* "chorde/clients/_async.pyx":461
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)             # <<<<<<<<<<<<<<
  *                 elif self._cancelled:
  *                     raise CancelledError()
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_r = __pyx_t_3;
         __pyx_t_3 = 0;
         goto __pyx_L0;
 
-        /* "chorde/clients/_async.pyx":452
+        /* "chorde/clients/_async.pyx":460
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       }
 
-      /* "chorde/clients/_async.pyx":454
+      /* "chorde/clients/_async.pyx":462
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       __pyx_t_16 = (__pyx_v_self->_cancelled != 0);
       if (unlikely(__pyx_t_16)) {
 
-        /* "chorde/clients/_async.pyx":455
+        /* "chorde/clients/_async.pyx":463
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  *                     raise CancelledError()             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise TimeoutError()
  */
         __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -10318,31 +10571,31 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 455, __pyx_L1_error)
+        __PYX_ERR(0, 463, __pyx_L1_error)
 
-        /* "chorde/clients/_async.pyx":454
+        /* "chorde/clients/_async.pyx":462
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       }
 
-      /* "chorde/clients/_async.pyx":457
+      /* "chorde/clients/_async.pyx":465
  *                     raise CancelledError()
  *                 else:
  *                     raise TimeoutError()             # <<<<<<<<<<<<<<
  * 
  *     def result(self, timeout=None, norecurse=False):
  */
       /*else*/ {
@@ -10355,26 +10608,26 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 457, __pyx_L1_error)
+        __PYX_ERR(0, 465, __pyx_L1_error)
       }
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":422
+  /* "chorde/clients/_async.pyx":430
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10391,15 +10644,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF((PyObject *)__pyx_v_exc_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":459
+/* "chorde/clients/_async.pyx":467
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10442,15 +10695,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_norecurse);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(0, 459, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(0, 467, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -10459,15 +10712,15 @@
       }
     }
     __pyx_v_timeout = values[0];
     __pyx_v_norecurse = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 459, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 467, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_53result(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout, __pyx_v_norecurse);
 
@@ -10482,30 +10735,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("result", 0);
 
-  /* "chorde/clients/_async.pyx":465
+  /* "chorde/clients/_async.pyx":473
  *         and the specified time elapses without a result available, raises TimeoutError.
  *         """
  *         return self.c_result(timeout, norecurse)             # <<<<<<<<<<<<<<
  * 
  *     def exception(self, timeout=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L1_error)
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 473, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":459
+  /* "chorde/clients/_async.pyx":467
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10516,15 +10769,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":467
+/* "chorde/clients/_async.pyx":475
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -10557,29 +10810,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(0, 467, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(0, 475, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 467, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 475, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_55exception(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout);
 
@@ -10605,163 +10858,163 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exception", 0);
 
-  /* "chorde/clients/_async.pyx":477
+  /* "chorde/clients/_async.pyx":485
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":478
+    /* "chorde/clients/_async.pyx":486
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":479
+    /* "chorde/clients/_async.pyx":487
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":480
+      /* "chorde/clients/_async.pyx":488
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":481
+      /* "chorde/clients/_async.pyx":489
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 return CacheMissError
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 481, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 481, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         __Pyx_INCREF(__pyx_t_4);
         __pyx_t_3 = __pyx_t_4;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         goto __pyx_L5_bool_binop_done;
       }
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 481, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_3 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_L5_bool_binop_done:;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":479
+      /* "chorde/clients/_async.pyx":487
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     }
 
-    /* "chorde/clients/_async.pyx":482
+    /* "chorde/clients/_async.pyx":490
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":483
+      /* "chorde/clients/_async.pyx":491
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  *                 return CacheMissError             # <<<<<<<<<<<<<<
  *             else:
  *                 return None
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
       __pyx_r = __pyx_v_6chorde_7clients_6_async_CacheMissError;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":482
+      /* "chorde/clients/_async.pyx":490
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":485
+    /* "chorde/clients/_async.pyx":493
  *                 return CacheMissError
  *             else:
  *                 return None             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
 
-    /* "chorde/clients/_async.pyx":477
+    /* "chorde/clients/_async.pyx":485
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   }
 
-  /* "chorde/clients/_async.pyx":486
+  /* "chorde/clients/_async.pyx":494
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":487
+    /* "chorde/clients/_async.pyx":495
  *                 return None
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             try:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -10773,31 +11026,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 487, __pyx_L1_error)
+    __PYX_ERR(0, 495, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":486
+    /* "chorde/clients/_async.pyx":494
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":489
+  /* "chorde/clients/_async.pyx":497
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
   /*else*/ {
@@ -10806,106 +11059,106 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":490
+        /* "chorde/clients/_async.pyx":498
  *         else:
  *             try:
  *                 self.c_result(timeout, 0)             # <<<<<<<<<<<<<<
  *                 return None
  *             except CancelledError:
  */
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L7_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":491
+        /* "chorde/clients/_async.pyx":499
  *             try:
  *                 self.c_result(timeout, 0)
  *                 return None             # <<<<<<<<<<<<<<
  *             except CancelledError:
  *                 raise
  */
         __Pyx_XDECREF(__pyx_r);
         __pyx_r = Py_None; __Pyx_INCREF(Py_None);
         goto __pyx_L11_try_return;
 
-        /* "chorde/clients/_async.pyx":489
+        /* "chorde/clients/_async.pyx":497
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       }
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "chorde/clients/_async.pyx":492
+      /* "chorde/clients/_async.pyx":500
  *                 self.c_result(timeout, 0)
  *                 return None
  *             except CancelledError:             # <<<<<<<<<<<<<<
  *                 raise
  *             except Exception as e:
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_v_6chorde_7clients_6_async_CancelledError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 492, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 500, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_5);
 
-        /* "chorde/clients/_async.pyx":493
+        /* "chorde/clients/_async.pyx":501
  *                 return None
  *             except CancelledError:
  *                 raise             # <<<<<<<<<<<<<<
  *             except Exception as e:
  *                 try:
  */
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_4);
         __Pyx_XGIVEREF(__pyx_t_5);
         __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_4, __pyx_t_5);
         __pyx_t_3 = 0; __pyx_t_4 = 0; __pyx_t_5 = 0; 
-        __PYX_ERR(0, 493, __pyx_L9_except_error)
+        __PYX_ERR(0, 501, __pyx_L9_except_error)
       }
 
-      /* "chorde/clients/_async.pyx":494
+      /* "chorde/clients/_async.pyx":502
  *             except CancelledError:
  *                 raise
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 try:
  *                     return e
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(0, 494, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(0, 502, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __pyx_v_e = __pyx_t_4;
 
-        /* "chorde/clients/_async.pyx":495
+        /* "chorde/clients/_async.pyx":503
  *                 raise
  *             except Exception as e:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return e
  *                 finally:
  */
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":496
+          /* "chorde/clients/_async.pyx":504
  *             except Exception as e:
  *                 try:
  *                     return e             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del e
  */
           __Pyx_XDECREF(__pyx_r);
@@ -10913,15 +11166,15 @@
           __pyx_r = __pyx_v_e;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L19_return;
         }
 
-        /* "chorde/clients/_async.pyx":498
+        /* "chorde/clients/_async.pyx":506
  *                     return e
  *                 finally:
  *                     del e             # <<<<<<<<<<<<<<
  * 
  */
         /*finally:*/ {
           __pyx_L19_return: {
@@ -10934,15 +11187,15 @@
             goto __pyx_L10_except_return;
           }
         }
       }
       goto __pyx_L9_except_error;
       __pyx_L9_except_error:;
 
-      /* "chorde/clients/_async.pyx":489
+      /* "chorde/clients/_async.pyx":497
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       __Pyx_XGIVEREF(__pyx_t_6);
@@ -10961,15 +11214,15 @@
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_8);
       __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       goto __pyx_L0;
     }
   }
 
-  /* "chorde/clients/_async.pyx":467
+  /* "chorde/clients/_async.pyx":475
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -10985,14 +11238,96 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_exc_value);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "chorde/clients/_async.pxd":5
+ *     cdef object _value, _logger, _done_event, __weakref__
+ *     cdef int _running, _cancel_pending, _cancelled
+ *     cdef public bint _asyncio_future_blocking             # <<<<<<<<<<<<<<
+ * 
+ *     cdef int c_done(self) except -1
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking___get__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking___get__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->_asyncio_future_blocking); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("chorde.clients._async.Future._asyncio_future_blocking.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_2__set__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_2__set__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_v_self->_asyncio_future_blocking = __pyx_t_1;
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("chorde.clients._async.Future._asyncio_future_blocking.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
@@ -11569,14 +11904,32 @@
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_done_event);
   p->_done_event = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
+static PyObject *__pyx_getprop_6chorde_7clients_6_async_6Future__loop(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_6chorde_7clients_6_async_6Future_5_loop_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_6chorde_7clients_6_async_6Future__asyncio_future_blocking(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_1__get__(o);
+}
+
+static int __pyx_setprop_6chorde_7clients_6_async_6Future__asyncio_future_blocking(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_6chorde_7clients_6_async_6Future_24_asyncio_future_blocking_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
 static PyObject *__pyx_specialmethod___pyx_pw_6chorde_7clients_6_async_6Future_7__await__(PyObject *self, CYTHON_UNUSED PyObject *arg) {return __pyx_pw_6chorde_7clients_6_async_6Future_7__await__(self);}
 
 static PyMethodDef __pyx_methods_6chorde_7clients_6_async_Future[] = {
   {"_set_nothreads", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_3_set_nothreads, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_2_set_nothreads},
   {"set", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_5set, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_4set},
   {"__await__", (PyCFunction)__pyx_specialmethod___pyx_pw_6chorde_7clients_6_async_6Future_7__await__, METH_NOARGS|METH_COEXIST, 0},
   {"set_result", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_10set_result, METH_O, 0},
@@ -11590,28 +11943,34 @@
   {"on_exc", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_26on_exc, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_25on_exc},
   {"on_any", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6chorde_7clients_6_async_6Future_28on_any, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6chorde_7clients_6_async_6Future_27on_any},
   {"on_any_once", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6chorde_7clients_6_async_6Future_30on_any_once, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6chorde_7clients_6_async_6Future_29on_any_once},
   {"on_done", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_32on_done, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_31on_done},
   {"chain", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_34chain, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_33chain},
   {"chain_std", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_36chain_std, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_35chain_std},
   {"_on_stuff", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_38_on_stuff, METH_O, 0},
-  {"add_done_callback", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback, METH_O, __pyx_doc_6chorde_7clients_6_async_6Future_39add_done_callback},
+  {"add_done_callback", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6chorde_7clients_6_async_6Future_40add_done_callback, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6chorde_7clients_6_async_6Future_39add_done_callback},
   {"done", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_42done, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_41done},
   {"running", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_44running, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_43running},
   {"cancelled", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_46cancelled, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_45cancelled},
   {"cancel_pending", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_48cancel_pending, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_47cancel_pending},
   {"cancel", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_50cancel, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_49cancel},
   {"set_running_or_notify_cancelled", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_52set_running_or_notify_cancelled, METH_NOARGS, __pyx_doc_6chorde_7clients_6_async_6Future_51set_running_or_notify_cancelled},
   {"result", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6chorde_7clients_6_async_6Future_54result, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6chorde_7clients_6_async_6Future_53result},
   {"exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6chorde_7clients_6_async_6Future_56exception, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6chorde_7clients_6_async_6Future_55exception},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_58__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_6chorde_7clients_6_async_6Future_60__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
+static struct PyGetSetDef __pyx_getsets_6chorde_7clients_6_async_Future[] = {
+  {(char *)"_loop", __pyx_getprop_6chorde_7clients_6_async_6Future__loop, 0, (char *)0, 0},
+  {(char *)"_asyncio_future_blocking", __pyx_getprop_6chorde_7clients_6_async_6Future__asyncio_future_blocking, __pyx_setprop_6chorde_7clients_6_async_6Future__asyncio_future_blocking, (char *)0, 0},
+  {0, 0, 0, 0, 0}
+};
+
 #if PY_MAJOR_VERSION >= 3
 static __Pyx_PyAsyncMethodsStruct __pyx_tp_as_async_Future = {
   __pyx_pw_6chorde_7clients_6_async_6Future_7__await__, /*am_await*/
   0, /*am_aiter*/
   0, /*am_anext*/
   #if PY_VERSION_HEX >= 0x030A00A3
   0, /*am_send*/
@@ -11655,15 +12014,15 @@
   __pyx_tp_clear_6chorde_7clients_6_async_Future, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_6chorde_7clients_6_async_Future, /*tp_methods*/
   0, /*tp_members*/
-  0, /*tp_getset*/
+  __pyx_getsets_6chorde_7clients_6_async_Future, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
@@ -13135,30 +13494,36 @@
   {&__pyx_n_s_NONE, __pyx_k_NONE, sizeof(__pyx_k_NONE), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TimeoutError, __pyx_k_TimeoutError, sizeof(__pyx_k_TimeoutError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueCallback, __pyx_k_ValueCallback, sizeof(__pyx_k_ValueCallback), 0, 0, 1, 1},
   {&__pyx_n_s_WeakCallback, __pyx_k_WeakCallback, sizeof(__pyx_k_WeakCallback), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+  {&__pyx_n_s_asyncio, __pyx_k_asyncio, sizeof(__pyx_k_asyncio), 0, 0, 1, 1},
+  {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+  {&__pyx_n_s_asyncio_tasks, __pyx_k_asyncio_tasks, sizeof(__pyx_k_asyncio_tasks), 0, 0, 1, 1},
   {&__pyx_n_s_await, __pyx_k_await, sizeof(__pyx_k_await), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_callback, __pyx_k_callback, sizeof(__pyx_k_callback), 0, 0, 1, 1},
   {&__pyx_n_s_chorde_clients, __pyx_k_chorde_clients, sizeof(__pyx_k_chorde_clients), 0, 0, 1, 1},
   {&__pyx_n_s_chorde_clients__async, __pyx_k_chorde_clients__async, sizeof(__pyx_k_chorde_clients__async), 0, 0, 1, 1},
   {&__pyx_n_s_clear, __pyx_k_clear, sizeof(__pyx_k_clear), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+  {&__pyx_n_s_context, __pyx_k_context, sizeof(__pyx_k_context), 0, 0, 1, 1},
   {&__pyx_n_s_defer, __pyx_k_defer, sizeof(__pyx_k_defer), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_exc, __pyx_k_exc, sizeof(__pyx_k_exc), 0, 0, 1, 1},
   {&__pyx_n_s_exc_info, __pyx_k_exc_info, sizeof(__pyx_k_exc_info), 0, 0, 1, 1},
   {&__pyx_n_s_functools, __pyx_k_functools, sizeof(__pyx_k_functools), 0, 0, 1, 1},
+  {&__pyx_n_s_get_running_loop, __pyx_k_get_running_loop, sizeof(__pyx_k_get_running_loop), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_inspect, __pyx_k_inspect, sizeof(__pyx_k_inspect), 0, 0, 1, 1},
   {&__pyx_kp_s_lib_chorde_clients__async_pyx, __pyx_k_lib_chorde_clients__async_pyx, sizeof(__pyx_k_lib_chorde_clients__async_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
   {&__pyx_n_s_logging, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_me, __pyx_k_me, sizeof(__pyx_k_me), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
@@ -13180,14 +13545,15 @@
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_reason, __pyx_k_reason, sizeof(__pyx_k_reason), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_ref, __pyx_k_ref, sizeof(__pyx_k_ref), 0, 0, 1, 1},
   {&__pyx_n_s_reraise, __pyx_k_reraise, sizeof(__pyx_k_reraise), 0, 0, 1, 1},
+  {&__pyx_n_s_run, __pyx_k_run, sizeof(__pyx_k_run), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_set_exception, __pyx_k_set_exception, sizeof(__pyx_k_set_exception), 0, 0, 1, 1},
   {&__pyx_n_s_set_nothreads, __pyx_k_set_nothreads, sizeof(__pyx_k_set_nothreads), 0, 0, 1, 1},
   {&__pyx_n_s_set_result, __pyx_k_set_result, sizeof(__pyx_k_set_result), 0, 0, 1, 1},
   {&__pyx_n_s_set_strip_tracebacks, __pyx_k_set_strip_tracebacks, sizeof(__pyx_k_set_strip_tracebacks), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
@@ -13206,15 +13572,15 @@
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_wait, __pyx_k_wait, sizeof(__pyx_k_wait), 0, 0, 1, 1},
   {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
   {&__pyx_n_s_with_traceback, __pyx_k_with_traceback, sizeof(__pyx_k_with_traceback), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -13369,22 +13735,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "chorde/clients/_async.pyx":214
+  /* "chorde/clients/_async.pyx":216
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -13402,25 +13768,25 @@
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_tuple__20 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "chorde/clients/_async.pyx":29
+  /* "chorde/clients/_async.pyx":30
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_strip, __pyx_n_s_strip); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_strip, __pyx_n_s_strip); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_chorde_clients__async_pyx, __pyx_n_s_set_strip_tracebacks, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lib_chorde_clients__async_pyx, __pyx_n_s_set_strip_tracebacks, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 30, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NONE(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -13492,128 +13858,128 @@
   /*--- Type init code ---*/
   __pyx_vtabptr_6chorde_7clients_6_async_Future = &__pyx_vtable_6chorde_7clients_6_async_Future;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_done = (int (*)(struct __pyx_obj_6chorde_7clients_6_async_Future *))__pyx_f_6chorde_7clients_6_async_6Future_c_done;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_result = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int))__pyx_f_6chorde_7clients_6_async_6Future_c_result;
   __pyx_vtable_6chorde_7clients_6_async_Future._set_nothreads = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__set_nothreads;
   __pyx_vtable_6chorde_7clients_6_async_Future.set = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future_set;
   __pyx_vtable_6chorde_7clients_6_async_Future._on_stuff = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__on_stuff;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_Future.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_Future.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_Future.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_Future.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_Future, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_Future = &__pyx_type_6chorde_7clients_6_async_Future;
   __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper;
   __pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper.reraise = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *, int __pyx_skip_dispatch, struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise *__pyx_optional_args))__pyx_f_6chorde_7clients_6_async_16ExceptionWrapper_reraise;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionWrapper, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionWrapper, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_type_6chorde_7clients_6_async_ExceptionWrapper;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_WeakCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_WeakCallback = &__pyx_type_6chorde_7clients_6_async_WeakCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback = &__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ValueCallback = &__pyx_type_6chorde_7clients_6_async_ValueCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_MissCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_MissCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_MissCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_MissCallback = &__pyx_type_6chorde_7clients_6_async_MissCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionCallback = &__pyx_type_6chorde_7clients_6_async_ExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_AnyCallback = &__pyx_type_6chorde_7clients_6_async_AnyCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DoneCallback = &__pyx_type_6chorde_7clients_6_async_DoneCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_NONE.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_NONE.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_NONE = &__pyx_type_6chorde_7clients_6_async_NONE;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__.tp_dictoffset && __pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6chorde_7clients_6_async___pyx_scope_struct____await__ = &__pyx_type_6chorde_7clients_6_async___pyx_scope_struct____await__;
@@ -13875,161 +14241,173 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":3
  * import functools
  * import weakref
  * import threading             # <<<<<<<<<<<<<<
  * import logging
- * 
+ * import asyncio
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_threading, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "chorde/clients/_async.pyx":4
  * import weakref
  * import threading
  * import logging             # <<<<<<<<<<<<<<
+ * import asyncio
  * 
- * import cython
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_logging, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":8
+  /* "chorde/clients/_async.pyx":5
+ * import threading
+ * import logging
+ * import asyncio             # <<<<<<<<<<<<<<
+ * 
+ * import cython
+ */
+  __pyx_t_1 = __Pyx_patch_asyncio(__Pyx_Import(__pyx_n_s_asyncio, 0, -1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_asyncio, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "chorde/clients/_async.pyx":9
  * import cython
  * 
  * from chorde.clients import base             # <<<<<<<<<<<<<<
  * 
  * cdef object CacheMissError, CancelledError, TimeoutError
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_base);
   __Pyx_GIVEREF(__pyx_n_s_base);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_base);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_chorde_clients, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_chorde_clients, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_base, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_base, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":12
+  /* "chorde/clients/_async.pyx":13
  * cdef object CacheMissError, CancelledError, TimeoutError
  * cdef object wref, functools_partial
  * CacheMissError = base.CacheMissError             # <<<<<<<<<<<<<<
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CacheMissError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CacheMissError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_CacheMissError, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":13
+  /* "chorde/clients/_async.pyx":14
  * cdef object wref, functools_partial
  * CacheMissError = base.CacheMissError
  * CancelledError = base.CancelledError             # <<<<<<<<<<<<<<
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CancelledError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CancelledError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_CancelledError, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":14
+  /* "chorde/clients/_async.pyx":15
  * CacheMissError = base.CacheMissError
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError             # <<<<<<<<<<<<<<
  * wref = weakref.ref
  * functools_partial = functools.partial
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_TimeoutError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_TimeoutError, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":15
+  /* "chorde/clients/_async.pyx":16
  * CancelledError = base.CancelledError
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref             # <<<<<<<<<<<<<<
  * functools_partial = functools.partial
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_weakref); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ref); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ref); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_wref);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_wref, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":16
+  /* "chorde/clients/_async.pyx":17
  * TimeoutError = base.TimeoutError
  * wref = weakref.ref
  * functools_partial = functools.partial             # <<<<<<<<<<<<<<
  * 
  * cdef bint strip_tracebacks
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_functools); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_functools); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_partial); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async_functools_partial, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":19
+  /* "chorde/clients/_async.pyx":20
  * 
  * cdef bint strip_tracebacks
  * strip_tracebacks = False             # <<<<<<<<<<<<<<
  * 
  * cdef object _HTTPError = None
  */
   __pyx_v_6chorde_7clients_6_async_strip_tracebacks = 0;
 
-  /* "chorde/clients/_async.pyx":21
+  /* "chorde/clients/_async.pyx":22
  * strip_tracebacks = False
  * 
  * cdef object _HTTPError = None             # <<<<<<<<<<<<<<
  * 
  * try:
  */
   __Pyx_INCREF(Py_None);
   __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async__HTTPError);
   __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async__HTTPError, Py_None);
   __Pyx_GIVEREF(Py_None);
 
-  /* "chorde/clients/_async.pyx":23
+  /* "chorde/clients/_async.pyx":24
  * cdef object _HTTPError = None
  * 
  * try:             # <<<<<<<<<<<<<<
  *     from tornado.web import HTTPError as _HTTPError
  * except ImportError:
  */
   {
@@ -14037,39 +14415,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "chorde/clients/_async.pyx":24
+      /* "chorde/clients/_async.pyx":25
  * 
  * try:
  *     from tornado.web import HTTPError as _HTTPError             # <<<<<<<<<<<<<<
  * except ImportError:
  *     pass
  */
-      __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L2_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_n_s_HTTPError);
       __Pyx_GIVEREF(__pyx_n_s_HTTPError);
       PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_HTTPError);
-      __pyx_t_2 = __Pyx_Import(__pyx_n_s_tornado_web, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __pyx_t_2 = __Pyx_Import(__pyx_n_s_tornado_web, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L2_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_HTTPError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L2_error)
+      __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_HTTPError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L2_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XGOTREF(__pyx_v_6chorde_7clients_6_async__HTTPError);
       __Pyx_DECREF_SET(__pyx_v_6chorde_7clients_6_async__HTTPError, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "chorde/clients/_async.pyx":23
+      /* "chorde/clients/_async.pyx":24
  * cdef object _HTTPError = None
  * 
  * try:             # <<<<<<<<<<<<<<
  *     from tornado.web import HTTPError as _HTTPError
  * except ImportError:
  */
     }
@@ -14077,30 +14455,30 @@
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L7_try_end;
     __pyx_L2_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "chorde/clients/_async.pyx":25
+    /* "chorde/clients/_async.pyx":26
  * try:
  *     from tornado.web import HTTPError as _HTTPError
  * except ImportError:             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
     if (__pyx_t_6) {
       __Pyx_ErrRestore(0,0,0);
       goto __pyx_L3_exception_handled;
     }
     goto __pyx_L4_except_error;
     __pyx_L4_except_error:;
 
-    /* "chorde/clients/_async.pyx":23
+    /* "chorde/clients/_async.pyx":24
  * cdef object _HTTPError = None
  * 
  * try:             # <<<<<<<<<<<<<<
  *     from tornado.web import HTTPError as _HTTPError
  * except ImportError:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
@@ -14112,24 +14490,24 @@
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     __pyx_L7_try_end:;
   }
 
-  /* "chorde/clients/_async.pyx":29
+  /* "chorde/clients/_async.pyx":30
  * 
  * 
  * def set_strip_tracebacks(bint strip):             # <<<<<<<<<<<<<<
  *     """ Sets traceback stripping behavior for async futures
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_1set_strip_tracebacks, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6chorde_7clients_6_async_1set_strip_tracebacks, NULL, __pyx_n_s_chorde_clients__async); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_strip_tracebacks, __pyx_t_2) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_strip_tracebacks, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NONE(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -15651,14 +16029,162 @@
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
+/* PatchModuleWithCoroutine */
+static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
+#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
+    int result;
+    PyObject *globals, *result_obj;
+    globals = PyDict_New();  if (unlikely(!globals)) goto ignore;
+    result = PyDict_SetItemString(globals, "_cython_coroutine_type",
+    #ifdef __Pyx_Coroutine_USED
+        (PyObject*)__pyx_CoroutineType);
+    #else
+        Py_None);
+    #endif
+    if (unlikely(result < 0)) goto ignore;
+    result = PyDict_SetItemString(globals, "_cython_generator_type",
+    #ifdef __Pyx_Generator_USED
+        (PyObject*)__pyx_GeneratorType);
+    #else
+        Py_None);
+    #endif
+    if (unlikely(result < 0)) goto ignore;
+    if (unlikely(PyDict_SetItemString(globals, "_module", module) < 0)) goto ignore;
+    if (unlikely(PyDict_SetItemString(globals, "__builtins__", __pyx_b) < 0)) goto ignore;
+    result_obj = PyRun_String(py_code, Py_file_input, globals, globals);
+    if (unlikely(!result_obj)) goto ignore;
+    Py_DECREF(result_obj);
+    Py_DECREF(globals);
+    return module;
+ignore:
+    Py_XDECREF(globals);
+    PyErr_WriteUnraisable(module);
+    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch module with custom type", 1) < 0)) {
+        Py_DECREF(module);
+        module = NULL;
+    }
+#else
+    py_code++;
+#endif
+    return module;
+}
+
+/* PatchInspect */
+static PyObject* __Pyx_patch_inspect(PyObject* module) {
+#if defined(__Pyx_Generator_USED) && (!defined(CYTHON_PATCH_INSPECT) || CYTHON_PATCH_INSPECT)
+    static int inspect_patched = 0;
+    if (unlikely((!inspect_patched) && module)) {
+        module = __Pyx_Coroutine_patch_module(
+            module, ""
+"old_types = getattr(_module.isgenerator, '_cython_generator_types', None)\n"
+"if old_types is None or not isinstance(old_types, set):\n"
+"    old_types = set()\n"
+"    def cy_wrap(orig_func, type=type, cython_generator_types=old_types):\n"
+"        def cy_isgenerator(obj): return type(obj) in cython_generator_types or orig_func(obj)\n"
+"        cy_isgenerator._cython_generator_types = cython_generator_types\n"
+"        return cy_isgenerator\n"
+"    _module.isgenerator = cy_wrap(_module.isgenerator)\n"
+"old_types.add(_cython_generator_type)\n"
+        );
+        inspect_patched = 1;
+    }
+#else
+    if ((0)) return __Pyx_Coroutine_patch_module(module, NULL);
+#endif
+    return module;
+}
+
+/* PatchAsyncIO */
+static PyObject* __Pyx_patch_asyncio(PyObject* module) {
+#if PY_VERSION_HEX < 0x030500B2 &&\
+        (defined(__Pyx_Coroutine_USED) || defined(__Pyx_Generator_USED)) &&\
+        (!defined(CYTHON_PATCH_ASYNCIO) || CYTHON_PATCH_ASYNCIO)
+    PyObject *patch_module = NULL;
+    static int asyncio_patched = 0;
+    if (unlikely((!asyncio_patched) && module)) {
+        PyObject *package;
+        package = __Pyx_Import(__pyx_n_s_asyncio_coroutines, NULL, 0);
+        if (package) {
+            patch_module = __Pyx_Coroutine_patch_module(
+                PyObject_GetAttrString(package, "coroutines"), ""
+"try:\n"
+"    coro_types = _module._COROUTINE_TYPES\n"
+"except AttributeError: pass\n"
+"else:\n"
+"    if _cython_coroutine_type is not None and _cython_coroutine_type not in coro_types:\n"
+"        coro_types = tuple(coro_types) + (_cython_coroutine_type,)\n"
+"    if _cython_generator_type is not None and _cython_generator_type not in coro_types:\n"
+"        coro_types = tuple(coro_types) + (_cython_generator_type,)\n"
+"_module._COROUTINE_TYPES = coro_types\n"
+            );
+        } else {
+            PyErr_Clear();
+            package = __Pyx_Import(__pyx_n_s_asyncio_tasks, NULL, 0);
+            if (unlikely(!package)) goto asyncio_done;
+            patch_module = __Pyx_Coroutine_patch_module(
+                PyObject_GetAttrString(package, "tasks"), ""
+"if hasattr(_module, 'iscoroutine'):\n"
+"    old_types = getattr(_module.iscoroutine, '_cython_coroutine_types', None)\n"
+"    if old_types is None or not isinstance(old_types, set):\n"
+"        old_types = set()\n"
+"        def cy_wrap(orig_func, type=type, cython_coroutine_types=old_types):\n"
+"            def cy_iscoroutine(obj): return type(obj) in cython_coroutine_types or orig_func(obj)\n"
+"            cy_iscoroutine._cython_coroutine_types = cython_coroutine_types\n"
+"            return cy_iscoroutine\n"
+"        _module.iscoroutine = cy_wrap(_module.iscoroutine)\n"
+"    if _cython_coroutine_type is not None:\n"
+"        old_types.add(_cython_coroutine_type)\n"
+"    if _cython_generator_type is not None:\n"
+"        old_types.add(_cython_generator_type)\n"
+            );
+        }
+        Py_DECREF(package);
+        if (unlikely(!patch_module)) goto ignore;
+asyncio_done:
+        PyErr_Clear();
+        asyncio_patched = 1;
+#ifdef __Pyx_Generator_USED
+        {
+            PyObject *inspect_module;
+            if (patch_module) {
+                inspect_module = PyObject_GetAttr(patch_module, __pyx_n_s_inspect);
+                Py_DECREF(patch_module);
+            } else {
+                inspect_module = __Pyx_Import(__pyx_n_s_inspect, NULL, 0);
+            }
+            if (unlikely(!inspect_module)) goto ignore;
+            inspect_module = __Pyx_patch_inspect(inspect_module);
+            if (unlikely(!inspect_module)) {
+                Py_DECREF(module);
+                module = NULL;
+            }
+            Py_XDECREF(inspect_module);
+        }
+#else
+        if ((0)) return __Pyx_patch_inspect(module);
+#endif
+    }
+    return module;
+ignore:
+    PyErr_WriteUnraisable(module);
+    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch asyncio package with custom generator type", 1) < 0)) {
+        Py_DECREF(module);
+        module = NULL;
+    }
+#else
+    if ((0)) return __Pyx_patch_inspect(__Pyx_Coroutine_patch_module(module, NULL));
+#endif
+    return module;
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -17417,54 +17943,14 @@
     Py_XINCREF(code);
     gen->gi_code = code;
     gen->gi_frame = NULL;
     PyObject_GC_Track(gen);
     return gen;
 }
 
-/* PatchModuleWithCoroutine */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-    int result;
-    PyObject *globals, *result_obj;
-    globals = PyDict_New();  if (unlikely(!globals)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_coroutine_type",
-    #ifdef __Pyx_Coroutine_USED
-        (PyObject*)__pyx_CoroutineType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_generator_type",
-    #ifdef __Pyx_Generator_USED
-        (PyObject*)__pyx_GeneratorType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "_module", module) < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "__builtins__", __pyx_b) < 0)) goto ignore;
-    result_obj = PyRun_String(py_code, Py_file_input, globals, globals);
-    if (unlikely(!result_obj)) goto ignore;
-    Py_DECREF(result_obj);
-    Py_DECREF(globals);
-    return module;
-ignore:
-    Py_XDECREF(globals);
-    PyErr_WriteUnraisable(module);
-    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch module with custom type", 1) < 0)) {
-        Py_DECREF(module);
-        module = NULL;
-    }
-#else
-    py_code++;
-#endif
-    return module;
-}
-
 /* PatchGeneratorABC */
 #ifndef CYTHON_REGISTER_ABCS
 #define CYTHON_REGISTER_ABCS 1
 #endif
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
 static PyObject* __Pyx_patch_abc_module(PyObject *module);
 static PyObject* __Pyx_patch_abc_module(PyObject *module) {
```

### Comparing `chorde-1.0.8/lib/chorde/clients/_async.pyx` & `chorde-1.0.9/lib/chorde/clients/_async.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import weakref
 import threading
 import logging
+import asyncio
 
 import cython
 
 from chorde.clients import base
 
 cdef object CacheMissError, CancelledError, TimeoutError
 cdef object wref, functools_partial
@@ -172,14 +173,15 @@
         self._cb = None
         self._value = NONE
         self._logger = logger
         self._done_event = None
         self._running = 0
         self._cancel_pending = 0
         self._cancelled = 0
+        self._asyncio_future_blocking = True
 
     cpdef _set_nothreads(self, value):
         """
         Like set(), but assuming no threading is involved. It won't wake waiting threads,
         nor will it try to be thread-safe. Safe to call when the calling
         thread is the only one owning references to this future, and much faster.
         """
@@ -222,17 +224,21 @@
 
         if self._done_event is not None:
             # wake up waiting threads
             self._done_event.set()
 
     def __await__(self):
         if not self.c_done():
-            return (yield self)
+            yield self
         return self.c_result(0, 1)
 
+    @property
+    def _loop(self):
+        return asyncio.get_running_loop()
+
     def set_result(self, value):
         self.set(value)
 
     def miss(self):
         """
         Shorthand for setting a cache miss result
         """
@@ -332,19 +338,21 @@
             if self._cb is None:
                 self._cb = list()
             self._cb.append(callback)
         else:
             callback(self._value)
         return self
 
-    def add_done_callback(self, callback):
+    def add_done_callback(self, callback, *, context=None):
         """
         When the operatio is done, the callback will be invoked with the
         future object as argument.
         """
+        if context is not None:
+            callback = functools_partial(context.run, callback)
         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
 
     cdef int c_done(self) except -1:
         """
         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
         """
         if self._value is not NONE or self._cancelled:
```

### Comparing `chorde-1.0.8/lib/chorde/clients/async.c` & `chorde-1.0.9/lib/chorde/clients/async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/asyncache.c` & `chorde-1.0.9/lib/chorde/clients/asyncache.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/asyncache.py` & `chorde-1.0.9/lib/chorde/clients/asyncache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/base.c` & `chorde-1.0.9/lib/chorde/clients/base.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/base.py` & `chorde-1.0.9/lib/chorde/clients/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/coherent.py` & `chorde-1.0.9/lib/chorde/clients/coherent.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/elasticache.py` & `chorde-1.0.9/lib/chorde/clients/elasticache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/files.py` & `chorde-1.0.9/lib/chorde/clients/files.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/inproc.c` & `chorde-1.0.9/lib/chorde/clients/inproc.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/inproc.py` & `chorde-1.0.9/lib/chorde/clients/inproc.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/memcached.py` & `chorde-1.0.9/lib/chorde/clients/memcached.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/tiered.c` & `chorde-1.0.9/lib/chorde/clients/tiered.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/clients/tiered.py` & `chorde-1.0.9/lib/chorde/clients/tiered.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/decorators.c` & `chorde-1.0.9/lib/chorde/decorators.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/decorators.pxd` & `chorde-1.0.9/lib/chorde/decorators.pxd`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/decorators.py` & `chorde-1.0.9/lib/chorde/decorators.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/dnsutils.py` & `chorde-1.0.9/lib/chorde/dnsutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/external_integration.py` & `chorde-1.0.9/lib/chorde/external_integration.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/mq/coherence.py` & `chorde-1.0.9/lib/chorde/mq/coherence.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/mq/ipsub/base.py` & `chorde-1.0.9/lib/chorde/mq/ipsub/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/mq/ipsub/ipsub_zmq.py` & `chorde-1.0.9/lib/chorde/mq/ipsub/ipsub_zmq.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/sPickle.py` & `chorde-1.0.9/lib/chorde/sPickle.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/serialize.py` & `chorde-1.0.9/lib/chorde/serialize.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/shmemutils.py` & `chorde-1.0.9/lib/chorde/shmemutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/threadpool.py` & `chorde-1.0.9/lib/chorde/threadpool.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde/worker.py` & `chorde-1.0.9/lib/chorde/worker.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/lib/chorde.egg-info/PKG-INFO` & `chorde-1.0.9/lib/chorde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.8
+Version: 1.0.9
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.8/lib/chorde.egg-info/SOURCES.txt` & `chorde-1.0.9/lib/chorde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chorde-1.0.8/setup.py` & `chorde-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 no_pyrex = False
 try:
     from Cython.Distutils import build_ext, Extension
     from Cython.Build import cythonize
 except:
     no_pyrex = True
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 
 version_path = os.path.join(os.path.dirname(__file__), 'lib', 'chorde', '_version.py')
 if not os.path.exists(version_path):
     with open(version_path, "w") as version_file:
         pass
 with open(version_path, "r+") as version_file:
     version_content = "__version__ = %r" % (VERSION,)
```

