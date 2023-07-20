# Comparing `tmp/jdDesktopEntryEdit-1.1.tar.gz` & `tmp/jdDesktopEntryEdit-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdDesktopEntryEdit-1.1.tar", last modified: Tue Apr 18 12:31:58 2023, max compression
+gzip compressed data, was "jdDesktopEntryEdit-1.2.tar", last modified: Thu Jul 20 17:17:02 2023, max compression
```

## Comparing `jdDesktopEntryEdit-1.1.tar` & `jdDesktopEntryEdit-1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/
--rw-r--r--   0 root         (0) root         (0)     2060 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35080 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5309 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.257099 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/
--rw-r--r--   0 root         (0) root         (0)     1596 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.ui
--rw-r--r--   0 root         (0) root         (0)     4774 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3792 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Environment.py
--rw-r--r--   0 root         (0) root         (0)     5475 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Functions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Icon.svg
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Languages.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ListEditWidget.py
--rw-r--r--   0 root         (0) root         (0)    29363 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)    21447 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     4812 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2518 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.ui
--rw-r--r--   0 root         (0) root         (0)     1591 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Settings.py
--rw-r--r--   0 root         (0) root         (0)     3481 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.ui
--rw-r--r--   0 root         (0) root         (0)     4044 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.ui
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.ui
--rw-r--r--   0 root         (0) root         (0)      831 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.ui
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/categories.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/changelog.html
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/translators.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/
--rw-r--r--   0 root         (0) root         (0)    43488 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
--rw-r--r--   0 root         (0) root         (0)    43020 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts
--rw-r--r--   0 root         (0) root         (0)        3 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5309 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1558 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:17:02.939546 jdDesktopEntryEdit-1.2/
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35080 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-20 17:17:02.939546 jdDesktopEntryEdit-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:17:02.935546 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditActionDialog.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditActionDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Languages.py
+-rw-r--r--   0 root         (0) root         (0)     4243 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ListEditWidget.py
+-rw-r--r--   0 root         (0) root         (0)    30203 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)    21446 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ManageTemplatesWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ManageTemplatesWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/PreviewDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/PreviewDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/TranslateDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/TranslateDialog.ui
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ValidationDialog.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ValidationDialog.ui
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/WelcomeDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:17:02.935546 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/data/
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/data/categories.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/data/changelog.html
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/data/translators.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:17:02.939546 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/
+-rw-r--r--   0 root         (0) root         (0)    43966 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
+-rw-r--r--   0 root         (0) root         (0)    43444 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:17:02.935546 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-20 17:17:02.000000 jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-07-20 17:16:07.000000 jdDesktopEntryEdit-1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 17:17:02.939546 jdDesktopEntryEdit-1.2/setup.cfg
```

### Comparing `jdDesktopEntryEdit-1.1/BuildBackend.py` & `jdDesktopEntryEdit-1.2/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/LICENSE` & `jdDesktopEntryEdit-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/PKG-INFO` & `jdDesktopEntryEdit-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdDesktopEntryEdit
-Version: 1.1
+Version: 1.2
 Summary: A graphical Program to create and edit Desktop Entries
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDesktopEntryEdit
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdDesktopEntryEdit
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,.desktop,freedesktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
```

### Comparing `jdDesktopEntryEdit-1.1/README.md` & `jdDesktopEntryEdit-1.2/README.md`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/AboutDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditActionDialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             if self._current_identifier in self._action_data:
                 del self._action_data[self._current_identifier]
 
             self._env.translate_dialog.rename_translations(f"Action.{self._current_identifier}.Name", f"Action.{identifier}.Name")
             self._current_identifier = identifier
 
         self._action_data[identifier] = {}
-        self._action_data[identifier]["name"] = self.name_edit.text().strip()
-        self._action_data[identifier]["icon"] = self.icon_edit.text().strip()
-        self._action_data[identifier]["exec"] = self.exec_edit.text().strip()
+        self._action_data[identifier]["name"] = self.name_edit.text()
+        self._action_data[identifier]["icon"] = self.icon_edit.text()
+        self._action_data[identifier]["exec"] = self.exec_edit.text()
 
         self._ok = True
         self.close()
 
     def open_dialog(self, identifier: str) -> tuple[str, bool]:
         self._current_identifier= identifier
 
@@ -85,18 +85,21 @@
         self._action_data[identifier]["name"] = action.Name.default_text
         self._env.translate_dialog.set_translations(f"Action.{identifier}.Name", action.Name.translations)
         self._action_data[identifier]["icon"] = string_not_none(action.Icon)
         self._action_data[identifier]["exec"] = string_not_none(action.Exec)
 
     def get_desktop_action(self, identifier: str) -> desktop_entry_lib.DesktopAction:
         action = desktop_entry_lib.DesktopAction()
-        action.Name.default_text = self._action_data[identifier]["name"]
-        action.Name.translations = self._env.translate_dialog.get_translations(f"Action.{identifier}.Name")
-        action.Icon = none_if_empty_string(self._action_data[identifier]["icon"])
-        action.Exec = none_if_empty_string(self._action_data[identifier]["exec"])
+        if self._env.settings.get("stripSpaces"):
+            action.Name.default_text = self._action_data[identifier]["name"].strip()
+        else:
+            action.Name.default_text = self._action_data[identifier]["name"]
+        action.Name.translations = self._env.translate_dialog.get_translations(f"Action.{identifier}.Name", self._env.settings.get("stripSpaces"))
+        action.Icon = none_if_empty_string(self._action_data[identifier]["icon"], self._env.settings.get("stripSpaces"))
+        action.Exec = none_if_empty_string(self._action_data[identifier]["exec"], self._env.settings.get("stripSpaces"))
         return action
 
     def delete_action(self, identifier: str) -> None:
         self._env.translate_dialog.delete_translation(f"Action.{identifier}.Name")
         if identifier in self._action_data:
             del self._action_data[identifier]
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditActionDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         main_layout.addLayout(language_layout)
         main_layout.addWidget(self._list_widget)
         main_layout.addLayout(button_layout)
 
         self.setLayout(main_layout)
 
     def _ok_button_clicked(self) -> None:
-        language =self._language_edit.text().strip()
+        language = self._language_edit.text().strip()
 
         if language == "":
             QMessageBox.critical(self, QCoreApplication.translate("EditKeywordsTranslationDialog", "No Language"), QCoreApplication.translate("EditKeywordsTranslationDialog", "You have to enter a Language"))
             return
 
         if language != self._current_language:
             if list_widget_contains_item(self._main_window.keywords_language_list, language):
@@ -55,25 +55,28 @@
                 return
 
             if self._current_language is not None:
                 del self._translations[self._current_language]
 
             self._current_language = language
 
-        self._translations[language] = self._list_widget.get_list()
+        self._translations[language] = self._list_widget.get_list(False)
 
         self._current_language = language
         self._ok = True
 
         self.close()
 
     def open_dialog(self, language: Optional[str]) -> Optional[str]:
         self._current_language = language
 
-        self.setWindowTitle(QCoreApplication.translate("EditKeywordsTranslationDialog", "Edit Keywords for {{language}}").replace("{{language}}", language))
+        if language is None:
+            self.setWindowTitle(QCoreApplication.translate("EditKeywordsTranslationDialog", "Add new Keywords translation"))
+        else:
+            self.setWindowTitle(QCoreApplication.translate("EditKeywordsTranslationDialog", "Edit Keywords for {{language}}").replace("{{language}}", language))
 
         if language is None:
             self._language_edit.setText("")
             self._list_widget.clear()
         else:
             self._language_edit.setText(language)
             self._list_widget.set_list(self._translations[language])
@@ -86,16 +89,22 @@
             return None
         else:
             return self._current_language
 
     def set_translation(self, language: str, translation: list[str]) -> None:
         self._translations[language] = translation
 
-    def get_translation(self, language: str) -> list[str]:
-        return self._translations[language]
+    def get_translation(self, language: str, strip_spaces: bool) -> list[str]:
+        translated_list: list[str] = []
+        for i in self._translations[language]:
+            if strip_spaces:
+                translated_list.append(i.strip())
+            else:
+                translated_list.append(i)
+        return translated_list
 
     def delete_translation(self, language: str) -> None:
         if language in self._translations:
             del self._translations[language]
 
     def clear(self) -> None:
         self._translations.clear()
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Environment.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Environment.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Functions.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,22 @@
 def string_not_none(string: Optional[str]) -> str:
     if string is None:
         return ""
     else:
         return string
 
 
-def none_if_empty_string(string: str) -> Optional[str]:
+def none_if_empty_string(string: str, strip_spaces: bool) -> Optional[str]:
     if string.strip() == "":
         return None
     else:
-        return string
+        if strip_spaces:
+            return string.strip()
+        else:
+            return string
 
 
 def boolean_not_none(boolean: Optional[bool]) -> bool:
     if boolean is None:
         return False
     else:
         return boolean
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Icon.svg` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ListEditWidget.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ListEditWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def _update_buttons_enabled(self) -> None:
         enabled = self._list_widget.currentRow() != -1
         self._edit_button.setEnabled(enabled)
         self._remove_button.setEnabled(enabled)
 
     def _add_button_clicked(self) -> None:
