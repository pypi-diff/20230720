# Comparing `tmp/pas.plugins.oidc-1.0a5.tar.gz` & `tmp/pas.plugins.oidc-1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pas.plugins.oidc-1.0a5.tar", last modified: Tue Apr  4 22:05:00 2023, max compression
+gzip compressed data, was "pas.plugins.oidc-1.0a6.tar", last modified: Thu Jul 20 15:53:50 2023, max compression
```

## Comparing `pas.plugins.oidc-1.0a5.tar` & `pas.plugins.oidc-1.0a6.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1045 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      121 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      653 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       60 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9122 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6723 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.023533 pas.plugins.oidc-1.0a5/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7899 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       71 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      543 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2692 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.023533 pas.plugins.oidc-1.0a5/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.023533 pas.plugins.oidc-1.0a5/src/pas/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      692 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1043 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11759 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/view.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1651 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      264 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.023533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/en/LC_MESSAGES/pas.plugins.oidc.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/pas.plugins.oidc.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1781 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      485 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16580 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/plugins.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.023533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       88 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      126 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4137 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1553 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4599 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_functional.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1731 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_plugin.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2343 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1971 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/utils.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-04-04 22:05:00.027533 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9122 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1506 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      121 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       16 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      157 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        4 2023-04-04 22:04:59.000000 pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1303 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      160 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      572 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      653 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       60 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12249 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9582 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7899 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       71 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      543 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2649 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas/plugins/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      692 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1043 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11641 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/view.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1651 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      264 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      603 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      887 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/en/LC_MESSAGES/pas.plugins.oidc.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/es/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1399 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/es/LC_MESSAGES/pas.plugins.oidc.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1006 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/pas.plugins.oidc.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1781 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      485 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16799 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/plugins.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       88 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      126 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4137 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1478 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.388388 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4599 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_functional.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1731 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_plugin.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2343 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1971 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/utils.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 15:53:50.384388 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12249 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1570 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      121 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       16 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      143 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        4 2023-07-20 15:53:50.000000 pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/top_level.txt
```

### Comparing `pas.plugins.oidc-1.0a5/CHANGES.rst` & `pas.plugins.oidc-1.0a6/CHANGES.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+1.0a6 (2023-07-20)
+------------------
+
+- Added Spanish translation
+  [macagua]
+
+- Added improvements about i18n support
+  [macagua]
+
+- Drop python 2.7 and Plone 4 support
+  [erral]
+
+- Add support for the post_logout parameter for logout api.
+  [ramiroluz]
+
+
 1.0a5 (2023-04-05)
 ------------------
 
 - Catch exceptions during the OAuth process
   [erral]
 - Update the plugin to make challenges.
   An anonymous user who visits a page for which you have to be authenticated,
```

### Comparing `pas.plugins.oidc-1.0a5/LICENSE.GPL` & `pas.plugins.oidc-1.0a6/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/LICENSE.rst` & `pas.plugins.oidc-1.0a6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/docs/conf.py` & `pas.plugins.oidc-1.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/setup.cfg` & `pas.plugins.oidc-1.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/setup.py` & `pas.plugins.oidc-1.0a6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,25 +12,26 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="pas.plugins.oidc",
-    version='1.0a5',
+    version="1.0a6",
     description="An add-on for Plone",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
