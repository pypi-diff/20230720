# Comparing `tmp/indico_plugin_livesync_debug-3.0-py3-none-any.whl.zip` & `tmp/indico_plugin_livesync_debug-3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4047 bytes, number of entries: 8
+Zip file size: 4059 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 20-Nov-09 23:13 indico_livesync_debug/__init__.py
--rw-r--r--  2.0 unx     3420 b- defN 21-Jun-18 15:11 indico_livesync_debug/backend.py
--rw-r--r--  2.0 unx      562 b- defN 21-Jan-26 15:55 indico_livesync_debug/plugin.py
--rw-r--r--  2.0 unx      967 b- defN 21-Jul-16 10:09 indico_plugin_livesync_debug-3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-16 10:09 indico_plugin_livesync_debug-3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       84 b- defN 21-Jul-16 10:09 indico_plugin_livesync_debug-3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 21-Jul-16 10:09 indico_plugin_livesync_debug-3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      750 b- defN 21-Jul-16 10:09 indico_plugin_livesync_debug-3.0.dist-info/RECORD
-8 files, 5897 bytes uncompressed, 2699 bytes compressed:  54.2%
+-rw-r--r--  2.0 unx     3420 b- defN 23-Jun-01 10:35 indico_livesync_debug/backend.py
+-rw-r--r--  2.0 unx      562 b- defN 23-Jun-01 10:35 indico_livesync_debug/plugin.py
+-rw-r--r--  2.0 unx     1087 b- defN 23-Jul-20 19:35 indico_plugin_livesync_debug-3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:35 indico_plugin_livesync_debug-3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-20 19:35 indico_plugin_livesync_debug-3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 19:35 indico_plugin_livesync_debug-3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      751 b- defN 23-Jul-20 19:35 indico_plugin_livesync_debug-3.2.dist-info/RECORD
+8 files, 6017 bytes uncompressed, 2711 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: indico_livesync_debug/backend.py
 Comment: 
 
 Filename: indico_livesync_debug/plugin.py
 Comment: 
 
-Filename: indico_plugin_livesync_debug-3.0.dist-info/METADATA
+Filename: indico_plugin_livesync_debug-3.2.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_livesync_debug-3.0.dist-info/WHEEL
+Filename: indico_plugin_livesync_debug-3.2.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_livesync_debug-3.0.dist-info/entry_points.txt
+Filename: indico_plugin_livesync_debug-3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_livesync_debug-3.0.dist-info/top_level.txt
+Filename: indico_plugin_livesync_debug-3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_livesync_debug-3.0.dist-info/RECORD
+Filename: indico_plugin_livesync_debug-3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_livesync_debug/backend.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2021 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import collections
 from pprint import pformat
```

## indico_livesync_debug/plugin.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2021 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from indico_livesync import LiveSyncPluginBase
 from indico_livesync_debug.backend import LiveSyncDebugBackend
```

## Comparing `indico_plugin_livesync_debug-3.0.dist-info/METADATA` & `indico_plugin_livesync_debug-3.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: indico-plugin-livesync-debug
-Version: 3.0
+Version: 3.2
 Summary: Debug target for the Indico LiveSync plugin
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: ~=3.9.0
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: indico (>=3.0)
 Requires-Dist: indico-plugin-livesync (>=3.0.dev0)
 
 # LiveSync Debug Plugin
 
 The LiveSync debug plugin is meant for developers who want to see the
 queue entries and how they are simplified into actual CRUD-like updates.
 
 It's only intended for developers and thus it is not included when installing
 plugins via the `indico-plugins` meta package.
 
 ## Changelog
 
-### 3.0
+### 3.2
 
-- Initial release for Indico 3.0
+- Support Python 3.11
 
+### 3.0
 
+- Initial release for Indico 3.0
```

## Comparing `indico_plugin_livesync_debug-3.0.dist-info/RECORD` & `indico_plugin_livesync_debug-3.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 indico_livesync_debug/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-indico_livesync_debug/backend.py,sha256=FgkM1K9wa4lOXg0NUN0VTGkDrVroccxKSTWdpSE_dKM,3420
-indico_livesync_debug/plugin.py,sha256=AYvo0XOzJ2Oi0DH5CZQnWRultpp5-3lKeuoxap9pGsc,562
-indico_plugin_livesync_debug-3.0.dist-info/METADATA,sha256=kLw25_nn91F5c1Ga7teczc3mDMnfh9IPTBSGD4Yhsc4,967
-indico_plugin_livesync_debug-3.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-indico_plugin_livesync_debug-3.0.dist-info/entry_points.txt,sha256=ljjRWIjBbwV-yTB9koM4VgK7r7yhFmzp2j39mVStdek,84
-indico_plugin_livesync_debug-3.0.dist-info/top_level.txt,sha256=3g7lCNQM2czQMT-h-rc9DKcqTEUiADmj0IrAbjntCrs,22
-indico_plugin_livesync_debug-3.0.dist-info/RECORD,,
+indico_livesync_debug/backend.py,sha256=TyvOWPoBsTNbIn7Xq_rmwO9A-RhorwcI8Je-YpKRXVU,3420
+indico_livesync_debug/plugin.py,sha256=eLXaOFFSIGPRVxiE0OI7f0je6hJbYKvhNekhDbEeNyY,562
+indico_plugin_livesync_debug-3.2.dist-info/METADATA,sha256=DspMxhVe0vkGYu5zyK9gzFs5WpjO8KtC7L4PnMGx7RI,1087
+indico_plugin_livesync_debug-3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_livesync_debug-3.2.dist-info/entry_points.txt,sha256=qAYYpg8mh9lYnSPQWWge3QwDhiV9P5JIZEZPwAsrywc,83
+indico_plugin_livesync_debug-3.2.dist-info/top_level.txt,sha256=3g7lCNQM2czQMT-h-rc9DKcqTEUiADmj0IrAbjntCrs,22
+indico_plugin_livesync_debug-3.2.dist-info/RECORD,,
```

