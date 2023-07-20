# Comparing `tmp/collective.dms.mailcontent-1.8.tar.gz` & `tmp/collective.dms.mailcontent-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.dms.mailcontent-1.8.tar", last modified: Thu Mar 17 15:58:36 2022, max compression
+gzip compressed data, was "collective.dms.mailcontent-1.9.tar", last modified: Fri Mar 25 08:34:18 2022, max compression
```

## Comparing `collective.dms.mailcontent-1.8.tar` & `collective.dms.mailcontent-1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)      173 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/.gitignore
--rw-rw-r--   0 sge       (1000) sge       (1000)      398 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/.travis.yml
--rw-rw-r--   0 sge       (1000) sge       (1000)     5437 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      138 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       78 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     9290 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      726 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      381 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     6158 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/bootstrap.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      141 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/buildout.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      284 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/checkouts.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      738 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/docs/LICENSE.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      727 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/jenkins-base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       96 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/jenkins.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       43 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     2183 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1243 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/sources.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/
--rw-rw-r--   0 sge       (1000) sge       (1000)      639 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      874 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/behaviors.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      422 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/behaviors.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1736 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     6270 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/reply_form.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4232 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/settings.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      406 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3524 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/views.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3258 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      760 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsincomingmail_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)    14074 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsmail.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      767 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsoutgoingmail_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)     3230 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/indexers.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4129 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/collective.dms.mailcontent.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4064 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/collective.dms.mailcontent.po
--rw-rw-r--   0 sge       (1000) sge       (1000)      956 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     5771 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/collective.dms.mailcontent.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1046 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)      917 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/manual.pot
--rw-rw-r--   0 sge       (1000) sge       (1000)     1021 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/plone.pot
--rwxrwxr-x   0 sge       (1000) sge       (1000)      256 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      415 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/permissions.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      844 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)       14 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/collective_dms_mailcontent_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      544 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      526 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/import_steps.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      381 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      125 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      485 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/rolemap.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2394 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types/dmsincomingmail.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2309 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types/dmsoutgoingmail.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      297 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      177 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/collectivedmsmailcontent_testing_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      247 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      638 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/registry.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1909 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/types/testtype.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      230 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/types.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1558 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      664 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      556 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/testing.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1564 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_behaviors.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6378 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_content.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4354 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_indexers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3702 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_reply_form.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    14525 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_settings.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.111487 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2720 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     4327 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2483 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-17 15:58:36.107488 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     9290 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     3713 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       26 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      287 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-03-17 15:58:36.000000 collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      128 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/travis.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1082 2022-03-17 15:58:35.000000 collective.dms.mailcontent-1.8/versions.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      173 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/.gitignore
+-rw-rw-r--   0 sge       (1000) sge       (1000)      398 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/.travis.yml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5609 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      138 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       78 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9526 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      726 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      381 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/base.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6158 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/bootstrap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      141 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      284 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/checkouts.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      738 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/docs/LICENSE.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      727 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/jenkins-base.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       96 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/jenkins.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       43 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2183 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1243 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/sources.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      639 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      874 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/behaviors.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      422 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/behaviors.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1736 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6270 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/reply_form.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4232 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/settings.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      406 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3524 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3258 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      760 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsincomingmail_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)    14074 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsmail.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      767 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsoutgoingmail_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3230 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/indexers.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4290 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/collective.dms.mailcontent.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4225 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/collective.dms.mailcontent.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)      956 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5971 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/collective.dms.mailcontent.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1046 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1078 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/manual.pot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1021 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/plone.pot
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      256 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/update.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)      415 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/permissions.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      844 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)       14 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/collective_dms_mailcontent_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      544 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/controlpanel.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      526 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/import_steps.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      381 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      125 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      485 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/rolemap.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2394 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types/dmsincomingmail.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2309 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types/dmsoutgoingmail.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      297 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      177 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/collectivedmsmailcontent_testing_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      247 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      638 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/registry.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1909 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/types/testtype.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      230 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/types.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1558 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      664 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      556 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1564 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_behaviors.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6378 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_content.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4354 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_indexers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3702 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_reply_form.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    14525 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_settings.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2720 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4327 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/upgrades.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2902 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/vocabularies.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-03-25 08:34:18.204123 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9526 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3713 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       81 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       26 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      287 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-03-25 08:34:18.000000 collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      128 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/travis.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1082 2022-03-25 08:34:17.000000 collective.dms.mailcontent-1.9/versions.cfg
```

### Comparing `collective.dms.mailcontent-1.8/CHANGES.rst` & `collective.dms.mailcontent-1.9/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.9 (2022-03-25)
+----------------
+
+- When listing attachments, do not include filename if it's the same than title.
+  [sgeulette]
+- Marked signed attachment
+  [sgeulette]
+
 1.8 (2022-03-17)
 ----------------
 
 - Made separate `add_content` method to be overrided.
   [sgeulette]
 
 1.7 (2022-02-10)