-        item = QInputDialog.getText(self, QCoreApplication.translate("ListEditWidget", "Add Item"), QCoreApplication.translate("ListEditWidget", "Please enter a new Item"))[0].strip()
+        item = QInputDialog.getText(self, QCoreApplication.translate("ListEditWidget", "Add Item"), QCoreApplication.translate("ListEditWidget", "Please enter a new Item"))[0]
 
         if item == "":
             return
 
         if list_widget_contains_item(self._list_widget, item):
             QMessageBox.critical(QCoreApplication.translate("ListEditWidget", "Item in List"), QCoreApplication.translate("ListEditWidget", "This Item is already in the List"))
             return
@@ -95,17 +95,20 @@
             self._main_window.set_file_edited(True)
 
     def set_list(self, item_list: list[str]) -> None:
         self._list_widget.clear()
         for i in item_list:
             self._list_widget.addItem(i)
 
-    def get_list(self) -> list[str]:
+    def get_list(self, strip_spaces: bool) -> list[str]:
         item_list = []
         for i in range(self._list_widget.count()):
-            item_list.append(self._list_widget.item(i).text())
+            if strip_spaces:
+                item_list.append(self._list_widget.item(i).text().strip())
+            else:
+                item_list.append(self._list_widget.item(i).text())
         return item_list
 
     def clear(self) -> None:
         self._list_widget.clear()
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/MainWindow.py`

 * *Files 12% similar despite different names*

```diff
@@ -529,74 +529,80 @@
 
         clear_table_widget(self.custom_table)
         for custom_key, custom_value in entry.CustomKeys.items():
             self._add_custom_row(key=custom_key, value=custom_value)
 
         self._current_entry = entry
 
