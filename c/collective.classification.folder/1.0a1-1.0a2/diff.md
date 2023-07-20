# Comparing `tmp/collective.classification.folder-1.0a1.tar.gz` & `tmp/collective.classification.folder-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.classification.folder-1.0a1.tar", last modified: Wed Mar 29 08:29:23 2023, max compression
+gzip compressed data, was "collective.classification.folder-1.0a2.tar", last modified: Thu Jul 20 08:24:57 2023, max compression
```

## Comparing `collective.classification.folder-1.0a1.tar` & `collective.classification.folder-1.0a2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/
--rw-rw-r--   0 sge       (1000) sge       (1000)      242 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       62 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      677 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     3971 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2619 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/README.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7943 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/docs/conf.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      119 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/docs/index.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       39 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      525 2023-03-29 08:29:23.411104 collective.classification.folder-1.0a1/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     3098 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/
--rw-rw-r--   0 sge       (1000) sge       (1000)      149 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2704 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      740 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1964 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/autocomplete.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6741 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     9435 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/faceted.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      276 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/helper.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/overrides/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/overrides/.gitkeep
--rw-rw-r--   0 sge       (1000) sge       (1000)     2229 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/settings.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/.gitkeep
--rw-rw-r--   0 sge       (1000) sge       (1000)      810 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/ClassificationFolder.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)      729 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)       85 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/faceted.css
--rw-rw-r--   0 sge       (1000) sge       (1000)     1056 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/import.svg
--rw-rw-r--   0 sge       (1000) sge       (1000)       86 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/progressbar.css
--rw-rw-r--   0 sge       (1000) sge       (1000)    30033 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/progressbar.min.js
--rw-rw-r--   0 sge       (1000) sge       (1000)      941 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/tables.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1357 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3909 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      905 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/display.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     8635 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/folder-listing.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     4325 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/browser/widget.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2073 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/content/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     8405 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1063 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_folders.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1289 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_subfolder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2526 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2011 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/dataprovider.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1072 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/indexers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10045 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/content/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/form/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      718 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     4191 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/import.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)    15151 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/importform.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/form/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    30030 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/form/tests/test_importform.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      497 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/interfaces.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)      611 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6399 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/collective.classification.folder.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     6261 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     8245 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1590 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/update.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      533 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      778 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/permissions.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      221 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      809 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      549 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      250 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/cssregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      625 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1081 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      863 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/rolemap.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2911 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2843 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2781 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      459 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/uninstall/
--rw-rw-r--   0 sge       (1000) sge       (1000)      142 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/services/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/services/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1554 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/services/add.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      531 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/services/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1797 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/services/update.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3305 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2453 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/testing.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2059 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/robot/test_example.robot
--rw-rw-r--   0 sge       (1000) sge       (1000)     1075 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_behavior_classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    15052 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_folder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3118 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_folders.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2673 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_subfolder.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      990 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2754 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10796 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    11557 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      623 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/to1001/
--rw-rw-r--   0 sge       (1000) sge       (1000)      505 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/to1001/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      172 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/to1001/cssregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      583 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/to1001/jsregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1051 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     7233 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1349 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective/classification/folder/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:29:23.407104 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     3971 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     6131 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      157 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      554 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-03-29 08:29:23.000000 collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/top_level.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.227706 collective.classification.folder-1.0a2/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      361 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       62 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      677 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       81 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4072 2023-07-20 08:24:57.227706 collective.classification.folder-1.0a2/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2619 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7943 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/docs/conf.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      119 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/docs/index.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       39 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      525 2023-07-20 08:24:57.227706 collective.classification.folder-1.0a2/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3080 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      149 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2704 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      740 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1964 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/autocomplete.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6741 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9435 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/faceted.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      276 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/helper.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/overrides/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/overrides/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2229 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/settings.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)      810 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/ClassificationFolder.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      729 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       85 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/faceted.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1056 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/import.svg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       86 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/progressbar.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)    30033 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/progressbar.min.js
+-rw-rw-r--   0 sge       (1000) sge       (1000)      941 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/tables.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1357 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3909 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      905 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/display.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8635 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/folder-listing.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4325 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/browser/widget.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2073 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/content/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8429 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1063 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_folders.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1289 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_subfolder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2526 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2011 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/dataprovider.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1072 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/indexers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    10045 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/content/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/form/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      718 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4191 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/import.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)    15151 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/importform.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/form/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    30030 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/form/tests/test_importform.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      497 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      611 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6399 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/collective.classification.folder.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6261 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8245 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1590 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/update.py
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      533 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/locales/update.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)      778 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/permissions.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      221 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      809 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      549 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/controlpanel.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      250 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      625 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1081 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      863 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/rolemap.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2911 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2843 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2781 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      459 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/uninstall/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      142 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/services/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/services/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1554 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/services/add.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      531 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/services/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1797 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/services/update.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3305 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2453 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/testing.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2059 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/robot/test_example.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1075 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_behavior_classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    15052 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_folder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3118 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_folders.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2673 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_subfolder.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      990 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2754 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    10796 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    11557 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.227706 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      623 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.227706 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/to1001/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      505 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/to1001/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      172 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/to1001/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      583 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/to1001/jsregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1051 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/upgrades.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7233 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1349 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective/classification/folder/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:57.223706 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4072 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6131 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      157 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      554 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-07-20 08:24:57.000000 collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/top_level.txt
```

### Comparing `collective.classification.folder-1.0a1/LICENSE.GPL` & `collective.classification.folder-1.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/LICENSE.rst` & `collective.classification.folder-1.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/PKG-INFO` & `collective.classification.folder-1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.classification.folder
-Version: 1.0a1
+Version: 1.0a2
 Summary: Addon to manage classification folders
