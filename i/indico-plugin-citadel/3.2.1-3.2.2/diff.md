# Comparing `tmp/indico_plugin_citadel-3.2.1-py3-none-any.whl.zip` & `tmp/indico_plugin_citadel-3.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,45 @@
-Zip file size: 77105 bytes, number of entries: 41
--rw-r--r--  2.0 unx      327 b- defN 23-Jan-08 16:35 indico_citadel/__init__.py
--rw-r--r--  2.0 unx    17661 b- defN 23-May-02 13:41 indico_citadel/backend.py
--rw-r--r--  2.0 unx     2691 b- defN 23-Jan-08 16:35 indico_citadel/cli.py
--rw-r--r--  2.0 unx     4964 b- defN 23-Apr-06 08:37 indico_citadel/plugin.py
--rw-r--r--  2.0 unx     3366 b- defN 23-Jan-08 16:35 indico_citadel/result_schemas.py
--rw-r--r--  2.0 unx     5968 b- defN 23-Jan-08 16:35 indico_citadel/result_schemas_test.py
--rw-r--r--  2.0 unx     9019 b- defN 23-Jan-08 16:35 indico_citadel/schemas.py
--rw-r--r--  2.0 unx    17756 b- defN 23-Jan-08 16:35 indico_citadel/schemas_test.py
--rw-r--r--  2.0 unx     5019 b- defN 23-May-02 13:41 indico_citadel/search.py
--rw-r--r--  2.0 unx     7410 b- defN 23-Apr-03 11:35 indico_citadel/util.py
--rw-r--r--  2.0 unx    10981 b- defN 23-Jan-08 16:35 indico_citadel/util_test.py
+Zip file size: 82085 bytes, number of entries: 43
+-rw-r--r--  2.0 unx      327 b- defN 23-Jun-01 10:35 indico_citadel/__init__.py
+-rw-r--r--  2.0 unx    17661 b- defN 23-Jun-01 10:35 indico_citadel/backend.py
+-rw-r--r--  2.0 unx     2691 b- defN 23-Jun-01 10:35 indico_citadel/cli.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-Jun-01 10:35 indico_citadel/plugin.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-Jun-01 10:35 indico_citadel/result_schemas.py
+-rw-r--r--  2.0 unx     5968 b- defN 23-Jun-01 10:35 indico_citadel/result_schemas_test.py
+-rw-r--r--  2.0 unx     9019 b- defN 23-Jun-01 10:35 indico_citadel/schemas.py
+-rw-r--r--  2.0 unx    17756 b- defN 23-Jun-01 10:35 indico_citadel/schemas_test.py
+-rw-r--r--  2.0 unx     5019 b- defN 23-Jun-01 10:35 indico_citadel/search.py
+-rw-r--r--  2.0 unx     7410 b- defN 23-Jun-01 10:35 indico_citadel/util.py
+-rw-r--r--  2.0 unx    10981 b- defN 23-Jun-01 10:35 indico_citadel/util_test.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-07 14:48 indico_citadel/migrations/.no-headers
 -rw-r--r--  2.0 unx     3027 b- defN 21-May-07 14:48 indico_citadel/migrations/20210330_1742_0cf18be7ade1_add_mapping_table.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-07 14:48 indico_citadel/models/__init__.py
--rw-r--r--  2.0 unx     5827 b- defN 23-Jan-08 16:35 indico_citadel/models/id_map.py
+-rw-r--r--  2.0 unx     5828 b- defN 23-Jul-05 15:04 indico_citadel/models/id_map.py
 -rw-r--r--  2.0 unx     4191 b- defN 22-Aug-24 10:11 indico_citadel/translations/messages.pot
--rw-r--r--  2.0 unx     4572 b- defN 22-Aug-24 21:47 indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6413 b- defN 22-Aug-24 21:58 indico_citadel/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx      511 b- defN 22-Aug-24 21:47 indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     4274 b- defN 22-Aug-24 21:58 indico_citadel/translations/en_GB/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4704 b- defN 22-Aug-24 21:47 indico_citadel/translations/es_ES/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6361 b- defN 22-Aug-24 21:58 indico_citadel/translations/es_ES/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4979 b- defN 22-Aug-24 21:47 indico_citadel/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6644 b- defN 22-Aug-24 21:58 indico_citadel/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     5717 b- defN 22-Aug-24 21:47 indico_citadel/translations/mn_MN/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     7360 b- defN 22-Aug-24 21:58 indico_citadel/translations/mn_MN/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4775 b- defN 22-Aug-24 21:47 indico_citadel/translations/pl_PL/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6467 b- defN 22-Aug-24 21:58 indico_citadel/translations/pl_PL/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4688 b- defN 22-Aug-24 21:47 indico_citadel/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6348 b- defN 22-Aug-24 21:58 indico_citadel/translations/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4679 b- defN 22-Aug-24 21:47 indico_citadel/translations/tr_TR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     6335 b- defN 22-Aug-24 21:58 indico_citadel/translations/tr_TR/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     6226 b- defN 22-Aug-24 21:47 indico_citadel/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     7898 b- defN 22-Aug-24 21:58 indico_citadel/translations/uk_UA/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     4115 b- defN 22-Aug-24 21:47 indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx     5729 b- defN 21-Jul-09 11:16 indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--  2.0 unx     1170 b- defN 23-May-26 14:32 indico_plugin_citadel-3.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:32 indico_plugin_citadel-3.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-May-26 14:32 indico_plugin_citadel-3.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-May-26 14:32 indico_plugin_citadel-3.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4167 b- defN 23-May-26 14:32 indico_plugin_citadel-3.2.1.dist-info/RECORD
-41 files, 212509 bytes uncompressed, 70177 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     4603 b- defN 23-Jul-11 13:08 indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6318 b- defN 23-Jul-14 16:17 indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4572 b- defN 23-Jul-11 13:07 indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6412 b- defN 23-Jul-14 16:17 indico_citadel/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx      511 b- defN 23-Jul-11 13:08 indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     4274 b- defN 23-Jul-14 16:17 indico_citadel/translations/en_GB/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4704 b- defN 23-Jul-11 13:08 indico_citadel/translations/es_ES/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6361 b- defN 23-Jul-14 16:17 indico_citadel/translations/es_ES/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4960 b- defN 23-Jul-11 13:08 indico_citadel/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6622 b- defN 23-Jul-14 16:17 indico_citadel/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     5717 b- defN 23-Jul-11 13:08 indico_citadel/translations/mn_MN/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     7360 b- defN 23-Jul-14 16:17 indico_citadel/translations/mn_MN/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4775 b- defN 23-Jul-11 13:08 indico_citadel/translations/pl_PL/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6467 b- defN 23-Jul-14 16:17 indico_citadel/translations/pl_PL/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4688 b- defN 23-Jul-11 13:08 indico_citadel/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6348 b- defN 23-Jul-14 16:17 indico_citadel/translations/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4679 b- defN 23-Jul-11 13:08 indico_citadel/translations/tr_TR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     6335 b- defN 23-Jul-14 16:17 indico_citadel/translations/tr_TR/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     6226 b- defN 23-Jul-11 13:08 indico_citadel/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     7898 b- defN 23-Jul-14 16:17 indico_citadel/translations/uk_UA/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     4115 b- defN 23-Jul-11 13:08 indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx     5728 b- defN 23-Jul-14 16:17 indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--  2.0 unx     1286 b- defN 23-Jul-20 19:35 indico_plugin_citadel-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:35 indico_plugin_citadel-3.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-20 19:35 indico_plugin_citadel-3.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-20 19:35 indico_plugin_citadel-3.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4395 b- defN 23-Jul-20 19:35 indico_plugin_citadel-3.2.2.dist-info/RECORD
+43 files, 223732 bytes uncompressed, 74777 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -42,14 +42,20 @@
 
 Filename: indico_citadel/models/id_map.py
 Comment: 
 
 Filename: indico_citadel/translations/messages.pot
 Comment: 
 
