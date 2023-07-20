# Comparing `tmp/plone.app.multilingual-7.0.2.tar.gz` & `tmp/plone.app.multilingual-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.multilingual-7.0.2.tar", last modified: Fri Jul 14 10:12:31 2023, max compression
+gzip compressed data, was "plone.app.multilingual-8.0.0.tar", last modified: Fri Jul 14 10:14:32 2023, max compression
```

## Comparing `plone.app.multilingual-7.0.2.tar` & `plone.app.multilingual-8.0.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.427896 plone.app.multilingual-7.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    28024 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      536 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    43655 2023-07-14 10:12:31.428080 plone.app.multilingual-7.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    14047 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.386777 plone.app.multilingual-7.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/LICENSE.gpl
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5620 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)     8041 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/conf.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.388819 plone.app.multilingual-7.0.2/docs/images/
--rwxr-xr-x   0 maurits    (501) staff       (20)   135534 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/images/image00.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136010 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/images/image01.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136026 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/images/image02.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    99720 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/images/image03.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    36518 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/docs/images/image04.png
--rw-r--r--   0 maurits    (501) staff       (20)     1761 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1187 2023-07-14 10:12:31.428625 plone.app.multilingual-7.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1756 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.380241 plone.app.multilingual-7.0.2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.389135 plone.app.multilingual-7.0.2/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.392029 plone.app.multilingual-7.0.2/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.398143 plone.app.multilingual-7.0.2/src/plone/app/multilingual/
--rw-r--r--   0 maurits    (501) staff       (20)      331 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1683 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.403601 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7170 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/add.py
--rw-r--r--   0 maurits    (501) staff       (20)    11381 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10300 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3821 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)    10414 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/helper_views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.403852 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)     6926 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/images/gtranslate.png
--rw-r--r--   0 maurits    (501) staff       (20)     2511 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.404960 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/
--rw-r--r--   0 maurits    (501) staff       (20)     9667 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/babel_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)   162462 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/jit-yc.js
--rw-r--r--   0 maurits    (501) staff       (20)     9667 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/mmap_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)    22949 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/menu.py
--rw-r--r--   0 maurits    (501) staff       (20)    14381 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/migrator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3352 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/modify.py
--rw-r--r--   0 maurits    (501) staff       (20)     4024 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/selector.py
--rw-r--r--   0 maurits    (501) staff       (20)    10594 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.405249 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/stylesheet/
--rw-r--r--   0 maurits    (501) staff       (20)     2297 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/stylesheet/multilingual.css
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/switcher.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.409720 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1330 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/alternate-languages.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3843 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/cleanup.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1237 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/cleanup_results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1938 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2877 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1732 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1563 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/languages-notice.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/languageselector.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11015 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/migration.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1208 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/migrator-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5387 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/mmap.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6884 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/modify_translations.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3307 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1152 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/reindex-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1218 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/relocate-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3295 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/translate.py
--rw-r--r--   0 maurits    (501) staff       (20)     1084 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/update.py
--rw-r--r--   0 maurits    (501) staff       (20)     6724 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      470 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     5012 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/viewlets.py
--rw-r--r--   0 maurits    (501) staff       (20)     5962 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     6674 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.411557 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      602 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lif.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lif.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lrf.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.414977 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/
--rw-r--r--   0 maurits    (501) staff       (20)       48 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4430 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/cloner.py
--rw-r--r--   0 maurits    (501) staff       (20)     2725 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1640 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3157 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/form.py
--rw-r--r--   0 maurits    (501) staff       (20)      770 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/language.py
--rw-r--r--   0 maurits    (501) staff       (20)      456 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/languageindependent.py
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     4955 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     1100 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2994 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     3338 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)      366 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1571 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/itg.py
--rw-r--r--   0 maurits    (501) staff       (20)     8502 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)      151 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      234 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.382274 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.417415 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      427 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
--rw-r--r--   0 maurits    (501) staff       (20)      113 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1344 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      343 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.417987 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2680 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2711 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types/LRF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      240 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      412 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.420278 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      211 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      418 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      202 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.382781 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.382489 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.420778 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1025 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.421115 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)      276 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.421459 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_4/
--rw-r--r--   0 maurits    (501) staff       (20)      975 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2988 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/shared_uuid.py
--rw-r--r--   0 maurits    (501) staff       (20)     6530 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     9607 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      183 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.426623 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.427694 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3534 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_add_translation.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3418 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_translate_content.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1434 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_alternates.py
--rw-r--r--   0 maurits    (501) staff       (20)    11045 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_api.py
--rw-r--r--   0 maurits    (501) staff       (20)     2147 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1878 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     8744 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_form.py
--rw-r--r--   0 maurits    (501) staff       (20)     5819 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_helper_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     9471 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_lif.py
--rw-r--r--   0 maurits    (501) staff       (20)     5354 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3299 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_menu.py
--rw-r--r--   0 maurits    (501) staff       (20)      532 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    39142 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_selector.py
--rw-r--r--   0 maurits    (501) staff       (20)     4727 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     3326 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     8330 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_switcher.py
--rw-r--r--   0 maurits    (501) staff       (20)     1601 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_uninstall.py
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     8055 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     2687 2023-07-14 10:12:30.000000 plone.app.multilingual-7.0.2/src/plone/app/multilingual/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:12:31.391755 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    43655 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7054 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      733 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 10:12:31.000000 plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.212434 plone.app.multilingual-8.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    28143 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      536 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/CREDITS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    43774 2023-07-14 10:14:32.212674 plone.app.multilingual-8.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    14047 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.166508 plone.app.multilingual-8.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/LICENSE.gpl
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5620 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/Makefile
+-rw-r--r--   0 maurits    (501) staff       (20)     8041 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/conf.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.168621 plone.app.multilingual-8.0.0/docs/images/
+-rwxr-xr-x   0 maurits    (501) staff       (20)   135534 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/images/image00.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)   136010 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/images/image01.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)   136026 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/images/image02.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)    99720 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/images/image03.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)    36518 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/docs/images/image04.png
+-rw-r--r--   0 maurits    (501) staff       (20)     1761 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1187 2023-07-14 10:14:32.213435 plone.app.multilingual-8.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1785 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.159473 plone.app.multilingual-8.0.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.168933 plone.app.multilingual-8.0.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.171751 plone.app.multilingual-8.0.0/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.177673 plone.app.multilingual-8.0.0/src/plone/app/multilingual/
+-rw-r--r--   0 maurits    (501) staff       (20)      331 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1683 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/api.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.184140 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7170 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/add.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11381 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    10300 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3821 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10414 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/helper_views.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.184431 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)     6926 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/images/gtranslate.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2511 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.185827 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/
+-rw-r--r--   0 maurits    (501) staff       (20)     9667 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/babel_helper.js
+-rw-r--r--   0 maurits    (501) staff       (20)   162462 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/jit-yc.js
+-rw-r--r--   0 maurits    (501) staff       (20)     9667 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/mmap_helper.js
+-rw-r--r--   0 maurits    (501) staff       (20)    22949 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14381 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/migrator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3352 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/modify.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4024 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/selector.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10594 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.186086 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/stylesheet/
+-rw-r--r--   0 maurits    (501) staff       (20)     2297 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/stylesheet/multilingual.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1342 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/switcher.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.191394 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1330 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/alternate-languages.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3843 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/cleanup.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1237 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/cleanup_results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1938 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2877 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1732 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1563 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/languages-notice.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/languageselector.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11015 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/migration.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1208 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/migrator-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5387 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/mmap.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6885 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/modify_translations.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3307 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1152 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/reindex-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1218 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/relocate-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3295 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/translate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1084 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/update.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6724 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      470 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5012 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/viewlets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5962 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6674 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.192720 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      602 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lif.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lif.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lrf.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.196977 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)       48 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4430 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/cloner.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2725 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1640 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3157 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/form.py
+-rw-r--r--   0 maurits    (501) staff       (20)      770 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)      456 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/languageindependent.py
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4955 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/subscriber.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1100 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2994 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3338 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      366 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1571 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/itg.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8502 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)       67 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.161707 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.200215 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      113 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/reference_catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1344 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      343 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.200847 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2680 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types/LIF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2711 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types/LRF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      412 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.203683 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      211 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      418 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.162359 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.162037 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.204479 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1025 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.204799 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_3/
+-rw-r--r--   0 maurits    (501) staff       (20)      276 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.205087 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_4/
+-rw-r--r--   0 maurits    (501) staff       (20)      975 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2988 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/shared_uuid.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6530 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/subscriber.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9607 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      183 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.210723 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.212041 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3534 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_add_translation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3418 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_translate_content.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1434 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_alternates.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11045 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_api.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2147 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1878 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8744 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_form.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5819 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_helper_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9471 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_lif.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5354 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3299 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)      532 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    39142 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_selector.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4727 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3326 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8330 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_switcher.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1601 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_uninstall.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8055 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2687 2023-07-14 10:14:31.000000 plone.app.multilingual-8.0.0/src/plone/app/multilingual/upgrades.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:14:32.171456 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    43774 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7054 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      751 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 10:14:32.000000 plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/top_level.txt
```

### Comparing `plone.app.multilingual-7.0.2/CHANGES.rst` & `plone.app.multilingual-8.0.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-7.0.2 (2023-07-14)
+8.0.0 (2023-07-14)
 ------------------
 