@@ -47,21 +48,20 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["pas", "pas.plugins"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
+    python_requires=">=3.7",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "z3c.jbot",
         "plone.api>=1.8.4",
-        "plone.restapi",
         # 'oidcrp',
         # "oic<1; python_version < 3",
         "oic",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
```

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/__init__.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/configure.zcml` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/browser/view.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/browser/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,14 @@
     # Python 2
     from urllib import quote
 
 
 logger = logging.getLogger(__name__)
 
 
-# https://zope.readthedocs.io/en/latest/zopebook/Sessions.html#alternative-server-side-session-backends-for-zope-4
-# in produzione usare: https://pypi.org/project/Products.mcdutils/
-# XXX: attualmente implementata sessione su cookie
 class Session(object):
     session_cookie_name = "__ac_session"
     _session = {}
 
     def __init__(self, request, use_session_data_manager=False):
         self.request = request
         self.use_session_data_manager = use_session_data_manager
@@ -186,20 +183,23 @@
 
         redirect_uri = api.portal.get().absolute_url()
 
         # Volto frontend mapping exception
         if redirect_uri.endswith('/api'):
             redirect_uri = redirect_uri[:-4]
 
-        args = {
-            # 'state': session.get('end_session_state'),
-            # TODO: ....
-            # 'post_logout_redirect_uri': api.portal.get().absolute_url(),
-            "redirect_uri": redirect_uri,
-        }
+        if self.context.getProperty("use_deprecated_redirect_uri_for_logout"):
+            args = {
+                "redirect_uri": redirect_uri,
+                }
+        else:
+            args = {
+                "post_logout_redirect_uri": redirect_uri,
+                "client_id": self.context.getProperty("client_id"),
+                }
 
         pas = getToolByName(self.context, "acl_users")
         auth_cookie_name = pas.credentials_cookie_auth.cookie_name
 
         # end_req = client.construct_EndSessionRequest(request_args=args)
         end_req = EndSessionRequest(**args)
         logout_url = end_req.request(client.end_session_endpoint)
@@ -249,15 +249,15 @@
         resp = client.do_access_token_request(
             state=aresp["state"],
             request_args=args,
             authn_method="client_secret_basic",
         )
 
         if isinstance(resp, AccessTokenResponse):
-            # If it’s an AccessTokenResponse the information in the response will be stored in the
+            # If it's an AccessTokenResponse the information in the response will be stored in the
             # client instance with state as the key for future use.
             if client.userinfo_endpoint:
                 # https://openid.net/specs/openid-connect-core-1_0.html#UserInfo
 
                 # XXX: Not completely sure if this is even needed
                 #      We do not have a OpenID connect provider with userinfo endpoint
                 #      enabled and with the weird treatment of boolean values, so we cannot test this
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/configure.zcml` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/configure.zcml`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/README.rst` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     $ mkdir de
 
 For updating locales
 
 .. code-block:: console
 
-    $ ./bin/update_locale
+    $ ./update.sh
 
 Note
 ----
 
 The script uses gettext package for internationalization.
 
 Install it before running the script.
```

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/locales/update.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/locales/update.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/plugins.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     create_ticket = True
     create_restapi_ticket = False
     create_user = True
     create_groups = False
     user_property_as_groupid = "groups"
     scope = ("profile", "email", "phone")
     use_pkce = False
+    use_deprecated_redirect_uri_for_logout = False
     use_modified_openid_schema = False
     user_property_as_userid = "sub"
 
     _properties = (
         dict(id="issuer", type="string", mode="w", label="OIDC/Oauth2 Issuer"),
         dict(id="client_id", type="string", mode="w", label="Client ID"),
         dict(id="client_secret", type="string", mode="w", label="Client secret"),
@@ -122,14 +123,15 @@
         dict(
             id="scope",
             type="lines",
             mode="w",
             label="Open ID scopes to request to the server",
         ),
         dict(id="use_pkce", type="boolean", mode="w", label="Use PKCE. "),
+        dict(id="use_deprecated_redirect_uri_for_logout", type="boolean", mode="w", label="Use deprecated redirect_uri for logout url(/Plone/acl_users/oidc/logout)."),
         dict(
             id="use_modified_openid_schema",
             type="boolean",
             mode="w",
             label="Use a modified OpenID Schema for email_verified and phone_number_verified boolean values coming as string. ",
         ),
         dict(
```

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/setuphandlers.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/testing.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/testing.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
-        import plone.restapi
-
-        self.loadZCML(package=plone.restapi)
         self.loadZCML(package=pas.plugins.oidc)
 
     def setUpPloneSite(self, portal):
         applyProfile(portal, "pas.plugins.oidc:default")
 
 
 PAS_PLUGINS_OIDC_FIXTURE = PasPluginsOidcLayer()
```

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_functional.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_plugin.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/tests/test_setup.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas/plugins/oidc/utils.py` & `pas.plugins.oidc-1.0a6/src/pas/plugins/oidc/utils.py`

 * *Files identical despite different names*

### Comparing `pas.plugins.oidc-1.0a5/src/pas.plugins.oidc.egg-info/SOURCES.txt` & `pas.plugins.oidc-1.0a6/src/pas.plugins.oidc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/pas/plugins/oidc/browser/view.py
 src/pas/plugins/oidc/locales/README.rst
 src/pas/plugins/oidc/locales/__init__.py
 src/pas/plugins/oidc/locales/pas.plugins.oidc.pot
 src/pas/plugins/oidc/locales/update.py
 src/pas/plugins/oidc/locales/update.sh
 src/pas/plugins/oidc/locales/en/LC_MESSAGES/pas.plugins.oidc.po
+src/pas/plugins/oidc/locales/es/LC_MESSAGES/pas.plugins.oidc.po
 src/pas/plugins/oidc/profiles/default/browserlayer.xml
 src/pas/plugins/oidc/profiles/default/metadata.xml
 src/pas/plugins/oidc/profiles/uninstall/browserlayer.xml
 src/pas/plugins/oidc/tests/__init__.py
 src/pas/plugins/oidc/tests/test_functional.py
 src/pas/plugins/oidc/tests/test_plugin.py
 src/pas/plugins/oidc/tests/test_setup.py
```

