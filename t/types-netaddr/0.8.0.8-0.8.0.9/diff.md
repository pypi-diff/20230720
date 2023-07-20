# Comparing `tmp/types-netaddr-0.8.0.8.tar.gz` & `tmp/types-netaddr-0.8.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-netaddr-0.8.0.8.tar", last modified: Thu Apr 13 12:31:03 2023, max compression
+gzip compressed data, was "types-netaddr-0.8.0.9.tar", last modified: Thu Jul 20 15:19:07 2023, max compression
```

## Comparing `types-netaddr-0.8.0.8.tar` & `types-netaddr-0.8.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/netaddr-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/contrib/subnet_splitter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/eui/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/eui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/eui/ieee.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/fbsocket.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/ip/
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/iana.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/nmap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/rfc1924.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/sets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui48.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv6.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/types_netaddr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.907273 types-netaddr-0.8.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.899273 types-netaddr-0.8.0.9/netaddr-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/netaddr-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/netaddr-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/contrib/subnet_splitter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/netaddr-stubs/eui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/eui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/eui/ieee.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/fbsocket.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/netaddr-stubs/ip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/iana.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/nmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/rfc1924.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/ip/sets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/netaddr-stubs/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/strategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/strategy/eui48.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/strategy/eui64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/strategy/ipv4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-20 15:15:13.000000 types-netaddr-0.8.0.9/netaddr-stubs/strategy/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:07.907273 types-netaddr-0.8.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:07.903273 types-netaddr-0.8.0.9/types_netaddr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/types_netaddr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/types_netaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/types_netaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:19:07.000000 types-netaddr-0.8.0.9/types_netaddr.egg-info/top_level.txt
```

### Comparing `types-netaddr-0.8.0.8/CHANGELOG.md` & `types-netaddr-0.8.0.9/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.8.0.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.8.0.8 (2023-04-13)
 
 Style: prefer `type[Foo | Bar]` over `type[Foo] | type[Bar]` (#10039)
 
 ## 0.8.0.7 (2023-03-27)
 
 Add defaults for third-party stubs M-O (#9956)
```

### Comparing `types-netaddr-0.8.0.8/PKG-INFO` & `types-netaddr-0.8.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 0.8.0.8
+Version: 0.8.0.9
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/__init__.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/core.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/eui/__init__.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/eui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/eui/ieee.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/eui/ieee.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/ip/__init__.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/ip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/ip/glob.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/ip/glob.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/ip/iana.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/ip/iana.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/ip/sets.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/ip/sets.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/strategy/__init__.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/strategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui48.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/strategy/eui48.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui64.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/strategy/eui64.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv4.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/strategy/ipv4.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv6.pyi` & `types-netaddr-0.8.0.9/netaddr-stubs/strategy/ipv6.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.8/setup.py` & `types-netaddr-0.8.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.8.0.8",
+      version="0.8.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md",
```

### Comparing `types-netaddr-0.8.0.8/types_netaddr.egg-info/PKG-INFO` & `types-netaddr-0.8.0.9/types_netaddr.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 0.8.0.8
+Version: 0.8.0.9
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-netaddr-0.8.0.8/types_netaddr.egg-info/SOURCES.txt` & `types-netaddr-0.8.0.9/types_netaddr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

