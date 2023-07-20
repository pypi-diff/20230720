# Comparing `tmp/types-boltons-23.0.0.0.tar.gz` & `tmp/types-boltons-23.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-boltons-23.0.0.0.tar", last modified: Wed Jun  7 09:14:21 2023, max compression
+gzip compressed data, was "types-boltons-23.0.0.1.tar", last modified: Thu Jul 20 15:18:25 2023, max compression
```

## Comparing `types-boltons-23.0.0.0.tar` & `types-boltons-23.0.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:21.756643 types-boltons-23.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 09:14:18.000000 types-boltons-23.0.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 09:14:18.000000 types-boltons-23.0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 09:14:21.756643 types-boltons-23.0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:21.756643 types-boltons-23.0.0.0/boltons-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 09:14:18.000000 types-boltons-23.0.0.0/boltons-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/cacheutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/debugutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/deprutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/dictutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/easterutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/ecoutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/excutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/fileutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/formatutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/funcutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/gcutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/ioutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/iterutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/jsonutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/listutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/mathutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/mboxutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/namedutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/pathutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/queueutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/setutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/socketutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/statsutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/strutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/tableutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/tbutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/timeutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/typeutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-07 09:14:02.000000 types-boltons-23.0.0.0/boltons-stubs/urlutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:14:21.756643 types-boltons-23.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 09:14:18.000000 types-boltons-23.0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:21.756643 types-boltons-23.0.0.0/types_boltons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 09:14:21.000000 types-boltons-23.0.0.0/types_boltons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-07 09:14:21.000000 types-boltons-23.0.0.0/types_boltons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:14:21.000000 types-boltons-23.0.0.0/types_boltons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 09:14:21.000000 types-boltons-23.0.0.0/types_boltons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:25.754740 types-boltons-23.0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 15:18:24.000000 types-boltons-23.0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:24.000000 types-boltons-23.0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 15:18:25.754740 types-boltons-23.0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:25.754740 types-boltons-23.0.0.1/boltons-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 15:18:24.000000 types-boltons-23.0.0.1/boltons-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/cacheutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/debugutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/deprutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/dictutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/easterutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/ecoutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/excutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/fileutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/formatutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/funcutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/gcutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/ioutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/iterutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/jsonutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/listutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/mathutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/mboxutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/namedutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/pathutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/queueutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/setutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/socketutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/statsutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/strutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/tableutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/tbutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/timeutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/typeutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-20 15:15:13.000000 types-boltons-23.0.0.1/boltons-stubs/urlutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:25.754740 types-boltons-23.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-20 15:18:24.000000 types-boltons-23.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:25.754740 types-boltons-23.0.0.1/types_boltons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 15:18:25.000000 types-boltons-23.0.0.1/types_boltons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-20 15:18:25.000000 types-boltons-23.0.0.1/types_boltons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:25.000000 types-boltons-23.0.0.1/types_boltons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:18:25.000000 types-boltons-23.0.0.1/types_boltons.egg-info/top_level.txt
```

### Comparing `types-boltons-23.0.0.0/PKG-INFO` & `types-boltons-23.0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boltons
-Version: 23.0.0.0
+Version: 23.0.0.1
 Summary: Typing stubs for boltons
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e1ab1ad2fb29a920865a118d0a160482db9735f2`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-boltons-23.0.0.0/boltons-stubs/cacheutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/cacheutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/dictutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/dictutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/ecoutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/ecoutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/fileutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/fileutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/formatutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/formatutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/funcutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/funcutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/ioutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/ioutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/iterutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/iterutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/jsonutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/jsonutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/listutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/listutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/mathutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/mathutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/queueutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/queueutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/setutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/setutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/socketutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/socketutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/statsutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/statsutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/strutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/strutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/tableutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/tableutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/tbutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/tbutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/timeutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/timeutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/boltons-stubs/urlutils.pyi` & `types-boltons-23.0.0.1/boltons-stubs/urlutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.0.0.0/setup.py` & `types-boltons-23.0.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e1ab1ad2fb29a920865a118d0a160482db9735f2`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="23.0.0.0",
+      version="23.0.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md",
```

### Comparing `types-boltons-23.0.0.0/types_boltons.egg-info/PKG-INFO` & `types-boltons-23.0.0.1/types_boltons.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boltons
-Version: 23.0.0.0
+Version: 23.0.0.1
 Summary: Typing stubs for boltons
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e1ab1ad2fb29a920865a118d0a160482db9735f2`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-boltons-23.0.0.0/types_boltons.egg-info/SOURCES.txt` & `types-boltons-23.0.0.1/types_boltons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

