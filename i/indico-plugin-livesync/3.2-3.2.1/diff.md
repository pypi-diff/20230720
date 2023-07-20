# Comparing `tmp/indico_plugin_livesync-3.2-py3-none-any.whl.zip` & `tmp/indico_plugin_livesync-3.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,54 +1,56 @@
-Zip file size: 83773 bytes, number of entries: 52
--rw-r--r--  2.0 unx      835 b- defN 22-Jan-05 10:41 indico_livesync/__init__.py
--rw-r--r--  2.0 unx     9892 b- defN 22-Jan-05 10:41 indico_livesync/base.py
--rw-r--r--  2.0 unx      786 b- defN 22-Jan-05 10:41 indico_livesync/blueprint.py
--rw-r--r--  2.0 unx    10196 b- defN 22-Jan-05 10:41 indico_livesync/cli.py
--rw-r--r--  2.0 unx     3685 b- defN 22-Jan-05 10:41 indico_livesync/controllers.py
--rw-r--r--  2.0 unx      593 b- defN 22-Jan-05 10:41 indico_livesync/forms.py
--rw-r--r--  2.0 unx    10341 b- defN 22-Jan-05 10:41 indico_livesync/handler.py
--rw-r--r--  2.0 unx    16395 b- defN 22-Jun-10 11:38 indico_livesync/initial.py
--rw-r--r--  2.0 unx     3770 b- defN 22-Jan-05 10:41 indico_livesync/plugin.py
--rw-r--r--  2.0 unx    16135 b- defN 22-Jan-05 10:41 indico_livesync/simplify.py
--rw-r--r--  2.0 unx     1345 b- defN 22-Jan-05 10:41 indico_livesync/task.py
--rw-r--r--  2.0 unx     3919 b- defN 22-Jan-05 10:41 indico_livesync/uploader.py
--rw-r--r--  2.0 unx     3960 b- defN 22-Jan-05 10:41 indico_livesync/util.py
+Zip file size: 89754 bytes, number of entries: 54
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-01 10:35 indico_livesync/__init__.py
+-rw-r--r--  2.0 unx     9892 b- defN 23-Jun-01 10:35 indico_livesync/base.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Jun-01 10:35 indico_livesync/blueprint.py
+-rw-r--r--  2.0 unx    10196 b- defN 23-Jun-01 10:35 indico_livesync/cli.py
+-rw-r--r--  2.0 unx     3685 b- defN 23-Jun-01 10:35 indico_livesync/controllers.py
+-rw-r--r--  2.0 unx      593 b- defN 23-Jun-01 10:35 indico_livesync/forms.py
+-rw-r--r--  2.0 unx    10341 b- defN 23-Jun-01 10:35 indico_livesync/handler.py
+-rw-r--r--  2.0 unx    16395 b- defN 23-Jun-01 10:35 indico_livesync/initial.py
+-rw-r--r--  2.0 unx     3770 b- defN 23-Jun-01 10:35 indico_livesync/plugin.py
+-rw-r--r--  2.0 unx    16136 b- defN 23-Jul-05 15:04 indico_livesync/simplify.py
+-rw-r--r--  2.0 unx     1345 b- defN 23-Jun-01 10:35 indico_livesync/task.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Jun-01 10:35 indico_livesync/uploader.py
+-rw-r--r--  2.0 unx     3960 b- defN 23-Jun-01 10:35 indico_livesync/util.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Nov-09 23:13 indico_livesync/migrations/.no-headers
 -rw-r--r--  2.0 unx     4407 b- defN 20-Nov-10 12:03 indico_livesync/migrations/20170630_1557_aa0dbc6c14aa_create_tables.py
 -rw-r--r--  2.0 unx     5227 b- defN 21-May-07 14:48 indico_livesync/migrations/20201023_1224_6ef9616e57cb_add_note_id_and_update_constraints.py
 -rw-r--r--  2.0 unx     6294 b- defN 21-May-07 14:48 indico_livesync/migrations/20210427_1359_d8e65cb6160d_add_attachment_id_to_queue.py
 -rw-r--r--  2.0 unx      907 b- defN 21-May-07 14:48 indico_livesync/migrations/20210506_1917_02a78555cdcb_add_location_changed_change_type.py
 -rw-r--r--  2.0 unx      906 b- defN 21-Jun-04 15:04 indico_livesync/migrations/20210602_1307_330e32d26232_add_undeleted_change_type.py
 -rw-r--r--  2.0 unx      934 b- defN 21-Jun-09 08:46 indico_livesync/migrations/20210608_1713_ff1323696f67_add_published_change_type.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Nov-09 23:13 indico_livesync/models/__init__.py
--rw-r--r--  2.0 unx     1764 b- defN 22-Jan-05 10:41 indico_livesync/models/agents.py
--rw-r--r--  2.0 unx     8543 b- defN 22-Jan-05 10:41 indico_livesync/models/queue.py
+-rw-r--r--  2.0 unx     1764 b- defN 23-Jun-01 10:35 indico_livesync/models/agents.py
+-rw-r--r--  2.0 unx     8542 b- defN 23-Jul-05 15:04 indico_livesync/models/queue.py
 -rw-r--r--  2.0 unx      269 b- defN 20-Nov-09 23:13 indico_livesync/templates/edit_agent.html
 -rw-r--r--  2.0 unx     5807 b- defN 21-May-07 14:48 indico_livesync/templates/plugin_details_extra.html
 -rw-r--r--  2.0 unx     4604 b- defN 22-Aug-24 10:11 indico_livesync/translations/messages.pot
--rw-r--r--  2.0 unx     4198 b- defN 22-Aug-24 22:13 indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6538 b- defN 22-Aug-24 21:58 indico_livesync/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx      507 b- defN 22-Aug-24 22:13 indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     4691 b- defN 22-Aug-24 21:58 indico_livesync/translations/en_GB/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     3739 b- defN 22-Aug-24 22:13 indico_livesync/translations/es_ES/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6203 b- defN 22-Aug-24 21:58 indico_livesync/translations/es_ES/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     3672 b- defN 23-Jul-20 19:35 indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6192 b- defN 23-Jul-14 16:17 indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4199 b- defN 23-Jul-20 19:35 indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6540 b- defN 23-Jul-14 16:17 indico_livesync/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx      507 b- defN 23-Jul-20 19:35 indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     4691 b- defN 23-Jul-14 16:17 indico_livesync/translations/en_GB/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4214 b- defN 23-Jul-20 19:35 indico_livesync/translations/es_ES/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6495 b- defN 23-Jul-14 16:17 indico_livesync/translations/es_ES/LC_MESSAGES/messages.po
 -rw-r--r--  2.0 unx      818 b- defN 20-Nov-09 23:13 indico_livesync/translations/fr_FR/LC_MESSAGES/messages-js.po