+Filename: indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.mo
+Comment: 
+
+Filename: indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.po
+Comment: 
+
 Filename: indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: indico_citadel/translations/de_DE/LC_MESSAGES/messages.po
 Comment: 
 
 Filename: indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo
@@ -102,23 +108,23 @@
 
 Filename: indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po
 Comment: 
 
-Filename: indico_plugin_citadel-3.2.1.dist-info/METADATA
+Filename: indico_plugin_citadel-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_citadel-3.2.1.dist-info/WHEEL
+Filename: indico_plugin_citadel-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_citadel-3.2.1.dist-info/entry_points.txt
+Filename: indico_plugin_citadel-3.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_citadel-3.2.1.dist-info/top_level.txt
+Filename: indico_plugin_citadel-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_citadel-3.2.1.dist-info/RECORD
+Filename: indico_plugin_citadel-3.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_citadel/models/id_map.py

```diff
@@ -8,19 +8,19 @@
 from indico.core.db import db
 from indico.core.db.sqlalchemy import PyIntEnum
 from indico.modules.attachments import Attachment
 from indico.modules.events import Event
 from indico.modules.events.contributions import Contribution
 from indico.modules.events.contributions.models.subcontributions import SubContribution
 from indico.modules.events.notes.models.notes import EventNote
-from indico.util.enum import IndicoEnum
+from indico.util.enum import IndicoIntEnum
 from indico.util.string import format_repr
 
 
-class EntryType(int, IndicoEnum):
+class EntryType(IndicoIntEnum):
     event = 1
     contribution = 2
     subcontribution = 3
     attachment = 4
     note = 5
```

## indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-06-09 14:18+0200\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Dirk Hoffmann <Hoffmann@cppm.in2p3.fr>, 2022\n"
 "Language: de_DE\n"
-"Language-Team: German (Germany) (https://www.transifex.com/indico/teams/6478/"
+"Language-Team: German (Germany) (https://app.transifex.com/indico/teams/6478/"
 "de_DE/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Einer Veranstaltung zugeordneter Schlüsselbegriff"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr ""
 "Institut oder Arbeitgeber eines Sprechers, Authors oder Veranstaltungsleiters"
```

## indico_citadel/translations/de_DE/LC_MESSAGES/messages.po

```diff
@@ -1,206 +1,206 @@
 # Translations template for PROJECT.
-# Copyright (C) 2021 ORGANIZATION
+# Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2022
 # Pedro Ferreira <pedro.ferreira@cern.ch>, 2022
 # HRZ SHK <indico1@uni-bonn.de>, 2022
 # Damian Bucher <bucher@uni-muenster.de>, 2022
 # Dirk Hoffmann <Hoffmann@cppm.in2p3.fr>, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-06-09 14:18+0200\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Dirk Hoffmann <Hoffmann@cppm.in2p3.fr>, 2022\n"
-"Language-Team: German (Germany) (https://www.transifex.com/indico/teams/6478/de_DE/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/indico/teams/6478/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.3\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: indico_citadel/plugin.py:25
+#: indico_citadel/plugin.py:24
 msgid "Citadel URL"
 msgstr "Citadel-URL"
 
-#: indico_citadel/plugin.py:26
+#: indico_citadel/plugin.py:25
 msgid "The URL of the Citadel server"
 msgstr "URL des Citadel-Servers"
 
-#: indico_citadel/plugin.py:27
+#: indico_citadel/plugin.py:26
 msgid "Citadel API token"
 msgstr "Citadel API Token"
 
-#: indico_citadel/plugin.py:28
+#: indico_citadel/plugin.py:27
 msgid "The authentication token to access Citadel"
 msgstr "Authentifizierungstoken für Citadel-Zugriff"
 
-#: indico_citadel/plugin.py:29
+#: indico_citadel/plugin.py:28
 msgid "File extensions"
 msgstr "Dateiendungen"
 
-#: indico_citadel/plugin.py:30
+#: indico_citadel/plugin.py:29
 msgid "File extensions to upload for full-text search"
 msgstr "Dateierweiterung zum Hochladen für Volltextsuche"
 
-#: indico_citadel/plugin.py:31
+#: indico_citadel/plugin.py:30
 msgid "Max. file size"
 msgstr "max. Dateigröße"
 
-#: indico_citadel/plugin.py:33
+#: indico_citadel/plugin.py:32
 msgid ""
 "Maximum size (in MB) to upload for full-text search. Note that increasing "
 "this after the initial export will upload all files for indexing that have "
 "not been uploaded before during the next queue run, which may take a long "
 "time on larger instances. You may want to run a manual upload for the new "
 "file size first!"
 msgstr ""
 "Maximale Dateigröße (in MB) zum Hochladen für Volltextsuche. Bitte beachten,"
 " dass eine Erhöhung dieses Werts nach den ersten Herunterladen dazu führt, "
 "dass alle Dateien, die nicht vor zum Indizieren hochgeladen worden sind, "
 "beim nächsten Durchgang hochgeladen werden. Das kann zu großen Verzögerungen"
 " auf größeren Systemen führen. Ein erstmaliges manuelles Hochladen für die "
 "neue Dateigröße wird empfohlen!"
 
-#: indico_citadel/plugin.py:38
+#: indico_citadel/plugin.py:37
 msgid "Parallel threads (records)"
 msgstr "Parallele Prozesse (Einträge)"
 
-#: indico_citadel/plugin.py:39
+#: indico_citadel/plugin.py:38
 msgid "Number of threads to use when uploading records."
 msgstr "Anzahl Prozesse beim Hochladen von Einträgen."
 
