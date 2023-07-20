# Comparing `tmp/types-PyAutoGUI-0.9.3.6.tar.gz` & `tmp/types-PyAutoGUI-0.9.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyAutoGUI-0.9.3.6.tar", last modified: Thu May 25 09:14:24 2023, max compression
+gzip compressed data, was "types-PyAutoGUI-0.9.3.7.tar", last modified: Thu Jul 20 15:21:49 2023, max compression
```

## Comparing `types-PyAutoGUI-0.9.3.6.tar` & `types-PyAutoGUI-0.9.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:24.576594 types-PyAutoGUI-0.9.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 09:14:22.000000 types-PyAutoGUI-0.9.3.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:14:22.000000 types-PyAutoGUI-0.9.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-25 09:14:24.576594 types-PyAutoGUI-0.9.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:24.572594 types-PyAutoGUI-0.9.3.6/pyautogui-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 09:14:22.000000 types-PyAutoGUI-0.9.3.6/pyautogui-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-05-25 09:14:07.000000 types-PyAutoGUI-0.9.3.6/pyautogui-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:14:24.576594 types-PyAutoGUI-0.9.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-25 09:14:22.000000 types-PyAutoGUI-0.9.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:24.576594 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-25 09:14:24.000000 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-25 09:14:24.000000 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:14:24.000000 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 09:14:24.000000 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 09:14:24.000000 types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-20 15:15:13.000000 types-PyAutoGUI-0.9.3.7/pyautogui-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 15:21:48.000000 types-PyAutoGUI-0.9.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:49.201236 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:21:49.000000 types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/top_level.txt
```

### Comparing `types-PyAutoGUI-0.9.3.6/CHANGELOG.md` & `types-PyAutoGUI-0.9.3.7/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.9.3.7 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.9.3.6 (2023-05-25)
 
 Update pyautogui (#10209)
 
 Fixes #10207
 
 ## 0.9.3.5 (2023-02-21)
```

### Comparing `types-PyAutoGUI-0.9.3.6/PKG-INFO` & `types-PyAutoGUI-0.9.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyAutoGUI
-Version: 0.9.3.6
+Version: 0.9.3.7
 Summary: Typing stubs for PyAutoGUI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyAutoGUI`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a4e33d4053e3c3310459f480890cee1b1bb97753`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-PyAutoGUI-0.9.3.6/pyautogui-stubs/__init__.pyi` & `types-PyAutoGUI-0.9.3.7/pyautogui-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyAutoGUI-0.9.3.6/setup.py` & `types-PyAutoGUI-0.9.3.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyAutoGUI`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a4e33d4053e3c3310459f480890cee1b1bb97753`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.3.6",
+      version="0.9.3.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md",
```

### Comparing `types-PyAutoGUI-0.9.3.6/types_PyAutoGUI.egg-info/PKG-INFO` & `types-PyAutoGUI-0.9.3.7/types_PyAutoGUI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyAutoGUI
-Version: 0.9.3.6
+Version: 0.9.3.7
 Summary: Typing stubs for PyAutoGUI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyAutoGUI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyAutoGUI`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyAutoGUI. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a4e33d4053e3c3310459f480890cee1b1bb97753`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

