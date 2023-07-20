# Comparing `tmp/types-python-dateutil-2.8.8.tar.gz` & `tmp/types-python-dateutil-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-dateutil-2.8.8.tar", last modified: Thu Jan 20 01:09:54 2022, max compression
+gzip compressed data, was "types-python-dateutil-2.8.9.tar", last modified: Mon Jan 31 00:58:09 2022, max compression
```

## Comparing `types-python-dateutil-2.8.8.tar` & `types-python-dateutil-2.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-01-20 01:09:53.000000 types-python-dateutil-2.8.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-20 01:09:53.000000 types-python-dateutil-2.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:54.331529 types-python-dateutil-2.8.8/dateutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-20 01:09:53.000000 types-python-dateutil-2.8.8/dateutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/easter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/dateutil-stubs/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/parser/isoparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/relativedelta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/rrule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/dateutil-stubs/tz/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/tz/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/tz/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/tz/tz.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-01-20 01:09:25.000000 types-python-dateutil-2.8.8/dateutil-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-01-20 01:09:53.000000 types-python-dateutil-2.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 01:09:54.335529 types-python-dateutil-2.8.8/types_python_dateutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-20 01:09:54.000000 types-python-dateutil-2.8.8/types_python_dateutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-01-20 01:09:54.000000 types-python-dateutil-2.8.8/types_python_dateutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 01:09:54.000000 types-python-dateutil-2.8.8/types_python_dateutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-20 01:09:54.000000 types-python-dateutil-2.8.8/types_python_dateutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-01-31 00:58:08.000000 types-python-dateutil-2.8.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-31 00:58:08.000000 types-python-dateutil-2.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/dateutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-31 00:58:08.000000 types-python-dateutil-2.8.9/dateutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/easter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/dateutil-stubs/parser/
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/parser/isoparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/relativedelta.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/rrule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/dateutil-stubs/tz/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/tz/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/tz/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/tz/tz.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-01-31 00:57:40.000000 types-python-dateutil-2.8.9/dateutil-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-01-31 00:58:08.000000 types-python-dateutil-2.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:58:09.407666 types-python-dateutil-2.8.9/types_python_dateutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-01-31 00:58:09.000000 types-python-dateutil-2.8.9/types_python_dateutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-01-31 00:58:09.000000 types-python-dateutil-2.8.9/types_python_dateutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 00:58:09.000000 types-python-dateutil-2.8.9/types_python_dateutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-31 00:58:09.000000 types-python-dateutil-2.8.9/types_python_dateutil.egg-info/top_level.txt
```

### Comparing `types-python-dateutil-2.8.8/CHANGELOG.md` & `types-python-dateutil-2.8.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.8.9 (2022-01-31)
+
+Upgrade black version (#7089)
+
 ## 2.8.8 (2022-01-20)
 
 Remove nearly all `__str__` and `__repr__` methods from typeshed (#6968)
 
 ## 2.8.7 (2022-01-17)
 
 Use `_typeshed.Self` in Python 2, too (#6932)
```

### Comparing `types-python-dateutil-2.8.8/PKG-INFO` & `types-python-dateutil-2.8.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: types-python-dateutil
-Version: 2.8.8
+Version: 2.8.9
 Summary: Typing stubs for python-dateutil
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
+Project-URL: GitHub, https://github.com/python/typeshed
+Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-dateutil.md
+Project-URL: Issue tracker, https://github.com/python/typeshed/issues
+Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for python-dateutil
 
 This is a PEP 561 type stub package for the `python-dateutil` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `python-dateutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/python-dateutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `aea52b35d1f5a9306f66e1b98314f4ecbe0ffa7a`.
+This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
```

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/parser/__init__.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/parser/isoparser.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/parser/isoparser.pyi`

 * *Files identical despite different names*

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/relativedelta.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/relativedelta.pyi`

 * *Files identical despite different names*

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/rrule.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/rrule.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         def __init__(self, genlist, gen) -> None: ...
         def __next__(self): ...
         next: Any = ...
         def __lt__(self, other): ...
         def __gt__(self, other): ...
         def __eq__(self, other): ...
         def __ne__(self, other): ...
+
     def __init__(self, cache: bool = ...) -> None: ...
     def rrule(self, rrule: _rrule): ...
     def rdate(self, rdate): ...
     def exrule(self, exrule): ...
     def exdate(self, exdate): ...
 
 class _rrulestr:
```

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/tz/_common.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/tz/_common.pyi`

 * *Files identical despite different names*

### Comparing `types-python-dateutil-2.8.8/dateutil-stubs/tz/tz.pyi` & `types-python-dateutil-2.8.9/dateutil-stubs/tz/tz.pyi`

 * *Files identical despite different names*

### Comparing `types-python-dateutil-2.8.8/setup.py` & `types-python-dateutil-2.8.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,23 +8,29 @@
 This is a PEP 561 type stub package for the `python-dateutil` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `python-dateutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/python-dateutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `aea52b35d1f5a9306f66e1b98314f4ecbe0ffa7a`.
+This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.8.8",
+      version="2.8.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
+      project_urls={
+          "GitHub": "https://github.com/python/typeshed",
+          "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-dateutil.md",
+          "Issue tracker": "https://github.com/python/typeshed/issues",
+          "Chat": "https://gitter.im/python/typing",
+      },
       install_requires=[],
       packages=['dateutil-stubs'],
       package_data={'dateutil-stubs': ['__init__.pyi', '_common.pyi', 'easter.pyi', 'parser/__init__.pyi', 'parser/isoparser.pyi', 'relativedelta.pyi', 'rrule.pyi', 'tz/__init__.pyi', 'tz/_common.pyi', 'tz/tz.pyi', 'utils.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Typing :: Stubs Only",
```

### Comparing `types-python-dateutil-2.8.8/types_python_dateutil.egg-info/PKG-INFO` & `types-python-dateutil-2.8.9/types_python_dateutil.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: types-python-dateutil
-Version: 2.8.8
+Version: 2.8.9
 Summary: Typing stubs for python-dateutil
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
+Project-URL: GitHub, https://github.com/python/typeshed
+Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-dateutil.md
+Project-URL: Issue tracker, https://github.com/python/typeshed/issues
+Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for python-dateutil
 
 This is a PEP 561 type stub package for the `python-dateutil` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `python-dateutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/python-dateutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `aea52b35d1f5a9306f66e1b98314f4ecbe0ffa7a`.
+This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
```

### Comparing `types-python-dateutil-2.8.8/types_python_dateutil.egg-info/SOURCES.txt` & `types-python-dateutil-2.8.9/types_python_dateutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