-#: indico_citadel/plugin.py:40
+#: indico_citadel/plugin.py:39
 msgid "Parallel threads (records, initial export)"
 msgstr "Parallele Prozesse (Einträge, Erstexport)"
 
-#: indico_citadel/plugin.py:42
+#: indico_citadel/plugin.py:41
 msgid ""
 "Number of threads to use when uploading records during the initial export."
 msgstr "Anzahl beim ersten Herunterladen benutzter Prozesse "
 
-#: indico_citadel/plugin.py:44
+#: indico_citadel/plugin.py:43
 msgid "Parallel threads (files)"
 msgstr "Parallele Prozesse (Dateien)"
 
-#: indico_citadel/plugin.py:45
+#: indico_citadel/plugin.py:44
 msgid "Number of threads to use when uploading files."
 msgstr "Anzahl Prozesse beim Hochladen der Dateien."
 
-#: indico_citadel/plugin.py:46
+#: indico_citadel/plugin.py:45
 msgid "Parallel threads (files, initial export)"
 msgstr "Parallele Prozesse (Dateien, Erstexport)"
 
-#: indico_citadel/plugin.py:48
+#: indico_citadel/plugin.py:47
 msgid ""
 "Number of threads to use when uploading files during the initial export."
 msgstr "Anzahl Prozesse beim Hochladen der Dateien beim Erstexport."
 
-#: indico_citadel/plugin.py:50
+#: indico_citadel/plugin.py:49
 msgid "Disable search"
 msgstr "Suche abschalten"
 
-#: indico_citadel/plugin.py:51
+#: indico_citadel/plugin.py:50
 msgid ""
 "This disables the search integration of the plugin. When this option is "
 "used, the internal Indico search interface will be used. This may be useful "
 "when you are still running a larger initial export and do not want people to"
 " get incomplete search results during that time."
 msgstr ""
 "Hierdurch wird die Suchfunktion des Plugins abgeschaltet. Bei Benutzung "
 "dieser Option wird stattdessen die interne Suchfunktion von Indico "
 "verwendet. Das kann sinnvoll sein, falls ein längerer Export läuft und die "
 "Benutzer währenddessen keine unvollständigen Ergebnisse sehen sollen."
 
-#: indico_citadel/search.py:95
+#: indico_citadel/search.py:92
 msgid "The title of an event, contribution, etc."
 msgstr "Titel einer Veranstaltung, eines Beitrags usw."
 
-#: indico_citadel/search.py:95
+#: indico_citadel/search.py:93
 msgid "A speaker, author or event chair's name"
 msgstr "Name eines Sprechers, Authors oder Veranstaltungsleiters"
 
-#: indico_citadel/search.py:96
+#: indico_citadel/search.py:94
 msgid "A speaker, author or event chair's affiliation"
 msgstr ""
 "Institut oder Arbeitgeber eines Sprechers, Authors oder "
 "Veranstaltungsleiters"
 
-#: indico_citadel/search.py:97
+#: indico_citadel/search.py:95
 msgid "An entry type (such as conference, meeting, file, etc.)"
 msgstr "Art des Eintrags (Konferenz, Besprechung, Datei usw.)"
 
-#: indico_citadel/search.py:98
+#: indico_citadel/search.py:96
 msgid "Name of the venue"
 msgstr "Name des Veranstaltungsortes"
 
-#: indico_citadel/search.py:99
+#: indico_citadel/search.py:97
 msgid "Name of the room"
 msgstr "Name des Raumes"
 
-#: indico_citadel/search.py:100
+#: indico_citadel/search.py:98
 msgid "Address of the venue"
 msgstr "Adresse des Veransaltungsortes"
 
-#: indico_citadel/search.py:101
+#: indico_citadel/search.py:99
 msgid "Name of the attached file"
 msgstr "Name der angehängten Datei"
 
-#: indico_citadel/search.py:102
+#: indico_citadel/search.py:100
 msgid "A keyword associated with an event"
 msgstr "Einer Veranstaltung zugeordneter Schlüsselbegriff"
 
-#: indico_citadel/search.py:103
+#: indico_citadel/search.py:101
 msgid "The category of an event"
 msgstr "Kategorie einer Veranstaltung"
 
-#: indico_citadel/search.py:111
+#: indico_citadel/search.py:109
 msgid "Most relevant"
 msgstr "Relevanteste"
 
-#: indico_citadel/search.py:112
+#: indico_citadel/search.py:110
 msgid "Newest first"
 msgstr "Neueste Einträge zuerst"
 
-#: indico_citadel/search.py:113
+#: indico_citadel/search.py:111
 msgid "Oldest first"
 msgstr "Älteste Einträge zuerst"
 
-#: indico_citadel/search.py:117
+#: indico_citadel/search.py:115
 msgid "Affiliation"
 msgstr "Arbeitgeber oder Institut"
 
-#: indico_citadel/search.py:118
+#: indico_citadel/search.py:116
 msgid "Person"
 msgstr "Person"
 
-#: indico_citadel/search.py:119
+#: indico_citadel/search.py:117
 msgid "Type"
 msgstr "Typ"
 
-#: indico_citadel/search.py:120
+#: indico_citadel/search.py:118
 msgid "Location"
 msgstr "Ort"
 
-#: indico_citadel/search.py:121
+#: indico_citadel/search.py:119
 msgid "Date"
 msgstr "Datum"
 
-#: indico_citadel/search.py:122
+#: indico_citadel/search.py:120
 msgid "Category"
 msgstr "Kategorie"
 
-#: indico_citadel/search.py:123
+#: indico_citadel/search.py:121
 msgid "Category ID"
 msgstr "Kategorie-ID"
 
-#: indico_citadel/search.py:124
+#: indico_citadel/search.py:122
 msgid "Event ID"
 msgstr "Veranstaltungs-ID"
```

## indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: PROJECT VERSION*

```diff
@@ -13,20 +13,20 @@
 000000c0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000d0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000e0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
 000000f0: 0a4c 616e 6775 6167 653a 2065 6e5f 4742  .Language: en_GB
 00000100: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000110: 456e 676c 6973 6820 2855 6e69 7465 6420  English (United 
 00000120: 4b69 6e67 646f 6d29 2028 6874 7470 733a  Kingdom) (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
 00000140: 636f 6d2f 696e 6469 636f 2f74 6561 6d73  com/indico/teams
 00000150: 2f36 3437 382f 656e 5f47 422f 290a 506c  /6478/en_GB/).Pl
 00000160: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
 00000170: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
 00000180: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 00000190: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001a0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 000001b0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 000001c0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 000001d0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 000001e0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-000001f0: 2042 6162 656c 2032 2e31 302e 330a 00     Babel 2.10.3..
