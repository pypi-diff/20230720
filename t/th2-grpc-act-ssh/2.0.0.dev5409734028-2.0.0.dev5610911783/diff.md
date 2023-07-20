# Comparing `tmp/th2_grpc_act_ssh-2.0.0.dev5409734028.tar.gz` & `tmp/th2_grpc_act_ssh-2.0.0.dev5610911783.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_ssh-2.0.0.dev5409734028.tar", last modified: Thu Jun 29 07:47:22 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_ssh-2.0.0.dev5610911783.tar", last modified: Thu Jul 20 12:23:07 2023, max compression
```

## Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028.tar` & `th2_grpc_act_ssh-2.0.0.dev5610911783.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-29 07:46:31.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4522 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-29 07:47:06.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_service.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-07-20 12:22:10.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-20 12:22:10.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4522 2023-07-20 12:22:10.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-07-20 12:22:10.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-07-20 12:22:46.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 12:23:07.000000 th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/PKG-INFO` & `th2_grpc_act_ssh-2.0.0.dev5610911783/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_ssh
-Version: 2.0.0.dev5409734028
+Version: 2.0.0.dev5610911783
 Summary: th2_grpc_act_ssh
 Home-page: https://github.com/th2-net/th2-grpc-act-ssh
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (2.0.0)
```

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/README.md` & `th2_grpc_act_ssh-2.0.0.dev5610911783/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/setup.py` & `th2_grpc_act_ssh-2.0.0.dev5610911783/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh.proto` & `th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.py` & `th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.pyi` & `th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2_grpc.py` & `th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh/act_ssh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/PKG-INFO` & `th2_grpc_act_ssh-2.0.0.dev5610911783/th2_grpc_act_ssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-ssh
-Version: 2.0.0.dev5409734028
+Version: 2.0.0.dev5610911783
 Summary: th2_grpc_act_ssh
 Home-page: https://github.com/th2-net/th2-grpc-act-ssh
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (2.0.0)
```

