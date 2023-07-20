# Comparing `tmp/types-invoke-2.0.0.8.tar.gz` & `tmp/types-invoke-2.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-invoke-2.0.0.8.tar", last modified: Tue May 16 09:14:30 2023, max compression
+gzip compressed data, was "types-invoke-2.0.0.9.tar", last modified: Thu Jul 20 15:15:37 2023, max compression
```

## Comparing `types-invoke-2.0.0.8.tar` & `types-invoke-2.0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-16 09:14:27.000000 types-invoke-2.0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:14:27.000000 types-invoke-2.0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/invoke-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 09:14:27.000000 types-invoke-2.0.0.8/invoke-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/collection.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/invoke-stubs/completion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/completion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/completion/complete.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/env.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/executor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/main.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/invoke-stubs/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/parser/argument.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/parser/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/parser/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/program.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/runners.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/terminals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 09:14:13.000000 types-invoke-2.0.0.8/invoke-stubs/watchers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 09:14:27.000000 types-invoke-2.0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:30.065822 types-invoke-2.0.0.8/types_invoke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 09:14:30.000000 types-invoke-2.0.0.8/types_invoke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-16 09:14:30.000000 types-invoke-2.0.0.8/types_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:14:30.000000 types-invoke-2.0.0.8/types_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 09:14:30.000000 types-invoke-2.0.0.8/types_invoke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:37.780673 types-invoke-2.0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-20 15:15:36.000000 types-invoke-2.0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:36.000000 types-invoke-2.0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 15:15:37.780673 types-invoke-2.0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:37.776673 types-invoke-2.0.0.9/invoke-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 15:15:36.000000 types-invoke-2.0.0.9/invoke-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/collection.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:37.776673 types-invoke-2.0.0.9/invoke-stubs/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/completion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/completion/complete.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/env.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/main.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:37.776673 types-invoke-2.0.0.9/invoke-stubs/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/parser/argument.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/parser/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/parser/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/program.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/runners.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/terminals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 15:15:13.000000 types-invoke-2.0.0.9/invoke-stubs/watchers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:37.780673 types-invoke-2.0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-20 15:15:36.000000 types-invoke-2.0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:37.780673 types-invoke-2.0.0.9/types_invoke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 15:15:37.000000 types-invoke-2.0.0.9/types_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 15:15:37.000000 types-invoke-2.0.0.9/types_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:37.000000 types-invoke-2.0.0.9/types_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:15:37.000000 types-invoke-2.0.0.9/types_invoke.egg-info/top_level.txt
```

### Comparing `types-invoke-2.0.0.8/CHANGELOG.md` & `types-invoke-2.0.0.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.0.0.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.0.0.8 (2023-05-16)
 
 Mark `invoke` as obsolete since `2.1.2` (#10100)
 
 ## 2.0.0.7 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
```

### Comparing `types-invoke-2.0.0.8/PKG-INFO` & `types-invoke-2.0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-invoke
-Version: 2.0.0.8
+Version: 2.0.0.9
 Summary: Typing stubs for invoke
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/invoke.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,9 +26,15 @@
 types and metadata should be contributed there.
 
 *Note:* The `invoke` package includes type annotations or type stubs
 since version 2.1.2. Please uninstall the `types-invoke`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-invoke-2.0.0.8/invoke-stubs/__init__.pyi` & `types-invoke-2.0.0.9/invoke-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/collection.pyi` & `types-invoke-2.0.0.9/invoke-stubs/collection.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/config.pyi` & `types-invoke-2.0.0.9/invoke-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/context.pyi` & `types-invoke-2.0.0.9/invoke-stubs/context.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/exceptions.pyi` & `types-invoke-2.0.0.9/invoke-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/executor.pyi` & `types-invoke-2.0.0.9/invoke-stubs/executor.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/parser/argument.pyi` & `types-invoke-2.0.0.9/invoke-stubs/parser/argument.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/parser/context.pyi` & `types-invoke-2.0.0.9/invoke-stubs/parser/context.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/parser/parser.pyi` & `types-invoke-2.0.0.9/invoke-stubs/parser/parser.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/program.pyi` & `types-invoke-2.0.0.9/invoke-stubs/program.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/runners.pyi` & `types-invoke-2.0.0.9/invoke-stubs/runners.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/tasks.pyi` & `types-invoke-2.0.0.9/invoke-stubs/tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/util.pyi` & `types-invoke-2.0.0.9/invoke-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/invoke-stubs/watchers.pyi` & `types-invoke-2.0.0.9/invoke-stubs/watchers.pyi`

 * *Files identical despite different names*

### Comparing `types-invoke-2.0.0.8/setup.py` & `types-invoke-2.0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,33 +16,39 @@
 types and metadata should be contributed there.
 
 *Note:* The `invoke` package includes type annotations or type stubs
 since version 2.1.2. Please uninstall the `types-invoke`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.8",
+      version="2.0.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/invoke.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['invoke-stubs'],
-      package_data={'invoke-stubs': ['__init__.pyi', 'collection.pyi', 'completion/__init__.pyi', 'completion/complete.pyi', 'config.pyi', 'context.pyi', 'env.pyi', 'exceptions.pyi', 'executor.pyi', 'loader.pyi', 'main.pyi', 'parser/__init__.pyi', 'parser/argument.pyi', 'parser/context.pyi', 'parser/parser.pyi', 'program.pyi', 'runners.pyi', 'tasks.pyi', 'terminals.pyi', 'util.pyi', 'watchers.pyi', 'METADATA.toml']},
+      package_data={'invoke-stubs': ['__init__.pyi', 'collection.pyi', 'completion/__init__.pyi', 'completion/complete.pyi', 'config.pyi', 'context.pyi', 'env.pyi', 'exceptions.pyi', 'executor.pyi', 'loader.pyi', 'main.pyi', 'parser/__init__.pyi', 'parser/argument.pyi', 'parser/context.pyi', 'parser/parser.pyi', 'program.pyi', 'runners.pyi', 'tasks.pyi', 'terminals.pyi', 'util.pyi', 'watchers.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-invoke-2.0.0.8/types_invoke.egg-info/PKG-INFO` & `types-invoke-2.0.0.9/types_invoke.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-invoke
-Version: 2.0.0.8
+Version: 2.0.0.9
 Summary: Typing stubs for invoke
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/invoke.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,9 +26,15 @@
 types and metadata should be contributed there.
 
 *Note:* The `invoke` package includes type annotations or type stubs
 since version 2.1.2. Please uninstall the `types-invoke`
 package if you use this or a newer version.
 
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-invoke-2.0.0.8/types_invoke.egg-info/SOURCES.txt` & `types-invoke-2.0.0.9/types_invoke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