--rw-r--r--  2.0 unx     3833 b- defN 22-Aug-24 22:13 indico_livesync/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6299 b- defN 22-Aug-24 21:58 indico_livesync/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4722 b- defN 22-Aug-24 22:13 indico_livesync/translations/mn_MN/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     7231 b- defN 22-Aug-24 21:58 indico_livesync/translations/mn_MN/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4230 b- defN 22-Aug-24 22:13 indico_livesync/translations/pl_PL/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6754 b- defN 22-Aug-24 21:58 indico_livesync/translations/pl_PL/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     3721 b- defN 22-Aug-24 22:13 indico_livesync/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6291 b- defN 22-Aug-24 21:58 indico_livesync/translations/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     3660 b- defN 22-Aug-24 22:13 indico_livesync/translations/tr_TR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6168 b- defN 22-Aug-24 21:58 indico_livesync/translations/tr_TR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4643 b- defN 22-Aug-24 22:13 indico_livesync/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     7215 b- defN 22-Aug-24 21:58 indico_livesync/translations/uk_UA/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     3360 b- defN 22-Aug-24 22:13 indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     5486 b- defN 21-Jul-09 11:16 indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     1073 b- defN 22-Aug-24 22:13 indico_plugin_livesync-3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-24 22:13 indico_plugin_livesync-3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 22-Aug-24 22:13 indico_plugin_livesync-3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Aug-24 22:13 indico_plugin_livesync-3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5453 b- defN 22-Aug-24 22:13 indico_plugin_livesync-3.2.dist-info/RECORD
-52 files, 228521 bytes uncompressed, 74679 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx     4347 b- defN 23-Jul-20 19:35 indico_livesync/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6572 b- defN 23-Jul-14 16:17 indico_livesync/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4722 b- defN 23-Jul-20 19:35 indico_livesync/translations/mn_MN/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     7231 b- defN 23-Jul-14 16:17 indico_livesync/translations/mn_MN/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-20 19:35 indico_livesync/translations/pl_PL/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6789 b- defN 23-Jul-14 16:17 indico_livesync/translations/pl_PL/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4176 b- defN 23-Jul-20 19:35 indico_livesync/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6505 b- defN 23-Jul-14 16:17 indico_livesync/translations/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     3736 b- defN 23-Jul-20 19:35 indico_livesync/translations/tr_TR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6210 b- defN 23-Jul-14 16:17 indico_livesync/translations/tr_TR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4643 b- defN 23-Jul-20 19:35 indico_livesync/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     7215 b- defN 23-Jul-14 16:17 indico_livesync/translations/uk_UA/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     3371 b- defN 23-Jul-20 19:35 indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     5821 b- defN 23-Jul-14 16:17 indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     1245 b- defN 23-Jul-20 19:35 indico_plugin_livesync-3.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:35 indico_plugin_livesync-3.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-20 19:35 indico_plugin_livesync-3.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-20 19:35 indico_plugin_livesync-3.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Jul-20 19:35 indico_plugin_livesync-3.2.1.dist-info/RECORD
+54 files, 241591 bytes uncompressed, 80256 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -72,14 +72,20 @@
 
 Filename: indico_livesync/templates/plugin_details_extra.html
 Comment: 
 
 Filename: indico_livesync/translations/messages.pot
 Comment: 
 
+Filename: indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.mo
+Comment: 
+
+Filename: indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.po
+Comment: 
+
 Filename: indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: indico_livesync/translations/de_DE/LC_MESSAGES/messages.po
 Comment: 
 
 Filename: indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo
@@ -135,23 +141,23 @@
 
 Filename: indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po
 Comment: 
 
-Filename: indico_plugin_livesync-3.2.dist-info/METADATA
+Filename: indico_plugin_livesync-3.2.1.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_livesync-3.2.dist-info/WHEEL
+Filename: indico_plugin_livesync-3.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_livesync-3.2.dist-info/entry_points.txt
+Filename: indico_plugin_livesync-3.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_livesync-3.2.dist-info/top_level.txt
+Filename: indico_plugin_livesync-3.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_livesync-3.2.dist-info/RECORD
+Filename: indico_plugin_livesync-3.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_livesync/__init__.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from indico.core import signals
 from indico.util.i18n import make_bound_gettext
```

## indico_livesync/base.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from flask_pluginengine import depends, trim_docstring
 from sqlalchemy.orm import subqueryload
```

## indico_livesync/blueprint.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from indico.core.plugins import IndicoPluginBlueprint
```

## indico_livesync/cli.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import os
 import sys
```

## indico_livesync/controllers.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from flask import flash, redirect, request
 from flask_pluginengine import current_plugin, render_plugin_template
```

## indico_livesync/forms.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from wtforms.fields import StringField
 from wtforms.validators import DataRequired
```

## indico_livesync/handler.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from collections import defaultdict
```

## indico_livesync/initial.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from sqlalchemy.orm import contains_eager, joinedload, load_only, raiseload, selectinload
```

## indico_livesync/plugin.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from wtforms.fields import BooleanField, IntegerField
 from wtforms.validators import NumberRange
```

## indico_livesync/simplify.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import itertools
 from collections import defaultdict
@@ -15,21 +15,21 @@
 from indico.modules.attachments.models.folders import AttachmentFolder
 from indico.modules.categories.models.categories import Category
 from indico.modules.events.contributions.models.contributions import Contribution
 from indico.modules.events.contributions.models.subcontributions import SubContribution
 from indico.modules.events.models.events import Event
 from indico.modules.events.notes.models.notes import EventNote
 from indico.modules.events.sessions import Session
-from indico.util.enum import IndicoEnum
+from indico.util.enum import IndicoIntEnum
 
 from indico_livesync.models.queue import ChangeType, EntryType
 from indico_livesync.util import get_excluded_categories
 
 
-class SimpleChange(int, IndicoEnum):
+class SimpleChange(IndicoIntEnum):
     deleted = 1
     created = 2
     updated = 4
 
 
 CREATED_DELETED = SimpleChange.created | SimpleChange.deleted
```

## indico_livesync/task.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from celery.schedules import crontab
```

## indico_livesync/uploader.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import re
 from collections import defaultdict
```

## indico_livesync/util.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from datetime import timedelta
```

## indico_livesync/models/agents.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from sqlalchemy.dialects.postgresql import JSON
```

## indico_livesync/models/queue.py

