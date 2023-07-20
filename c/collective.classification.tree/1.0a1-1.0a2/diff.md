# Comparing `tmp/collective.classification.tree-1.0a1.tar.gz` & `tmp/collective.classification.tree-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.classification.tree-1.0a1.tar", last modified: Wed Mar 29 08:35:17 2023, max compression
+gzip compressed data, was "collective.classification.tree-1.0a2.tar", last modified: Thu Jul 20 08:24:26 2023, max compression
```

## Comparing `collective.classification.tree-1.0a1.tar` & `collective.classification.tree-1.0a2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/
--rw-rw-r--   0 sge       (1000) sge       (1000)       93 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       62 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      675 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     3789 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2583 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/README.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7939 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/docs/conf.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      113 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/docs/index.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       39 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      525 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     2995 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/
--rw-rw-r--   0 sge       (1000) sge       (1000)      147 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1593 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/classification.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      581 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4413 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/actions.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2706 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/category.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3265 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      702 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/container.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2681 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/container.py.back
--rw-rw-r--   0 sge       (1000) sge       (1000)      908 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/helper.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/overrides/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/overrides/.gitkeep
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/static/.gitkeep
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/templates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4346 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/templates/container.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2326 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/templates/delete_confirmation.pt
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3622 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/browser/tests/test_categories.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      857 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/caching.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3098 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6018 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/category.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2117 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/common.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1008 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2477 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/container.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     5639 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/contents/tests/test_categories.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/form/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      937 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)    11539 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/importform.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/form/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    47212 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/tests/test_importform.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      435 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/form/validation.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      278 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/interfaces.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)      611 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4955 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/collective.classification.tree.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4819 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/en/LC_MESSAGES/collective.classification.tree.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     6285 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/fr/LC_MESSAGES/collective.classification.tree.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1586 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/update.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      527 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      260 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/permissions.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2224 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/actions.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      215 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      239 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      258 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/metadata.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/registry/
--rw-rw-r--   0 sge       (1000) sge       (1000)      188 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/registry/main.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      118 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/rolemap.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1022 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types/ClassificationCategory.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2416 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types/ClassificationContainer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      261 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/uninstall/
--rw-rw-r--   0 sge       (1000) sge       (1000)      140 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)    11663 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/script.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/src/collective/classification/tree/serializer/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/serializer/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1611 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/serializer/category.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      263 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/serializer/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/src/collective/classification/tree/services/
--rw-rw-r--   0 sge       (1000) sge       (1000)       24 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/services/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      610 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/services/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3800 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/services/tree.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      607 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1915 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/testing.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.521293 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2051 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/robot/test_example.robot
--rw-rw-r--   0 sge       (1000) sge       (1000)      984 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2696 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    20436 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4751 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_vocabularies.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     9269 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6956 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective/classification/tree/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-03-29 08:35:17.517292 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     3789 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     4746 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      383 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      338 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-03-29 08:35:17.000000 collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/top_level.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      171 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       62 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      675 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       81 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3849 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2583 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7939 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/docs/conf.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      113 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/docs/index.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       39 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      525 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2977 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/tree/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      147 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1593 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/classification.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      581 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4413 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/actions.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2706 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/category.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3265 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      702 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/container.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2681 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/container.py.back
+-rw-rw-r--   0 sge       (1000) sge       (1000)      908 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/helper.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/overrides/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/overrides/.gitkeep
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/static/.gitkeep
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4346 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/templates/container.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2326 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/templates/delete_confirmation.pt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3622 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/browser/tests/test_categories.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      857 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/caching.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3098 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6018 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/category.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2117 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/common.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1008 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2477 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/container.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5639 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/contents/tests/test_categories.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/form/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      937 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)    11539 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/importform.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/form/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    47212 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/tests/test_importform.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      435 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/form/validation.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      278 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      611 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4955 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/collective.classification.tree.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4819 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/en/LC_MESSAGES/collective.classification.tree.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6285 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/fr/LC_MESSAGES/collective.classification.tree.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1586 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/update.py
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      527 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/locales/update.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)      260 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/permissions.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2224 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/actions.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      215 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      239 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      258 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/registry/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      188 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/registry/main.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      118 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/rolemap.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1022 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types/ClassificationCategory.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2416 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types/ClassificationContainer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      261 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/uninstall/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      140 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)    11663 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/script.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/serializer/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/serializer/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1611 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/serializer/category.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      263 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/serializer/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/services/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       24 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/services/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      610 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/services/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3800 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/services/tree.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      607 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1915 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/testing.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.155501 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2051 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/robot/test_example.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)      984 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2696 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    20436 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4751 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_vocabularies.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9269 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6956 2023-07-20 08:24:25.000000 collective.classification.tree-1.0a2/src/collective/classification/tree/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 08:24:26.151501 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3849 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4746 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      383 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      338 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-07-20 08:24:26.000000 collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/top_level.txt
```

### Comparing `collective.classification.tree-1.0a1/LICENSE.GPL` & `collective.classification.tree-1.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/LICENSE.rst` & `collective.classification.tree-1.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/PKG-INFO` & `collective.classification.tree-1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.classification.tree
-Version: 1.0a1
+Version: 1.0a2
 Summary: Addon to manage complex content classification tree