```

### Comparing `collective.dms.mailcontent-1.8/PKG-INFO` & `collective.dms.mailcontent-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.dms.mailcontent
-Version: 1.8
+Version: 1.9
 Summary: Mail content type for document management system
 Home-page: https://github.com/collective/collective.dms.mailcontent
 Author: Ecreall, Entrouvert, IMIO
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Download-URL: https://pypi.org/project/collective.dms.mailcontent
 Description: Introduction
@@ -39,14 +39,22 @@
         - Vincent Fretin, Ecreall
         - Cédric Messiant, Ecreall
         - Frédéric Peters, Entr'ouvert
         
         Changelog
         =========
         
+        1.9 (2022-03-25)
+        ----------------
+        
+        - When listing attachments, do not include filename if it's the same than title.
+          [sgeulette]
+        - Marked signed attachment
+          [sgeulette]
+        
         1.8 (2022-03-17)
         ----------------
         
         - Made separate `add_content` method to be overrided.
           [sgeulette]
         
         1.7 (2022-02-10)
```

### Comparing `collective.dms.mailcontent-1.8/README.rst` & `collective.dms.mailcontent-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/bootstrap.py` & `collective.dms.mailcontent-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/docs/LICENSE.GPL` & `collective.dms.mailcontent-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/docs/LICENSE.txt` & `collective.dms.mailcontent-1.9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/jenkins-base.cfg` & `collective.dms.mailcontent-1.9/jenkins-base.cfg`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/setup.py` & `collective.dms.mailcontent-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! -*- coding: utf8 -*-
 
 from setuptools import setup, find_packages
 
-version = '1.8'
+version = '1.9'
 
 long_description = (
     open('README.rst').read()
     + '\n' +
     'Contributors\n'
     '============\n'
     + '\n' +
```

### Comparing `collective.dms.mailcontent-1.8/sources.cfg` & `collective.dms.mailcontent-1.9/sources.cfg`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/__init__.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/behaviors.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/configure.zcml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/reply_form.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/reply_form.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/settings.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/settings.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/browser/views.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/configure.zcml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsincomingmail_icon.png` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsincomingmail_icon.png`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsmail.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsmail.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/dmsoutgoingmail_icon.png` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/dmsoutgoingmail_icon.png`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/indexers.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/indexers.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/collective.dms.mailcontent.pot` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/collective.dms.mailcontent.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-12-01 14:25+0000\n"
+"POT-Creation-Date: 2022-03-25 08:04+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -18,22 +18,30 @@
 "Domain: collective.dms.mailcontent\n"
 
 #: ../vocabularies.py:34
 msgid "${ref} (dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:34
+msgid "${ref} (dmsmainfile signed) => ${title}"
+msgstr ""
+
+#: ../vocabularies.py:34
 msgid "${ref} (dmsmainfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:25
 msgid "(dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:25
+msgid "(dmsmainfile signed) => ${title}"
+msgstr ""
+
+#: ../vocabularies.py:25
 msgid "(dmsmainfile) => ${title}"
 msgstr ""
 
 #: ../browser/settings.py:16
 msgid "Always hide"
 msgstr ""
 
@@ -165,15 +173,15 @@
 msgid "Recipients"
 msgstr ""
 
 #: ../behaviors.py:15
 msgid "Registered"
 msgstr ""
 
-#: ../browser/reply_form.py:25
+#: ../browser/reply_form.py:49
 msgid "Reply to ${ref}"
 msgstr ""
 
 #: ../dmsmail.py:89
 msgid "Sender"
 msgstr ""