-Home-page: https://github.com/collective/collective.classification.folder
+Home-page: https://github.com/imio/collective.classification.folder
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.folder
-Project-URL: Source, https://github.com/collective/collective.classification.folder
-Project-URL: Tracker, https://github.com/collective/collective.classification.folder/issues
+Project-URL: Source, https://github.com/imio/collective.classification.folder
+Project-URL: Tracker, https://github.com/imio/collective.classification.folder/issues
 Keywords: Python Plone CMS
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
@@ -126,14 +126,20 @@
 - Martin Peeters [original author]
 
 
 Changelog
 =========
 
 
+1.0a2 (2023-07-20)
+------------------
+
+- Set classification_categories field on folders as not required
+  [sgeulette]
+
 1.0a1 (2023-03-29)
 ------------------
 
 - Initial release.
   [mpeeters, sgeulette]
 - Replaced collective.z3cform.chosen widget by collective.z3cform.select2.
   Must remove "chosen" packages in next release.
```

### Comparing `collective.classification.folder-1.0a1/README.rst` & `collective.classification.folder-1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/docs/conf.py` & `collective.classification.folder-1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/setup.cfg` & `collective.classification.folder-1.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/setup.py` & `collective.classification.folder-1.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.classification.folder",
-    version="1.0a1",
+    version="1.0a2",
     description="Addon to manage classification folders",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -29,20 +29,20 @@
         "Programming Language :: Python :: 2.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone CMS",
     author="Martin Peeters",
     author_email="support@imio.be",