+    def _strip_spaces(self, string: str) -> str:
+        if self._env.settings.get("stripSpaces"):
+            return string.strip()
+        else:
+            return string
+
     def get_desktop_entry(self) -> desktop_entry_lib.DesktopEntry:
         entry = copy.deepcopy(self._current_entry)
 
         if self.application_type_rad.isChecked():
             entry.Type = "Application"
         elif self.link_type_rad.isChecked():
             entry.Type = "Link"
         elif self.directory_type_rad.isChecked():
             entry.Type = "Directory"
 
-        entry.Name.default_text = self.name_edit.text().strip()
-        entry.Name.translations = self._env.translate_dialog.get_translations("Name")
+        entry.Name.default_text = self._strip_spaces(self.name_edit.text())
+        entry.Name.translations = self._env.translate_dialog.get_translations("Name", self._env.settings.get("stripSpaces"))
 
-        entry.GenericName.default_text = self.generic_name_edit.text().strip()
-        entry.GenericName.translations = self._env.translate_dialog.get_translations("GenericName")
+        entry.GenericName.default_text = self._strip_spaces(self.generic_name_edit.text())
+        entry.GenericName.translations = self._env.translate_dialog.get_translations("GenericName", self._env.settings.get("stripSpaces"))
 
-        entry.Comment.default_text = self.comment_edit.text().strip()
-        entry.Comment.translations = self._env.translate_dialog.get_translations("Comment")
+        entry.Comment.default_text = self._strip_spaces(self.comment_edit.text())
+        entry.Comment.translations = self._env.translate_dialog.get_translations("Comment", self._env.settings.get("stripSpaces"))
 
-        entry.Icon = none_if_empty_string(self.icon_edit.text())
-        entry.Exec = none_if_empty_string(self.exec_edit.text())
-        entry.TryExec = none_if_empty_string(self.try_exec_edit.text())
-        entry.Path = none_if_empty_string(self.path_edit.text())
-        entry.StartupWMClass = none_if_empty_string(self.startup_wm_class_edit.text())
-        entry.URL = none_if_empty_string(self.url_edit.text())
+        entry.Icon = none_if_empty_string(self.icon_edit.text(), self._env.settings.get("stripSpaces"))
+        entry.Exec = none_if_empty_string(self.exec_edit.text(), self._env.settings.get("stripSpaces"))
+        entry.TryExec = none_if_empty_string(self.try_exec_edit.text(), self._env.settings.get("stripSpaces"))
+        entry.Path = none_if_empty_string(self.path_edit.text(), self._env.settings.get("stripSpaces"))
+        entry.StartupWMClass = none_if_empty_string(self.startup_wm_class_edit.text(), self._env.settings.get("stripSpaces"))
+        entry.URL = none_if_empty_string(self.url_edit.text(),self._env.settings.get("stripSpaces"))
 
         entry.NoDisplay = none_if_false(self.no_display_checkbox.isChecked())
         entry.Hidden = none_if_false(self.hidden_checkbox.isChecked())
         entry.DBusActivatable = none_if_false(self.dbus_activatable_checkbox.isChecked())
         entry.Terminal = none_if_false(self.terminal_checkbox.isChecked())
         entry.StartupNotify = none_if_false(self.startup_notify_checkbox.isChecked())
         entry.PrefersNonDefaultGPU = none_if_false(self.prefers_non_default_gpu_checkbox.isChecked())
         entry.SingleMainWindow = none_if_false(self.single_main_window_checkbox.isChecked())
 
         entry.Categories.clear()
         for i in range(self.categories_list.count()):
-            entry.Categories.append(self.categories_list.item(i).text().strip())
+            entry.Categories.append(self._strip_spaces(self.categories_list.item(i).text()))
 
-        entry.MimeType = self._edit_mime_type_widget.get_list()
+        entry.MimeType = self._edit_mime_type_widget.get_list(self._env.settings.get("stripSpaces"))
 
         entry.Keywords.clear()
-        entry.Keywords.default_list = self._edit_untranslated_keywords_widget.get_list()
+        entry.Keywords.default_list = self._edit_untranslated_keywords_widget.get_list(self._env.settings.get("stripSpaces"))
         for i in range(self.keywords_language_list.count()):
-            language = self.keywords_language_list.item(i).text().strip()
-            entry.Keywords.translations[language] = self._edit_keywords_translation_dialog.get_translation(language)
+            language = self._strip_spaces(self.keywords_language_list.item(i).text())
+            entry.Keywords.translations[language] = self._edit_keywords_translation_dialog.get_translation(language, self._env.settings.get("stripSpaces"))
 
         entry.Actions.clear()
         for i in range(self.actions_list.count()):
-            action_name = self.actions_list.item(i).text().strip()
+            action_name = self._strip_spaces(self.actions_list.item(i).text())
             entry.Actions[action_name] = self._edit_action_dialog.get_desktop_action(action_name)
 
-        entry.Implements = self._edit_implements_widget.get_list()
-        entry.OnlyShowIn = self._edit_only_show_in_widget.get_list()
-        entry.NotShowIn = self._edit_not_show_in_widget.get_list()
+        entry.Implements = self._edit_implements_widget.get_list(self._env.settings.get("stripSpaces"))
+        entry.OnlyShowIn = self._edit_only_show_in_widget.get_list(self._env.settings.get("stripSpaces"))
+        entry.NotShowIn = self._edit_not_show_in_widget.get_list(self._env.settings.get("stripSpaces"))
 
         entry.CustomKeys.clear()
         for i in get_logical_table_row_list(self.custom_table):
             key = self.custom_table.item(i, 0).text()
             if desktop_entry_lib.is_custom_key_name_valid(key):
