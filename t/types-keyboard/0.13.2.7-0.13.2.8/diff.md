# Comparing `tmp/types-keyboard-0.13.2.7.tar.gz` & `tmp/types-keyboard-0.13.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-keyboard-0.13.2.7.tar", last modified: Mon Apr 17 12:30:50 2023, max compression
+gzip compressed data, was "types-keyboard-0.13.2.8.tar", last modified: Thu Jul 20 15:18:21 2023, max compression
```

## Comparing `types-keyboard-0.13.2.7.tar` & `types-keyboard-0.13.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:50.408463 types-keyboard-0.13.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-17 12:30:49.000000 types-keyboard-0.13.2.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 12:30:49.000000 types-keyboard-0.13.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 12:30:50.408463 types-keyboard-0.13.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:50.404463 types-keyboard-0.13.2.7/keyboard-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-17 12:30:49.000000 types-keyboard-0.13.2.7/keyboard-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/_canonical_names.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/_generic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/_keyboard_event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/_mouse_event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-17 12:30:30.000000 types-keyboard-0.13.2.7/keyboard-stubs/mouse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:30:50.408463 types-keyboard-0.13.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-17 12:30:49.000000 types-keyboard-0.13.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:50.408463 types-keyboard-0.13.2.7/types_keyboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 12:30:50.000000 types-keyboard-0.13.2.7/types_keyboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 12:30:50.000000 types-keyboard-0.13.2.7/types_keyboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:30:50.000000 types-keyboard-0.13.2.7/types_keyboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 12:30:50.000000 types-keyboard-0.13.2.7/types_keyboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:21.922685 types-keyboard-0.13.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:18:21.922685 types-keyboard-0.13.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:21.922685 types-keyboard-0.13.2.8/keyboard-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/keyboard-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/_canonical_names.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/_generic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/_keyboard_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/_mouse_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-20 15:15:13.000000 types-keyboard-0.13.2.8/keyboard-stubs/mouse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:21.922685 types-keyboard-0.13.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:21.922685 types-keyboard-0.13.2.8/types_keyboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/types_keyboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/types_keyboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/types_keyboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:18:21.000000 types-keyboard-0.13.2.8/types_keyboard.egg-info/top_level.txt
```

### Comparing `types-keyboard-0.13.2.7/CHANGELOG.md` & `types-keyboard-0.13.2.8/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.13.2.8 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.13.2.7 (2023-04-17)
 
 `keyboard` : Update `stubtest_allowlist` and add comments for missing defaults (#9965)
 
 ## 0.13.2.6 (2023-03-27)
 
 Add defaults for third-party stubs I-L (#9955)
```

### Comparing `types-keyboard-0.13.2.7/PKG-INFO` & `types-keyboard-0.13.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-keyboard
-Version: 0.13.2.7
+Version: 0.13.2.8
 Summary: Typing stubs for keyboard
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/keyboard.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `keyboard`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/keyboard. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-keyboard-0.13.2.7/keyboard-stubs/__init__.pyi` & `types-keyboard-0.13.2.8/keyboard-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-keyboard-0.13.2.7/keyboard-stubs/_generic.pyi` & `types-keyboard-0.13.2.8/keyboard-stubs/_generic.pyi`

 * *Files identical despite different names*

### Comparing `types-keyboard-0.13.2.7/keyboard-stubs/_keyboard_event.pyi` & `types-keyboard-0.13.2.8/keyboard-stubs/_keyboard_event.pyi`

 * *Files identical despite different names*

### Comparing `types-keyboard-0.13.2.7/keyboard-stubs/_mouse_event.pyi` & `types-keyboard-0.13.2.8/keyboard-stubs/_mouse_event.pyi`

 * *Files identical despite different names*

### Comparing `types-keyboard-0.13.2.7/keyboard-stubs/mouse.pyi` & `types-keyboard-0.13.2.8/keyboard-stubs/mouse.pyi`

 * *Files identical despite different names*

### Comparing `types-keyboard-0.13.2.7/setup.py` & `types-keyboard-0.13.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `keyboard`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/keyboard. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.13.2.7",
+      version="0.13.2.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/keyboard.md",
```

### Comparing `types-keyboard-0.13.2.7/types_keyboard.egg-info/PKG-INFO` & `types-keyboard-0.13.2.8/types_keyboard.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-keyboard
-Version: 0.13.2.7
+Version: 0.13.2.8
 Summary: Typing stubs for keyboard
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/keyboard.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `keyboard`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/keyboard. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