```diff
@@ -1,40 +1,40 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from flask import g
 
 from indico.core.db.sqlalchemy import PyIntEnum, UTCDateTime, db
 from indico.modules.attachments.models.attachments import Attachment
 from indico.modules.categories.models.categories import Category
 from indico.util.date_time import now_utc
-from indico.util.enum import IndicoEnum
+from indico.util.enum import IndicoIntEnum
 from indico.util.string import format_repr
 
 from indico_livesync.models.agents import LiveSyncAgent
 from indico_livesync.util import obj_deref
 
 
-class ChangeType(int, IndicoEnum):
+class ChangeType(IndicoIntEnum):
     created = 1
     deleted = 2
     moved = 3
     data_changed = 4
     protection_changed = 5
     location_changed = 6
     undeleted = 7
     published = 8
     unpublished = 9
 
 
-class EntryType(int, IndicoEnum):
+class EntryType(IndicoIntEnum):
     category = 1
     event = 2
     contribution = 3
     subcontribution = 4
     session = 5
     note = 6
     attachment = 7
```

## indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: bbb user, 2022\n"
+"Last-Translator: bbbuserde, 2022\n"
 "Language: de_DE\n"
-"Language-Team: German (Germany) (http://www.transifex.com/indico/indico/"
+"Language-Team: German (Germany) (http://app.transifex.com/indico/indico/"
 "language/de_DE/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Aktionen"
 
 msgid "Add"
 msgstr "Hinzufügen"
```

## indico_livesync/translations/de_DE/LC_MESSAGES/messages.po

```diff
@@ -1,24 +1,24 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
 # Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2021
-# bbb user, 2022
+# bbbuserde, 2022
 # Dirk Hoffmann <Hoffmann@cppm.in2p3.fr>, 2015,2020
 # Jacqueline Meister <JMeister@age.mpg.de>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: bbb user, 2022\n"
-"Language-Team: German (Germany) (http://www.transifex.com/indico/indico/language/de_DE/)\n"
+"Last-Translator: bbbuserde, 2022\n"
+"Language-Team: German (Germany) (http://app.transifex.com/indico/indico/language/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

## indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version:  Indico*