-                entry.CustomKeys[key] = self.custom_table.item(i, 1).text()
+                entry.CustomKeys[key] = self._strip_spaces(self.custom_table.item(i, 1).text())
 
         if self._env.settings.get("addCommentSave"):
             entry.leading_comment = f"Created with jdDesktopEntryEdit {self._env.version}"
 
         return entry
 
     def save_file(self, path: str) -> None:
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/MainWindow.ui`

 * *Files 0% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/MainWindow.ui`

```diff
@@ -437,15 +437,15 @@
               <attribute name="title">
                 <string>Custom</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_4">
                 <item>
                   <widget class="QLabel" name="label_12">
                     <property name="text">
-                      <string>All Ccustom Keys of your Desktop Entry. Make sure the Keys starts with X-.</string>
+                      <string>All Custom Keys of your Desktop Entry. Make sure the Keys starts with X-.</string>
                     </property>
                     <property name="alignment">
                       <set>Qt::AlignCenter</set>
                     </property>
                     <property name="wordWrap">
                       <bool>true</bool>
                     </property>
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ManageTemplatesWindow.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ManageTemplatesWindow.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/PreviewDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/PreviewDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Settings.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/Settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         self._default_settings = {
             "language": "default",
             "recentFilesLength": 10,
             "windowTitleType": "filename",
             "checkSaveBeforeClosing": True,
             "showEditedTitle": True,
             "addCommentSave": True,
+            "stripSpaces": True,
             "showWelcomeDialog": True
         }
 
         self._user_settings = {}
 
     def get(self, key: str) -> Any:
         """Returns the given setting"""
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/SettingsDialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,26 +49,28 @@
             self.language_box.setCurrentIndex(index)
 
         self.recent_files_spin_box.setValue(self._env.settings.get("recentFilesLength"))
         select_combo_box_data(self.window_title_box, self._env.settings.get("windowTitleType"))
         self.check_save_check_box.setChecked(self._env.settings.get("checkSaveBeforeClosing"))
         self.title_edited_check_box.setChecked(self._env.settings.get("showEditedTitle"))
         self.add_comment_check_box.setChecked(self._env.settings.get("addCommentSave"))
+        self.strip_spaces_check_box.setChecked(self._env.settings.get("stripSpaces"))
 
     def _reset_button_clicked(self):
         self._env.settings.reset()
         self._update_widgets()
 
     def _ok_button_clicked(self):
         self._env.settings.set("language", self.language_box.currentData())
         self._env.settings.set("recentFilesLength",  self.recent_files_spin_box.value())
         self._env.settings.set("windowTitleType",  self.window_title_box.currentData())
         self._env.settings.set("checkSaveBeforeClosing", self.check_save_check_box.isChecked())
         self._env.settings.set("showEditedTitle", self.title_edited_check_box.isChecked())
         self._env.settings.set("addCommentSave", self.add_comment_check_box.isChecked())
+        self._env.settings.set("stripSpaces", self.strip_spaces_check_box.isChecked())
 
         self._env.save_recent_files()
 
         self._main_window.update_window_title()
 
         self._env.settings.save(os.path.join(self._env.data_dir, "settings.json"))
         self.close()
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/SettingsDialog.ui`

 * *Files 5% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/SettingsDialog.ui`

```diff
@@ -84,14 +84,21 @@
         <widget class="QCheckBox" name="add_comment_check_box">
           <property name="text">
             <string>Add comment to Files</string>
           </property>
         </widget>
       </item>
       <item>
+        <widget class="QCheckBox" name="strip_spaces_check_box">
+          <property name="text">
+            <string>Remove extra spaces when saving</string>
+          </property>
+        </widget>
+      </item>
+      <item>
         <spacer name="verticalSpacer">
           <property name="orientation">
             <enum>Qt::Vertical</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/TranslateDialog.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,25 +64,34 @@
 
     def _ok_button_clicked(self) -> None:
         if not self._check_valid():
             return
 
         current_translations: dict[str, str] = {}
         for i in range(self.table_widget.rowCount()):
-            current_translations[self.table_widget.item(i, 0).text().strip()] = self.table_widget.item(i, 1).text().strip()
+            current_translations[self.table_widget.item(i, 0)] = self.table_widget.item(i, 1).text()
 
         self._translations[self._current_key] = current_translations
 
         self.close()
 
     def set_translations(self, key: str, translations: dict[str, str]) -> None:
         self._translations[key] = copy.deepcopy(translations)
 
-    def get_translations(self, key: str) -> dict[str, str]:
-        return self._translations.get(key, {})
+    def get_translations(self, key: str, strip_spaces: bool) -> dict[str, str]:
+        current_translations: dict[str, str] = {}
+
+        for key, value in self._translations.get(key, {}).items():
+            if strip_spaces:
+                current_translations[key.strip()] = value.strip()
+            else:
+                current_translations[key] = value
+
+        return current_translations
+
 
     def rename_translations(self, old_key: str, new_key: str) -> None:
         if old_key not in self._translations:
             return
 
         translations = copy.deepcopy(self._translations[old_key])
         self._translations[new_key] = translations
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/TranslateDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ValidationDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/ValidationDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.ui` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__init__.py` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/__init__.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/categories.txt` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/data/categories.txt`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts`

 * *Files 1% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts`

