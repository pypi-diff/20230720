# Comparing `tmp/types-requests-2.31.0.1.tar.gz` & `tmp/types-requests-2.31.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.31.0.1.tar", last modified: Mon May 29 06:19:45 2023, max compression
+gzip compressed data, was "types-requests-2.31.0.2.tar", last modified: Thu Jul 20 15:21:35 2023, max compression
```

## Comparing `types-requests-2.31.0.1.tar` & `types-requests-2.31.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:19:45.340577 types-requests-2.31.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-05-29 06:19:43.000000 types-requests-2.31.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 06:19:43.000000 types-requests-2.31.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-29 06:19:45.340577 types-requests-2.31.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:19:45.340577 types-requests-2.31.0.1/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 06:19:43.000000 types-requests-2.31.0.1/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-29 06:19:26.000000 types-requests-2.31.0.1/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:19:45.340577 types-requests-2.31.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-29 06:19:43.000000 types-requests-2.31.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:19:45.340577 types-requests-2.31.0.1/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-29 06:19:45.000000 types-requests-2.31.0.1/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-29 06:19:45.000000 types-requests-2.31.0.1/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:19:45.000000 types-requests-2.31.0.1/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 06:19:45.000000 types-requests-2.31.0.1/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 06:19:45.000000 types-requests-2.31.0.1/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:35.837069 types-requests-2.31.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:21:35.837069 types-requests-2.31.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:35.833069 types-requests-2.31.0.2/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-20 15:15:13.000000 types-requests-2.31.0.2/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:35.837069 types-requests-2.31.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:35.837069 types-requests-2.31.0.2/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:21:35.000000 types-requests-2.31.0.2/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.31.0.1/CHANGELOG.md` & `types-requests-2.31.0.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.31.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.31.0.1 (2023-05-29)
 
 Allowlist requests.compat.bytes.__buffer__ (#10231)
 
 ## 2.31.0.0 (2023-05-23)
 
 [stubsabot] Bump requests to 2.31.* (#10199)
```

### Comparing `types-requests-2.31.0.1/PKG-INFO` & `types-requests-2.31.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.1
+Version: 2.31.0.2
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0d0cbb6b977361ad46456eb295aca6f63e7e0b24`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-requests-2.31.0.1/requests-stubs/__init__.pyi` & `types-requests-2.31.0.2/requests-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/adapters.pyi` & `types-requests-2.31.0.2/requests-stubs/adapters.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/api.pyi` & `types-requests-2.31.0.2/requests-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/auth.pyi` & `types-requests-2.31.0.2/requests-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/compat.pyi` & `types-requests-2.31.0.2/requests-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/cookies.pyi` & `types-requests-2.31.0.2/requests-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/exceptions.pyi` & `types-requests-2.31.0.2/requests-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/help.pyi` & `types-requests-2.31.0.2/requests-stubs/help.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/models.pyi` & `types-requests-2.31.0.2/requests-stubs/models.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/sessions.pyi` & `types-requests-2.31.0.2/requests-stubs/sessions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/structures.pyi` & `types-requests-2.31.0.2/requests-stubs/structures.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/requests-stubs/utils.pyi` & `types-requests-2.31.0.2/requests-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.1/setup.py` & `types-requests-2.31.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0d0cbb6b977361ad46456eb295aca6f63e7e0b24`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.31.0.1",
+      version="2.31.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
```

### Comparing `types-requests-2.31.0.1/types_requests.egg-info/PKG-INFO` & `types-requests-2.31.0.2/types_requests.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.1
+Version: 2.31.0.2
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0d0cbb6b977361ad46456eb295aca6f63e7e0b24`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-requests-2.31.0.1/types_requests.egg-info/SOURCES.txt` & `types-requests-2.31.0.2/types_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