```

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/collective.dms.mailcontent.po` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/collective.dms.mailcontent.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-12-01 14:25+0000\n"
+"POT-Creation-Date: 2022-03-25 08:04+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -16,22 +16,30 @@
 "X-is-fallback-for: en-au en-ca en-gb en-us\n"
 
 #: ../vocabularies.py:34
 msgid "${ref} (dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:34
+msgid "${ref} (dmsmainfile signed) => ${title}"
+msgstr ""
+
+#: ../vocabularies.py:34
 msgid "${ref} (dmsmainfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:25
 msgid "(dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:25
+msgid "(dmsmainfile signed) => ${title}"
+msgstr ""
+
+#: ../vocabularies.py:25
 msgid "(dmsmainfile) => ${title}"
 msgstr ""
 
 #: ../browser/settings.py:16
 msgid "Always hide"
 msgstr ""
 
@@ -163,15 +171,15 @@
 msgid "Recipients"
 msgstr ""
 
 #: ../behaviors.py:15
 msgid "Registered"
 msgstr ""
 
-#: ../browser/reply_form.py:25
+#: ../browser/reply_form.py:49
 msgid "Reply to ${ref}"
 msgstr ""
 
 #: ../dmsmail.py:89
 msgid "Sender"
 msgstr ""
```

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/plone.po` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/collective.dms.mailcontent.po` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/collective.dms.mailcontent.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-12-01 14:25+0000\n"
+"POT-Creation-Date: 2022-03-25 08:04+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -16,22 +16,30 @@
 "X-is-fallback-for: fr-fr fr-be fr-ca\n"
 
 #: ../vocabularies.py:34
 msgid "${ref} (dmsappendixfile) => ${title}"
 msgstr "${ref} (A) => ${title}"
 
 #: ../vocabularies.py:34
+msgid "${ref} (dmsmainfile signed) => ${title}"
+msgstr "${ref} (VS) => ${title}"
+
+#: ../vocabularies.py:34
 msgid "${ref} (dmsmainfile) => ${title}"
 msgstr "${ref} (V) => ${title}"
 
 #: ../vocabularies.py:25
 msgid "(dmsappendixfile) => ${title}"
 msgstr "(A) => ${title}"
 
 #: ../vocabularies.py:25
+msgid "(dmsmainfile signed) => ${title}"
+msgstr "(VS) => ${title}"
+
+#: ../vocabularies.py:25
 msgid "(dmsmainfile) => ${title}"
 msgstr "(V) => ${title}"
 
 #: ../browser/settings.py:16
 msgid "Always hide"
 msgstr "Toujours cacher"
 
@@ -163,15 +171,15 @@
 msgid "Recipients"
 msgstr "Destinataires"
 
 #: ../behaviors.py:15
 msgid "Registered"
 msgstr "Par recommandé"
 
-#: ../browser/reply_form.py:25
+#: ../browser/reply_form.py:49
 msgid "Reply to ${ref}"
 msgstr "Répondre à ${ref}"
 
 #: ../dmsmail.py:89
 msgid "Sender"
 msgstr "Expéditeur"
```

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/plone.po` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/manual.pot` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/manual.pot`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 msgid "(dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:25
 msgid "(dmsmainfile) => ${title}"
 msgstr ""
 
+#: ../vocabularies.py:25
+msgid "(dmsmainfile signed) => ${title}"
+msgstr ""
+
 #: ../vocabularies.py:34
 msgid "${ref} (dmsappendixfile) => ${title}"
 msgstr ""
 
 #: ../vocabularies.py:34
 msgid "${ref} (dmsmainfile) => ${title}"
 msgstr ""
+
+#: ../vocabularies.py:34
+msgid "${ref} (dmsmainfile signed) => ${title}"
+msgstr ""
```

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/locales/plone.pot` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/catalog.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/controlpanel.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/import_steps.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types/dmsincomingmail.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types/dmsincomingmail.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/default/types/dmsoutgoingmail.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/default/types/dmsoutgoingmail.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/registry.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/profiles/testing/types/testtype.xml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/profiles/testing/types/testtype.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/setuphandlers.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/testing.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/testing.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/testing.zcml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_behaviors.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_content.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_indexers.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_reply_form.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_reply_form.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/tests/test_settings.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/configure.zcml` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/upgrades/upgrades.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/src/collective/dms/mailcontent/vocabularies.py` & `collective.dms.mailcontent-1.9/src/collective/dms/mailcontent/vocabularies.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,44 @@
     """ Vocabulary listing outgoing mail files and related ones, as possible email attachments """
     implements(IVocabularyFactory)
 
     def __call__(self, context):
         terms = []
         # first we find context files, unrestrictedly
         brains = find(context=context, unrestricted=True, object_provides=[IDmsAppendixFile.__identifier__,
-                                                                           IDmsFile.__identifier__])
+                      IDmsFile.__identifier__], sort_on='created', sort_order='descending')
         for brain in brains:
             obj = brain._unrestrictedGetObject()
