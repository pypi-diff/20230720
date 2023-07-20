# Comparing `tmp/collective.dms.scanbehavior-1.1.tar.gz` & `tmp/collective.dms.scanbehavior-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.dms.scanbehavior-1.1.tar", last modified: Thu Jan  4 14:27:20 2018, max compression
+gzip compressed data, was "collective.dms.scanbehavior-1.2.tar", last modified: Thu Jul 20 09:08:36 2023, max compression
```

## Comparing `collective.dms.scanbehavior-1.1.tar` & `collective.dms.scanbehavior-1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1030 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       86 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3914 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      231 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      888 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/upgrades.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      241 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       68 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/default/collectivedmsscanbehavior_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      544 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4811 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      275 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/interfaces.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1301 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      633 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/test_robot.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1392 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/robot/test_scanbehavior.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/robot/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      251 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1069 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/browser/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      364 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/browser/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      184 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1959 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/behaviors.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1760 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/collective.dms.scanbehavior.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1805 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/collective.dms.scanbehavior.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      152 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/update.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3914 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2069 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      193 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      241 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2018-01-04 14:27:20.000000 collective.dms.scanbehavior-1.1/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1729 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1152 2018-01-04 14:27:19.000000 collective.dms.scanbehavior-1.1/CHANGES.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1244 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       86 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      241 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2950 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1030 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      732 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/docs/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1729 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      231 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      184 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/__init__.py
+-rwxrwxr-x   0 sge       (1000) sge       (1000)     2057 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/behaviors.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      696 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      364 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/browser/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/browser/static/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1069 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      275 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1760 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/collective.dms.scanbehavior.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1805 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/collective.dms.scanbehavior.po
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      152 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/update.sh
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      181 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      329 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/default/collectivedmsscanbehavior_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       68 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/default/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      241 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/profiles/testing/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      251 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4811 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      544 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/robot/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1392 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/robot/test_scanbehavior.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)      633 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1301 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      888 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/upgrades.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-07-20 09:08:36.493587 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2950 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2069 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       26 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      193 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-07-20 09:08:36.000000 collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.dms.scanbehavior-1.1/docs/LICENSE.rst` & `collective.dms.scanbehavior-1.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/docs/LICENSE.GPL` & `collective.dms.scanbehavior-1.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/README.rst` & `collective.dms.scanbehavior-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/upgrades.py` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/testing.zcml` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/testing.py` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/testing.py`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/test_setup.py` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/test_robot.py` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/tests/robot/test_scanbehavior.robot` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/tests/robot/test_scanbehavior.robot`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/configure.zcml` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/behaviors.py` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/behaviors.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.indexer import indexer
 from plone.supermodel import model
 from Products.CMFPlone.utils import base_hasattr
 from Products.PluginIndexes.common.UnIndex import _marker
 from collective.dms.scanbehavior import _
 
+import datetime
 
 class IScanFields(model.Schema):
 
     model.fieldset(
         'scan',
         label=_(u'Scan'),
         fields=(
@@ -51,14 +52,16 @@
 
     scan_date = schema.Datetime(
         title=_(
             u'scan_date',
             default=u'Scan date',
         ),
         required=False,
+        min=datetime.datetime(1990, 1, 1),
+        max=datetime.datetime.today(),
     )
 
     scan_user = schema.TextLine(
         title=_(
             u'scan_user',
             default=u'Scan user',
         ),
```

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/behaviors/configure.zcml` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/collective.dms.scanbehavior.pot` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/collective.dms.scanbehavior.pot`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/collective.dms.scanbehavior.po` & `collective.dms.scanbehavior-1.2/src/collective/dms/scanbehavior/locales/fr/LC_MESSAGES/collective.dms.scanbehavior.po`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/src/collective.dms.scanbehavior.egg-info/SOURCES.txt` & `collective.dms.scanbehavior-1.2/src/collective.dms.scanbehavior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.dms.scanbehavior-1.1/setup.py` & `collective.dms.scanbehavior-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='collective.dms.scanbehavior',
-    version='1.1',
+    version='1.2',
     description="Behavior adding scan metadata",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `collective.dms.scanbehavior-1.1/CHANGES.rst` & `collective.dms.scanbehavior-1.2/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+1.2 (2023-07-20)
+----------------
+
+- fix : [DMS-949] min & max for scan_date
+  [bleybaert]
+
 1.1 (2018-01-04)
 ----------------
 
 - Added field `to_sign` to the behavior.
   [gbastien]
 
 1.0 (2017-05-30)
```

