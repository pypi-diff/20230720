# Comparing `tmp/types-httplib2-0.22.0.1.tar.gz` & `tmp/types-httplib2-0.22.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-httplib2-0.22.0.1.tar", last modified: Mon Mar 27 18:24:33 2023, max compression
+gzip compressed data, was "types-httplib2-0.22.0.2.tar", last modified: Thu Jul 20 15:19:11 2023, max compression
```

## Comparing `types-httplib2-0.22.0.1.tar` & `types-httplib2-0.22.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:33.939282 types-httplib2-0.22.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:24:33.939282 types-httplib2-0.22.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:33.935282 types-httplib2-0.22.0.1/httplib2-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/httplib2-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/iri2uri.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-27 18:21:24.000000 types-httplib2-0.22.0.1/httplib2-stubs/socks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:33.939282 types-httplib2-0.22.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:33.939282 types-httplib2-0.22.0.1/types_httplib2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/types_httplib2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/types_httplib2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/types_httplib2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:24:33.000000 types-httplib2-0.22.0.1/types_httplib2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:11.411317 types-httplib2-0.22.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-20 15:19:10.000000 types-httplib2-0.22.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:10.000000 types-httplib2-0.22.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:19:11.411317 types-httplib2-0.22.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:11.411317 types-httplib2-0.22.0.2/httplib2-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 15:19:10.000000 types-httplib2-0.22.0.2/httplib2-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/iri2uri.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 15:15:13.000000 types-httplib2-0.22.0.2/httplib2-stubs/socks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:11.411317 types-httplib2-0.22.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-20 15:19:10.000000 types-httplib2-0.22.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:11.411317 types-httplib2-0.22.0.2/types_httplib2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:19:11.000000 types-httplib2-0.22.0.2/types_httplib2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 15:19:11.000000 types-httplib2-0.22.0.2/types_httplib2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:11.000000 types-httplib2-0.22.0.2/types_httplib2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:19:11.000000 types-httplib2-0.22.0.2/types_httplib2.egg-info/top_level.txt
```

### Comparing `types-httplib2-0.22.0.1/CHANGELOG.md` & `types-httplib2-0.22.0.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.22.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.22.0.1 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
 
 ## 0.22.0.0 (2023-03-22)
 
 [stubsabot] Bump httplib2 to 0.22.* (#9916)
```

### Comparing `types-httplib2-0.22.0.1/PKG-INFO` & `types-httplib2-0.22.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-httplib2
-Version: 0.22.0.1
+Version: 0.22.0.2
 Summary: Typing stubs for httplib2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/httplib2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `httplib2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/httplib2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-httplib2-0.22.0.1/httplib2-stubs/__init__.pyi` & `types-httplib2-0.22.0.2/httplib2-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-httplib2-0.22.0.1/httplib2-stubs/error.pyi` & `types-httplib2-0.22.0.2/httplib2-stubs/error.pyi`

 * *Files identical despite different names*

### Comparing `types-httplib2-0.22.0.1/httplib2-stubs/socks.pyi` & `types-httplib2-0.22.0.2/httplib2-stubs/socks.pyi`

 * *Files identical despite different names*

### Comparing `types-httplib2-0.22.0.1/setup.py` & `types-httplib2-0.22.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `httplib2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/httplib2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.22.0.1",
+      version="0.22.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/httplib2.md",
```

### Comparing `types-httplib2-0.22.0.1/types_httplib2.egg-info/PKG-INFO` & `types-httplib2-0.22.0.2/types_httplib2.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-httplib2
-Version: 0.22.0.1
+Version: 0.22.0.2
 Summary: Typing stubs for httplib2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/httplib2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `httplib2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/httplib2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

