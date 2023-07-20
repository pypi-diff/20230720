# Comparing `tmp/tarn-0.9.4.tar.gz` & `tmp/tarn-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.9.4.tar", last modified: Tue Jul 18 13:22:11 2023, max compression
+gzip compressed data, was "tarn-0.9.5.tar", last modified: Thu Jul 20 11:27:18 2023, max compression
```

## Comparing `tarn-0.9.4.tar` & `tarn-0.9.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.434451 tarn-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-18 13:22:09.000000 tarn-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 13:22:09.000000 tarn-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 13:22:11.434451 tarn-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 13:22:09.000000 tarn-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 13:22:09.000000 tarn-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 13:22:09.000000 tarn-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:22:11.434451 tarn-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-18 13:22:09.000000 tarn-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.434451 tarn-0.9.4/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-20 11:27:13.000000 tarn-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 11:27:13.000000 tarn-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-20 11:27:18.258111 tarn-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 11:27:13.000000 tarn-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-20 11:27:13.000000 tarn-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 11:27:13.000000 tarn-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:27:18.258111 tarn-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-20 11:27:13.000000 tarn-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.254111 tarn-0.9.5/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.254111 tarn-0.9.5/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.254111 tarn-0.9.5/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.258111 tarn-0.9.5/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-20 11:27:13.000000 tarn-0.9.5/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:27:18.254111 tarn-0.9.5/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-20 11:27:18.000000 tarn-0.9.5/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 11:27:18.000000 tarn-0.9.5/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:27:18.000000 tarn-0.9.5/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 11:27:18.000000 tarn-0.9.5/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 11:27:18.000000 tarn-0.9.5/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.9.4/LICENSE` & `tarn-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/PKG-INFO` & `tarn-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.4
+Version: 0.9.5
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.5.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.4/README.md` & `tarn-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/pyproject.toml` & `tarn-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/setup.py` & `tarn-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/cache/storage.py` & `tarn-0.9.5/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/compat.py` & `tarn-0.9.5/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/config.py` & `tarn-0.9.5/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/digest.py` & `tarn-0.9.5/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/interface.py` & `tarn-0.9.5/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/local/storage.py` & `tarn-0.9.5/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/disk_dict.py` & `tarn-0.9.5/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/fanout.py` & `tarn-0.9.5/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/interface.py` & `tarn-0.9.5/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/levels.py` & `tarn-0.9.5/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/nginx.py` & `tarn-0.9.5/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/redis.py` & `tarn-0.9.5/tarn/location/redis.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/location/s3.py` & `tarn-0.9.5/tarn/location/s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,18 +35,20 @@
         self, key: Key, return_labels: bool
     ) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         try:
             path = self._key_to_path(key)
             try:
                 if return_labels:
                     self.update_usage_date(path)
-                    yield self._get_buffer(path), self.get_labels(path)
+                    with self._get_buffer(path) as buffer:
+                        yield buffer, self.get_labels(path)
                 else:
                     self.update_usage_date(path)
-                    yield self._get_buffer(path)
+                    with self._get_buffer(path) as buffer:
+                        yield buffer
 
             except ClientError as e:
                 if (
                     e.response['ResponseMetadata']['HTTPStatusCode'] == 404
                     or e.response['Error']['Code'] == 'NoSuchKey'
                 ):  # file doesn't exist
                     yield
@@ -64,37 +66,39 @@
 
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager:
         try:
             path = self._key_to_path(key)
             with value_to_buffer(value) as value:
                 try:
