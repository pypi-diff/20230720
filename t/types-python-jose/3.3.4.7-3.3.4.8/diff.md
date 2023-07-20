# Comparing `tmp/types-python-jose-3.3.4.7.tar.gz` & `tmp/types-python-jose-3.3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-jose-3.3.4.7.tar", last modified: Thu Apr 13 12:31:11 2023, max compression
+gzip compressed data, was "types-python-jose-3.3.4.8.tar", last modified: Thu Jul 20 15:21:23 2023, max compression
```

## Comparing `types-python-jose-3.3.4.7.tar` & `types-python-jose-3.3.4.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:11.700419 types-python-jose-3.3.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 12:31:11.700419 types-python-jose-3.3.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:11.696419 types-python-jose-3.3.4.7/jose-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/jose-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:11.696419 types-python-jose-3.3.4.7/jose-stubs/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/_asn1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/cryptography_backend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/ecdsa_backend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/native.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/backends/rsa_backend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/jwe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/jwk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/jws.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/jwt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-13 12:30:41.000000 types-python-jose-3.3.4.7/jose-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:31:11.700419 types-python-jose-3.3.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:11.700419 types-python-jose-3.3.4.7/types_python_jose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/types_python_jose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/types_python_jose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/types_python_jose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/types_python_jose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:31:11.000000 types-python-jose-3.3.4.7/types_python_jose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:23.776924 types-python-jose-3.3.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:21:23.776924 types-python-jose-3.3.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:23.772924 types-python-jose-3.3.4.8/jose-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/jose-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:23.776924 types-python-jose-3.3.4.8/jose-stubs/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/_asn1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/cryptography_backend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/ecdsa_backend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/native.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/backends/rsa_backend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/jwe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/jwk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/jws.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/jwt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 15:15:13.000000 types-python-jose-3.3.4.8/jose-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:23.776924 types-python-jose-3.3.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:23.776924 types-python-jose-3.3.4.8/types_python_jose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/types_python_jose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/types_python_jose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/types_python_jose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/types_python_jose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:21:23.000000 types-python-jose-3.3.4.8/types_python_jose.egg-info/top_level.txt
```

### Comparing `types-python-jose-3.3.4.7/CHANGELOG.md` & `types-python-jose-3.3.4.8/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.3.4.8 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.3.4.7 (2023-04-13)
 
 Style: prefer `type[Foo | Bar]` over `type[Foo] | type[Bar]` (#10039)
 
 ## 3.3.4.6 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
```

### Comparing `types-python-jose-3.3.4.7/PKG-INFO` & `types-python-jose-3.3.4.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-jose
-Version: 3.3.4.7
+Version: 3.3.4.8
 Summary: Typing stubs for python-jose
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-jose.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-jose`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-jose. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/__init__.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/_asn1.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/_asn1.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/base.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/cryptography_backend.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/cryptography_backend.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/ecdsa_backend.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/ecdsa_backend.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/native.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/native.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/backends/rsa_backend.pyi` & `types-python-jose-3.3.4.8/jose-stubs/backends/rsa_backend.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/constants.pyi` & `types-python-jose-3.3.4.8/jose-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/jwe.pyi` & `types-python-jose-3.3.4.8/jose-stubs/jwe.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/jwk.pyi` & `types-python-jose-3.3.4.8/jose-stubs/jwk.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/jws.pyi` & `types-python-jose-3.3.4.8/jose-stubs/jws.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/jwt.pyi` & `types-python-jose-3.3.4.8/jose-stubs/jwt.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/jose-stubs/utils.pyi` & `types-python-jose-3.3.4.8/jose-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-python-jose-3.3.4.7/setup.py` & `types-python-jose-3.3.4.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-jose`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-jose. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.3.4.7",
+      version="3.3.4.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-jose.md",
```

### Comparing `types-python-jose-3.3.4.7/types_python_jose.egg-info/PKG-INFO` & `types-python-jose-3.3.4.8/types_python_jose.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-jose
-Version: 3.3.4.7
+Version: 3.3.4.8
 Summary: Typing stubs for python-jose
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-jose.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-jose`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-jose. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-python-jose-3.3.4.7/types_python_jose.egg-info/SOURCES.txt` & `types-python-jose-3.3.4.8/types_python_jose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

