# Comparing `tmp/types-dj-database-url-1.3.0.3.tar.gz` & `tmp/types-dj-database-url-1.3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-dj-database-url-1.3.0.3.tar", last modified: Thu May 11 18:17:59 2023, max compression
+gzip compressed data, was "types-dj-database-url-1.3.0.4.tar", last modified: Thu Jul 20 15:17:40 2023, max compression
```

## Comparing `types-dj-database-url-1.3.0.3.tar` & `types-dj-database-url-1.3.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:17:59.882321 types-dj-database-url-1.3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-11 18:17:56.000000 types-dj-database-url-1.3.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 18:17:56.000000 types-dj-database-url-1.3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-11 18:17:59.878320 types-dj-database-url-1.3.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:17:59.878320 types-dj-database-url-1.3.0.3/dj_database_url-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 18:17:56.000000 types-dj-database-url-1.3.0.3/dj_database_url-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 18:17:56.000000 types-dj-database-url-1.3.0.3/dj_database_url-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:17:59.882321 types-dj-database-url-1.3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-11 18:17:56.000000 types-dj-database-url-1.3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:17:59.878320 types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-11 18:17:59.000000 types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 18:17:59.000000 types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:17:59.000000 types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 18:17:59.000000 types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:40.734166 types-dj-database-url-1.3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-20 15:17:39.000000 types-dj-database-url-1.3.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:39.000000 types-dj-database-url-1.3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-20 15:17:40.734166 types-dj-database-url-1.3.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:40.734166 types-dj-database-url-1.3.0.4/dj_database_url-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 15:17:39.000000 types-dj-database-url-1.3.0.4/dj_database_url-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-20 15:17:39.000000 types-dj-database-url-1.3.0.4/dj_database_url-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:40.734166 types-dj-database-url-1.3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 15:17:39.000000 types-dj-database-url-1.3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:40.734166 types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-20 15:17:40.000000 types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-20 15:17:40.000000 types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:40.000000 types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:17:40.000000 types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/top_level.txt
```

### Comparing `types-dj-database-url-1.3.0.3/CHANGELOG.md` & `types-dj-database-url-1.3.0.4/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.3.0.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.3.0.3 (2023-05-11)
 
 Bump `mypy` to `1.3.0` (#10173)
 
 Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
 
 ## 1.3.0.2 (2023-04-28)
```

### Comparing `types-dj-database-url-1.3.0.3/PKG-INFO` & `types-dj-database-url-1.3.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,10 @@
 
 *Note:* The `dj-database-url` package includes type annotations or type stubs
 since version 2.0.0. Please uninstall the `types-dj-database-url`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-dj-database-url-1.3.0.3/dj_database_url-stubs/__init__.pyi` & `types-dj-database-url-1.3.0.4/dj_database_url-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-dj-database-url-1.3.0.3/setup.py` & `types-dj-database-url-1.3.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 
 *Note:* The `dj-database-url` package includes type annotations or type stubs
 since version 2.0.0. Please uninstall the `types-dj-database-url`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.0.3",
+      version="1.3.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md",
```

### Comparing `types-dj-database-url-1.3.0.3/types_dj_database_url.egg-info/PKG-INFO` & `types-dj-database-url-1.3.0.4/types_dj_database_url.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,10 @@
 
 *Note:* The `dj-database-url` package includes type annotations or type stubs
 since version 2.0.0. Please uninstall the `types-dj-database-url`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