+000001f0: 2042 6162 656c 2032 2e31 322e 310a 00     Babel 2.12.1..
```

## indico_citadel/translations/en_GB/LC_MESSAGES/messages.po

```diff
@@ -6,15 +6,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
-"Language-Team: English (United Kingdom) (https://www.transifex.com/indico/teams/6478/en_GB/)\n"
+"Language-Team: English (United Kingdom) (https://app.transifex.com/indico/teams/6478/en_GB/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: en_GB\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

## indico_citadel/translations/es_ES/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,22 +2,22 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
 "Language: es_ES\n"
-"Language-Team: Spanish (Spain) (https://www.transifex.com/indico/teams/6478/"
+"Language-Team: Spanish (Spain) (https://app.transifex.com/indico/teams/6478/"
 "es_ES/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Una palabra clave asociada a un evento."
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Afiliación de un orador, autor o presidente del evento."
```

## indico_citadel/translations/es_ES/LC_MESSAGES/messages.po

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
-"Language-Team: Spanish (Spain) (https://www.transifex.com/indico/teams/6478/es_ES/)\n"
+"Language-Team: Spanish (Spain) (https://app.transifex.com/indico/teams/6478/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

## indico_citadel/translations/fr_FR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
-"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2021\n"
+"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2023\n"
 "Language: fr_FR\n"
-"Language-Team: French (France) (https://www.transifex.com/indico/teams/6478/"
+"Language-Team: French (France) (https://app.transifex.com/indico/teams/6478/"
 "fr_FR/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Un mot-clé associé à un événement"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "L'affiliation d'un orateur, auteur ou responsable d'événement"
 
@@ -54,36 +54,36 @@
 msgid "Event ID"
 msgstr "L'identifiant de l'événement"
 
 msgid "File extensions"
 msgstr "Extensions de fichier"
 
 msgid "File extensions to upload for full-text search"
-msgstr "Extension de fichier à télécharger pour la recherche en texte intégral"
+msgstr "Extension de fichier à télédéposer pour la recherche en texte intégral"
 
 msgid "Location"
 msgstr "Site"
 
 msgid "Max. file size"
 msgstr "Taille maximale de fichier"
 
 msgid ""
 "Maximum size (in MB) to upload for full-text search. Note that increasing "
 "this after the initial export will upload all files for indexing that have "
 "not been uploaded before during the next queue run, which may take a long "
 "time on larger instances. You may want to run a manual upload for the new "
 "file size first!"
 msgstr ""
-"Taille maximale (en MB) du téléchargement pour la recherche en texte "
-"intégral. Veuillez noter que l'augmentation de ce paramètre après l'export "
-"initial résultera dans le téléchargement de tous les fichiers qui n'ont pas "
-"encore été téléchargés pour indexation à la prochaine exécution de la file "
-"d'attente, ce qui pourrait prendre du temps sur les serveurs les plus "
-"importants. Vous voudrez peut-être d'abord exécuter un téléchargement manuel "
-"pour la nouvelle taille de fichier!"
+"Taille maximale (en MB) du télédépôt pour la recherche en texte intégral. "
+"Veuillez noter que l'augmentation de ce paramètre après l'export initial "
+"résultera dans le télédépôt de tous les fichiers qui n'ont pas encore été "
+"télédéposés pour indexation à la prochaine exécution de la file d'attente, "
+"ce qui pourrait prendre du temps sur les serveurs les plus importants. Vous "
+"voudrez peut-être d'abord exécuter un télédépôt manuel pour la nouvelle "
+"taille de fichier!"
 
 msgid "Most relevant"
 msgstr "Les plus pertinents"
 
 msgid "Name of the attached file"
 msgstr "Nom du fichier attaché"
 
@@ -95,29 +95,28 @@
 
 msgid "Newest first"
 msgstr "Les plus récents en premier"
 
 msgid ""
 "Number of threads to use when uploading files during the initial export."
 msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des fichiers pour "
+"Nombre de processus à utiliser lors du télédépôt des fichiers pour "
 "l'exportation initiale."
 
 msgid "Number of threads to use when uploading files."
-msgstr "Nombre de processus à utiliser lors du téléchargement des fichiers."
+msgstr "Nombre de processus à utiliser lors du télédépôt des fichiers."
 
 msgid ""
 "Number of threads to use when uploading records during the initial export."
 msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des fichiers pour "
+"Nombre de processus à utiliser lors du télédépôt des fichiers pour "
 "l'exportation initiale."
 
 msgid "Number of threads to use when uploading records."
-msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des enregistrements."
+msgstr "Nombre de processus à utiliser lors du télédépôt des enregistrements."
 
 msgid "Oldest first"
 msgstr "Les plus anciens en premier"
 
 msgid "Parallel threads (files)"
 msgstr "Processus parallèles (fichiers)"
```

## indico_citadel/translations/fr_FR/LC_MESSAGES/messages.po

