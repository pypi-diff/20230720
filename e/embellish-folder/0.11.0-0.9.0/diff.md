# Comparing `tmp/embellish-folder-0.11.0.tar.gz` & `tmp/embellish-folder-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embellish-folder-0.11.0.tar", last modified: Thu Jul 20 11:53:16 2023, max compression
+gzip compressed data, was "embellish-folder-0.9.0.tar", last modified: Mon Dec 12 07:43:47 2022, max compression
```

## Comparing `embellish-folder-0.11.0.tar` & `embellish-folder-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:53:16.186523 embellish-folder-0.11.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/src/embellish_folder/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/base_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/fileicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/src/embellish_folder/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/src/embellish_folder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:53:16.000000 embellish-folder-0.11.0/src/embellish_folder.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:53:16.190523 embellish-folder-0.11.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:52:57.000000 embellish-folder-0.11.0/tests/test_compose_icon.py
+drwxr-xr-x   0 rjs        (501) staff       (20)        0 2022-12-12 07:43:47.710294 embellish-folder-0.9.0/
+-rw-r--r--   0 rjs        (501) staff       (20)     1071 2022-05-04 08:56:10.000000 embellish-folder-0.9.0/LICENSE.txt
+-rw-r--r--   0 rjs        (501) staff       (20)     2595 2022-12-12 07:43:47.710357 embellish-folder-0.9.0/PKG-INFO
+-rw-r--r--   0 rjs        (501) staff       (20)      746 2022-12-04 15:23:51.000000 embellish-folder-0.9.0/README.md
+-rw-r--r--   0 rjs        (501) staff       (20)      374 2022-05-04 08:56:10.000000 embellish-folder-0.9.0/pyproject.toml
+-rw-r--r--   0 rjs        (501) staff       (20)     1045 2022-12-12 07:43:47.710643 embellish-folder-0.9.0/setup.cfg
+drwxr-xr-x   0 rjs        (501) staff       (20)        0 2022-12-12 07:43:47.707828 embellish-folder-0.9.0/src/
+drwxr-xr-x   0 rjs        (501) staff       (20)        0 2022-12-12 07:43:47.709308 embellish-folder-0.9.0/src/embellish_folder/
+-rw-r--r--   0 rjs        (501) staff       (20)       67 2022-12-10 21:46:18.000000 embellish-folder-0.9.0/src/embellish_folder/__init__.py
+-rw-r--r--   0 rjs        (501) staff       (20)       52 2022-12-11 09:26:22.000000 embellish-folder-0.9.0/src/embellish_folder/__main__.py
+-rw-r--r--   0 rjs        (501) staff       (20)     1966 2022-12-11 15:18:58.000000 embellish-folder-0.9.0/src/embellish_folder/api.py
+-rw-r--r--   0 rjs        (501) staff       (20)      540 2022-12-10 19:11:39.000000 embellish-folder-0.9.0/src/embellish_folder/app.py
+-rw-r--r--   0 rjs        (501) staff       (20)     2356 2022-12-10 21:31:17.000000 embellish-folder-0.9.0/src/embellish_folder/base_icons.py
+-rw-r--r--   0 rjs        (501) staff       (20)     1919 2022-12-11 15:40:12.000000 embellish-folder-0.9.0/src/embellish_folder/cli.py
+-rw-r--r--   0 rjs        (501) staff       (20)     3588 2022-12-11 17:19:55.000000 embellish-folder-0.9.0/src/embellish_folder/fileicon.py
+-rw-r--r--   0 rjs        (501) staff       (20)      485 2022-12-08 20:49:58.000000 embellish-folder-0.9.0/src/embellish_folder/read.py
+-rw-r--r--   0 rjs        (501) staff       (20)      175 2022-12-10 18:31:30.000000 embellish-folder-0.9.0/src/embellish_folder/version.py
+-rw-r--r--   0 rjs        (501) staff       (20)     2348 2022-12-10 21:40:19.000000 embellish-folder-0.9.0/src/embellish_folder/write.py
+drwxr-xr-x   0 rjs        (501) staff       (20)        0 2022-12-12 07:43:47.709988 embellish-folder-0.9.0/src/embellish_folder.egg-info/
+-rw-r--r--   0 rjs        (501) staff       (20)     2595 2022-12-12 07:43:47.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/PKG-INFO
+-rw-r--r--   0 rjs        (501) staff       (20)      613 2022-12-12 07:43:47.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/SOURCES.txt
+-rw-r--r--   0 rjs        (501) staff       (20)        1 2022-12-12 07:43:47.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/dependency_links.txt
+-rw-r--r--   0 rjs        (501) staff       (20)      111 2022-12-12 07:43:47.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/requires.txt
+-rw-r--r--   0 rjs        (501) staff       (20)       17 2022-12-12 07:43:47.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/top_level.txt
+-rw-r--r--   0 rjs        (501) staff       (20)        1 2022-12-11 15:38:23.000000 embellish-folder-0.9.0/src/embellish_folder.egg-info/zip-safe
```

### Comparing `embellish-folder-0.11.0/LICENSE.txt` & `embellish-folder-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/PKG-INFO` & `embellish-folder-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embellish-folder
-Version: 0.11.0
+Version: 0.9.0
 Summary: Embellish a folder icon
 Home-page: https://github.com/sixty-north/embellish_folder
 Author: Sixty North AS
 Author-email: systems+embellish_folder@sixty-north.com
 License: MIT License
 Keywords: icons
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,17 +18,21 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Embellish Folder
 
