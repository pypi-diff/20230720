# Comparing `tmp/indico_plugin_previewer_code-3.2-py3-none-any.whl.zip` & `tmp/indico_plugin_previewer_code-3.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3920 bytes, number of entries: 8
--rw-r--r--  2.0 unx      401 b- defN 22-Jan-05 10:41 indico_previewer_code/__init__.py
--rw-r--r--  2.0 unx     2415 b- defN 22-Jan-05 10:41 indico_previewer_code/plugin.py
+Zip file size: 3963 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      401 b- defN 23-Jun-01 10:35 indico_previewer_code/__init__.py
+-rw-r--r--  2.0 unx     2415 b- defN 23-Jun-01 10:35 indico_previewer_code/plugin.py
 -rw-r--r--  2.0 unx      234 b- defN 20-Nov-09 23:13 indico_previewer_code/templates/pygments_preview.html
--rw-r--r--  2.0 unx      969 b- defN 22-Aug-24 22:56 indico_plugin_previewer_code-3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-24 22:56 indico_plugin_previewer_code-3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 22-Aug-24 22:56 indico_plugin_previewer_code-3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 22-Aug-24 22:56 indico_plugin_previewer_code-3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      773 b- defN 22-Aug-24 22:56 indico_plugin_previewer_code-3.2.dist-info/RECORD
-8 files, 4982 bytes uncompressed, 2530 bytes compressed:  49.2%
+-rw-r--r--  2.0 unx     1107 b- defN 23-Jul-20 19:36 indico_plugin_previewer_code-3.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:36 indico_plugin_previewer_code-3.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-20 19:36 indico_plugin_previewer_code-3.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 19:36 indico_plugin_previewer_code-3.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      784 b- defN 23-Jul-20 19:36 indico_plugin_previewer_code-3.2.1.dist-info/RECORD
+8 files, 5131 bytes uncompressed, 2553 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: indico_previewer_code/plugin.py
 Comment: 
 
 Filename: indico_previewer_code/templates/pygments_preview.html
 Comment: 
 
-Filename: indico_plugin_previewer_code-3.2.dist-info/METADATA
+Filename: indico_plugin_previewer_code-3.2.1.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_previewer_code-3.2.dist-info/WHEEL
+Filename: indico_plugin_previewer_code-3.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_previewer_code-3.2.dist-info/entry_points.txt
+Filename: indico_plugin_previewer_code-3.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_previewer_code-3.2.dist-info/top_level.txt
+Filename: indico_plugin_previewer_code-3.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_previewer_code-3.2.dist-info/RECORD
+Filename: indico_plugin_previewer_code-3.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_previewer_code/__init__.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 """Syntax highlighting for common programming languages and related formats."""
```

## indico_previewer_code/plugin.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import mimetypes
```

## Comparing `indico_plugin_previewer_code-3.2.dist-info/METADATA` & `indico_plugin_previewer_code-3.2.1.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: indico-plugin-previewer-code
-Version: 3.2
+Version: 3.2.1
 Summary: Syntax highlighter for code attachments in Indico
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <3.11,>=3.9.0
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: indico (>=3.2)
 Requires-Dist: Pygments (<3,>=2.7.2)
 
 # Code Preview Plugin
 
 This plugin adds syntax highlighting (using the Pygments syntax highlighter)
@@ -30,14 +32,18 @@
 - JavaScript
 - PHP
 - Python
 - Ruby
 
 ## Changelog
 
+### 3.2.1
+
+- Support Python 3.11
+
 ### 3.2
 
 - Declare compatibility with Python 3.10
 
 ### 3.0
 
 - Initial release for Indico 3.0
```

## Comparing `indico_plugin_previewer_code-3.2.dist-info/RECORD` & `indico_plugin_previewer_code-3.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-indico_previewer_code/__init__.py,sha256=hGbfzmhS97Tn0WCnuXH27-9OsLlDAo2ykQ2zLdlT4aw,401
-indico_previewer_code/plugin.py,sha256=EXYsHYcznhLFLU-zgkf3GGq9qrxnJY2oEz2-VwTjizU,2415
+indico_previewer_code/__init__.py,sha256=rSa-pZmKdbSB9ECqvcLX68ULLRJ_z0KfBxEuPs21-vI,401
+indico_previewer_code/plugin.py,sha256=L0ibuyxd3a68Iq4kytNijrEvM9HIGnqb4QKJfNx7CfI,2415
 indico_previewer_code/templates/pygments_preview.html,sha256=RlTiCN65mkJ5QuQI1OVZ2FQk7SHQYFzqCbbRidywR00,234
-indico_plugin_previewer_code-3.2.dist-info/METADATA,sha256=9KalLSExJvHbQuwEd5xITijmxsV0LIQsYuC7J2EAnY4,969
-indico_plugin_previewer_code-3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-indico_plugin_previewer_code-3.2.dist-info/entry_points.txt,sha256=LeMdLQw2GoNclrQAVjcg_8Vm0hfdiD1D_S8p_065dnA,76
-indico_plugin_previewer_code-3.2.dist-info/top_level.txt,sha256=3WgUqUWkxWA9m4gzyNKxqf1MkblikxmK9092FR8DZYY,22
-indico_plugin_previewer_code-3.2.dist-info/RECORD,,
+indico_plugin_previewer_code-3.2.1.dist-info/METADATA,sha256=Q9KTw3WUqdULhBPW6M06Qf9z72WvTcnjYqq_8UlN00E,1107
+indico_plugin_previewer_code-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_previewer_code-3.2.1.dist-info/entry_points.txt,sha256=LeMdLQw2GoNclrQAVjcg_8Vm0hfdiD1D_S8p_065dnA,76
+indico_plugin_previewer_code-3.2.1.dist-info/top_level.txt,sha256=3WgUqUWkxWA9m4gzyNKxqf1MkblikxmK9092FR8DZYY,22
+indico_plugin_previewer_code-3.2.1.dist-info/RECORD,,
```