```diff
@@ -12,21 +12,21 @@
 000000b0: 3131 2031 363a 3533 2b30 3030 300a 4c61  11 16:53+0000.La
 000000c0: 7374 2d54 7261 6e73 6c61 746f 723a 2046  st-Translator: F
 000000d0: 554c 4c20 4e41 4d45 203c 454d 4149 4c40  ULL NAME <EMAIL@
 000000e0: 4144 4452 4553 533e 0a4c 616e 6775 6167  ADDRESS>.Languag
 000000f0: 653a 2065 6e5f 4742 0a4c 616e 6775 6167  e: en_GB.Languag
 00000100: 652d 5465 616d 3a20 456e 676c 6973 6820  e-Team: English 
 00000110: 2855 6e69 7465 6420 4b69 6e67 646f 6d29  (United Kingdom)
-00000120: 2028 6874 7470 3a2f 2f77 7777 2e74 7261   (http://www.tra
+00000120: 2028 6874 7470 3a2f 2f61 7070 2e74 7261   (http://app.tra
 00000130: 6e73 6966 6578 2e63 6f6d 2f69 6e64 6963  nsifex.com/indic
 00000140: 6f2f 696e 6469 636f 2f6c 616e 6775 6167  o/indico/languag
 00000150: 652f 656e 5f47 422f 290a 506c 7572 616c  e/en_GB/).Plural
 00000160: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
 00000170: 3d32 3b20 706c 7572 616c 3d28 6e20 213d  =2; plural=(n !=
 00000180: 2031 293b 0a4d 494d 452d 5665 7273 696f   1);.MIME-Versio
 00000190: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
 000001a0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
 000001b0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
 000001c0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
 000001d0: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
 000001e0: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
-000001f0: 656c 2032 2e31 302e 330a 00              el 2.10.3..
+000001f0: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

## indico_livesync/translations/en_GB/LC_MESSAGES/messages.po

```diff
@@ -6,15 +6,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: English (United Kingdom) (http://www.transifex.com/indico/indico/language/en_GB/)\n"
+"Language-Team: English (United Kingdom) (http://app.transifex.com/indico/indico/language/en_GB/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: en_GB\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

## indico_livesync/translations/es_ES/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,23 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2017,2021\n"
+"Last-Translator: Leonardo J. Caballero G. <leonardocaballero@gmail.com>, "
+"2022\n"
 "Language: es_ES\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/indico/indico/"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/indico/indico/"
 "language/es_ES/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Acciones"
 
 msgid "Add"
 msgstr "Añadir"
 
@@ -114,14 +115,26 @@
 
 msgid "Queue entry TTL"
 msgstr "Entrada de cola TTL"
 
 msgid "Ready"
 msgstr "Listo"
 
+msgid "Skip category changes"
+msgstr "Omitir cambios de categoría"
+
+msgid ""
+"Skip category changes when processing the queue. This can be useful in large "
+"instances when there are significant changes to large categories in order to "
+"avoid processing those immediately."
+msgstr ""
+"Omitir los cambios de categoría al procesar la cola. Esto puede ser útil en "
+"instancias grandes cuando hay cambios significativos en categorías grandes "
+"para evitar procesarlos de inmediato."
+
 msgid "Status"
 msgstr "Estado"
 
 msgid "The name of the agent. Only used in the administration interface."
 msgstr "Nombre del agente. Solo se utiliza en la interfaz de administración."
 
 msgid "This backend is already in use"
```

## indico_livesync/translations/es_ES/LC_MESSAGES/messages.po

```diff
@@ -1,21 +1,22 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
 # Jesús Martín <jesusmartin@sallep.net>, 2017,2021
+# Leonardo J. Caballero G. <leonardocaballero@gmail.com>, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2017,2021\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/indico/indico/language/es_ES/)\n"
+"Last-Translator: Leonardo J. Caballero G. <leonardocaballero@gmail.com>, 2022\n"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/indico/indico/language/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -84,22 +85,22 @@
 
 #: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "Desacivar todas las ejecuciones programadas en cola. "
 
 #: indico_livesync/plugin.py:37
 msgid "Skip category changes"
-msgstr ""
+msgstr "Omitir cambios de categoría"
 
 #: indico_livesync/plugin.py:38
 msgid ""
 "Skip category changes when processing the queue. This can be useful in large"
 " instances when there are significant changes to large categories in order "
 "to avoid processing those immediately."
-msgstr ""
+msgstr "Omitir los cambios de categoría al procesar la cola. Esto puede ser útil en instancias grandes cuando hay cambios significativos en categorías grandes para evitar procesarlos de inmediato."
 
 #: indico_livesync/templates/edit_agent.html:9
 msgid "Cancel"
 msgstr "Cancelar"
 
 #: indico_livesync/templates/plugin_details_extra.html:7
 #: indico_livesync/templates/plugin_details_extra.html:11
```

## indico_livesync/translations/fr_FR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021\n"
+"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021-2022\n"
 "Language: fr_FR\n"
-"Language-Team: French (France) (http://www.transifex.com/indico/indico/"
+"Language-Team: French (France) (http://app.transifex.com/indico/indico/"
 "language/fr_FR/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Actions"
 
 msgid "Add"
 msgstr "Ajouter"
 
@@ -116,14 +116,26 @@
 
 msgid "Queue entry TTL"
 msgstr "TTL d'une entrée dans la file d'attente"
 
 msgid "Ready"
 msgstr "Prêt"
 
+msgid "Skip category changes"
+msgstr "Sauter les changements des catégories"
+
+msgid ""
+"Skip category changes when processing the queue. This can be useful in large "
+"instances when there are significant changes to large categories in order to "
+"avoid processing those immediately."
+msgstr ""
+"Sauter les changements des catégories dans le traitement de la queue. Ceci "
+"peut être utile dans les grandes instances lors de changements importants "
+"dans des grandes catégories afin d'éviter de les traiter immédiatement."
+
 msgid "Status"
 msgstr "Statut"
 
 msgid "The name of the agent. Only used in the administration interface."
 msgstr ""
 "Le nom de l'agent. Utilisé uniquement dans l'interface d'administration."
```

## indico_livesync/translations/fr_FR/LC_MESSAGES/messages.po

```diff
@@ -1,21 +1,21 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
-# Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021
+# Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021-2022
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021\n"
-"Language-Team: French (France) (http://www.transifex.com/indico/indico/language/fr_FR/)\n"
+"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2015,2017,2021-2022\n"
+"Language-Team: French (France) (http://app.transifex.com/indico/indico/language/fr_FR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr_FR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -84,22 +84,22 @@
 
 #: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "Désactiver toutes les exécutions de file d'attente planifiées."
 
 #: indico_livesync/plugin.py:37
 msgid "Skip category changes"
-msgstr ""
+msgstr "Sauter les changements des catégories"
 
 #: indico_livesync/plugin.py:38
 msgid ""
 "Skip category changes when processing the queue. This can be useful in large"
 " instances when there are significant changes to large categories in order "
 "to avoid processing those immediately."
-msgstr ""
+msgstr "Sauter les changements des catégories dans le traitement de la queue. Ceci peut être utile dans les grandes instances lors de changements importants dans des grandes catégories afin d'éviter de les traiter immédiatement."
 
 #: indico_livesync/templates/edit_agent.html:9
 msgid "Cancel"
 msgstr "Annuler"
 
 #: indico_livesync/templates/plugin_details_extra.html:7
 #: indico_livesync/templates/plugin_details_extra.html:11
```

## indico_livesync/translations/mn_MN/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
 "Last-Translator: Batbayar Bat-Erdene <yertonts@gmail.com>, 2021\n"
 "Language: mn_MN\n"
-"Language-Team: Mongolian (Mongolia) (http://www.transifex.com/indico/indico/"
+"Language-Team: Mongolian (Mongolia) (http://app.transifex.com/indico/indico/"
 "language/mn_MN/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Үйлдлүүд"
 
 msgid "Add"
 msgstr "Нэмэх"
```

## indico_livesync/translations/mn_MN/LC_MESSAGES/messages.po

```diff
@@ -8,15 +8,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
 "Last-Translator: Batbayar Bat-Erdene <yertonts@gmail.com>, 2021\n"
-"Language-Team: Mongolian (Mongolia) (http://www.transifex.com/indico/indico/language/mn_MN/)\n"
+"Language-Team: Mongolian (Mongolia) (http://app.transifex.com/indico/indico/language/mn_MN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: mn_MN\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

## indico_livesync/translations/pl_PL/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,24 +1,25 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2021\n"
+"Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, "
+"2021,2023\n"
 "Language: pl_PL\n"
-"Language-Team: Polish (Poland) (http://www.transifex.com/indico/indico/"
+"Language-Team: Polish (Poland) (http://app.transifex.com/indico/indico/"
 "language/pl_PL/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Akcje"
 
 msgid "Add"
 msgstr "Dodaj"
 
@@ -116,14 +117,17 @@
 
 msgid "Queue entry TTL"
 msgstr "Czas życia wpisu w kolejce"
 
 msgid "Ready"
 msgstr "Gotowy"
 
+msgid "Skip category changes"
+msgstr "Pomiń zmiany w kategorii"
+
 msgid "Status"
 msgstr "Status"
 
 msgid "The name of the agent. Only used in the administration interface."
 msgstr "Nazwa agenta. Wykorzystywana tylko w interfejsie administracyjnym."
 
 msgid "This backend is already in use"
```

## indico_livesync/translations/pl_PL/LC_MESSAGES/messages.po

```diff
@@ -1,22 +1,22 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
 # Jerzy Pankiewicz <jerzy.pankiewicz@pwr.edu.pl>, 2018
-# Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2021
+# Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2021,2023
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2021\n"
-"Language-Team: Polish (Poland) (http://www.transifex.com/indico/indico/language/pl_PL/)\n"
+"Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2021,2023\n"
+"Language-Team: Polish (Poland) (http://app.transifex.com/indico/indico/language/pl_PL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl_PL\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
@@ -85,15 +85,15 @@
 
 #: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "Wyłącz wszystkie zaplanowane wyłączenia kolejek. "
 
 #: indico_livesync/plugin.py:37
 msgid "Skip category changes"
-msgstr ""
+msgstr "Pomiń zmiany w kategorii"
 
 #: indico_livesync/plugin.py:38
 msgid ""
 "Skip category changes when processing the queue. This can be useful in large"
 " instances when there are significant changes to large categories in order "
 "to avoid processing those immediately."
 msgstr ""
```

## indico_livesync/translations/pt_BR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Sedir G. Morais <philippi.sedir@gmail.com>, 2021\n"
+"Last-Translator: Andre Garcia <sambombe@gmail.com>, 2019,2022\n"
 "Language: pt_BR\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/indico/indico/"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/indico/indico/"
 "language/pt_BR/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Ações"
 
 msgid "Add"
 msgstr "Adicionar"
 
@@ -114,14 +114,26 @@
 
 msgid "Queue entry TTL"
 msgstr "Entrada na fila TTL"
 
 msgid "Ready"
 msgstr "Pronto"
 
+msgid "Skip category changes"
+msgstr "Pular mudanças de categoria"
+
+msgid ""
+"Skip category changes when processing the queue. This can be useful in large "
+"instances when there are significant changes to large categories in order to "
+"avoid processing those immediately."
+msgstr ""
+"Pular mudanças de categoria ao processar a fila. Isto pode ser útil quando "
+"existem alterações significativas em categorias grandes, no sentido de "
+"evitar processá-las imediatamente."
+
 msgid "Status"
 msgstr "Status"
 
 msgid "The name of the agent. Only used in the administration interface."
 msgstr "O nome do agente. Somente usado na administração da interface."
 
 msgid "This backend is already in use"
```

## indico_livesync/translations/pt_BR/LC_MESSAGES/messages.po

```diff
@@ -1,23 +1,23 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
-# Andre Garcia <sambombe@gmail.com>, 2019
+# Andre Garcia <sambombe@gmail.com>, 2019,2022
 # Fernanda Paulo Ramos <fernanda.ramos+transifex@gmail.com>, 2019
 # Sedir G. Morais <philippi.sedir@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: Sedir G. Morais <philippi.sedir@gmail.com>, 2021\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/indico/indico/language/pt_BR/)\n"
+"Last-Translator: Andre Garcia <sambombe@gmail.com>, 2019,2022\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/indico/indico/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -86,22 +86,22 @@
 
 #: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "Desativar todas as execuções de fila programadas."
 
 #: indico_livesync/plugin.py:37
 msgid "Skip category changes"
-msgstr ""
+msgstr "Pular mudanças de categoria"
 
 #: indico_livesync/plugin.py:38
 msgid ""
 "Skip category changes when processing the queue. This can be useful in large"
 " instances when there are significant changes to large categories in order "
 "to avoid processing those immediately."
-msgstr ""
+msgstr "Pular mudanças de categoria ao processar a fila. Isto pode ser útil quando existem alterações significativas em categorias grandes, no sentido de evitar processá-las imediatamente."
 
 #: indico_livesync/templates/edit_agent.html:9
 msgid "Cancel"
 msgstr "Cancelar"
 
 #: indico_livesync/templates/plugin_details_extra.html:7
 #: indico_livesync/templates/plugin_details_extra.html:11
```

## indico_livesync/translations/tr_TR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021\n"
+"Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021-2022\n"
 "Language: tr_TR\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/indico/indico/"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/indico/indico/"
 "language/tr_TR/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Eylemler"
 
 msgid "Add"
 msgstr "Ekle"
 
@@ -113,14 +113,17 @@
 
 msgid "Queue entry TTL"
 msgstr "Sıra girişi TTL"
 
 msgid "Ready"
 msgstr "Hazır"
 
+msgid "Skip category changes"
+msgstr "Kategori değişikliklerini atla"
+
 msgid "Status"
 msgstr "Durum"
 
 msgid "The name of the agent. Only used in the administration interface."
 msgstr "Araç adı. Yalnızca yönetim arayüzünde kullanılır."
 
 msgid "This backend is already in use"
```

## indico_livesync/translations/tr_TR/LC_MESSAGES/messages.po

```diff
@@ -1,22 +1,22 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
 # Gökhan Kalayci <gkmediagokhan@gmail.com>, 2017
-# selcuk bilmis <selcukbilmis@gmail.com>, 2021
+# selcuk bilmis <selcukbilmis@gmail.com>, 2021-2022
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
-"Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/indico/indico/language/tr_TR/)\n"
+"Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021-2022\n"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/indico/indico/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -85,15 +85,15 @@
 
 #: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "Zamanlanmış tüm kuyruk çalıştırmalarını devre dışı bırak"
 
 #: indico_livesync/plugin.py:37
 msgid "Skip category changes"
-msgstr ""
+msgstr "Kategori değişikliklerini atla"
 
 #: indico_livesync/plugin.py:38
 msgid ""
 "Skip category changes when processing the queue. This can be useful in large"
 " instances when there are significant changes to large categories in order "
 "to avoid processing those immediately."
 msgstr ""
```

## indico_livesync/translations/uk_UA/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,24 +2,24 @@
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
 "Last-Translator: Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2021\n"
 "Language: uk_UA\n"
-"Language-Team: Ukrainian (Ukraine) (http://www.transifex.com/indico/indico/"
+"Language-Team: Ukrainian (Ukraine) (http://app.transifex.com/indico/indico/"
 "language/uk_UA/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "Операції"
 
 msgid "Add"
 msgstr "Додати"
```

## indico_livesync/translations/uk_UA/LC_MESSAGES/messages.po

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2015-03-11 16:53+0000\n"
 "Last-Translator: Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2021\n"
-"Language-Team: Ukrainian (Ukraine) (http://www.transifex.com/indico/indico/language/uk_UA/)\n"
+"Language-Team: Ukrainian (Ukraine) (http://app.transifex.com/indico/indico/language/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
```

## indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-05-26 17:54+0200\n"
-"PO-Revision-Date: 2021-05-31 07:59+0000\n"
-"Last-Translator: Lanxin Ma <ma@ihep.ac.cn>\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
+"PO-Revision-Date: 2015-03-11 16:53+0000\n"
+"Last-Translator: Lanxin Ma <ma@ihep.ac.cn>, 2020-2021\n"
 "Language: zh_CN.GB2312\n"
-"Language-Team: Chinese (China) (GB2312) (http://www.transifex.com/indico/"
+"Language-Team: Chinese (China) (GB2312) (http://app.transifex.com/indico/"
 "indico/language/zh_CN.GB2312/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Actions"
 msgstr "操作"
 
 msgid "Add"
 msgstr "添加"
```

## indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po

```diff
@@ -1,25 +1,25 @@
 # Translations template for PROJECT.
-# Copyright (C) 2021 ORGANIZATION
+# Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # 
 # Translators:
 # Lanxin Ma <ma@ihep.ac.cn>, 2020-2021
 msgid ""
 msgstr ""
 "Project-Id-Version: Indico\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-05-26 17:54+0200\n"
-"PO-Revision-Date: 2021-05-31 07:59+0000\n"
-"Last-Translator: Lanxin Ma <ma@ihep.ac.cn>\n"
-"Language-Team: Chinese (China) (GB2312) (http://www.transifex.com/indico/indico/language/zh_CN.GB2312/)\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
+"PO-Revision-Date: 2015-03-11 16:53+0000\n"
+"Last-Translator: Lanxin Ma <ma@ihep.ac.cn>, 2020-2021\n"
+"Language-Team: Chinese (China) (GB2312) (http://app.transifex.com/indico/indico/language/zh_CN.GB2312/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.3\n"
 "Language: zh_CN.GB2312\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: indico_livesync/controllers.py:41
 msgid "Agent deleted"
 msgstr "已删除的代理"
 
@@ -48,48 +48,59 @@
 msgid "Name"
 msgstr "名字"
 
 #: indico_livesync/forms.py:18
 msgid "The name of the agent. Only used in the administration interface."
 msgstr "代理的名称。仅在管理界面中使用。"
 
-#: indico_livesync/plugin.py:26
+#: indico_livesync/plugin.py:25
 msgid "Queue entry TTL"
 msgstr "队列条目TTL"
 
-#: indico_livesync/plugin.py:27
+#: indico_livesync/plugin.py:26
 msgid ""
 "How many days should processed entries be kept in the queue. The time counts"
 " from the creation of the queue entries, so if the LiveSync task is not "
 "running for some time, queue entries may be deleted during the next run "
 "after processing them. Setting it to 0 disables automatic deletion."
 msgstr "应在队列中保留处理的条目的天数。从创建队列条目开始计算时间，因此，如果LiveSync任务有一段时间没有运行，则在处理队列条目后的下一次运行期间可能会删除它们。将其设置为 0 将禁用自动删除。"
 
-#: indico_livesync/plugin.py:32
+#: indico_livesync/plugin.py:31
 msgid "Excluded categories"
 msgstr "排除的类别"
 
-#: indico_livesync/plugin.py:33
+#: indico_livesync/plugin.py:32
 msgid "Category ID"
 msgstr "类别 ID"
 
-#: indico_livesync/plugin.py:34
+#: indico_livesync/plugin.py:33
 msgid ""
 "Changes to objects inside these categories or any of their subcategories are"
 " excluded."
 msgstr "不包括对这些类别或其任何子类别中的对象所做的更改。"
 
-#: indico_livesync/plugin.py:36
+#: indico_livesync/plugin.py:35
 msgid "Disable queue runs"
 msgstr "禁用队列运行"
 
-#: indico_livesync/plugin.py:37
+#: indico_livesync/plugin.py:36
 msgid "Disable all scheduled queue runs."
 msgstr "禁用所有计划的队列运行。"
 
+#: indico_livesync/plugin.py:37
+msgid "Skip category changes"
+msgstr ""
+
+#: indico_livesync/plugin.py:38
+msgid ""
+"Skip category changes when processing the queue. This can be useful in large"
+" instances when there are significant changes to large categories in order "
+"to avoid processing those immediately."
+msgstr ""
+
 #: indico_livesync/templates/edit_agent.html:9
 msgid "Cancel"
 msgstr "取消"
 
 #: indico_livesync/templates/plugin_details_extra.html:7
 #: indico_livesync/templates/plugin_details_extra.html:11
 #, python-format
```

## Comparing `indico_plugin_livesync-3.2.dist-info/METADATA` & `indico_plugin_livesync-3.2.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: indico-plugin-livesync
-Version: 3.2
+Version: 3.2.1
 Summary: Framework for pushing Indico event data to external services
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
-Requires-Dist: indico (>=3.2)
+Requires-Dist: indico (>=3.2.6)
 
 # LiveSync Plugin
 
 The LiveSync plugin provides a framework for exporting Indico event data to
 external services, typically to provide advanced search functionality.
 
 ## Changelog
 
+### 3.2.1
+
+- Adapt to Indico 3.2.6 changes
+- Support Python 3.11
+
 ### 3.2
 
 - Adapt to Indico 3.2 changes
 
 ### 3.1
 
 - Adapt to Indico 3.1 changes
```

## Comparing `indico_plugin_livesync-3.2.dist-info/RECORD` & `indico_plugin_livesync-3.2.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-indico_livesync/__init__.py,sha256=3-eirkdKapyhvVZNSHw3DXKL5rH5YoImilQCRE2LM0U,835
-indico_livesync/base.py,sha256=rM7p2UxT_ffWBRG7yKNZLL3G5qxAut8wz2TQhTZH8qo,9892
-indico_livesync/blueprint.py,sha256=QJ2mEM5K1pv3_yWj3AWb3b6QEhuHv9E8NPZPx9-gLIc,786
-indico_livesync/cli.py,sha256=hZMz5L9vg7_zCM4kDNEU-Jy3FW1PU3CWKEXHy8ME3cE,10196
-indico_livesync/controllers.py,sha256=azFkbtua0ZEqLZBHloqZAxp6O2m9XCWioJJi-cWM-ms,3685
-indico_livesync/forms.py,sha256=HVhhJd3OUd8puR_KKA4jH4_TZyq5RnBNH5rZBL-zegs,593
-indico_livesync/handler.py,sha256=8kIlew_RjTVpz_RHUvEtasyKEhm9ox3B5Olu2m57i4U,10341
-indico_livesync/initial.py,sha256=AZ3Pfd-P9F7YjuBIFL21UXLyBsW0dMwIkAwd7GXTHiQ,16395
-indico_livesync/plugin.py,sha256=_BZBts-iQkUGro4Ax_N2xB3NxQhQgB7RrhZCs8closs,3770
-indico_livesync/simplify.py,sha256=Aok9ZnaJ3V_sOTUJ8JjIVQslXEvr0nvoDFhidKRPTNQ,16135
-indico_livesync/task.py,sha256=X9kx3qUU8dvoBb62cZfWX1R32lD_dxe49HklB9oY1fM,1345
-indico_livesync/uploader.py,sha256=o5zk6bpWte1eeVamT7t5yCPwAE2gueI10KdKoZTLRsM,3919
-indico_livesync/util.py,sha256=mkgsXUZrTrrhO0pC4q3IyRoJL2yscBbLhZzirmmYZM0,3960
+indico_livesync/__init__.py,sha256=lu9mQZ7SyVAFOGLaAuShWwCgAEA9Xkz4Tmh_i1c9HQg,835
+indico_livesync/base.py,sha256=-3NkXuPsB74B4xdptBs5haOa9C1S4r47nfZXBEckO0c,9892
+indico_livesync/blueprint.py,sha256=LN2jbzPumBj-N6HrT9A2beuAg6axfIY2KWvZ71jtClc,786
+indico_livesync/cli.py,sha256=mjAR1EHyq_OS3_fA78amgvMOzv1rMk7mcVRO-oT0B-A,10196
+indico_livesync/controllers.py,sha256=JApVzcDoT4qvPrYzhfQwRIgk0cCPJcPg2CGvgly-SgU,3685
+indico_livesync/forms.py,sha256=7UIGwY9SePwJw3Dc8wuUdR8brPOg-hD-bNadyCyOh2E,593
+indico_livesync/handler.py,sha256=un3DovbriPWJTVFJa7iMUXEp7NzHWTcOs7N-cACsz_A,10341
+indico_livesync/initial.py,sha256=iFCwrNl42GZJhHuMP3jBRNnPsCxAnMXztTSOCzng5p4,16395
+indico_livesync/plugin.py,sha256=gS0ql5PSZnFhPJ4EKRhzZFFmzMg2toCPFGhx_jYDsWg,3770
+indico_livesync/simplify.py,sha256=2JdfEnd3FRTuvzWLg9nqm4JpSaBO4YE-drHTlvev84U,16136
+indico_livesync/task.py,sha256=vb_0UKoebYxx4lG8SGBICHbZwazv00tYiD8ZMdi_VfI,1345
+indico_livesync/uploader.py,sha256=CgbZNtyYr1qh0QefpQpgQTabPAcaSWWLuACesupFTJM,3919
+indico_livesync/util.py,sha256=6WtVcEQPqOo5kXLhhFC4RCoMKbP1SxIILq0LxDfxb3E,3960
 indico_livesync/migrations/.no-headers,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 indico_livesync/migrations/20170630_1557_aa0dbc6c14aa_create_tables.py,sha256=hjjEpKpnYlEJAT1LXbu5rqsTLPxsZpVF17HI7e-MQ78,4407
 indico_livesync/migrations/20201023_1224_6ef9616e57cb_add_note_id_and_update_constraints.py,sha256=Zl9iGTwMKq4iLybyI0xabsS6DiPcOM753RdpuGLYmxM,5227
 indico_livesync/migrations/20210427_1359_d8e65cb6160d_add_attachment_id_to_queue.py,sha256=FuPN15zmVuwSbMRXaOJdzbYe_EYgICCQ_TmN3DE0yHQ,6294
 indico_livesync/migrations/20210506_1917_02a78555cdcb_add_location_changed_change_type.py,sha256=AlniNPmhdvUGYjE-mXpsgZTsCCvMFHQm-ZkyjdFigAI,907
 indico_livesync/migrations/20210602_1307_330e32d26232_add_undeleted_change_type.py,sha256=N8jYGc7aoS7Tu4ZoXgDtLHcmpfBkdVrfQ1gWFJzSyPQ,906
 indico_livesync/migrations/20210608_1713_ff1323696f67_add_published_change_type.py,sha256=phvxvDK8P8NGWKe97TbSGPAA0EjZXt4QsQdiyXcxcp4,934
 indico_livesync/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-indico_livesync/models/agents.py,sha256=siBQvDooy5JPHX7bH7oW3PE4cy-QTHLJLPAef1IqXYw,1764
-indico_livesync/models/queue.py,sha256=iaXF-rM-k_Gwbcl6SukChcCgi8u85R3lYTxVT09eCqw,8543
+indico_livesync/models/agents.py,sha256=SzuMjGtP-m4YEBougCV_ugI5tw6qruvDMbLGb0U1tLk,1764
+indico_livesync/models/queue.py,sha256=WwZhIOGYd_kzkc41NjJZqTCKkF72a9n5fH6r7qZt9RA,8542
 indico_livesync/templates/edit_agent.html,sha256=6qf7JxN7P6LFSts6AGyDoz4mqDXSHgkd8tiNLMHsLwE,269
 indico_livesync/templates/plugin_details_extra.html,sha256=JyrQr3xv6cV4pm4I-XqT6PUUQuY5egYk2EuIvggp9mc,5807
 indico_livesync/translations/messages.pot,sha256=PjvZBcWWm4fAdHLY1cxGi8Hb2yZicS8DxxiD5UJcBxA,4604
-indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo,sha256=gjU6rPFtvfXhwzT6xIi598ohFWDNFF6LFusB6zqhlHQ,4198
-indico_livesync/translations/de_DE/LC_MESSAGES/messages.po,sha256=gjH_UDYAFyjMZ_FEHSH8VyFRIeRltUtNVMgM0zYv4Y4,6538
-indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo,sha256=9A-lwJW78QpOZNY1GTIAUuOUQLWr9HSElmPHpOePB5s,507
-indico_livesync/translations/en_GB/LC_MESSAGES/messages.po,sha256=9nEVBS2OYeKTitwUbacMKf2OLy1dL_ludv6c2v987h4,4691
-indico_livesync/translations/es_ES/LC_MESSAGES/messages.mo,sha256=JB2Ko-FdufguSuulcvqT6DlnszvGXfE0FuueWOINObU,3739
-indico_livesync/translations/es_ES/LC_MESSAGES/messages.po,sha256=mqWBNrkzvazegVpL9eEs-4LL7nMYI1c2gJNpRczOLSg,6203
+indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.mo,sha256=j3FA_h4pMQjk35iSyeXho2TIvx-b8Wr_eil8Ec_5VuM,3672
+indico_livesync/translations/cs_CZ/LC_MESSAGES/messages.po,sha256=TyjDFF6ey4CxAd5N4Kr1fFm7EckQaBeU4iKVG28y-hE,6192
+indico_livesync/translations/de_DE/LC_MESSAGES/messages.mo,sha256=NLakNt0sKgG8C_U0B43zuYtJ02KgblbVkkiUOYYBodA,4199
+indico_livesync/translations/de_DE/LC_MESSAGES/messages.po,sha256=ep7GxQPBULd_3jGk-XAwOBldDsDOsv9YfCIiH8g55ZI,6540
+indico_livesync/translations/en_GB/LC_MESSAGES/messages.mo,sha256=-IW_XBKBvEifDDMhUYRHoWDEJfCBTZPkbz43g7Dh9i0,507
+indico_livesync/translations/en_GB/LC_MESSAGES/messages.po,sha256=XloMBoaiNPZzt4hDQJe23jwoy0Ygvdo-ObaR1h2bQnQ,4691
+indico_livesync/translations/es_ES/LC_MESSAGES/messages.mo,sha256=OTya4fgHSMa2QTwjjf6SVJt-MGPMBvTrb4O9tclWoHU,4214
+indico_livesync/translations/es_ES/LC_MESSAGES/messages.po,sha256=O4n35iNk0WvSP7r9vYY7CYVfbXLpQGgBS9hHXdd6Yow,6495
 indico_livesync/translations/fr_FR/LC_MESSAGES/messages-js.po,sha256=RVxAAClIOsR8OkGSZmbJXyz-qtUQeEu1CXgqDQs9Zrw,818
-indico_livesync/translations/fr_FR/LC_MESSAGES/messages.mo,sha256=rmjpOOox14h2XM9ihw7nHnPVhLJ51Acc_VMCFDl76u0,3833
-indico_livesync/translations/fr_FR/LC_MESSAGES/messages.po,sha256=yqIcQRmfYAQQ4JPT3UqPi2klNGqVo7y5CuYyBNSUwtY,6299
-indico_livesync/translations/mn_MN/LC_MESSAGES/messages.mo,sha256=cgmI8aUZr3kowAeAQQMPUOJ4Vk_wC0-snrDD9V5fiAs,4722
-indico_livesync/translations/mn_MN/LC_MESSAGES/messages.po,sha256=3e422SnIf8eMIhsQwZrLh4l6pSeIxaCuWwszMW7x5sY,7231
-indico_livesync/translations/pl_PL/LC_MESSAGES/messages.mo,sha256=5oJnRaroL-H0YHe3hZFANRI2USUeP_CwFwcx4g2MI-Q,4230
-indico_livesync/translations/pl_PL/LC_MESSAGES/messages.po,sha256=GN0TI5ZwlNMnvbnPkwi17lKZuJjqOQnYY15sdagLOVg,6754
-indico_livesync/translations/pt_BR/LC_MESSAGES/messages.mo,sha256=N5se9xfkoTqRveDaPBk_gDgFuHKc03iCaNAPfEmMeKc,3721
-indico_livesync/translations/pt_BR/LC_MESSAGES/messages.po,sha256=F9ilUMQNEkbkPRLcb3fwmEQZxPlbBgHIx5kt8qBo7wI,6291
-indico_livesync/translations/tr_TR/LC_MESSAGES/messages.mo,sha256=4r7OycEXO7JRRu7zAz8iE_bLKN600f1ZHx5iP52JruE,3660
-indico_livesync/translations/tr_TR/LC_MESSAGES/messages.po,sha256=RGPyt7CYbz9GBLKU0d5_49f5X-EG4ZMjrFp3vNHDa0Q,6168
-indico_livesync/translations/uk_UA/LC_MESSAGES/messages.mo,sha256=f9CKs_Fg7jkl39i8JWyYUE2-oBhwdIOe2oIrNCFQplg,4643
-indico_livesync/translations/uk_UA/LC_MESSAGES/messages.po,sha256=8Eu7YMT1GpS8JdCo52Fs0HbEViMdL5aEbNlRKEuTCJY,7215
-indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo,sha256=BK8OkMsVEnjYitp9J3YrL7jOUADQ1-0uV-2IwFf0v5U,3360
-indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po,sha256=Pq9RtyG4oMymS93d4smwuhXnyVKTXVj6a-ey-VrTCKQ,5486
-indico_plugin_livesync-3.2.dist-info/METADATA,sha256=KUkqTk1gTWEKkIVy7t9g9lphqKTPugO4sA_L03Qu8Vc,1073
-indico_plugin_livesync-3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-indico_plugin_livesync-3.2.dist-info/entry_points.txt,sha256=XHlJdTWaSOpzutIS9U4olLQhzuZ3Z74tUZCABwmNRbs,66
-indico_plugin_livesync-3.2.dist-info/top_level.txt,sha256=0Inu0Xuoe4LDl-DGNO1r6XdC6k7b0We7rBE-kNze7iI,16
-indico_plugin_livesync-3.2.dist-info/RECORD,,
+indico_livesync/translations/fr_FR/LC_MESSAGES/messages.mo,sha256=UEVy403L20aBu4F5oPwN-UC7rkmKm3DlB5aclwMyv9s,4347
+indico_livesync/translations/fr_FR/LC_MESSAGES/messages.po,sha256=-MRoBmlogZGLaaY7KVpNqUtB6YwQSVF_PKvJCYeQTsw,6572
+indico_livesync/translations/mn_MN/LC_MESSAGES/messages.mo,sha256=te7LvTGdt9uOcDIjzYlET8JtC9BxtZN-QVfuN9sOM2c,4722
+indico_livesync/translations/mn_MN/LC_MESSAGES/messages.po,sha256=6V7PiGG_p2Y6Www5WGy2nC1ElMNMc6UP6KbenNN0zjU,7231
+indico_livesync/translations/pl_PL/LC_MESSAGES/messages.mo,sha256=GzgItm3JhxJALSFk_mVknYhpiFORdhNHrayc0FmASVM,4299
+indico_livesync/translations/pl_PL/LC_MESSAGES/messages.po,sha256=e51LkosjKFJVxlOO3NZdwoOeBP5U1-LCO7x9hARfYzo,6789
+indico_livesync/translations/pt_BR/LC_MESSAGES/messages.mo,sha256=aCg1dYSg0zzLuIToS2JD8D4LZK6kPjBespHxTS-MwDo,4176
+indico_livesync/translations/pt_BR/LC_MESSAGES/messages.po,sha256=V3C95D6fiA058splX-RNO2j51T6ecq98eACGIHnjyIs,6505
+indico_livesync/translations/tr_TR/LC_MESSAGES/messages.mo,sha256=vZ1cucuRMkykn3B3LKrt-usIqGY3RHivLGaXb7XGBu4,3736
+indico_livesync/translations/tr_TR/LC_MESSAGES/messages.po,sha256=-FAnScVU0VCTXsxWjBt82LG2Bvy6EdE7nCrIOVv2sYU,6210
+indico_livesync/translations/uk_UA/LC_MESSAGES/messages.mo,sha256=Fjn2oFG8L01OS4vM7HmOek8RHqrldQGsZY5tXd41MTE,4643
+indico_livesync/translations/uk_UA/LC_MESSAGES/messages.po,sha256=QPUVFhhVL4HzNvWC_bK3LCNkKNH-KdpuIAH8NrMOxOY,7215
+indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.mo,sha256=JD2pgR-aXYjcD7Lt-PEg5OCLy7d5kRfs1LkyhrPpDU8,3371
+indico_livesync/translations/zh_Hans_CN/LC_MESSAGES/messages.po,sha256=OK1OYn6EZQkvIfimPO2iw1qfWliXRgk6mRJGdvpmubg,5821
+indico_plugin_livesync-3.2.1.dist-info/METADATA,sha256=nNp9wQlgsuUOOEtQHls7COGUbAP5pufT0yafa9RIo6c,1245
+indico_plugin_livesync-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_livesync-3.2.1.dist-info/entry_points.txt,sha256=XHlJdTWaSOpzutIS9U4olLQhzuZ3Z74tUZCABwmNRbs,66
+indico_plugin_livesync-3.2.1.dist-info/top_level.txt,sha256=0Inu0Xuoe4LDl-DGNO1r6XdC6k7b0We7rBE-kNze7iI,16
+indico_plugin_livesync-3.2.1.dist-info/RECORD,,
```