-Home-page: https://github.com/collective/collective.classification.tree
+Home-page: https://github.com/imio/collective.classification.tree
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.tree
-Project-URL: Source, https://github.com/collective/collective.classification.tree
-Project-URL: Tracker, https://github.com/collective/collective.classification.tree/issues
+Project-URL: Source, https://github.com/imio/collective.classification.tree
+Project-URL: Tracker, https://github.com/imio/collective.classification.tree/issues
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
+- Corrected setup urls.
+  [sgeulette]
+
 1.0a1 (2023-03-29)
 ------------------
 
 - Initial release.
   [mpeeters]
```

### Comparing `collective.classification.tree-1.0a1/README.rst` & `collective.classification.tree-1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/docs/conf.py` & `collective.classification.tree-1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/setup.cfg` & `collective.classification.tree-1.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/setup.py` & `collective.classification.tree-1.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.classification.tree",
-    version="1.0a1",
+    version="1.0a2",
     description="Addon to manage complex content classification tree",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -29,19 +29,19 @@
         "Programming Language :: Python :: 2.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone CMS",
     author="Martin Peeters",
     author_email="support@imio.be",
-    url="https://github.com/collective/collective.classification.tree",
+    url="https://github.com/imio/collective.classification.tree",
     project_urls={
         "PyPI": "https://pypi.python.org/pypi/collective.classification.tree",
-        "Source": "https://github.com/collective/collective.classification.tree",
-        "Tracker": "https://github.com/collective/collective.classification.tree/issues",
+        "Source": "https://github.com/imio/collective.classification.tree",
+        "Tracker": "https://github.com/imio/collective.classification.tree/issues",
         # 'Documentation': 'https://collective.classification.tree.readthedocs.io/en/latest/',
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["collective", "collective.classification"],
     package_dir={"": "src"},
     include_package_data=True,
```

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/classification.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/classification.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/behaviors/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/actions.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/actions.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/category.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/category.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/container.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/container.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/container.py.back` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/container.py.back`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/helper.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/helper.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/templates/container.pt` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/templates/container.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/templates/delete_confirmation.pt` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/templates/delete_confirmation.pt`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/browser/tests/test_categories.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/browser/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/caching.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/caching.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/contents/category.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/contents/category.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/contents/common.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/contents/common.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/contents/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/contents/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/contents/container.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/contents/container.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/contents/tests/test_categories.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/contents/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/form/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/form/importform.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/form/importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/form/tests/test_importform.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/form/tests/test_importform.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/README.rst` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/collective.classification.tree.pot` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/collective.classification.tree.pot`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/en/LC_MESSAGES/collective.classification.tree.po` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/en/LC_MESSAGES/collective.classification.tree.po`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/fr/LC_MESSAGES/collective.classification.tree.po` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/fr/LC_MESSAGES/collective.classification.tree.po`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/update.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/locales/update.sh` & `collective.classification.tree-1.0a2/src/collective/classification/tree/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/actions.xml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types/ClassificationCategory.xml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types/ClassificationCategory.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/profiles/default/types/ClassificationContainer.xml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/profiles/default/types/ClassificationContainer.xml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/script.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/script.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/serializer/category.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/serializer/category.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/services/configure.zcml` & `collective.classification.tree-1.0a2/src/collective/classification/tree/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/services/tree.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/services/tree.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/setuphandlers.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/testing.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/testing.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/tests/robot/test_example.robot` & `collective.classification.tree-1.0a2/src/collective/classification/tree/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_robot.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_setup.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_utils.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/tests/test_vocabularies.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/utils.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/utils.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective/classification/tree/vocabularies.py` & `collective.classification.tree-1.0a2/src/collective/classification/tree/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/PKG-INFO` & `collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.classification.tree
-Version: 1.0a1
+Version: 1.0a2
 Summary: Addon to manage complex content classification tree
-Home-page: https://github.com/collective/collective.classification.tree
+Home-page: https://github.com/imio/collective.classification.tree
 Author: Martin Peeters
 Author-email: support@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.classification.tree
-Project-URL: Source, https://github.com/collective/collective.classification.tree
-Project-URL: Tracker, https://github.com/collective/collective.classification.tree/issues
+Project-URL: Source, https://github.com/imio/collective.classification.tree
+Project-URL: Tracker, https://github.com/imio/collective.classification.tree/issues
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
+- Corrected setup urls.
+  [sgeulette]
+
 1.0a1 (2023-03-29)
 ------------------
 
 - Initial release.
   [mpeeters]
```

### Comparing `collective.classification.tree-1.0a1/src/collective.classification.tree.egg-info/SOURCES.txt` & `collective.classification.tree-1.0a2/src/collective.classification.tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