-                    obj_body_buffer = self._get_buffer(path)
-                    try:
-                        match_buffers(value, obj_body_buffer, context=key.hex())
-                    except ValueError as e:
-                        raise CollisionError(
-                            f'Written value and the new one does not match: {key}'
-                        ) from e
-                    self.update_labels(path, labels)
-                    self.update_usage_date(path)
-                    yield self._get_buffer(path)
-                    return
+                    with self._get_buffer(path) as obj_body_buffer:
+                        try:
+                            match_buffers(value, obj_body_buffer, context=key.hex())
+                        except ValueError as e:
+                            raise CollisionError(
+                                f'Written value and the new one does not match: {key}'
+                            ) from e
+                        self.update_labels(path, labels)
+                        self.update_usage_date(path)
+                        with self._get_buffer(path) as buffer:
+                            yield buffer
+                            return
                 except ClientError as e:
                     if (
                         e.response['Error']['Code'] == '404'
                         or e.response['Error']['Code'] == 'NoSuchKey'
                     ):
                         self.s3.upload_fileobj(
                             Bucket=self.bucket, Key=path, Fileobj=value
                         )
                         self.update_labels(path, labels)
                         self.update_usage_date(path)
-                        yield self._get_buffer(path)
-                        return
+                        with self._get_buffer(path) as buffer:
+                            yield buffer
+                            return
                     else:
                         raise
                 except ConnectionError:
                     yield
         except StorageCorruption:
             self.delete(key)
 
@@ -134,14 +138,16 @@
             self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet']
         )
         if 'usage_date' in tags_dict:
             return datetime.fromtimestamp(float(tags_dict['usage_date']))
         return None
 
     def _get_buffer(self, path):
+        # with self.s3.get_object(Bucket=self.bucket, Key=path)['Body'] as obj_body:
+        #     assert False, obj_body.read()
         return StreamingBodyBuffer(self.s3.get_object, Bucket=self.bucket, Key=path)
 
     def _key_to_path(self, key: Key):
         return str(key_to_relative(key, [2, len(key) - 2]))
 
     def _path_to_key(self, path: str):
         return bytes.fromhex(path.replace('/', ''))
@@ -163,33 +169,35 @@
 
     def seek(self, offset: int, whence: int = SEEK_SET) -> int:
         # we can either return to the begining of the stream or do nothing
         #  everythnig else is too expensive
         if whence == SEEK_SET:
             if offset == 0:
                 self._streaming_body = self.getter(**self.kwargs).get('Body')
-                return
+                return 0
             if offset == self.tell():
-                return
+                return offset
 
         if whence == SEEK_CUR:
             if offset == 0:
-                return
+                return self.tell()
             if offset == -self.tell():
                 self._streaming_body = self.getter(**self.kwargs).get('Body')
-                return
-
-        if whence == SEEK_END:
-            if offset == 0:
-                return
+                return 0
 
         raise NotImplementedError('Cannot seek anywhere but the begining of the stream')
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type, value, traceback):
+        self.close()
+
     def __getattribute__(self, attr) -> Any:
-        if attr in ('seek', 'getter', 'kwargs'):
+        if attr in ('seek', 'getter', 'kwargs', '__enter__', '__exit__'):
             return super().__getattribute__(attr)
         streaming_body = super().__getattribute__('_streaming_body')
         return getattr(streaming_body, attr)
 
 
 class S3Meta(Meta):
     def __init__(self, path, location):
```

### Comparing `tarn-0.9.4/tarn/location/scp.py` & `tarn-0.9.5/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/pickler/compat.py` & `tarn-0.9.5/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/pickler/interface.py` & `tarn-0.9.5/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/pool/hash_key.py` & `tarn-0.9.5/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/pool/pickle_key.py` & `tarn-0.9.5/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/serializers.py` & `tarn-0.9.5/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/tools/labels.py` & `tarn-0.9.5/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/tools/locker.py` & `tarn-0.9.5/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/tools/size.py` & `tarn-0.9.5/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/tools/usage.py` & `tarn-0.9.5/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn/utils.py` & `tarn-0.9.5/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.4/tarn.egg-info/PKG-INFO` & `tarn-0.9.5/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.4
+Version: 0.9.5
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.5.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.4/tarn.egg-info/SOURCES.txt` & `tarn-0.9.5/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

