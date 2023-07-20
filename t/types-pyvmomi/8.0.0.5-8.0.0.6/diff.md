# Comparing `tmp/types-pyvmomi-8.0.0.5.tar.gz` & `tmp/types-pyvmomi-8.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyvmomi-8.0.0.5.tar", last modified: Tue May 30 12:31:43 2023, max compression
+gzip compressed data, was "types-pyvmomi-8.0.0.6.tar", last modified: Thu Jul 20 15:18:13 2023, max compression
```

## Comparing `types-pyvmomi-8.0.0.5.tar` & `types-pyvmomi-8.0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/option.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/view.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:13.806584 types-pyvmomi-8.0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-20 15:18:13.806584 types-pyvmomi-8.0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:13.802585 types-pyvmomi-8.0.0.6/pyVmomi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:13.802585 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/option.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/view.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:13.802585 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-20 15:15:13.000000 types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:13.806584 types-pyvmomi-8.0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:13.806584 types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:18:13.000000 types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/top_level.txt
```

### Comparing `types-pyvmomi-8.0.0.5/CHANGELOG.md` & `types-pyvmomi-8.0.0.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 8.0.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 8.0.0.5 (2023-05-30)
 
 [stubsabot] Mark pyvmomi as obsolete since 8.0.1.0.1 (#10172)
 
 ## 8.0.0.4 (2023-05-10)
 
 Revert "[stubsabot] Mark pyvmomi as obsolete since 8.0.1.0 (#10148)" (#10171)
```

### Comparing `types-pyvmomi-8.0.0.5/PKG-INFO` & `types-pyvmomi-8.0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.5
+Version: 8.0.0.6
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,9 +26,15 @@
 types and metadata should be contributed there.
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/__init__.pyi` & `types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/view.pyi` & `types-pyvmomi-8.0.0.6/pyVmomi-stubs/vim/view.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/__init__.pyi` & `types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/query.pyi` & `types-pyvmomi-8.0.0.6/pyVmomi-stubs/vmodl/query.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.5/setup.py` & `types-pyvmomi-8.0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,33 +16,39 @@
 types and metadata should be contributed there.
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="8.0.0.5",
+      version="8.0.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pyVmomi-stubs'],
-      package_data={'pyVmomi-stubs': ['__init__.pyi', 'vim/__init__.pyi', 'vim/event.pyi', 'vim/fault.pyi', 'vim/option.pyi', 'vim/view.pyi', 'vmodl/__init__.pyi', 'vmodl/fault.pyi', 'vmodl/query.pyi', 'METADATA.toml']},
+      package_data={'pyVmomi-stubs': ['__init__.pyi', 'vim/__init__.pyi', 'vim/event.pyi', 'vim/fault.pyi', 'vim/option.pyi', 'vim/view.pyi', 'vmodl/__init__.pyi', 'vmodl/fault.pyi', 'vmodl/query.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/PKG-INFO` & `types-pyvmomi-8.0.0.6/types_pyvmomi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.5
+Version: 8.0.0.6
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,9 +26,15 @@
 types and metadata should be contributed there.
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

