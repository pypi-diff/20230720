# Comparing `tmp/types-pyserial-3.5.0.8.tar.gz` & `tmp/types-pyserial-3.5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyserial-3.5.0.8.tar", last modified: Mon Mar 27 18:24:11 2023, max compression
+gzip compressed data, was "types-pyserial-3.5.0.9.tar", last modified: Thu Jul 20 15:16:38 2023, max compression
```

## Comparing `types-pyserial-3.5.0.8.tar` & `types-pyserial-3.5.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-27 18:24:10.000000 types-pyserial-3.5.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:10.000000 types-pyserial-3.5.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.579049 types-pyserial-3.5.0.8/serial-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-27 18:24:10.000000 types-pyserial-3.5.0.8/serial-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/rfc2217.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/rs485.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/serialcli.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/serialjava.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/serialposix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/serialutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/serialwin32.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/serial-stubs/threaded/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/threaded/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/serial-stubs/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/hexlify_codec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_linux.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_osx.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_posix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_windows.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/tools/miniterm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/serial-stubs/urlhandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_alt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_cp2110.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_hwgrep.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_loop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_rfc2217.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_socket.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_spy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-27 18:21:24.000000 types-pyserial-3.5.0.8/serial-stubs/win32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-27 18:24:10.000000 types-pyserial-3.5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:11.583049 types-pyserial-3.5.0.8/types_pyserial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:11.000000 types-pyserial-3.5.0.8/types_pyserial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-27 18:24:11.000000 types-pyserial-3.5.0.8/types_pyserial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:11.000000 types-pyserial-3.5.0.8/types_pyserial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:24:11.000000 types-pyserial-3.5.0.8/types_pyserial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.949419 types-pyserial-3.5.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:16:38.949419 types-pyserial-3.5.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.941419 types-pyserial-3.5.0.9/serial-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/serial-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/rfc2217.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/rs485.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/serialcli.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/serialjava.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/serialposix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/serialutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/serialwin32.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.941419 types-pyserial-3.5.0.9/serial-stubs/threaded/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/threaded/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.945419 types-pyserial-3.5.0.9/serial-stubs/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/hexlify_codec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_linux.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_osx.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_posix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/tools/miniterm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.949419 types-pyserial-3.5.0.9/serial-stubs/urlhandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_alt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_cp2110.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_hwgrep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_loop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_rfc2217.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_spy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-20 15:15:13.000000 types-pyserial-3.5.0.9/serial-stubs/win32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:38.949419 types-pyserial-3.5.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:38.949419 types-pyserial-3.5.0.9/types_pyserial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/types_pyserial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/types_pyserial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/types_pyserial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:16:38.000000 types-pyserial-3.5.0.9/types_pyserial.egg-info/top_level.txt
```

### Comparing `types-pyserial-3.5.0.8/CHANGELOG.md` & `types-pyserial-3.5.0.9/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.5.0.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.5.0.8 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 3.5.0.7 (2023-03-09)
 
 pyserial: Fix read and write methods (#9825)
```

### Comparing `types-pyserial-3.5.0.8/PKG-INFO` & `types-pyserial-3.5.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyserial
-Version: 3.5.0.8
+Version: 3.5.0.9
 Summary: Typing stubs for pyserial
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyserial.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyserial`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyserial. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyserial-3.5.0.8/serial-stubs/__init__.pyi` & `types-pyserial-3.5.0.9/serial-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/rfc2217.pyi` & `types-pyserial-3.5.0.9/serial-stubs/rfc2217.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/serialcli.pyi` & `types-pyserial-3.5.0.9/serial-stubs/serialcli.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/serialjava.pyi` & `types-pyserial-3.5.0.9/serial-stubs/serialjava.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/serialposix.pyi` & `types-pyserial-3.5.0.9/serial-stubs/serialposix.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/serialutil.pyi` & `types-pyserial-3.5.0.9/serial-stubs/serialutil.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/serialwin32.pyi` & `types-pyserial-3.5.0.9/serial-stubs/serialwin32.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/threaded/__init__.pyi` & `types-pyserial-3.5.0.9/serial-stubs/threaded/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/tools/hexlify_codec.pyi` & `types-pyserial-3.5.0.9/serial-stubs/tools/hexlify_codec.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_common.pyi` & `types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_common.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_osx.pyi` & `types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_osx.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/tools/list_ports_windows.pyi` & `types-pyserial-3.5.0.9/serial-stubs/tools/list_ports_windows.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/tools/miniterm.pyi` & `types-pyserial-3.5.0.9/serial-stubs/tools/miniterm.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_loop.pyi` & `types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_loop.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_socket.pyi` & `types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_socket.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/urlhandler/protocol_spy.pyi` & `types-pyserial-3.5.0.9/serial-stubs/urlhandler/protocol_spy.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/serial-stubs/win32.pyi` & `types-pyserial-3.5.0.9/serial-stubs/win32.pyi`

 * *Files identical despite different names*

### Comparing `types-pyserial-3.5.0.8/setup.py` & `types-pyserial-3.5.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyserial`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyserial. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.5.0.8",
+      version="3.5.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyserial.md",
```

### Comparing `types-pyserial-3.5.0.8/types_pyserial.egg-info/PKG-INFO` & `types-pyserial-3.5.0.9/types_pyserial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyserial
-Version: 3.5.0.8
+Version: 3.5.0.9
 Summary: Typing stubs for pyserial
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyserial.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyserial`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyserial. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyserial-3.5.0.8/types_pyserial.egg-info/SOURCES.txt` & `types-pyserial-3.5.0.9/types_pyserial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