```diff
@@ -1,24 +1,24 @@
 # Translations template for PROJECT.
 # Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Thomas Baron <thomas.baron@cern.ch>, 2021
+# Thomas Baron <thomas.baron@cern.ch>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
-"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2021\n"
-"Language-Team: French (France) (https://www.transifex.com/indico/teams/6478/fr_FR/)\n"
+"Last-Translator: Thomas Baron <thomas.baron@cern.ch>, 2023\n"
+"Language-Team: French (France) (https://app.transifex.com/indico/teams/6478/fr_FR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr_FR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -41,73 +41,72 @@
 #: indico_citadel/plugin.py:28
 msgid "File extensions"
 msgstr "Extensions de fichier"
 
 #: indico_citadel/plugin.py:29
 msgid "File extensions to upload for full-text search"
 msgstr ""
-"Extension de fichier à télécharger pour la recherche en texte intégral"
+"Extension de fichier à télédéposer pour la recherche en texte intégral"
 
 #: indico_citadel/plugin.py:30
 msgid "Max. file size"
 msgstr "Taille maximale de fichier"
 
 #: indico_citadel/plugin.py:32
 msgid ""
 "Maximum size (in MB) to upload for full-text search. Note that increasing "
 "this after the initial export will upload all files for indexing that have "
 "not been uploaded before during the next queue run, which may take a long "
 "time on larger instances. You may want to run a manual upload for the new "
 "file size first!"
 msgstr ""
-"Taille maximale (en MB) du téléchargement pour la recherche en texte "
-"intégral. Veuillez noter que l'augmentation de ce paramètre après l'export "
-"initial résultera dans le téléchargement de tous les fichiers qui n'ont pas "
-"encore été téléchargés pour indexation à la prochaine exécution de la file "
-"d'attente, ce qui pourrait prendre du temps sur les serveurs les plus "
-"importants. Vous voudrez peut-être d'abord exécuter un téléchargement manuel"
-" pour la nouvelle taille de fichier!"
+"Taille maximale (en MB) du télédépôt pour la recherche en texte intégral. "
+"Veuillez noter que l'augmentation de ce paramètre après l'export initial "
+"résultera dans le télédépôt de tous les fichiers qui n'ont pas encore été "
+"télédéposés pour indexation à la prochaine exécution de la file d'attente, "
+"ce qui pourrait prendre du temps sur les serveurs les plus importants. Vous "
+"voudrez peut-être d'abord exécuter un télédépôt manuel pour la nouvelle "
+"taille de fichier!"
 
 #: indico_citadel/plugin.py:37
 msgid "Parallel threads (records)"
 msgstr "Processus parallèles (enregistrements)"
 
 #: indico_citadel/plugin.py:38
 msgid "Number of threads to use when uploading records."
-msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des enregistrements."
+msgstr "Nombre de processus à utiliser lors du télédépôt des enregistrements."
 
 #: indico_citadel/plugin.py:39
 msgid "Parallel threads (records, initial export)"
 msgstr "Processus parallèles (enregistrements, export initial)"
 
 #: indico_citadel/plugin.py:41
 msgid ""
 "Number of threads to use when uploading records during the initial export."
 msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des fichiers pour "
+"Nombre de processus à utiliser lors du télédépôt des fichiers pour "
 "l'exportation initiale."
 
 #: indico_citadel/plugin.py:43
 msgid "Parallel threads (files)"
 msgstr "Processus parallèles (fichiers)"
 
 #: indico_citadel/plugin.py:44
 msgid "Number of threads to use when uploading files."
-msgstr "Nombre de processus à utiliser lors du téléchargement des fichiers."
+msgstr "Nombre de processus à utiliser lors du télédépôt des fichiers."
 
 #: indico_citadel/plugin.py:45
 msgid "Parallel threads (files, initial export)"
 msgstr "Processus parallèles (fichiers, export initial)"
 
 #: indico_citadel/plugin.py:47
 msgid ""
 "Number of threads to use when uploading files during the initial export."
 msgstr ""
-"Nombre de processus à utiliser lors du téléchargement des fichiers pour "
+"Nombre de processus à utiliser lors du télédépôt des fichiers pour "
 "l'exportation initiale."
 
 #: indico_citadel/plugin.py:49
 msgid "Disable search"
 msgstr "Désactiver la recherche"
 
 #: indico_citadel/plugin.py:50
```

## indico_citadel/translations/mn_MN/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Batbayar Bat-Erdene <yertonts@gmail.com>, 2021\n"
 "Language: mn_MN\n"
-"Language-Team: Mongolian (Mongolia) (https://www.transifex.com/indico/"
+"Language-Team: Mongolian (Mongolia) (https://app.transifex.com/indico/"
 "teams/6478/mn_MN/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Энэхүү үйл явдалтай холбоотой түлхүүр үг"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Илтгэгч, зохиогч, үйл явдлын удирдагчийн харьяалал"
```

## indico_citadel/translations/mn_MN/LC_MESSAGES/messages.po

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Batbayar Bat-Erdene <yertonts@gmail.com>, 2021\n"
-"Language-Team: Mongolian (Mongolia) (https://www.transifex.com/indico/teams/6478/mn_MN/)\n"
+"Language-Team: Mongolian (Mongolia) (https://app.transifex.com/indico/teams/6478/mn_MN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: mn_MN\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

## indico_citadel/translations/pl_PL/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,23 +2,23 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Marcin Miłek, 2021\n"
 "Language: pl_PL\n"
-"Language-Team: Polish (Poland) (https://www.transifex.com/indico/teams/6478/"
+"Language-Team: Polish (Poland) (https://app.transifex.com/indico/teams/6478/"
 "pl_PL/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Słowo kluczowe powiązane z wydarzeniem"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Afiliacja prelegenta, autora lub przewodniczącego wydarzenia"
```

## indico_citadel/translations/pl_PL/LC_MESSAGES/messages.po

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Marcin Miłek, 2021\n"
-"Language-Team: Polish (Poland) (https://www.transifex.com/indico/teams/6478/pl_PL/)\n"
+"Language-Team: Polish (Poland) (https://app.transifex.com/indico/teams/6478/pl_PL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl_PL\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

## indico_citadel/translations/pt_BR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,22 +2,22 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Sedir G. Morais <philippi.sedir@gmail.com>, 2021\n"
 "Language: pt_BR\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/indico/"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/indico/"
 "teams/6478/pt_BR/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Uma palavra-chave associada com um evento"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Afiliação de um palestrante, autor ou coordenador de evento"
```

## indico_citadel/translations/pt_BR/LC_MESSAGES/messages.po

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Sedir G. Morais <philippi.sedir@gmail.com>, 2021\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/indico/teams/6478/pt_BR/)\n"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/indico/teams/6478/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

## indico_citadel/translations/tr_TR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021\n"
 "Language: tr_TR\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/indico/teams/6478/"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/indico/teams/6478/"
 "tr_TR/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Bir etkinlikle ilişkili bir anahtar kelime"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Konuşmacı, yazar veya etkinlik başkanının kurumu"
```

## indico_citadel/translations/tr_TR/LC_MESSAGES/messages.po

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: selcuk bilmis <selcukbilmis@gmail.com>, 2021\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/indico/teams/6478/tr_TR/)\n"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/indico/teams/6478/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

## indico_citadel/translations/uk_UA/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -2,24 +2,24 @@
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2021\n"
 "Language: uk_UA\n"
-"Language-Team: Ukrainian (Ukraine) (https://www.transifex.com/indico/"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/indico/"
 "teams/6478/uk_UA/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "Ключові слова пов'язані з цим заходом"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "Приналежність спікера, автора або керівника події "
```

## indico_citadel/translations/uk_UA/LC_MESSAGES/messages.po

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Andrii Verbytskyi <andrii.verbytskyi@mpp.mpg.de>, 2021\n"
-"Language-Team: Ukrainian (Ukraine) (https://www.transifex.com/indico/teams/6478/uk_UA/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/indico/teams/6478/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
```

## indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-06-09 14:18+0200\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Lanxin Ma <ma@ihep.ac.cn>, 2021\n"
 "Language: zh_CN.GB2312\n"
-"Language-Team: Chinese (China) (GB2312) (https://www.transifex.com/indico/"
+"Language-Team: Chinese (China) (GB2312) (https://app.transifex.com/indico/"
 "teams/6478/zh_CN.GB2312/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "A keyword associated with an event"
 msgstr "与事件关联的关键字"
 
 msgid "A speaker, author or event chair's affiliation"
 msgstr "报告人、作者或事件主席的工作单位"
