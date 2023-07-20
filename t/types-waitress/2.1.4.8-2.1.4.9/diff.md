# Comparing `tmp/types-waitress-2.1.4.8.tar.gz` & `tmp/types-waitress-2.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-waitress-2.1.4.8.tar", last modified: Wed May 10 15:21:41 2023, max compression
+gzip compressed data, was "types-waitress-2.1.4.9.tar", last modified: Thu Jul 20 15:17:31 2023, max compression
```

## Comparing `types-waitress-2.1.4.8.tar` & `types-waitress-2.1.4.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:41.379812 types-waitress-2.1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-10 15:21:40.000000 types-waitress-2.1.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:40.000000 types-waitress-2.1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:21:41.379812 types-waitress-2.1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:41.379812 types-waitress-2.1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-10 15:21:40.000000 types-waitress-2.1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:41.375812 types-waitress-2.1.4.8/types_waitress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:21:41.000000 types-waitress-2.1.4.8/types_waitress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-10 15:21:41.000000 types-waitress-2.1.4.8/types_waitress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:41.000000 types-waitress-2.1.4.8/types_waitress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:21:41.000000 types-waitress-2.1.4.8/types_waitress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:41.379812 types-waitress-2.1.4.8/waitress-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 15:21:40.000000 types-waitress-2.1.4.8/waitress-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/adjustments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/buffers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/proxy_headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/receiver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/rfc7230.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/trigger.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/utilities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-10 15:19:44.000000 types-waitress-2.1.4.8/waitress-stubs/wasyncore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.302052 types-waitress-2.1.4.9/types_waitress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/waitress-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/waitress-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/adjustments.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/buffers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/proxy_headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/receiver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/rfc7230.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/trigger.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/utilities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/wasyncore.pyi
```

### Comparing `types-waitress-2.1.4.8/CHANGELOG.md` & `types-waitress-2.1.4.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.1.4.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.1.4.8 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 2.1.4.7 (2023-03-29)
 
 Remove unnecessary ellipsis expressions (#9976)
```

### Comparing `types-waitress-2.1.4.8/PKG-INFO` & `types-waitress-2.1.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-waitress
-Version: 2.1.4.8
+Version: 2.1.4.9
 Summary: Typing stubs for waitress
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `waitress`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-waitress-2.1.4.8/setup.py` & `types-waitress-2.1.4.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `waitress`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.4.8",
+      version="2.1.4.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['waitress-stubs'],
-      package_data={'waitress-stubs': ['__init__.pyi', 'adjustments.pyi', 'buffers.pyi', 'channel.pyi', 'compat.pyi', 'parser.pyi', 'proxy_headers.pyi', 'receiver.pyi', 'rfc7230.pyi', 'runner.pyi', 'server.pyi', 'task.pyi', 'trigger.pyi', 'utilities.pyi', 'wasyncore.pyi', 'METADATA.toml']},
+      package_data={'waitress-stubs': ['__init__.pyi', 'adjustments.pyi', 'buffers.pyi', 'channel.pyi', 'compat.pyi', 'parser.pyi', 'proxy_headers.pyi', 'receiver.pyi', 'rfc7230.pyi', 'runner.pyi', 'server.pyi', 'task.pyi', 'trigger.pyi', 'utilities.pyi', 'wasyncore.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-waitress-2.1.4.8/types_waitress.egg-info/PKG-INFO` & `types-waitress-2.1.4.9/types_waitress.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-waitress
-Version: 2.1.4.8
+Version: 2.1.4.9
 Summary: Typing stubs for waitress
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `waitress`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-waitress-2.1.4.8/types_waitress.egg-info/SOURCES.txt` & `types-waitress-2.1.4.9/types_waitress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/adjustments.pyi` & `types-waitress-2.1.4.9/waitress-stubs/adjustments.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/buffers.pyi` & `types-waitress-2.1.4.9/waitress-stubs/buffers.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/channel.pyi` & `types-waitress-2.1.4.9/waitress-stubs/channel.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/compat.pyi` & `types-waitress-2.1.4.9/waitress-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/parser.pyi` & `types-waitress-2.1.4.9/waitress-stubs/parser.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/proxy_headers.pyi` & `types-waitress-2.1.4.9/waitress-stubs/proxy_headers.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/receiver.pyi` & `types-waitress-2.1.4.9/waitress-stubs/receiver.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/server.pyi` & `types-waitress-2.1.4.9/waitress-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/task.pyi` & `types-waitress-2.1.4.9/waitress-stubs/task.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/trigger.pyi` & `types-waitress-2.1.4.9/waitress-stubs/trigger.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/utilities.pyi` & `types-waitress-2.1.4.9/waitress-stubs/utilities.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.8/waitress-stubs/wasyncore.pyi` & `types-waitress-2.1.4.9/waitress-stubs/wasyncore.pyi`

 * *Files identical despite different names*

