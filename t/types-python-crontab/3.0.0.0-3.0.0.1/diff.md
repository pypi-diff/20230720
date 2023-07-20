# Comparing `tmp/types-python-crontab-3.0.0.0.tar.gz` & `tmp/types-python-crontab-3.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-crontab-3.0.0.0.tar", last modified: Wed Jul 19 12:29:39 2023, max compression
+gzip compressed data, was "types-python-crontab-3.0.0.1.tar", last modified: Thu Jul 20 18:19:19 2023, max compression
```

## Comparing `types-python-crontab-3.0.0.0.tar` & `types-python-crontab-3.0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/cronlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/cronlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/cronlog-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/crontab-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontab-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontab-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/crontabs-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontabs-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontabs-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-19 12:29:39.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/cronlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/cronlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/cronlog-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/crontab-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/crontab-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/crontab-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/crontabs-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/crontabs-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/crontabs-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:19.899187 types-python-crontab-3.0.0.1/types_python_crontab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/types_python_crontab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/types_python_crontab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/types_python_crontab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 18:19:19.000000 types-python-crontab-3.0.0.1/types_python_crontab.egg-info/top_level.txt
```

### Comparing `types-python-crontab-3.0.0.0/CHANGELOG.md` & `types-python-crontab-3.0.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.0.0.1 (2023-07-20)
+
+Add a few more upstream_repository URLs (#10489)
+
 ## 3.0.0.0 (2023-07-19)
 
 Update `python-crontab` to `3.0.*` (#10475)
 
 ## 2.7.0.6 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-python-crontab-3.0.0.0/PKG-INFO` & `types-python-crontab-3.0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.0
+Version: 3.0.0.1
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-python-crontab-3.0.0.0/cronlog-stubs/__init__.pyi` & `types-python-crontab-3.0.0.1/cronlog-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.0/crontab-stubs/__init__.pyi` & `types-python-crontab-3.0.0.1/crontab-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.0/crontabs-stubs/__init__.pyi` & `types-python-crontab-3.0.0.1/crontabs-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.0/setup.py` & `types-python-crontab-3.0.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.0",
+      version="3.0.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md",
```

### Comparing `types-python-crontab-3.0.0.0/types_python_crontab.egg-info/PKG-INFO` & `types-python-crontab-3.0.0.1/types_python_crontab.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.0
+Version: 3.0.0.1
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