```

## indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po

```diff
@@ -1,194 +1,194 @@
 # Translations template for PROJECT.
-# Copyright (C) 2021 ORGANIZATION
+# Copyright (C) 2022 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Lanxin Ma <ma@ihep.ac.cn>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-06-09 14:18+0200\n"
+"POT-Creation-Date: 2022-08-24 12:05+0200\n"
 "PO-Revision-Date: 2021-05-26 16:26+0000\n"
 "Last-Translator: Lanxin Ma <ma@ihep.ac.cn>, 2021\n"
-"Language-Team: Chinese (China) (GB2312) (https://www.transifex.com/indico/teams/6478/zh_CN.GB2312/)\n"
+"Language-Team: Chinese (China) (GB2312) (https://app.transifex.com/indico/teams/6478/zh_CN.GB2312/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.3\n"
 "Language: zh_CN.GB2312\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: indico_citadel/plugin.py:25
+#: indico_citadel/plugin.py:24
 msgid "Citadel URL"
 msgstr "Citadel URL"
 
-#: indico_citadel/plugin.py:26
+#: indico_citadel/plugin.py:25
 msgid "The URL of the Citadel server"
 msgstr " Citadel 服务 URL "
 
-#: indico_citadel/plugin.py:27
+#: indico_citadel/plugin.py:26
 msgid "Citadel API token"
 msgstr "Citadel API 令牌"
 
-#: indico_citadel/plugin.py:28
+#: indico_citadel/plugin.py:27
 msgid "The authentication token to access Citadel"
 msgstr "访问 Citadel 的身份验证令牌"
 
-#: indico_citadel/plugin.py:29
+#: indico_citadel/plugin.py:28
 msgid "File extensions"
 msgstr "文件扩展名"
 
-#: indico_citadel/plugin.py:30
+#: indico_citadel/plugin.py:29
 msgid "File extensions to upload for full-text search"
 msgstr "为全文搜索上传的文件扩展名"
 
-#: indico_citadel/plugin.py:31
+#: indico_citadel/plugin.py:30
 msgid "Max. file size"
 msgstr "最大文件大小"
 
-#: indico_citadel/plugin.py:33
+#: indico_citadel/plugin.py:32
 msgid ""
 "Maximum size (in MB) to upload for full-text search. Note that increasing "
 "this after the initial export will upload all files for indexing that have "
 "not been uploaded before during the next queue run, which may take a long "
 "time on larger instances. You may want to run a manual upload for the new "
 "file size first!"
 msgstr ""
 "为全文搜索上传的最大大小（以 MB "
 "为单位）。请注意，初始导出后增加此值将上传在下一次队列运行期间之前未上传的所有文件用于索引，这在较大的实例上可能需要很长时间。您可能需要先手动上传新文件大小！"
 
-#: indico_citadel/plugin.py:38
+#: indico_citadel/plugin.py:37
 msgid "Parallel threads (records)"
 msgstr "并行线程 (记录)"
 
-#: indico_citadel/plugin.py:39
+#: indico_citadel/plugin.py:38
 msgid "Number of threads to use when uploading records."
 msgstr "上传记录时使用的线程数。"
 
-#: indico_citadel/plugin.py:40
+#: indico_citadel/plugin.py:39
 msgid "Parallel threads (records, initial export)"
 msgstr "并行线程 (记录、初始导出)"
 
-#: indico_citadel/plugin.py:42
+#: indico_citadel/plugin.py:41
 msgid ""
 "Number of threads to use when uploading records during the initial export."
 msgstr "在初始导出期间上传记录时使用的线程数。"
 
-#: indico_citadel/plugin.py:44
+#: indico_citadel/plugin.py:43
 msgid "Parallel threads (files)"
 msgstr "并行线程 (文件)"
 
-#: indico_citadel/plugin.py:45
+#: indico_citadel/plugin.py:44
 msgid "Number of threads to use when uploading files."
 msgstr "上传文件时使用的线程数。"
 
-#: indico_citadel/plugin.py:46
+#: indico_citadel/plugin.py:45
 msgid "Parallel threads (files, initial export)"
 msgstr "并行线程 (文件、初始导出)"
 
-#: indico_citadel/plugin.py:48
+#: indico_citadel/plugin.py:47
 msgid ""
 "Number of threads to use when uploading files during the initial export."
 msgstr "在初始导出期间上传文件时使用的线程数。"
 
-#: indico_citadel/plugin.py:50
+#: indico_citadel/plugin.py:49
 msgid "Disable search"
 msgstr "禁用搜索"
 
-#: indico_citadel/plugin.py:51
+#: indico_citadel/plugin.py:50
 msgid ""
 "This disables the search integration of the plugin. When this option is "
 "used, the internal Indico search interface will be used. This may be useful "
 "when you are still running a larger initial export and do not want people to"
 " get incomplete search results during that time."
 msgstr ""
 "这将禁用插件的搜索集成。 使用此选项时，将使用 Indico 内部搜索界面。 "
 "当您仍在运行较大的初始导出并且不希望人们在此期间获得不完整的搜索结果时，这可能很有用。"
 
-#: indico_citadel/search.py:95
+#: indico_citadel/search.py:92
 msgid "The title of an event, contribution, etc."
 msgstr "事件，报告等的标题。"
 
-#: indico_citadel/search.py:95
+#: indico_citadel/search.py:93
 msgid "A speaker, author or event chair's name"
 msgstr "报告人、作者或事件主席的姓名"
 
-#: indico_citadel/search.py:96
+#: indico_citadel/search.py:94
 msgid "A speaker, author or event chair's affiliation"
 msgstr "报告人、作者或事件主席的工作单位"
 
-#: indico_citadel/search.py:97
+#: indico_citadel/search.py:95
 msgid "An entry type (such as conference, meeting, file, etc.)"
 msgstr "条目类型（例如大会、会议、文件等）"
 
-#: indico_citadel/search.py:98
+#: indico_citadel/search.py:96
 msgid "Name of the venue"
 msgstr "会场名称"
 
-#: indico_citadel/search.py:99
+#: indico_citadel/search.py:97
 msgid "Name of the room"
 msgstr "会议室名称"
 
-#: indico_citadel/search.py:100
+#: indico_citadel/search.py:98
 msgid "Address of the venue"
 msgstr "会场地址"
 
-#: indico_citadel/search.py:101
+#: indico_citadel/search.py:99
 msgid "Name of the attached file"
 msgstr "附件名称"
 
-#: indico_citadel/search.py:102
+#: indico_citadel/search.py:100
 msgid "A keyword associated with an event"
 msgstr "与事件关联的关键字"
 
-#: indico_citadel/search.py:103
+#: indico_citadel/search.py:101
 msgid "The category of an event"
 msgstr "事件的类别"
 
