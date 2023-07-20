# Comparing `tmp/types-console-menu-0.8.0.2.tar.gz` & `tmp/types-console-menu-0.8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-console-menu-0.8.0.2.tar", last modified: Mon Mar 27 18:21:55 2023, max compression
+gzip compressed data, was "types-console-menu-0.8.0.3.tar", last modified: Thu Jul 20 15:16:35 2023, max compression
```

## Comparing `types-console-menu-0.8.0.2.tar` & `types-console-menu-0.8.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/consolemenu-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/consolemenu-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/console_menu.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/consolemenu-stubs/format/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/format/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_margins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_padding.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_style.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/consolemenu-stubs/items/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/command_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/external_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/function_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/selection_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/items/submenu_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/menu_component.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/menu_formatter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/multiselect_menu.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/prompt_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/screen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/selection_menu.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/consolemenu-stubs/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/validators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/validators/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/validators/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/validators/url.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-console-menu-0.8.0.2/consolemenu-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:55.945636 types-console-menu-0.8.0.2/types_console_menu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/types_console_menu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/types_console_menu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/types_console_menu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:21:55.000000 types-console-menu-0.8.0.2/types_console_menu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.605379 types-console-menu-0.8.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-20 15:16:34.000000 types-console-menu-0.8.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:34.000000 types-console-menu-0.8.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 15:16:35.605379 types-console-menu-0.8.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.601379 types-console-menu-0.8.0.3/consolemenu-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 15:16:34.000000 types-console-menu-0.8.0.3/consolemenu-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/console_menu.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.601379 types-console-menu-0.8.0.3/consolemenu-stubs/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/format/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_margins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_padding.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_style.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.601379 types-console-menu-0.8.0.3/consolemenu-stubs/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/command_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/external_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/function_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/selection_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/items/submenu_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/menu_component.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/menu_formatter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/multiselect_menu.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/prompt_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/screen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/selection_menu.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.605379 types-console-menu-0.8.0.3/consolemenu-stubs/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/validators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/validators/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/validators/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/validators/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-console-menu-0.8.0.3/consolemenu-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:35.605379 types-console-menu-0.8.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-20 15:16:34.000000 types-console-menu-0.8.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:35.605379 types-console-menu-0.8.0.3/types_console_menu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 15:16:35.000000 types-console-menu-0.8.0.3/types_console_menu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-20 15:16:35.000000 types-console-menu-0.8.0.3/types_console_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:35.000000 types-console-menu-0.8.0.3/types_console_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:16:35.000000 types-console-menu-0.8.0.3/types_console_menu.egg-info/top_level.txt
```

### Comparing `types-console-menu-0.8.0.2/PKG-INFO` & `types-console-menu-0.8.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-console-menu
-Version: 0.8.0.2
+Version: 0.8.0.3
 Summary: Typing stubs for console-menu
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/console-menu.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `console-menu`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/console-menu. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/console_menu.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/console_menu.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/format/__init__.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/format/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_borders.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_borders.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_margins.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_margins.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_padding.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_padding.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/format/menu_style.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/format/menu_style.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/items/command_item.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/items/command_item.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/items/function_item.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/items/function_item.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/items/submenu_item.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/items/submenu_item.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/menu_component.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/menu_component.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/menu_formatter.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/menu_formatter.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/multiselect_menu.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/multiselect_menu.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/prompt_utils.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/prompt_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/consolemenu-stubs/selection_menu.pyi` & `types-console-menu-0.8.0.3/consolemenu-stubs/selection_menu.pyi`

 * *Files identical despite different names*

### Comparing `types-console-menu-0.8.0.2/setup.py` & `types-console-menu-0.8.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `console-menu`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/console-menu. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.8.0.2",
+      version="0.8.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/console-menu.md",
```

### Comparing `types-console-menu-0.8.0.2/types_console_menu.egg-info/PKG-INFO` & `types-console-menu-0.8.0.3/types_console_menu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-console-menu
-Version: 0.8.0.2
+Version: 0.8.0.3
 Summary: Typing stubs for console-menu
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/console-menu.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `console-menu`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/console-menu. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-console-menu-0.8.0.2/types_console_menu.egg-info/SOURCES.txt` & `types-console-menu-0.8.0.3/types_console_menu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