```diff
@@ -137,78 +137,83 @@
     </message>
     <message>
       <location filename="../EditKeywordsTranslationDialog.py" line="54"/>
       <source>This Language already exists</source>
       <translation>Diese Sprache existiert bereits</translation>
     </message>
     <message>
-      <location filename="../EditKeywordsTranslationDialog.py" line="72"/>
+      <location filename="../EditKeywordsTranslationDialog.py" line="73"/>
+      <source>Add new Keywords translation</source>
+      <translation>Eine neue Schlüsselwörterübersetzung hinzufügen</translation>
+    </message>
+    <message>
+      <location filename="../EditKeywordsTranslationDialog.py" line="75"/>
       <source>Edit Keywords for {{language}}</source>
       <translation>Schlüsselwörter für {{language}} bearbeiten</translation>
     </message>
   </context>
   <context>
     <name>Functions</name>
     <message>
-      <location filename="../Functions.py" line="130"/>
+      <location filename="../Functions.py" line="133"/>
       <source>{{module}} not installed</source>
       <translation>{{module}} nicht installiert</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="130"/>
+      <location filename="../Functions.py" line="133"/>
       <source>Optional module {{module}} not found. It is required to use this Feature.</source>
       <translation>Das optionale Modul {{module}} wurde nicht gefunden. Es wird zum benutzen dieses features benötigt.</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="141"/>
+      <location filename="../Functions.py" line="144"/>
       <source>Invalid URL</source>
       <translation>Ungültige URL</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="141"/>
+      <location filename="../Functions.py" line="144"/>
       <source>The given URL is not valid</source>
       <translation>Die angegebene URL ist ungültig</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="143"/>
+      <location filename="../Functions.py" line="146"/>
       <source>Invalid Schema</source>
       <translation>Ungültiges Schema</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="143"/>
+      <location filename="../Functions.py" line="146"/>
       <source>Only http and https are supported</source>
       <translation>Es werden nur http und https unterstützt</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="145"/>
+      <location filename="../Functions.py" line="148"/>
       <source>Could not connect</source>
       <translation>Kann keine Verbindung aufbauen</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="145"/>
+      <location filename="../Functions.py" line="148"/>
       <source>Could not connect to the Website</source>
       <translation>Kann nihct zur Webseite verbinden</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="147"/>
+      <location filename="../Functions.py" line="150"/>
       <source>Unknown Error</source>
       <translation>Unbekannter Fehler</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="147"/>
+      <location filename="../Functions.py" line="150"/>
       <source>An unknown Error happened while trying to conenct to the given URL</source>
       <translation>Während des verbindens zur URL ist ein unbekannter Fehler aufgetreten</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="150"/>
+      <location filename="../Functions.py" line="153"/>
       <source>Could not get data</source>
       <translation>Kann keine Daten erhalten</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="150"/>
+      <location filename="../Functions.py" line="153"/>
       <source>Could not get data from the URL</source>
       <translation>Von der angegebenen URL können keine Daten erhalten werden</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
@@ -288,15 +293,15 @@
       <location filename="../MainWindow.py" line="45"/>
       <source>The untranslated Keywords</source>
       <translation>Du unübersetzten Schlüsselwörter</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="46"/>
       <source>A list of interfaces that this application implements. If you don't know what this means, you probably won't need it.</source>
-      <translation>Eine Liste der Interfaces, die dieses programm implementiert. Wenn du nicht weisst wass es bedeutet, brauchst du es wahrscheinlich nicht.</translation>
+      <translation>Eine Liste der Interfaces, die dieses Programm implementiert. Wenn du nicht weisst was es bedeutet, brauchst du es wahrscheinlich nicht.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="47"/>
       <source>If set, the Application is only visble when using this Desktop Environments</source>
       <translation>Wenn gesetzt, wird der Desktopeintrag nur in diesen Desktopumgebungen angezeigt</translation>
     </message>
     <message>
@@ -573,15 +578,15 @@
       <location filename="../MainWindow.ui" line="0"/>
       <source>Program has a single main window (SingleMainWindow)</source>
       <translation>Programm hat ein einzelnes Hauptfenster (SingleMainWindow)</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Run on a more powerful discrete GPU if available (PrefersNonDefaultGPU)</source>
-      <translation>Falls verfügbar auf einem eistungsstärkeren diskreten Grafikprozessor ausführen (PrefersNonDefualtGPU)</translation>
+      <translation>Falls verfügbar auf einem leistungsstärkeren diskreten Grafikprozessor ausführen (PrefersNonDefaultGPU)</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Send a Message when started (StartupNotify)</source>
       <translation>Das Programms sendet beim Starten eine Nachricht (StartupNotify)</translation>
     </message>
     <message>
@@ -666,15 +671,15 @@
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Custom</source>
       <translation>Eigen</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
-      <source>All Ccustom Keys of your Desktop Entry. Make sure the Keys starts with X-.</source>
+      <source>All Custom Keys of your Desktop Entry. Make sure the Keys starts with X-.</source>
       <translation>Alle eigenen Einträge deines Desktopeintrags. Stelle sicher, dass die Schlüssel mit X- beginnen.</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Key</source>
       <translation>Schlüssel</translation>
     </message>
@@ -960,14 +965,19 @@
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Add comment to Files</source>
       <translation>Kommentar zu Dateien hinzufügen</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
+      <source>Remove extra spaces when saving</source>
+      <translation>Zusätzliche Leerzeichen beim Speichern entfernen</translation>
+    </message>
+    <message>
+      <location filename="../SettingsDialog.ui" line="0"/>
       <source>Reset</source>
       <translation>Zurücksetzen</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>OK</source>
       <translation>OK</translation>
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts`

 * *Files 2% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts`

```diff
@@ -33,15 +33,15 @@
       <location filename="../AboutDialog.ui" line="0"/>
       <source>The following people translated jdDesktopEntryEdit:</source>
       <translation>Deze mensen hebben jdDesktopEntryEdit vertaald:</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>Changelog</source>
-      <translation>Wijzigingslog</translation>
+      <translation>Wĳzigingslog</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>Close</source>
       <translation>Sluiten</translation>
     </message>
   </context>
