# Comparing `tmp/types-tqdm-4.65.0.1.tar.gz` & `tmp/types-tqdm-4.65.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tqdm-4.65.0.1.tar", last modified: Tue Mar 28 12:33:20 2023, max compression
+gzip compressed data, was "types-tqdm-4.65.0.2.tar", last modified: Thu Jul 20 15:17:43 2023, max compression
```

## Comparing `types-tqdm-4.65.0.1.tar` & `types-tqdm-4.65.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-28 12:33:19.000000 types-tqdm-4.65.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:19.000000 types-tqdm-4.65.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-28 12:33:19.000000 types-tqdm-4.65.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/tqdm-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-28 12:33:19.000000 types-tqdm-4.65.0.1/tqdm-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_dist_ver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_main.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_tqdm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_tqdm_gui.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_tqdm_notebook.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_tqdm_pandas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/auto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/autonotebook.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/tqdm-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/bells.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/concurrent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/discord.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/itertools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/slack.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/telegram.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/contrib/utils_worker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/dask.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/gui.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/keras.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/notebook.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/rich.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/std.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/tk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 12:32:25.000000 types-tqdm-4.65.0.1/tqdm-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:20.569042 types-tqdm-4.65.0.1/types_tqdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-28 12:33:20.000000 types-tqdm-4.65.0.1/types_tqdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-28 12:33:20.000000 types-tqdm-4.65.0.1/types_tqdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:20.000000 types-tqdm-4.65.0.1/types_tqdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 12:33:20.000000 types-tqdm-4.65.0.1/types_tqdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:43.794204 types-tqdm-4.65.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-20 15:17:42.000000 types-tqdm-4.65.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:42.000000 types-tqdm-4.65.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 15:17:43.790204 types-tqdm-4.65.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:43.794204 types-tqdm-4.65.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-20 15:17:42.000000 types-tqdm-4.65.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:43.790204 types-tqdm-4.65.0.2/tqdm-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 15:17:42.000000 types-tqdm-4.65.0.2/tqdm-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_dist_ver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_main.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_tqdm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_tqdm_gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_tqdm_notebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_tqdm_pandas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/auto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/autonotebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:43.790204 types-tqdm-4.65.0.2/tqdm-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/bells.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/concurrent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/discord.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/itertools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/slack.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/telegram.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/contrib/utils_worker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/dask.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/keras.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/notebook.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/rich.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/std.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/tk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-tqdm-4.65.0.2/tqdm-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:43.790204 types-tqdm-4.65.0.2/types_tqdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 15:17:43.000000 types-tqdm-4.65.0.2/types_tqdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-20 15:17:43.000000 types-tqdm-4.65.0.2/types_tqdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:43.000000 types-tqdm-4.65.0.2/types_tqdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:17:43.000000 types-tqdm-4.65.0.2/types_tqdm.egg-info/top_level.txt
```

### Comparing `types-tqdm-4.65.0.1/CHANGELOG.md` & `types-tqdm-4.65.0.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.65.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 4.65.0.1 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 4.65.0.0 (2023-03-04)
 
 Update `tqdm` stubs to 4.65.* (#9840)
```

### Comparing `types-tqdm-4.65.0.1/PKG-INFO` & `types-tqdm-4.65.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tqdm
-Version: 4.65.0.1
+Version: 4.65.0.2
 Summary: Typing stubs for tqdm
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tqdm`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-tqdm-4.65.0.1/setup.py` & `types-tqdm-4.65.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tqdm`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.65.0.1",
+      version="4.65.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md",
```

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/__init__.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/_monitor.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/_monitor.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/asyncio.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/asyncio.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/contrib/__init__.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/contrib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/contrib/discord.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/contrib/discord.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/contrib/logging.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/contrib/logging.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/contrib/slack.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/contrib/slack.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/contrib/telegram.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/contrib/telegram.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/dask.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/dask.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/gui.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/gui.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/keras.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/keras.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/notebook.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/notebook.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/rich.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/rich.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/std.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/std.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/tk.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/tk.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/tqdm-stubs/utils.pyi` & `types-tqdm-4.65.0.2/tqdm-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-tqdm-4.65.0.1/types_tqdm.egg-info/PKG-INFO` & `types-tqdm-4.65.0.2/types_tqdm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tqdm
-Version: 4.65.0.1
+Version: 4.65.0.2
 Summary: Typing stubs for tqdm
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tqdm.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tqdm`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tqdm. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-tqdm-4.65.0.1/types_tqdm.egg-info/SOURCES.txt` & `types-tqdm-4.65.0.2/types_tqdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