+            ftitle = safe_unicode(brain.Title)
+            # TODO Mark signed version
+            if ftitle.lower() == obj.file.filename.lower():
+                title = ftitle
+            else:
+                title = u'{}  (« {} »)'.format(ftitle, obj.file.filename)
+            if brain.signed:
+                typ = u'{} signed'.format(brain.portal_type)
+            else:
+                typ = brain.portal_type
             terms.append(SimpleTerm(brain.UID, brain.UID,
-                                    _tr(u'({}) => ${{title}}'.format(brain.portal_type),
-                                        mapping={'title': u'{}  (« {} »)'.format(safe_unicode(brain.Title),
-                                                                                 obj.file.filename)})))
+                                    _tr(u'({}) => ${{title}}'.format(typ), mapping={'title': title})))
         # then we find files of related mails
         pc = api.portal.get_tool('portal_catalog')
         for rv in getattr(context, 'reply_to', []) or []:
             brains = pc.unrestrictedSearchResults(path=rv.to_path, object_provides=[IDmsAppendixFile.__identifier__,
-                                                                                    IDmsFile.__identifier__])
+                                                  IDmsFile.__identifier__], sort_on='created', sort_order='descending')
             for brain in brains:
                 obj = brain._unrestrictedGetObject()
+                ftitle = safe_unicode(brain.Title)
+                if ftitle.lower() == obj.file.filename.lower():
+                    title = ftitle
+                else:
+                    title = u'{}  (« {} »)'.format(ftitle, obj.file.filename)
+                if brain.signed:
+                    typ = u'{} signed'.format(brain.portal_type)
+                else:
+                    typ = brain.portal_type
                 terms.append(SimpleTerm(brain.UID, brain.UID,
-                                        _tr(u'${{ref}} ({}) => ${{title}}'.format(brain.portal_type),
-                                            mapping={'ref': rv.to_object.internal_reference_no,
-                                                     'title': u'{}  (« {} »)'.format(safe_unicode(brain.Title),
-                                                                                     obj.file.filename)})))
+                                        _tr(u'${{ref}} ({}) => ${{title}}'.format(typ),
+                                            mapping={'ref': rv.to_object.internal_reference_no, 'title': title})))
 
         terms.sort(key=lambda trm: trm.title.lower())
         return SimpleVocabulary(terms)
```

### Comparing `collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/PKG-INFO` & `collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.dms.mailcontent
-Version: 1.8
+Version: 1.9
 Summary: Mail content type for document management system
 Home-page: https://github.com/collective/collective.dms.mailcontent
 Author: Ecreall, Entrouvert, IMIO
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Download-URL: https://pypi.org/project/collective.dms.mailcontent
 Description: Introduction
@@ -39,14 +39,22 @@
         - Vincent Fretin, Ecreall
         - Cédric Messiant, Ecreall
         - Frédéric Peters, Entr'ouvert
         
         Changelog
         =========
         
+        1.9 (2022-03-25)
+        ----------------
+        
+        - When listing attachments, do not include filename if it's the same than title.
+          [sgeulette]
+        - Marked signed attachment
+          [sgeulette]
+        
         1.8 (2022-03-17)
         ----------------
         
         - Made separate `add_content` method to be overrided.
           [sgeulette]
         
         1.7 (2022-02-10)
```

### Comparing `collective.dms.mailcontent-1.8/src/collective.dms.mailcontent.egg-info/SOURCES.txt` & `collective.dms.mailcontent-1.9/src/collective.dms.mailcontent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.dms.mailcontent-1.8/versions.cfg` & `collective.dms.mailcontent-1.9/versions.cfg`

 * *Files identical despite different names*