@@ -51,15 +51,15 @@
       <location filename="../EditActionDialog.py" line="35"/>
       <source>Identifier empty</source>
       <translation>Blanco identificatie</translation>
     </message>
     <message>
       <location filename="../EditActionDialog.py" line="35"/>
       <source>The Identifier can't be empty</source>
-      <translation>De identificatie mag niet blanco zijn</translation>
+      <translation>De identificatie mag niet blanco zĳn</translation>
     </message>
     <message>
       <location filename="../EditActionDialog.py" line="40"/>
       <source>Invalid Identifier</source>
       <translation>Ongeldige identificatie</translation>
     </message>
     <message>
@@ -137,78 +137,83 @@
     </message>
     <message>
       <location filename="../EditKeywordsTranslationDialog.py" line="54"/>
       <source>This Language already exists</source>
       <translation>Deze taal is al in gebruik</translation>
     </message>
     <message>
-      <location filename="../EditKeywordsTranslationDialog.py" line="72"/>
+      <location filename="../EditKeywordsTranslationDialog.py" line="73"/>
+      <source>Add new Keywords translation</source>
+      <translation>Trefwoordvertalingen invoeren</translation>
+    </message>
+    <message>
+      <location filename="../EditKeywordsTranslationDialog.py" line="75"/>
       <source>Edit Keywords for {{language}}</source>
       <translation>Trefwoorden van {{language}} bewerken</translation>
     </message>
   </context>
   <context>
     <name>Functions</name>
     <message>
-      <location filename="../Functions.py" line="130"/>
+      <location filename="../Functions.py" line="133"/>
       <source>{{module}} not installed</source>
       <translation>{{module}} is niet geïnstalleerd</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="130"/>
+      <location filename="../Functions.py" line="133"/>
       <source>Optional module {{module}} not found. It is required to use this Feature.</source>
       <translation>De optionele module ‘{{module}}’ is niet aangetroffen. Deze module is vereist om deze functie te kunnen gebruiken.</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="141"/>
+      <location filename="../Functions.py" line="144"/>
       <source>Invalid URL</source>
       <translation>Ongeldige url</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="141"/>
+      <location filename="../Functions.py" line="144"/>
       <source>The given URL is not valid</source>
       <translation>Deze opgegeven url is ongeldig</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="143"/>
+      <location filename="../Functions.py" line="146"/>
       <source>Invalid Schema</source>
       <translation>Ongeldig schema</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="143"/>
+      <location filename="../Functions.py" line="146"/>
       <source>Only http and https are supported</source>
-      <translation>Alleen http en https zijn geldig</translation>
+      <translation>Alleen http en https zĳn geldig</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="145"/>
+      <location filename="../Functions.py" line="148"/>
       <source>Could not connect</source>
-      <translation>Geen verbinding mogelijk</translation>
+      <translation>Geen verbinding mogelĳk</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="145"/>
+      <location filename="../Functions.py" line="148"/>
       <source>Could not connect to the Website</source>
       <translation>Er kan geen verbinding met de website worden gemaakt</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="147"/>
+      <location filename="../Functions.py" line="150"/>
       <source>Unknown Error</source>
       <translation>Onbekende foutmelding</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="147"/>
+      <location filename="../Functions.py" line="150"/>
       <source>An unknown Error happened while trying to conenct to the given URL</source>
-      <translation>Er is een onbekende foutmelding opgetreden tijdens het verbinden met de opgegeven url</translation>
+      <translation>Er is een onbekende foutmelding opgetreden tĳdens het verbinden met de opgegeven url</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="150"/>
+      <location filename="../Functions.py" line="153"/>
       <source>Could not get data</source>
       <translation>Geen gegevens opgehaald</translation>
     </message>
     <message>
-      <location filename="../Functions.py" line="150"/>
+      <location filename="../Functions.py" line="153"/>
       <source>Could not get data from the URL</source>
       <translation>Er kunnen geen gegevens van de url worden opgehaald</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
@@ -238,15 +243,15 @@
       <location filename="../ListEditWidget.py" line="23"/>
       <source>Edit</source>
       <translation>Bewerken</translation>
     </message>
     <message>
       <location filename="../ListEditWidget.py" line="24"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Verwĳderen</translation>
     </message>
     <message>
       <location filename="../ListEditWidget.py" line="52"/>
       <source>Add Item</source>
       <translation>Item toevoegen</translation>
     </message>
     <message>
@@ -254,21 +259,21 @@
       <source>Please enter a new Item</source>
       <translation>Geef het nieuwe item een naam</translation>
     </message>
     <message>
       <location filename="../ListEditWidget.py" line="76"/>
       <location filename="../ListEditWidget.py" line="58"/>
       <source>Item in List</source>
-      <translation>Item op lijst</translation>
+      <translation>Item op lĳst</translation>
     </message>
     <message>
       <location filename="../ListEditWidget.py" line="76"/>
       <location filename="../ListEditWidget.py" line="58"/>
       <source>This Item is already in the List</source>
-      <translation>Dit item staat al op de lijst</translation>
+      <translation>Dit item staat al op de lĳst</translation>
     </message>
     <message>
       <location filename="../ListEditWidget.py" line="70"/>
       <source>Edit Item</source>
       <translation>Item bewerken</translation>
     </message>
     <message>
@@ -278,45 +283,45 @@
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
       <location filename="../MainWindow.py" line="44"/>
       <source>A list of MimeTypes that this Application can open</source>
