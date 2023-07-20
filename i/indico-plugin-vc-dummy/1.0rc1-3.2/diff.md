# Comparing `tmp/indico_plugin_vc_dummy-1.0rc1-py2-none-any.whl.zip` & `tmp/indico_plugin_vc_dummy-3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,15 @@
-Zip file size: 4078 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 17-Sep-14 15:47 indico_vc_dummy/__init__.py
--rw-r--r--  2.0 unx     2766 b- defN 17-Oct-06 10:23 indico_vc_dummy/plugin.py
--rw-r--r--  2.0 unx       10 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx       64 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      881 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx      593 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx      863 b- defN 17-Nov-10 12:02 indico_plugin_vc_dummy-1.0rc1.dist-info/RECORD
-9 files, 5285 bytes uncompressed, 2556 bytes compressed:  51.6%
+Zip file size: 15678 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 20-Nov-09 23:13 indico_vc_dummy/__init__.py
+-rw-r--r--  2.0 unx     2218 b- defN 23-Jun-01 10:35 indico_vc_dummy/plugin.py
+-rw-r--r--  2.0 unx     3380 b- defN 20-Nov-09 23:13 indico_vc_dummy/static/images/dummy_icon.png
+-rw-r--r--  2.0 unx     6790 b- defN 20-Nov-09 23:13 indico_vc_dummy/static/images/dummy_logo.png
+-rw-r--r--  2.0 unx      387 b- defN 20-Nov-09 23:13 indico_vc_dummy/templates/info_box.html
+-rw-r--r--  2.0 unx      632 b- defN 20-Nov-09 23:13 indico_vc_dummy/templates/manage_event_create_room.html
+-rw-r--r--  2.0 unx      387 b- defN 20-Nov-09 23:13 indico_vc_dummy/templates/manage_event_info_box.html
+-rw-r--r--  2.0 unx     1048 b- defN 22-Aug-24 10:11 indico_vc_dummy/translations/messages.pot
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jul-20 19:36 indico_plugin_vc_dummy-3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:36 indico_plugin_vc_dummy-3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-20 19:36 indico_plugin_vc_dummy-3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-20 19:36 indico_plugin_vc_dummy-3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Jul-20 19:36 indico_plugin_vc_dummy-3.2.dist-info/RECORD
+13 files, 17398 bytes uncompressed, 13548 bytes compressed:  22.1%
```

## zipnote {}

```diff
@@ -1,28 +1,40 @@
 Filename: indico_vc_dummy/__init__.py
 Comment: 
 
 Filename: indico_vc_dummy/plugin.py
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/DESCRIPTION.rst
+Filename: indico_vc_dummy/static/images/dummy_icon.png
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/entry_points.txt
+Filename: indico_vc_dummy/static/images/dummy_logo.png
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/metadata.json
+Filename: indico_vc_dummy/templates/info_box.html
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/top_level.txt
+Filename: indico_vc_dummy/templates/manage_event_create_room.html
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/WHEEL
+Filename: indico_vc_dummy/templates/manage_event_info_box.html
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/METADATA
+Filename: indico_vc_dummy/translations/messages.pot
 Comment: 
 
-Filename: indico_plugin_vc_dummy-1.0rc1.dist-info/RECORD
+Filename: indico_plugin_vc_dummy-3.2.dist-info/METADATA
+Comment: 
+
+Filename: indico_plugin_vc_dummy-3.2.dist-info/WHEEL
+Comment: 
+
+Filename: indico_plugin_vc_dummy-3.2.dist-info/entry_points.txt
+Comment: 
+
+Filename: indico_plugin_vc_dummy-3.2.dist-info/top_level.txt
+Comment: 
+
+Filename: indico_plugin_vc_dummy-3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_vc_dummy/plugin.py

```diff
@@ -1,27 +1,16 @@
-# This file is part of Indico.
-# Copyright (C) 2002 - 2017 European Organization for Nuclear Research (CERN).
+# This file is part of the Indico plugins.
+# Copyright (C) 2002 - 2023 CERN
 #
-# Indico is free software; you can redistribute it and/or
-# modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 3 of the
-# License, or (at your option) any later version.
-#
-# Indico is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Indico; if not, see <http://www.gnu.org/licenses/>.
-
-from __future__ import unicode_literals
+# The Indico plugins are free software; you can redistribute
+# them and/or modify them under the terms of the MIT License;
+# see the LICENSE file for more details.
 
 from sqlalchemy.orm.attributes import flag_modified
-from wtforms.fields.core import BooleanField
+from wtforms.fields import BooleanField
 
 from indico.core.plugins import IndicoPlugin, IndicoPluginBlueprint, url_for_plugin
 from indico.modules.vc import VCPluginMixin
 from indico.modules.vc.forms import VCRoomAttachFormBase, VCRoomFormBase
 from indico.web.forms.widgets import SwitchWidget
 
 
@@ -67,13 +56,13 @@
     def update_room(self, vc_room, event):
         pass
 
     def refresh_room(self, vc_room, event):
         pass
 
     def update_data_association(self, event, vc_room, event_vc_room, data):
-        super(DummyPlugin, self).update_data_association(event, vc_room, event_vc_room, data)
+        super().update_data_association(event, vc_room, event_vc_room, data)
         event_vc_room.data.update({key: data.pop(key) for key in [
             'show_phone_numbers'
         ]})
 
         flag_modified(event_vc_room, 'data')
```

