# Comparing `tmp/abst-1.9.8.tar.gz` & `tmp/abst-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.8.tar", last modified: Wed Jul 12 12:16:20 2023, max compression
+gzip compressed data, was "abst-1.9.9.tar", last modified: Thu Jul 20 14:46:24 2023, max compression
```

## Comparing `abst-1.9.8.tar` & `abst-1.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.750786 abst-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 12:16:10.000000 abst-1.9.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-12 12:16:20.750786 abst-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-12 12:16:10.000000 abst-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.742786 abst-1.9.8/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-12 12:16:10.000000 abst-1.9.8/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22990 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-12 12:16:10.000000 abst-1.9.8/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-12 12:16:10.000000 abst-1.9.8/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-12 12:16:10.000000 abst-1.9.8/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-12 12:16:10.000000 abst-1.9.8/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 12:16:10.000000 abst-1.9.8/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-12 12:16:10.000000 abst-1.9.8/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 12:16:10.000000 abst-1.9.8/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:16:20.750786 abst-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-12 12:16:10.000000 abst-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.750786 abst-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 12:16:10.000000 abst-1.9.8/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.194506 abst-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 14:46:12.000000 abst-1.9.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 14:46:24.194506 abst-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-20 14:46:12.000000 abst-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 14:46:12.000000 abst-1.9.9/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-20 14:46:12.000000 abst-1.9.9/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-20 14:46:12.000000 abst-1.9.9/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-20 14:46:12.000000 abst-1.9.9/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 14:46:12.000000 abst-1.9.9/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-20 14:46:12.000000 abst-1.9.9/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:12.000000 abst-1.9.9/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-20 14:46:12.000000 abst-1.9.9/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 14:46:12.000000 abst-1.9.9/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 14:46:12.000000 abst-1.9.9/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.190506 abst-1.9.9/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:46:24.000000 abst-1.9.9/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:46:24.194506 abst-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 14:46:12.000000 abst-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:46:24.194506 abst-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-20 14:46:12.000000 abst-1.9.9/tests/test_sample_dict.py
```

### Comparing `abst-1.9.8/LICENSE.md` & `abst-1.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/PKG-INFO` & `abst-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.8
+Version: 1.9.9
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.8/README.md` & `abst-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.9/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/bastion_support/oci_bastion.py` & `abst-1.9.9/abst/bastion_support/oci_bastion.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
     def run_ssh_tunnel_managed_session(self, bid, host, private_key_path, username,
                                        ip, port,
                                        shell):
         print(f"Bastion {self.get_print_name()} initialized")
         print(f"Initializing SSH Tunnel for {self.get_print_name()}")
 
-        ssh_tunnel_args = f'ssh -i {private_key_path} -o ProxyCommand="ssh -i {private_key_path} -W %h:%p -p {port} {bid}@{host} -A" -p {port} {username}@{ip} -A'
+        ssh_tunnel_args = f'ssh -i {private_key_path} -o ServerAliveInterval=20 -o ProxyCommand="ssh -i {private_key_path} -W %h:%p -p {port} {bid}@{host} -A" -p {port} {username}@{ip} -A'
         self.__run_ssh_tunnel_call(ssh_tunnel_args, shell, already_split=True)
         return ssh_tunnel_args
 
     def run_ssh_tunnel_port_forward(self, bid, host, ip, port, shell, local_port, ssh_pub_key_path):
         print(f"Bastion {self.get_print_name()} initialized")
         print(f"Initializing SSH Tunnel for {self.get_print_name()}")
         ssh_tunnel_arg_str = f"ssh -o ServerAliveInterval=20 -N -L {local_port}:{ip}:{port} -p 22 {bid}@{host} -vvv -i {ssh_pub_key_path.strip('.pub')}"
```

### Comparing `abst-1.9.8/abst/cfg_func.py` & `abst-1.9.9/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/config.py` & `abst-1.9.9/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/dialogs.py` & `abst-1.9.9/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/main.py` & `abst-1.9.9/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/notifier/version_notifier.py` & `abst-1.9.9/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/tools.py` & `abst-1.9.9/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst/wrappers.py` & `abst-1.9.9/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/abst.egg-info/PKG-INFO` & `abst-1.9.9/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.8
+Version: 1.9.9
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.8/abst.egg-info/SOURCES.txt` & `abst-1.9.9/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.8/setup.py` & `abst-1.9.9/setup.py`

 * *Files identical despite different names*