-      <translation>Een lijst met mimetypes die dit programma kan openen</translation>
+      <translation>Een lĳst met mimetypes die dit programma kan openen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="45"/>
       <source>The untranslated Keywords</source>
       <translation>Onvertaalde trefwoorden</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="46"/>
       <source>A list of interfaces that this application implements. If you don't know what this means, you probably won't need it.</source>
-      <translation>Een lijst met interfaces die dit programma gebruikt. Als u niet weet wat dit inhoudt, dan kunt u deze optie negeren.</translation>
+      <translation>Een lĳst met interfaces die dit programma gebruikt. Als u niet weet wat dit inhoudt, dan kunt u deze optie negeren.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="47"/>
       <source>If set, the Application is only visble when using this Desktop Environments</source>
       <translation>Stel in om het programma alleen in deze werkomgevingen te tonen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="48"/>
       <source>The Application is not visble when using this Desktop Environments</source>
       <translation>Dit programma wordt niet in deze werkomgevingen getoond</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="138"/>
       <source>Unsaved changes</source>
-      <translation>Niet-opgeslagen wijzigingen</translation>
+      <translation>Niet-opgeslagen wĳzigingen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="138"/>
       <source>You have unsaved changes. Do you want to save now?</source>
-      <translation>U heeft niet-opgeslagen wijzigingen. Wilt u ze nu opslaan?</translation>
+      <translation>U heeft niet-opgeslagen wĳzigingen. Wilt u ze nu opslaan?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="148"/>
       <source>Untitled</source>
       <translation>Naamloos</translation>
     </message>
     <message>
@@ -365,15 +370,15 @@
       <location filename="../MainWindow.py" line="281"/>
       <source>Add a Categorie</source>
       <translation>Categorie toevoegen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="281"/>
       <source>Please select a Categorie from the list below</source>
-      <translation>Kies een categorie van onderstaande lijst</translation>
+      <translation>Kies een categorie van onderstaande lĳst</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="285"/>
       <source>Categorie already added</source>
       <translation>Categorie reeds toegevoegd</translation>
     </message>
     <message>
@@ -420,28 +425,28 @@
       <location filename="../MainWindow.py" line="354"/>
       <source>This Identifier already exists</source>
       <translation>Deze identificatie is al in gebruik</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="378"/>
       <source>Delete Action</source>
-      <translation>Actie verwijderen</translation>
+      <translation>Actie verwĳderen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="378"/>
       <source>Are you really want to delete {{identifier}}?</source>
-      <translation>Weet u zeker dat u {{identifier}} wilt verwijderen?</translation>
+      <translation>Weet u zeker dat u {{identifier}} wilt verwĳderen?</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.py" line="403"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Verwĳderen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="422"/>
       <source>Invalid Key</source>
       <translation>Ongeldige sleutel</translation>
     </message>
     <message>
@@ -453,15 +458,15 @@
       <location filename="../MainWindow.py" line="426"/>
       <source>Everything valid</source>
       <translation>Alles is in orde</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="426"/>
       <source>No issues found</source>
-      <translation>Er zijn geen problemen aangetroffen</translation>
+      <translation>Er zĳn geen problemen aangetroffen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="439"/>
       <source>File not found</source>
       <translation>Bestand niet gevonden</translation>
     </message>
     <message>
@@ -469,21 +474,21 @@
       <source>{{path}} was not found</source>
       <translation>{{path}} is niet aangetroffen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="468"/>
       <location filename="../MainWindow.py" line="443"/>
       <source>Error loading Desktop Entry</source>
-      <translation>Fout tijdens laden van item</translation>
+      <translation>Fout tĳdens laden van item</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="468"/>
       <location filename="../MainWindow.py" line="443"/>
       <source>This Desktop Entry couldn't be loaded. Make sure, it is in the right format.</source>
-      <translation>Er is een fout opgetreden tijdens het laden van het item. Controleer of het bestandsformaat juist is.</translation>
+      <translation>Er is een fout opgetreden tĳdens het laden van het item. Controleer of het bestandsformaat juist is.</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>General</source>
       <translation>Algemeen</translation>
     </message>
     <message>
@@ -626,15 +631,15 @@
       <location filename="../MainWindow.ui" line="0"/>
       <source>Translated</source>
       <translation>Vertaald</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>A List of Languages in which are the Keywords translated</source>
-      <translation>Een lijst met talen waarin de trefwoorden zijn vertaald</translation>
+      <translation>Een lĳst met talen waarin de trefwoorden zĳn vertaald</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Edit</source>
       <translation>Bewerken</translation>
     </message>
@@ -642,15 +647,15 @@
       <location filename="../MainWindow.ui" line="0"/>
       <source>Actions</source>
       <translation>Acties</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <translation>Verwĳderen</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Implements</source>
       <translation>Implementeert</translation>
     </message>
     <message>
@@ -666,16 +671,16 @@
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Custom</source>
       <translation>Aangepast</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
-      <source>All Ccustom Keys of your Desktop Entry. Make sure the Keys starts with X-.</source>
-      <translation>Alle aangepaste sleutels van uw desktopbestand. Let op: de sleutels dienen te beginnen met X-.</translation>
+      <source>All Custom Keys of your Desktop Entry. Make sure the Keys starts with X-.</source>
+      <translation>Alle eigen sleutels van uw desktopitem. Let op: sleutels dienen te beginnen met X-.</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Key</source>
       <translation>Sleutel</translation>
     </message>
     <message>
@@ -778,15 +783,15 @@
       <location filename="../MainWindow.ui" line="0"/>
       <source>Show Welcome Dialog</source>
       <translation>Welkomstvenster tonen</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Broncode bekijken</translation>