+Breaking changes:
+
+
+- Make a core add-on by adding `Products.CMFPlone` to package dependencies.
+  [@folix-01] (#417)
+
+
 Bug fixes:
 
 
 - Do not unset the language on the Indonesian root language folder when saving the control panel.
   This language has ``id`` as code.  This is not allowed as an id in Plone, so it is created as ``id-id`` instead.
   This needs some special handling.
   Added upgrade to recursively fix this language folder to set the Indonesian language.  This is only done when the folder itself has the wrong language.
```

### Comparing `plone.app.multilingual-7.0.2/CREDITS.rst` & `plone.app.multilingual-8.0.0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/PKG-INFO` & `plone.app.multilingual-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 7.0.2
+Version: 8.0.0
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
 Keywords: language,multilingual,content
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -380,17 +380,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-7.0.2 (2023-07-14)
+8.0.0 (2023-07-14)
 ------------------
 
+Breaking changes:
+
+
+- Make a core add-on by adding `Products.CMFPlone` to package dependencies.
+  [@folix-01] (#417)
+
+
 Bug fixes:
 
 
 - Do not unset the language on the Indonesian root language folder when saving the control panel.
   This language has ``id`` as code.  This is not allowed as an id in Plone, so it is created as ``id-id`` instead.
   This needs some special handling.
   Added upgrade to recursively fix this language folder to set the Indonesian language.  This is only done when the folder itself has the wrong language.
```

### Comparing `plone.app.multilingual-7.0.2/README.rst` & `plone.app.multilingual-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/LICENSE.gpl` & `plone.app.multilingual-8.0.0/docs/LICENSE.gpl`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/LICENSE.txt` & `plone.app.multilingual-8.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/Makefile` & `plone.app.multilingual-8.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/conf.py` & `plone.app.multilingual-8.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/images/image00.png` & `plone.app.multilingual-8.0.0/docs/images/image00.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/images/image01.png` & `plone.app.multilingual-8.0.0/docs/images/image01.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/images/image02.png` & `plone.app.multilingual-8.0.0/docs/images/image02.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/images/image03.png` & `plone.app.multilingual-8.0.0/docs/images/image03.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/docs/images/image04.png` & `plone.app.multilingual-8.0.0/docs/images/image04.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/pyproject.toml` & `plone.app.multilingual-8.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/setup.cfg` & `plone.app.multilingual-8.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
-version = 7.0.2
+version = 8.0.0
 name = plone.app.multilingual
 description = Multilingual Plone Content package
 long_description = file: README.rst, CREDITS.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Plone
-	Framework :: Plone :: 6.0
+	Framework :: Plone :: 6.1
 	Framework :: Plone :: Core
 	Framework :: Zope :: 5
 	License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `plone.app.multilingual-7.0.2/setup.py` & `plone.app.multilingual-8.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "plone.i18n>=4.0.4",
         "setuptools",
         "BTrees",
         "Products.CMFCore",
+        "Products.CMFPlone",
         "Products.GenericSetup",
         "Products.statusmessages",
         "plone.app.content",
         "plone.app.contentmenu",
         "plone.app.dexterity",
         "plone.app.event",
         "plone.app.i18n",
```

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/api.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/api.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/add.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/configure.zcml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/controlpanel.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/edit.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/helper_views.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/helper_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/images/gtranslate.png` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/images/gtranslate.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/interfaces.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/babel_helper.js` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/babel_helper.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/jit-yc.js` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/jit-yc.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/javascript/mmap_helper.js` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/javascript/mmap_helper.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/menu.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/migrator.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/migrator.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/modify.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/selector.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/selector.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/setup.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/stylesheet/multilingual.css` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/stylesheet/multilingual.css`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/switcher.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/switcher.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/cleanup.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/cleanup.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/cleanup_results.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/cleanup_results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/controlpanel.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/dexterity_edit.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/dexterity_edit.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/disconnect_translation.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/disconnect_translation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/dx_babel_view.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/dx_babel_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/languages-notice.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/languages-notice.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/languageselector.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/languageselector.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/migration.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/migration.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/migrator-results.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/migrator-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/mmap.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/mmap.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/modify_translations.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/modify_translations.pt`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
               </td>
               <td class="align-middle text-center">
                 <tal:hastranslation condition="python:translation and translation != context">
                   <a class="pat-plone-modal disconnectTranslationAction"
                      href="#"
                      title="Disconnect translation"
                      tal:attributes="
-                       href string:${context/absolute_url}/disconnect_translation?came_from=${context/UID}&language=${lang};;
+                       href string:${context/absolute_url}/disconnect_translation?came_from=${context/UID}&language=${lang};;;
                      "
                      i18n:attributes="title disconnect_translation"
                   >
                     <img class="icon me-2"
                          alt=""
                          height="20"
                          src=""
```

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/not_translated_yet.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/not_translated_yet.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/reindex-results.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/reindex-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/templates/relocate-results.pt` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/templates/relocate-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/translate.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/translate.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/update.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/update.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/utils.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/viewlets.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/browser/vocabularies.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/browser/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/configure.zcml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lif.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lif.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/content/lrf.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/content/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/cloner.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/cloner.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/configure.zcml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/directives.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/form.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/interfaces.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/language.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/language.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/schemaeditor.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/subscriber.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/subscriber.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/dx/supermodel.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/dx/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/events.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/events.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/factory.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/factory.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/interfaces.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/itg.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/itg.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/manager.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/registry.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types/LIF.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types/LIF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/default/types/LRF.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/default/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/setuphandlers.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/shared_uuid.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/shared_uuid.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/subscriber.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/subscriber.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/testing.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_add_translation.robot` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_add_translation.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/robot/test_translate_content.robot` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/robot/test_translate_content.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_alternates.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_alternates.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_api.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_catalog.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_directives.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_form.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_helper_views.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_helper_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_lif.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_lif.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_lrf.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_menu.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_robot.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_selector.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_setup.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_sitemap.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_subscribers.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_switcher.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_switcher.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_uninstall.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/tests/test_vocabularies.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/upgrades.py` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone/app/multilingual/upgrades.zcml` & `plone.app.multilingual-8.0.0/src/plone/app/multilingual/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/PKG-INFO` & `plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 7.0.2
+Version: 8.0.0
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
 Keywords: language,multilingual,content
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -380,17 +380,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-7.0.2 (2023-07-14)
+8.0.0 (2023-07-14)
 ------------------
 
+Breaking changes:
+
+
+- Make a core add-on by adding `Products.CMFPlone` to package dependencies.
+  [@folix-01] (#417)
+
+
 Bug fixes:
 
 
 - Do not unset the language on the Indonesian root language folder when saving the control panel.
   This language has ``id`` as code.  This is not allowed as an id in Plone, so it is created as ``id-id`` instead.
   This needs some special handling.
   Added upgrade to recursively fix this language folder to set the Indonesian language.  This is only done when the folder itself has the wrong language.
```

### Comparing `plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/SOURCES.txt` & `plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-7.0.2/src/plone.app.multilingual.egg-info/requires.txt` & `plone.app.multilingual-8.0.0/src/plone.app.multilingual.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 plone.i18n>=4.0.4
 setuptools
 BTrees
 Products.CMFCore
+Products.CMFPlone
 Products.GenericSetup
 Products.statusmessages
 plone.app.content
 plone.app.contentmenu
 plone.app.dexterity
 plone.app.event
 plone.app.i18n
```