+[![Documentation Status](https://readthedocs.org/projects/embellish-folder/badge/?version=latest)](https://embellish-folder.readthedocs.io/en/latest/?badge=latest)
+
 ![CI](https://github.com/sixty-north/embellish_folder/actions/workflows/actions.yml/badge.svg)
 
 
+[![codecov](https://codecov.io/gh/sixty-north/embellish_folder/branch/master/graph/badge.svg?token=66QU3UW6N3)](https://codecov.io/gh/sixty-north/embellish_folder)
+
 ## Installation
 
     $ pip install embellish_folder
 
 
 ## Examples
 
@@ -38,15 +42,14 @@
     >>> embellish_folder("/Users/janet/MyStuff", stuff_image)
     
 
 ## CI/CD
 
     $ bumpversion patch
     $ git push --follow-tags
-
 MIT License
 
 Copyright (c) 2020 Sixty North AS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `embellish-folder-0.11.0/setup.cfg` & `embellish-folder-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder/api.py` & `embellish-folder-0.9.0/src/embellish_folder/api.py`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder/app.py` & `embellish-folder-0.9.0/src/embellish_folder/app.py`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder/base_icons.py` & `embellish-folder-0.9.0/src/embellish_folder/base_icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     foreground.thumbnail((ideal_thumbnail_width, ideal_thumbnail_height))
     actual_thumbnail_width, actual_thumbnail_height = foreground.size
 
     image_x = (icon_width - actual_thumbnail_width) // 2
     image_y = int(
         target_region_top + target_region_padding + (target_region_height - actual_thumbnail_height) / 2
     )
-    foreground = foreground.convert("RGBA")
+
     folder_icon.paste(foreground, (image_x, image_y), foreground)
 
     draw = ImageDraw.Draw(folder_icon)
 
     rx0 = image_x - border
     ry0 = image_y - border
     rx1 = image_x + actual_thumbnail_width + border
```

### Comparing `embellish-folder-0.11.0/src/embellish_folder/cli.py` & `embellish-folder-0.9.0/src/embellish_folder/cli.py`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder/fileicon.py` & `embellish-folder-0.9.0/src/embellish_folder/fileicon.py`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder/write.py` & `embellish-folder-0.9.0/src/embellish_folder/write.py`

 * *Files identical despite different names*

### Comparing `embellish-folder-0.11.0/src/embellish_folder.egg-info/PKG-INFO` & `embellish-folder-0.9.0/src/embellish_folder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embellish-folder
-Version: 0.11.0
+Version: 0.9.0
 Summary: Embellish a folder icon
 Home-page: https://github.com/sixty-north/embellish_folder
 Author: Sixty North AS
 Author-email: systems+embellish_folder@sixty-north.com
 License: MIT License
 Keywords: icons
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,17 +18,21 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Embellish Folder
 
+[![Documentation Status](https://readthedocs.org/projects/embellish-folder/badge/?version=latest)](https://embellish-folder.readthedocs.io/en/latest/?badge=latest)
+
 ![CI](https://github.com/sixty-north/embellish_folder/actions/workflows/actions.yml/badge.svg)
 
 
+[![codecov](https://codecov.io/gh/sixty-north/embellish_folder/branch/master/graph/badge.svg?token=66QU3UW6N3)](https://codecov.io/gh/sixty-north/embellish_folder)
+
 ## Installation
 
     $ pip install embellish_folder
 
 
 ## Examples
 
@@ -38,15 +42,14 @@
     >>> embellish_folder("/Users/janet/MyStuff", stuff_image)
     
 
 ## CI/CD
 
     $ bumpversion patch
     $ git push --follow-tags
-
 MIT License
 
 Copyright (c) 2020 Sixty North AS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