+      <translation>Broncode bekĳken</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Report Bug</source>
       <translation>Bug melden</translation>
     </message>
     <message>
@@ -830,50 +835,50 @@
       <location filename="../ManageTemplatesWindow.py" line="82"/>
       <source>Error</source>
       <translation>Foutmelding</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="82"/>
       <source>A error occurred while renaming</source>
-      <translation>Er is een fout opgetreden tijdens het wijzigen van de naam</translation>
+      <translation>Er is een fout opgetreden tĳdens het wĳzigen van de naam</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="92"/>
       <source>Delete {{name}}</source>
-      <translation>{{name}} verwijderen</translation>
+      <translation>{{name}} verwĳderen</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="92"/>
       <source>Are you sure you want to delete {{name}}?</source>
-      <translation>Weet u zeker dat u {{name}} wilt verwijderen?</translation>
+      <translation>Weet u zeker dat u {{name}} wilt verwĳderen?</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="99"/>
       <source>A error occurred while deleting</source>
-      <translation>Er is een fout opgetreden tijdens het verwijderen</translation>
+      <translation>Er is een fout opgetreden tĳdens het verwĳderen</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.ui" line="0"/>
       <source>Manage templates</source>
       <translation>Sjablonen beheren</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.ui" line="0"/>
       <source>Save</source>
       <translation>Opslaan</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Naam wijzigen</translation>
+      <translation>Naam wĳzigen</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <translation>Verwĳderen</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.ui" line="0"/>
       <source>Close</source>
       <translation>Sluiten</translation>
     </message>
   </context>
@@ -883,15 +888,15 @@
       <location filename="../PreviewDialog.ui" line="0"/>
       <source>Preview</source>
       <translation>Voorvertoning</translation>
     </message>
     <message>
       <location filename="../PreviewDialog.ui" line="0"/>
       <source>Preview of your desktop entry</source>
-      <translation>Bekijk hoe uw desktopitem er uit komt te zien</translation>
+      <translation>Bekĳk hoe uw desktopitem er uit komt te zien</translation>
     </message>
     <message>
       <location filename="../PreviewDialog.ui" line="0"/>
       <source>Copy</source>
       <translation>Kopiëren</translation>
     </message>
     <message>
@@ -946,28 +951,33 @@
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Window title:</source>
       <translation>Venstertitel:</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Ask before closing unsaved File</source>
-      <translation>Om bevestiging vragen bij niet-opgeslagen bestand</translation>
+      <translation>Om bevestiging vragen bĳ niet-opgeslagen bestand</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Show in Title if File is edited</source>
       <translation>In titel aangeven of bestand bewerkt is</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Add comment to Files</source>
       <translation>Opmerking toevoegen aan bestanden</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
+      <source>Remove extra spaces when saving</source>
+      <translation>Witruimtes wissen na opslaan</translation>
+    </message>
+    <message>
+      <location filename="../SettingsDialog.ui" line="0"/>
       <source>Reset</source>
       <translation>Standaardwaarden</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>OK</source>
       <translation>Oké</translation>
@@ -980,15 +990,15 @@
   </context>
   <context>
     <name>TranslateDialog</name>
     <message>
       <location filename="../TranslateDialog.ui" line="0"/>
       <location filename="../TranslateDialog.py" line="38"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Verwĳderen</translation>
     </message>
     <message>
       <location filename="../TranslateDialog.py" line="54"/>
       <source>No Language</source>
       <translation>Geen taal</translation>
     </message>
     <message>
@@ -1086,11 +1096,11 @@
       <location filename="../WelcomeDialog.ui" line="0"/>
       <source>You can validate your Desktop Entry at Tools&gt;Validate.</source>
       <translation>U kunt uw item verifiëren via Hulpmiddelen → Verifiëren.</translation>
     </message>
     <message>
       <location filename="../WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Altijd tonen na opstarten</translation>
+      <translation>Altĳd tonen na opstarten</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/PKG-INFO` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdDesktopEntryEdit
-Version: 1.1
+Version: 1.2
 Summary: A graphical Program to create and edit Desktop Entries
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDesktopEntryEdit
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdDesktopEntryEdit
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,.desktop,freedesktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
```

### Comparing `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/SOURCES.txt` & `jdDesktopEntryEdit-1.2/jdDesktopEntryEdit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.1/pyproject.toml` & `jdDesktopEntryEdit-1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -33,17 +33,30 @@
   "desktop-entry-lib"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://codeberg.org/JakobDev/jdDesktopEntryEdit"
 Issues = "https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues"
+Translate = "https://translate.codeberg.org/projects/jdDesktopEntryEdit"
 Donation = "https://ko-fi.com/jakobdev"
 
 [project.gui-scripts]
 jdDesktopEntryEdit = "jdDesktopEntryEdit:main"
 
 [tool.setuptools]
 packages = ["jdDesktopEntryEdit"]
 
 [tool.setuptools.dynamic]
 version = { file = "jdDesktopEntryEdit/version.txt" }
+
+[tool.pyproject-appimage]
+script = "jdDesktopEntryEdit"
+output = "jdDesktopEntryEdit.AppImage"
+icon = "jdDesktopEntryEdit/Icon.svg"
+rename-icon = "page.codeberg.JakobDev.jdDesktopEntryEdit.svg"
+desktop-entry = "deploy/page.codeberg.JakobDev.jdDesktopEntryEdit.desktop"
+gettext-desktop-entry = true
+appstream = "deploy/page.codeberg.JakobDev.jdDesktopEntryEdit.metainfo.xml"
+gettext-appstream = true
+gettext-directory = "deploy/translations"
+python-version = "3.11"
```