-#: indico_citadel/search.py:111
+#: indico_citadel/search.py:109
 msgid "Most relevant"
 msgstr "最相关"
 
-#: indico_citadel/search.py:112
+#: indico_citadel/search.py:110
 msgid "Newest first"
 msgstr "最新优先"
 
-#: indico_citadel/search.py:113
+#: indico_citadel/search.py:111
 msgid "Oldest first"
 msgstr "最老优先"
 
-#: indico_citadel/search.py:117
+#: indico_citadel/search.py:115
 msgid "Affiliation"
 msgstr "工作单位"
 
-#: indico_citadel/search.py:118
+#: indico_citadel/search.py:116
 msgid "Person"
 msgstr "人"
 
-#: indico_citadel/search.py:119
+#: indico_citadel/search.py:117
 msgid "Type"
 msgstr "类型"
 
-#: indico_citadel/search.py:120
+#: indico_citadel/search.py:118
 msgid "Location"
 msgstr "地点"
 
-#: indico_citadel/search.py:121
+#: indico_citadel/search.py:119
 msgid "Date"
 msgstr "日期"
 
-#: indico_citadel/search.py:122
+#: indico_citadel/search.py:120
 msgid "Category"
 msgstr "类别"
 
-#: indico_citadel/search.py:123
+#: indico_citadel/search.py:121
 msgid "Category ID"
 msgstr "类别ID"
 
-#: indico_citadel/search.py:124
+#: indico_citadel/search.py:122
 msgid "Event ID"
 msgstr "事件ID"
```

## Comparing `indico_plugin_citadel-3.2.1.dist-info/METADATA` & `indico_plugin_citadel-3.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: indico-plugin-citadel
-Version: 3.2.1
+Version: 3.2.2
 Summary: Indico search+livesync backend using Citadel+ElasticSearch
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.9.0
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Requires-Dist: indico (>=3.2)
-Requires-Dist: indico-plugin-livesync (>=3.0.dev0)
+Requires-Dist: indico (>=3.2.6)
+Requires-Dist: indico-plugin-livesync (>=3.2.1)
 
 # Citadel Search Plugin
 
 The Citadel plugin integrates Indico with the [Citadel][citadel] microservice
 to provide advanced search functionality using an Elasticsearch backend.
 
 ## Changelog
 
+### 3.2.2
+
+- Adapt to Indico 3.2.6 changes
+- Support Python 3.11
+
 ### 3.2.1
 
 - Stop using deprecated URL utils from werkzeug
 
 ### 3.2
 
 - Update translations
```

## Comparing `indico_plugin_citadel-3.2.1.dist-info/RECORD` & `indico_plugin_citadel-3.2.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 indico_citadel/schemas_test.py,sha256=qShwVPQ012y_zzVVrGetZ7UPnXZ4J4nj34tmxqyedGY,17756
 indico_citadel/search.py,sha256=jiUVgo7YnCgB1IpG2HoggrzCj8JOJ-rKjZO_lL8Y_tM,5019
 indico_citadel/util.py,sha256=kNSgWlBB-003uDeFJLiC1oqYgkf2N_vLK6g1J6hc8d8,7410
 indico_citadel/util_test.py,sha256=5LuKj6bnP6xQCLUqU8_LXowxc2YJGlsFLR9wXLHulkU,10981
 indico_citadel/migrations/.no-headers,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 indico_citadel/migrations/20210330_1742_0cf18be7ade1_add_mapping_table.py,sha256=n7RxKviLjbqPUnK53bVHwJn4Bs5tOr7FOX76AOS4rOI,3027
 indico_citadel/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-indico_citadel/models/id_map.py,sha256=Ybwryv_kQ630eT9mDlFW52e5tsclhQRAeOGOKbA4r2Q,5827
+indico_citadel/models/id_map.py,sha256=83NKiHD8q64KAMB1_F-j0Upsqs8IiJPBE73NS02PcEg,5828
 indico_citadel/translations/messages.pot,sha256=-eT9t710TLumkPtVBvJ014fX0J9tjLbcAe5LaCVj9Oc,4191
-indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo,sha256=UMEvN8yP3HHIMxhWfauwRSO1QwSq5ySWqsPzdEbAyJU,4572
-indico_citadel/translations/de_DE/LC_MESSAGES/messages.po,sha256=w926M1lrsm6tJueV50HM17_3SgVdH52iQsD846ViFwc,6413
-indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo,sha256=VVo1wr9qNVbizE-vNlgkmN9HwKy6JoLsAwUd8z0x8oI,511
-indico_citadel/translations/en_GB/LC_MESSAGES/messages.po,sha256=S1Egtf2taUvrerk1ix2JMHPi947omesSOJEdAn4Wrp8,4274
-indico_citadel/translations/es_ES/LC_MESSAGES/messages.mo,sha256=lNGWwhnDOApOYp1hRLy1vqIEGNoTO_GO-5sBqbHa-BI,4704
-indico_citadel/translations/es_ES/LC_MESSAGES/messages.po,sha256=NnwEQEMZKg_FnqxZzMSAzJ5ZDBSGTO3eR2AMPOAok2I,6361
-indico_citadel/translations/fr_FR/LC_MESSAGES/messages.mo,sha256=N0jgrNkzSoX1REZB0c8-d3YSmoOSoVyK0ptn9FnwQLc,4979
-indico_citadel/translations/fr_FR/LC_MESSAGES/messages.po,sha256=V6A1fsiKQzDLOqWYPRhkBDwM4M3mbkc2-VVMRO-a8ns,6644
-indico_citadel/translations/mn_MN/LC_MESSAGES/messages.mo,sha256=bFGI9iq9akh7RhjhOdj2JYtNPqAhKDe8nMv4AtmTBUk,5717
-indico_citadel/translations/mn_MN/LC_MESSAGES/messages.po,sha256=c4-wO3zVh_g4bosaBVtp2RJcJ60thAXkZF-lKEqTP3k,7360
-indico_citadel/translations/pl_PL/LC_MESSAGES/messages.mo,sha256=wMUs0bhqE5Dil6qdHjZlrJAV2apO-pPj1CJkwVK9Frw,4775
-indico_citadel/translations/pl_PL/LC_MESSAGES/messages.po,sha256=fdeOOGnmmAfGDHlWGA_6NL9qYFu26wPLqemnt5i8r1A,6467
-indico_citadel/translations/pt_BR/LC_MESSAGES/messages.mo,sha256=vwNYQJpqSIk7cwhTPODw9PuVZFoScogbsmmUfuvLgBk,4688
-indico_citadel/translations/pt_BR/LC_MESSAGES/messages.po,sha256=7BLQNyY2Kdyz8OvsoWdn64s04Rk8TBwXtbCF2KuzWrI,6348
-indico_citadel/translations/tr_TR/LC_MESSAGES/messages.mo,sha256=MzF4Ph2q0mx1L0t-Bp4mvexLC2tORAn3crA1saVk1WM,4679
-indico_citadel/translations/tr_TR/LC_MESSAGES/messages.po,sha256=UygyRMIqVcoMYA6rFaLUPT-BwSsZHFQDAPVw5pNfRYM,6335
-indico_citadel/translations/uk_UA/LC_MESSAGES/messages.mo,sha256=FEkI1KbJ32XXsK4ECNsaCqXtnIfK8ag-DQZCh01TIt0,6226
-indico_citadel/translations/uk_UA/LC_MESSAGES/messages.po,sha256=a_EV76dgA3fwSdoRUma95Xaxf-xl6MW3okmOVhafhwo,7898
-indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo,sha256=OKsA0w0PZllEwktgVIQ0tn2bajqMcyofBgaqu6iH1fY,4115
-indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po,sha256=yR_qIwyGuXwQhsoro2y-1RRLL7sXK5aIIsE_s5jTjIo,5729
-indico_plugin_citadel-3.2.1.dist-info/METADATA,sha256=mZZdetJyqKxnc8ui0CaXqhW8qf37B0SjSDAPkRpuA-k,1170
-indico_plugin_citadel-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-indico_plugin_citadel-3.2.1.dist-info/entry_points.txt,sha256=jyIhKm7xnF04s5wp2hrR17q0U3imN2vj0BYOyEwL6fI,63
-indico_plugin_citadel-3.2.1.dist-info/top_level.txt,sha256=-gBQ9pGxnNoejN9Yrr_Lyl35tbysQP1Vvi03IUAbrCA,15
-indico_plugin_citadel-3.2.1.dist-info/RECORD,,
+indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.mo,sha256=pV-aAYj9JmVjTRq0b6m6wNP63uE-gNbDVJaLjrU621E,4603
+indico_citadel/translations/cs_CZ/LC_MESSAGES/messages.po,sha256=VgsJd1stqTTKMbMq1QzeEzz5YcOHuWtRDuoUyDUfxco,6318
+indico_citadel/translations/de_DE/LC_MESSAGES/messages.mo,sha256=Kd53mjPum3fBPrkV70lDijyMwkGQ6jY2F4qtM-pgxlM,4572
+indico_citadel/translations/de_DE/LC_MESSAGES/messages.po,sha256=Nfib92TUY17M4z7qafudm8iOLCpcHrwEe5SRnnGm9Pc,6412
+indico_citadel/translations/en_GB/LC_MESSAGES/messages.mo,sha256=3jVbZZgwALB3tiPleB7DOuXYHtKgfmUqUWxaD3Baogc,511
+indico_citadel/translations/en_GB/LC_MESSAGES/messages.po,sha256=7ir2ZxQKbyF79PvTvhf8PVufpeEpl_f7DFANuTji4Co,4274
+indico_citadel/translations/es_ES/LC_MESSAGES/messages.mo,sha256=-aU-raPfjb0kD7onjZWO76jDHxV6knjoCyGEYX6uzKc,4704
+indico_citadel/translations/es_ES/LC_MESSAGES/messages.po,sha256=Mm-VdoLarxfSouUyQWZK5dyrCuYkq-HlUIMHwFuOFK4,6361
+indico_citadel/translations/fr_FR/LC_MESSAGES/messages.mo,sha256=QB8bmF-EMY9DCmcQE0ljKsyNVhW_kO3UnsXS_51if2Q,4960
+indico_citadel/translations/fr_FR/LC_MESSAGES/messages.po,sha256=W734bi73TTppb6p5BblcD72SEcUiSpgqYegZC-C3pa0,6622
+indico_citadel/translations/mn_MN/LC_MESSAGES/messages.mo,sha256=0Fzqd3G4sn9KQYaPTrPoR-6z9w3JNJAChjzKJARRXq0,5717
+indico_citadel/translations/mn_MN/LC_MESSAGES/messages.po,sha256=VzZz5ofnPyhbDBeKElMjgZAnh9Ffj8yexHp1PgrPSzw,7360
+indico_citadel/translations/pl_PL/LC_MESSAGES/messages.mo,sha256=zkzWbkSbrQwu7LFVX5eqFLouNMrr_h5uT5ri0LHqn6E,4775
+indico_citadel/translations/pl_PL/LC_MESSAGES/messages.po,sha256=SnDwYkOLrp5C-nshcRxDOd3F7h8yYOc0L9xvzddM7xI,6467
+indico_citadel/translations/pt_BR/LC_MESSAGES/messages.mo,sha256=oBR1Mkux7NNrOquYBXAhXrOGpEkOonAxv5UQrWM4-SY,4688
+indico_citadel/translations/pt_BR/LC_MESSAGES/messages.po,sha256=2-OG6Km-xmotcs68voeozs2_sztXIFrKUolWTTr8lC8,6348
+indico_citadel/translations/tr_TR/LC_MESSAGES/messages.mo,sha256=6q5OIpxE77CrgIoF5BQXgHliTeDXj-eQ3N-AzpTgZy4,4679
+indico_citadel/translations/tr_TR/LC_MESSAGES/messages.po,sha256=J-aHtVBxyxD5eDKvuxQTWCETBro2FWFbnO2e566TDBE,6335
+indico_citadel/translations/uk_UA/LC_MESSAGES/messages.mo,sha256=Ff64M-VMeMTkhhQh-FfrMccWjZqhveQNMlD5PuhY7Kg,6226
+indico_citadel/translations/uk_UA/LC_MESSAGES/messages.po,sha256=X0ELnlWiqknzYSm_PTIgCfX3WiZdAbAAiiNMz_SXJnI,7898
+indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.mo,sha256=fkr7zJ5_Ln912KRjhuEsy2xLbzIWLyIliwbwq09hv00,4115
+indico_citadel/translations/zh_Hans_CN/LC_MESSAGES/messages.po,sha256=bOrjYpw0ygO7lEgfwsfd1G2kjUwqz0eFiXebt1xvn9U,5728
+indico_plugin_citadel-3.2.2.dist-info/METADATA,sha256=-u8ctSYBnM4t5cgXIZOZ4mpjyN8FNAe8BmR26vR_0K0,1286
+indico_plugin_citadel-3.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_citadel-3.2.2.dist-info/entry_points.txt,sha256=jyIhKm7xnF04s5wp2hrR17q0U3imN2vj0BYOyEwL6fI,63
+indico_plugin_citadel-3.2.2.dist-info/top_level.txt,sha256=-gBQ9pGxnNoejN9Yrr_Lyl35tbysQP1Vvi03IUAbrCA,15
+indico_plugin_citadel-3.2.2.dist-info/RECORD,,
```

