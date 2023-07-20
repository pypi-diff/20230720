# Comparing `tmp/collective.immediatecreate-2.0.0.tar.gz` & `tmp/collective.immediatecreate-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.immediatecreate-2.0.0.tar", last modified: Wed Jun 14 08:27:58 2023, max compression
+gzip compressed data, was "collective.immediatecreate-2.0.1.tar", last modified: Thu Jul 20 14:46:50 2023, max compression
```

## Comparing `collective.immediatecreate-2.0.0.tar` & `collective.immediatecreate-2.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      379 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/CHANGES.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      148 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/CONTRIBUTORS.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    18092 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/LICENSE.GPL
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      670 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/LICENSE.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      137 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/MANIFEST.in
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     6456 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     5076 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/README.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       55 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/constraints.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      123 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/requirements.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      245 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/setup.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1692 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/setup.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.309770 collective.immediatecreate-2.0.0/src/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      119 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/__init__.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1785 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/adding.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      327 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/behaviors.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1215 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/cleanup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2393 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/configure.zcml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3929 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/editing.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      417 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/events.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      268 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/indexer.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      251 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/interfaces.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/collective.immediatecreate.pot
--rwxrwxr-x   0 jensens   (1000) jensens   (1000)      515 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/update.sh
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.309770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      197 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/browserlayer.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      201 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/catalog.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      195 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/metadata.xml
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      129 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      173 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/catalog.xml
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      571 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/setuphandlers.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1965 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/testing.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)   218068 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_image.jpg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4229 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2556 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_adding.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      934 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_robot.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2302 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_setup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      171 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/upgrades.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      404 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/upgrades.zcml
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     6456 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1925 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/SOURCES.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/dependency_links.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       40 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/entry_points.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/namespace_packages.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/not-zip-safe
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      117 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/requires.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/top_level.txt
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      519 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/CHANGES.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      148 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/CONTRIBUTORS.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    18092 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/LICENSE.GPL
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      670 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/LICENSE.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      137 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/MANIFEST.in
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6596 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     5076 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/README.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       55 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/constraints.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      123 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/requirements.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      245 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/setup.cfg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1692 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/setup.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.457207 collective.immediatecreate-2.0.1/src/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.461207 collective.immediatecreate-2.0.1/src/collective/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.469207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      119 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1785 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/adding.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      327 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/behaviors.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1215 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/cleanup.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2393 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/configure.zcml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4000 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/editing.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      417 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/events.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      268 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/indexer.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      251 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/interfaces.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.469207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/locales/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/locales/collective.immediatecreate.pot
+-rwxrwxr-x   0 jensens   (1000) jensens   (1000)      515 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/locales/update.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.461207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.469207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/default/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      197 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/default/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      201 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/default/catalog.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      195 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/default/metadata.xml
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/uninstall/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      129 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      173 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/profiles/uninstall/catalog.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      571 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/setuphandlers.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1965 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/testing.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.473207 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/robot/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)   218068 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/robot/test_image.jpg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4229 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2556 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_adding.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      934 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_robot.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2302 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_setup.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      171 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/upgrades.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      404 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective/immediatecreate/upgrades.zcml
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-20 14:46:50.469207 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6596 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1925 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       40 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/entry_points.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/not-zip-safe
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      117 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-07-20 14:46:50.000000 collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/top_level.txt
```

### Comparing `collective.immediatecreate-2.0.0/LICENSE.GPL` & `collective.immediatecreate-2.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/LICENSE.rst` & `collective.immediatecreate-2.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/PKG-INFO` & `collective.immediatecreate-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.immediatecreate
-Version: 2.0.0
+Version: 2.0.1
 Summary: Create dexterity items immediatly and skips add form.
 Home-page: https://pypi.python.org/pypi/collective.immediatecreate
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -167,14 +167,21 @@
 - Gogo Bernhard, g.bernhard@akbild.ac.at
 - Markus Hilbert, markus.hilbert@iham.at
 
 
 Changelog
 =========
 
+2.0.1 (2023-07-20)
+------------------
+
+- Fix cancel button on form validation if immediate create for has a validation error.
+  [jensens]
+
+
 2.0.0 (2023-06-14)
 ------------------
 
 - Towards Plone 6, Python 3 (only).
   [jensens]
 
 1.0a3 (2018-11-07)
```

### Comparing `collective.immediatecreate-2.0.0/README.rst` & `collective.immediatecreate-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/setup.py` & `collective.immediatecreate-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.immediatecreate",
-    version="2.0.0",
+    version="2.0.1",
     description="Create dexterity items immediatly and skips add form.",
     long_description=long_description,
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 6.0",
```

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/adding.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/adding.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/cleanup.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/cleanup.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/configure.zcml` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/editing.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/editing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from Acquisition import aq_parent
 from collective.immediatecreate import _
 from plone import api
 from plone.app.lockingbehavior.behaviors import ILocking
+from plone.app.z3cform.views import BootstrapActions
 from plone.dexterity.browser.base import DexterityExtensibleForm
 from plone.dexterity.events import EditBegunEvent
 from plone.dexterity.events import EditCancelledEvent
 from plone.dexterity.events import EditFinishedEvent
 from plone.dexterity.i18n import MessageFactory as _dx
 from plone.dexterity.interfaces import IDexterityEditForm
 from plone.dexterity.interfaces import IDexterityFTI
@@ -18,15 +19,15 @@
 from zExceptions import Redirect
 from zope.component import getUtility
 from zope.container.interfaces import INameChooser
 from zope.event import notify
 from zope.interface import classImplements
 
 
-class ImmediateEditForm(DexterityExtensibleForm, form.EditForm):
+class ImmediateEditForm(DexterityExtensibleForm, BootstrapActions, form.EditForm):
 
     success_message = _("New content saved")
 
     @button.buttonAndHandler(_dx("Save"), name="save")
     def handleApply(self, action):
         data, errors = self.extractData()
         if errors:
```

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/update.sh` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/setuphandlers.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/testing.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/testing.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_image.jpg` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/robot/test_image.jpg`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_adding.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_adding.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_robot.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_setup.py` & `collective.immediatecreate-2.0.1/src/collective/immediatecreate/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/PKG-INFO` & `collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.immediatecreate
-Version: 2.0.0
+Version: 2.0.1
 Summary: Create dexterity items immediatly and skips add form.
 Home-page: https://pypi.python.org/pypi/collective.immediatecreate
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -167,14 +167,21 @@
 - Gogo Bernhard, g.bernhard@akbild.ac.at
 - Markus Hilbert, markus.hilbert@iham.at
 
 
 Changelog
 =========
 
+2.0.1 (2023-07-20)
+------------------
+
+- Fix cancel button on form validation if immediate create for has a validation error.
+  [jensens]
+
+
 2.0.0 (2023-06-14)
 ------------------
 
 - Towards Plone 6, Python 3 (only).
   [jensens]
 
 1.0a3 (2018-11-07)
```

### Comparing `collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/SOURCES.txt` & `collective.immediatecreate-2.0.1/src/collective.immediatecreate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