-    url="https://github.com/collective/collective.classification.folder",
+    url="https://github.com/imio/collective.classification.folder",
     project_urls={
         "PyPI": "https://pypi.python.org/pypi/collective.classification.folder",
-        "Source": "https://github.com/collective/collective.classification.folder",
+        "Source": "https://github.com/imio/collective.classification.folder",
         "Tracker": (
-            "https://github.com/collective/collective.classification.folder/issues"
+            "https://github.com/imio/collective.classification.folder/issues"
         ),
         # 'Documentation': 'https://collective.classification.folder.readthedocs.io/en/latest/',
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["collective", "collective.classification"],
     package_dir={"": "src"},
```

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/classification_folder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/behaviors/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/autocomplete.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/autocomplete.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/faceted.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/faceted.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/settings.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/settings.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/ClassificationFolder.svg` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/ClassificationFolder.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/ClassificationSubfolder.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/import.svg` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/import.svg`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/static/progressbar.min.js` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/static/progressbar.min.js`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/tables.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/tables.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/classification-folder-faceted.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/classification-folders-faceted.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/display.pt` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/display.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/templates/folder-listing.pt` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/templates/folder-listing.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/browser/widget.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/browser/widget.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_folder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     classification_categories = schema.List(
         title=_(u"Classification categories"),
         # description=_(u"List of categories / subcategories"),
         value_type=schema.Choice(
             source=ClassificationTreeSourceBinder(enabled=True),
         ),
         min_length=1,
+        required=False,
     )
 
     treating_groups = LocalRoleField(
         title=_(u"Service in charge"),
         # description=_(u"ID of the service that are in charge of this folder"),
         source=ServiceInChargeSourceBinder(),
         required=False,
```

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_folders.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_folders.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/classification_subfolder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/classification_subfolder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/dataprovider.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/dataprovider.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/indexers.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/indexers.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/content/vocabularies.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/content/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/form/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/form/import.pt` & `collective.classification.folder-1.0a2/src/collective/classification/folder/form/import.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/form/importform.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/form/importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/form/tests/test_importform.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/form/tests/test_importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/README.rst` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/collective.classification.folder.pot` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/collective.classification.folder.pot`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/en/LC_MESSAGES/collective.classification.folder.po`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/fr/LC_MESSAGES/collective.classification.folder.po`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/update.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/locales/update.sh` & `collective.classification.folder-1.0a2/src/collective/classification/folder/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/permissions.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/catalog.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/controlpanel.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/metadata.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/registry.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/rolemap.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationFolder.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationFolders.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/profiles/default/types/ClassificationSubfolder.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/services/add.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/services/add.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/services/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/services/update.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/services/update.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/setuphandlers.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/testing.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/testing.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/robot/test_example.robot` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_behavior_classification_folder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_behavior_classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_folder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_folder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_folders.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_folders.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_ct_classification_subfolder.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_ct_classification_subfolder.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_robot.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_setup.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_utils.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/tests/test_vocabularies.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/configure.zcml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/to1001/jsregistry.xml` & `collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/to1001/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/upgrades/upgrades.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/utils.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective/classification/folder/vocabularies.py` & `collective.classification.folder-1.0a2/src/collective/classification/folder/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/PKG-INFO` & `collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.classification.folder
-Version: 1.0a1
+Version: 1.0a2
 Summary: Addon to manage classification folders
-Home-page: https://github.com/collective/collective.classification.folder
+Home-page: https://github.com/imio/collective.classification.folder
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.folder
-Project-URL: Source, https://github.com/collective/collective.classification.folder
-Project-URL: Tracker, https://github.com/collective/collective.classification.folder/issues
+Project-URL: Source, https://github.com/imio/collective.classification.folder
+Project-URL: Tracker, https://github.com/imio/collective.classification.folder/issues
 Keywords: Python Plone CMS
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
@@ -126,14 +126,20 @@
 - Martin Peeters [original author]
 
 
 Changelog
 =========
 
 
+1.0a2 (2023-07-20)
+------------------
+
+- Set classification_categories field on folders as not required
+  [sgeulette]
+
 1.0a1 (2023-03-29)
 ------------------
 
 - Initial release.
   [mpeeters, sgeulette]
 - Replaced collective.z3cform.chosen widget by collective.z3cform.select2.
   Must remove "chosen" packages in next release.
```

### Comparing `collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/SOURCES.txt` & `collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.classification.folder-1.0a1/src/collective.classification.folder.egg-info/requires.txt` & `collective.classification.folder-1.0a2/src/collective.classification.folder.egg-info/requires.txt`

 * *Files identical despite different names*

