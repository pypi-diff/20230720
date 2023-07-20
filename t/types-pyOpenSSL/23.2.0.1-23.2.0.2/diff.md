# Comparing `tmp/types-pyOpenSSL-23.2.0.1.tar.gz` & `tmp/types-pyOpenSSL-23.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyOpenSSL-23.2.0.1.tar", last modified: Wed Jun 21 21:14:18 2023, max compression
+gzip compressed data, was "types-pyOpenSSL-23.2.0.2.tar", last modified: Thu Jul 20 15:20:40 2023, max compression
```

## Comparing `types-pyOpenSSL-23.2.0.1.tar` & `types-pyOpenSSL-23.2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/SSL.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:40.796423 types-pyOpenSSL-23.2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:40.792423 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-20 15:15:13.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/SSL.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-20 15:15:13.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 15:15:13.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 15:15:13.000000 types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-20 15:20:40.796423 types-pyOpenSSL-23.2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:40.796423 types-pyOpenSSL-23.2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:40.796423 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:40.000000 types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/top_level.txt
```

### Comparing `types-pyOpenSSL-23.2.0.1/CHANGELOG.md` & `types-pyOpenSSL-23.2.0.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 23.2.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 23.2.0.1 (2023-06-21)
 
 Add missing constants to `OpenSSL/crypto.pyi` (#10345)
 
 Adds typing for missing constants `TYPE_DH` and `TYPE_EC`
 
 See https://github.com/pyca/pyopenssl/blob/main/src/OpenSSL/crypto.py#L94-L95
```

### Comparing `types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/SSL.pyi` & `types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/SSL.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/crypto.pyi` & `types-pyOpenSSL-23.2.0.2/OpenSSL-stubs/crypto.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-23.2.0.1/PKG-INFO` & `types-pyOpenSSL-23.2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.2.0.1
+Version: 23.2.0.2
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyOpenSSL-23.2.0.1/setup.py` & `types-pyOpenSSL-23.2.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="23.2.0.1",
+      version="23.2.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md",
```

### Comparing `types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/PKG-INFO` & `types-pyOpenSSL-23.2.0.2/types_pyOpenSSL.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.2.0.1
+Version: 23.2.0.2
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

