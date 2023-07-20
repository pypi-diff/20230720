# Comparing `tmp/collective.contact.core-1.8.tar.gz` & `tmp/collective.contact.core-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.contact.core-1.8.tar", last modified: Thu Mar 31 09:34:40 2016, max compression
+gzip compressed data, was "dist/collective.contact.core-1.9.tar", last modified: Thu Jul  7 13:36:41 2016, max compression
```

## Comparing `collective.contact.core-1.8.tar` & `collective.contact.core-1.9.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/docs/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      733 2016-03-31 09:34:40.000000 collective.contact.core-1.8/docs/LICENSE.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    18092 2016-03-31 09:34:40.000000 collective.contact.core-1.8/docs/LICENSE.GPL
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2292 2016-03-31 09:34:40.000000 collective.contact.core-1.8/setup.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      242 2016-03-31 09:34:40.000000 collective.contact.core-1.8/travis.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       52 2016-03-31 09:34:40.000000 collective.contact.core-1.8/TODO.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       80 2016-03-31 09:34:40.000000 collective.contact.core-1.8/buildout.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1378 2016-03-31 09:34:40.000000 collective.contact.core-1.8/sources.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       59 2016-03-31 09:34:40.000000 collective.contact.core-1.8/setup.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      296 2016-03-31 09:34:40.000000 collective.contact.core-1.8/checkouts.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      557 2016-03-31 09:34:40.000000 collective.contact.core-1.8/base.cfg
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        1 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/not-zip-safe
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      453 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/requires.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       89 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/entry_points.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    15525 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/PKG-INFO
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        1 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/dependency_links.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     8951 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/SOURCES.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       30 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/namespace_packages.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       11 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective.contact.core.egg-info/top_level.txt
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       56 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/__init__.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      211 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/fields.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      422 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/propertiestool.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       14 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/collective_contact_core_marker.txt
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4916 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/definition.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1354 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/registry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      709 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      249 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/rolemap.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2212 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2237 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/person.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2107 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/held_position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2203 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/directory.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2319 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/organization.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      265 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/catalog.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      264 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/cssregistry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      450 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/types.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      257 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/jsregistry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      532 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/metadata.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      473 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/default/skins.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/img/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3681 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/img/sgt_pepper.jpg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       14 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/collective_contact_core_test_data_marker.txt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      174 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/metadata.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/types/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2050 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/types/testtype.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      230 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/types.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      308 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/jsregistry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      175 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/profiles/testing/metadata.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2853 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/indexers.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4566 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/subscribers.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1273 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/testing.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7602 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/adapters.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      630 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/testing.zcml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      180 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/__init__.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/types/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      340 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/types/position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      338 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/types/person.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      345 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/types/held_position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      344 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v6/types/organization.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v9/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      422 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v9/propertiestool.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4853 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/definition.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      709 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2198 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2153 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/person.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2090 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/held_position.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2221 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/directory.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2313 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/organization.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      235 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/catalog.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      264 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/cssregistry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      257 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/jsregistry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      473 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/skins.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v8/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      475 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v8/registry.xml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v7/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      936 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v7/registry.xml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2205 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/upgrades.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/__init__.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3680 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/upgrades/configure.zcml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      630 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/directory.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       28 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/__init__.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    20138 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/addcontact.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2111 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/othercontacts.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1425 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/contact.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3410 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/heldpositions.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1672 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/directory.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1161 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/person.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1361 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/address.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4211 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/organization.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1049 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/ttwfields.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2667 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/contactdetails.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2014 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/templates/position.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      689 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/vcard_export.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3414 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/excelexport.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2455 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/person.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2133 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/utils.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      683 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/ttwfields.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/__init__.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1272 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/person.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1058 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/organization.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1239 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/held_position.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      518 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/position.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3436 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/basefields/views.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2556 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/configure.zcml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6200 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/contactable.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1602 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/contact.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3519 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/organization.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1112 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/address.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1342 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/position.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/static/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6581 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/static/forms.js
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      898 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/browser/excelexport.zcml
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/position_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/organization_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      847 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/style.css
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      774 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/position_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      525 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/person_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      614 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/person_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/directory_icon.png.metadata
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      860 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/contact_core_macros.pt
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      635 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/directory_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      441 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/organization_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      614 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/create_contact.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      774 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9693 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/behaviors.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3645 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/configure.zcml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2575 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/vocabulary.py
--rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)     2047 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/interfaces.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1275 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/fti.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1923 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/directory.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/__init__.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6483 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/held_position.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4316 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/person.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5819 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/organization.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3532 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/content/position.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/
--rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)      266 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/update.sh
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1413 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/plone.pot
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5190 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.mo
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      790 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9594 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.po
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1402 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4637 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.mo
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      779 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9419 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.po
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1503 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7915 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/locales/collective.contact.core.pot
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1065 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/behaviors.zcml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     8574 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/setuphandlers.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5802 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_adapters.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/__init__.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    12154 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_views.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1565 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_related.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      725 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_setup.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3790 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_search.py
-drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/robot/
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7653 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/robot/test_contacts.robot
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      739 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/robot/keywords.robot
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9444 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_content_types.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2397 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_workflow.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3068 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_behaviors.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      633 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/tests/test_robot.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      225 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/skins.zcml
--rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)       72 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/core/schema.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       56 2016-03-31 09:34:40.000000 collective.contact.core-1.8/src/collective/contact/__init__.py
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      300 2016-03-31 09:34:40.000000 collective.contact.core-1.8/development.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      167 2016-03-31 09:34:40.000000 collective.contact.core-1.8/CONTRIBUTORS.rst
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       95 2016-03-31 09:34:40.000000 collective.contact.core-1.8/.coveragerc
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      682 2016-03-31 09:34:40.000000 collective.contact.core-1.8/versions.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      251 2016-03-31 09:34:40.000000 collective.contact.core-1.8/demo.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       89 2016-03-31 09:34:40.000000 collective.contact.core-1.8/MANIFEST.in
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1727 2016-03-31 09:34:40.000000 collective.contact.core-1.8/README.rst
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    15525 2016-03-31 09:34:40.000000 collective.contact.core-1.8/PKG-INFO
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      221 2016-03-31 09:34:40.000000 collective.contact.core-1.8/.gitignore
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      727 2016-03-31 09:34:40.000000 collective.contact.core-1.8/jenkins-base.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9560 2016-03-31 09:34:40.000000 collective.contact.core-1.8/CHANGES.rst
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       93 2016-03-31 09:34:40.000000 collective.contact.core-1.8/jenkins.cfg
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1273 2016-03-31 09:34:40.000000 collective.contact.core-1.8/.travis.yml
--rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6158 2016-03-31 09:34:40.000000 collective.contact.core-1.8/bootstrap.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/docs/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      733 2016-07-07 13:36:41.000000 collective.contact.core-1.9/docs/LICENSE.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    18092 2016-07-07 13:36:41.000000 collective.contact.core-1.9/docs/LICENSE.GPL
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2292 2016-07-07 13:36:41.000000 collective.contact.core-1.9/setup.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      242 2016-07-07 13:36:41.000000 collective.contact.core-1.9/travis.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       52 2016-07-07 13:36:41.000000 collective.contact.core-1.9/TODO.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       80 2016-07-07 13:36:41.000000 collective.contact.core-1.9/buildout.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1378 2016-07-07 13:36:41.000000 collective.contact.core-1.9/sources.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       59 2016-07-07 13:36:41.000000 collective.contact.core-1.9/setup.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      296 2016-07-07 13:36:41.000000 collective.contact.core-1.9/checkouts.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      557 2016-07-07 13:36:41.000000 collective.contact.core-1.9/base.cfg
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        1 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/not-zip-safe
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      453 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/requires.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       89 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/entry_points.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    15810 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/PKG-INFO
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        1 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     8951 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       30 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       11 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective.contact.core.egg-info/top_level.txt
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       56 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/__init__.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      211 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/fields.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      422 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/propertiestool.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       14 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/collective_contact_core_marker.txt
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4916 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/definition.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1354 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/registry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      709 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      249 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/rolemap.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2212 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2237 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/person.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2107 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/held_position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2203 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/directory.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2319 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/organization.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      265 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/catalog.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      264 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/cssregistry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      450 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/types.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      257 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/jsregistry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      533 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/metadata.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      473 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/default/skins.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/img/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3681 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/img/sgt_pepper.jpg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       14 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/collective_contact_core_test_data_marker.txt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      174 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/metadata.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/types/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2050 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/types/testtype.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      230 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/types.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      308 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/jsregistry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      175 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/profiles/testing/metadata.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3205 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/indexers.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4750 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/subscribers.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1273 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/testing.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7602 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/adapters.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      630 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/testing.zcml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      180 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/__init__.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/types/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      340 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/types/position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      338 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/types/person.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      345 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/types/held_position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      344 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v6/types/organization.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v9/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      422 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v9/propertiestool.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4853 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/definition.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      709 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2198 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2153 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/person.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2090 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/held_position.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2221 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/directory.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2313 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/organization.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      235 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/catalog.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      264 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/cssregistry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      257 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/jsregistry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      473 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/skins.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v8/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      475 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v8/registry.xml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v7/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      936 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v7/registry.xml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2491 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/upgrades.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/__init__.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3911 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/upgrades/configure.zcml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      630 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/directory.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       28 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/__init__.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    20138 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/addcontact.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2111 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/othercontacts.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1425 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/contact.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3410 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/heldpositions.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1672 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/directory.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1161 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/person.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1361 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/address.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4211 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/organization.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1049 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/ttwfields.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2667 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/contactdetails.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2014 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/templates/position.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      689 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/vcard_export.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3414 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/excelexport.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2455 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/person.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2133 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/utils.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      683 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/ttwfields.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/__init__.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1272 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/person.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1058 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/organization.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1239 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/held_position.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      518 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/position.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3436 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/basefields/views.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2556 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/configure.zcml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6200 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/contactable.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1602 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/contact.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3519 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/organization.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1112 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/address.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1342 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/position.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/static/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6581 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/static/forms.js
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      898 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/browser/excelexport.zcml
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/position_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/organization_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      847 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/style.css
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      774 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/position_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      525 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/person_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      614 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/person_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       25 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/directory_icon.png.metadata
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      860 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/contact_core_macros.pt
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      635 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/directory_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      441 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/organization_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      614 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/create_contact.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      774 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9693 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/behaviors.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3783 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/configure.zcml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2575 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/vocabulary.py
+-rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)     2047 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/interfaces.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1275 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/fti.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1923 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/directory.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/__init__.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6483 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/held_position.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4316 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/person.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5819 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/organization.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3532 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/content/position.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/
+-rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)      266 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/update.sh
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1413 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/plone.pot
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5190 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.mo
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      790 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9594 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.po
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1402 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4637 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.mo
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      779 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9419 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.po
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1503 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7915 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/locales/collective.contact.core.pot
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1065 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/behaviors.zcml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     8574 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/setuphandlers.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     5802 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_adapters.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/__init__.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    12154 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_views.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1565 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_related.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      725 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_setup.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     4763 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_search.py
+drwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)        0 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/robot/
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     7653 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/robot/test_contacts.robot
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      739 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/robot/keywords.robot
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    10023 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_content_types.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     2397 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_workflow.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     3068 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_behaviors.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      633 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/tests/test_robot.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      225 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/skins.zcml
+-rwxr-xr-x   0 vincentfretin  (1000) vincentfretin  (1000)       72 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/core/schema.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       56 2016-07-07 13:36:41.000000 collective.contact.core-1.9/src/collective/contact/__init__.py
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      300 2016-07-07 13:36:41.000000 collective.contact.core-1.9/development.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      167 2016-07-07 13:36:41.000000 collective.contact.core-1.9/CONTRIBUTORS.rst
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       95 2016-07-07 13:36:41.000000 collective.contact.core-1.9/.coveragerc
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      682 2016-07-07 13:36:41.000000 collective.contact.core-1.9/versions.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      251 2016-07-07 13:36:41.000000 collective.contact.core-1.9/demo.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       89 2016-07-07 13:36:41.000000 collective.contact.core-1.9/MANIFEST.in
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1727 2016-07-07 13:36:41.000000 collective.contact.core-1.9/README.rst
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)    15810 2016-07-07 13:36:41.000000 collective.contact.core-1.9/PKG-INFO
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      221 2016-07-07 13:36:41.000000 collective.contact.core-1.9/.gitignore
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)      727 2016-07-07 13:36:41.000000 collective.contact.core-1.9/jenkins-base.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     9773 2016-07-07 13:36:41.000000 collective.contact.core-1.9/CHANGES.rst
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)       93 2016-07-07 13:36:41.000000 collective.contact.core-1.9/jenkins.cfg
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     1273 2016-07-07 13:36:41.000000 collective.contact.core-1.9/.travis.yml
+-rw-r--r--   0 vincentfretin  (1000) vincentfretin  (1000)     6158 2016-07-07 13:36:41.000000 collective.contact.core-1.9/bootstrap.py
```

### Comparing `collective.contact.core-1.8/docs/LICENSE.txt` & `collective.contact.core-1.9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/docs/LICENSE.GPL` & `collective.contact.core-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/setup.py` & `collective.contact.core-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     + '\n' +
     open('CONTRIBUTORS.rst').read()
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 setup(name='collective.contact.core',
-      version='1.8',
+      version='1.9',
       description="Core package for collective.contact add-ons",
       long_description=long_description,
       # Get more strings from
       # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.contact.core-1.8/sources.cfg` & `collective.contact.core-1.9/sources.cfg`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/base.cfg` & `collective.contact.core-1.9/base.cfg`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective.contact.core.egg-info/PKG-INFO` & `collective.contact.core-1.9/src/collective.contact.core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.contact.core
-Version: 1.8
+Version: 1.9
 Summary: Core package for collective.contact add-ons
 Home-page: http://svn.plone.org/svn/collective/
 Author: "Cedric Messiant"
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Description: .. contents::
         
@@ -61,14 +61,24 @@
         - Frédéric Peters, Entr'ouvert
         - Thomas Desvenain, Ecreall
         
         
         Changelog
         =========
         
+        1.9 (2016-07-07)
+        ----------------
+        
+        - Reindex suborganizations (and positions and held positions) when an
+          organization is modified.
+          [vincentfretin]
+        
+        - Use start and end indexes for held_position.
+          [sgeulette]
+        
         1.8 (2016-03-31)
         ----------------
         
         - Hide contact types from the navigation.
           [pcdummy]
         
         - Sort sub organizations by folder position in organization view
@@ -421,15 +431,14 @@
         0.9 (2013-03-07)
         ----------------
         
         - Initial release
           [cedricmessiant]
         
         
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.2
 Classifier: Framework :: Plone :: 4.3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `collective.contact.core-1.8/src/collective.contact.core.egg-info/SOURCES.txt` & `collective.contact.core-1.9/src/collective.contact.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/definition.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows/collective_contact_core_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/registry.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/workflows.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/position.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/position.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/person.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/person.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/held_position.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/held_position.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/directory.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/directory.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/types/organization.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/types/organization.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/metadata.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/metadata.xml`

 * *Files 2% similar despite different names*

#### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/default/metadata.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>9</version>
+  <version>10</version>
   <dependencies>
     <dependency>profile-collective.contact.widget:default</dependency>
     <dependency>profile-plone.app.dexterity:default</dependency>
     <dependency>profile-plone.formwidget.datetime:default</dependency>
     <dependency>profile-plone.formwidget.masterselect:default</dependency>
     <dependency>profile-plone.app.relationfield:default</dependency>
     <dependency>profile-collective.z3cform.datagridfield:default</dependency>
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/test_data/img/sgt_pepper.jpg` & `collective.contact.core-1.9/src/collective/contact/core/profiles/test_data/img/sgt_pepper.jpg`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/profiles/testing/types/testtype.xml` & `collective.contact.core-1.9/src/collective/contact/core/profiles/testing/types/testtype.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/indexers.py` & `collective.contact.core-1.9/src/collective/contact/core/indexers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import date
 from plone import api
 from plone.indexer import indexer
 from Products.CMFPlone.utils import normalizeString
 from Products.CMFPlone.utils import safe_unicode
 
 from collective.contact.core.content.held_position import IHeldPosition
 from collective.contact.core.content.organization import IOrganization
@@ -79,7 +80,23 @@
 @indexer(IHeldPosition)
 def held_position_sortable_title(obj):
     sortable_fullname = person_sortable_title(obj.get_person())()
     held_position_title = obj.Title()
     return u"%s-%s" % (sortable_fullname,
                        normalizeString(safe_unicode(held_position_title),
                                        context=obj))
+
+
+@indexer(IHeldPosition)
+def start_date(obj):
+    if obj.start_date:
+        return obj.start_date
+    # if empty, we return creation date
+    return obj.created()
+
+
+@indexer(IHeldPosition)
+def end_date(obj):
+    if obj.end_date:
+        return obj.end_date
+    # if empty we return future date
+    return date(2100, 01, 01)
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/subscribers.py` & `collective.contact.core-1.9/src/collective/contact/core/subscribers.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 
     for position in obj.get_positions():
         position.reindexObject(idxs=indexes_to_update)
         for held_position in position.get_held_positions():
             held_position.reindexObject(idxs=indexes_to_update)
             update_related_with_held_position(held_position)
 
+    for child in obj.values():
+        if IOrganization.providedBy(child):
+            child.reindexObject(idxs=indexes_to_update)
+            update_related_with_organization(child)
+
 
 def referenceRemoved(obj, event, toInterface=IContactContent):
     """Store information about the removed link integrity reference.
     """
     # inspired from z3c/relationfield/event.py:breakRelations
     # and plone/app/linkintegrity/handlers.py:referenceRemoved
     # if the object the event was fired on doesn't have a `REQUEST` attribute
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/testing.py` & `collective.contact.core-1.9/src/collective/contact/core/testing.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/adapters.py` & `collective.contact.core-1.9/src/collective/contact/core/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/testing.zcml` & `collective.contact.core-1.9/src/collective/contact/core/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/definition.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows/collective_contact_core_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/workflows.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/workflows.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/position.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/position.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/person.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/person.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/held_position.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/held_position.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/directory.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/directory.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v2/types/organization.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v2/types/organization.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/profiles/v7/registry.xml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/profiles/v7/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/upgrades.py` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/upgrades.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from z3c.relationfield.event import updateRelations
 from z3c.relationfield.interfaces import IHasRelations
 from zope.component import getUtility
 
 from plone import api
 
 from collective.contact.widget.interfaces import IContactContent
-
 from ecreall.helpers.upgrade.interfaces import IUpgradeTool
 
+from ..content.held_position import IHeldPosition
+
 
 def reindex_relations(context):
     """Clear the relation catalog to fix issues with interfaces that don't exist anymore.
     This actually fixes the from_interfaces_flattened and to_interfaces_flattened indexes.
     """
     rcatalog = getUtility(ICatalog)
     rcatalog.clear()
@@ -68,7 +69,14 @@
     tool = IUpgradeTool(context)
     tool.runProfile('collective.contact.core.upgrades:v8')
 
 
 def v9(context):
     tool = IUpgradeTool(context)
     tool.runProfile('collective.contact.core.upgrades:v9')
+
+
+def v10(context):
+    catalog = api.portal.get_tool('portal_catalog')
+    brains = catalog.searchResults(object_provides=IHeldPosition.__identifier__)
+    for brain in brains:
+        brain.getObject().reindexObject(['start', 'end'])
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/upgrades/configure.zcml` & `collective.contact.core-1.9/src/collective/contact/core/upgrades/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -105,8 +105,16 @@
       title="Upgrade from 8 to 9"
       description="Hide contact types from the navigation"
       source="8"
       destination="9"
       handler=".upgrades.v9"
       profile="collective.contact.core:default" />
 
+  <genericsetup:upgradeStep
+      title="Upgrade from 9 to 10"
+      description="Use start and end indexes"
+      source="9"
+      destination="10"
+      handler=".upgrades.v10"
+      profile="collective.contact.core:default" />
+
 </configure>
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/directory.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/directory.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/addcontact.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/addcontact.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/othercontacts.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/othercontacts.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/contact.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/contact.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/heldpositions.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/heldpositions.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/directory.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/directory.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/person.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/person.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/address.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/address.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/organization.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/organization.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/ttwfields.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/ttwfields.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/contactdetails.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/contactdetails.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/templates/position.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/templates/position.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/vcard_export.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/vcard_export.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/excelexport.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/excelexport.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/person.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/person.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/utils.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/ttwfields.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/ttwfields.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/person.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/person.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/organization.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/organization.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/held_position.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/held_position.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/basefields/templates/position.pt` & `collective.contact.core-1.9/src/collective/contact/core/browser/basefields/templates/position.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/basefields/views.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/basefields/views.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/configure.zcml` & `collective.contact.core-1.9/src/collective/contact/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/contactable.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/contactable.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/contact.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/contact.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/organization.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/organization.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/address.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/address.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/position.py` & `collective.contact.core-1.9/src/collective/contact/core/browser/position.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/static/forms.js` & `collective.contact.core-1.9/src/collective/contact/core/browser/static/forms.js`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/browser/excelexport.zcml` & `collective.contact.core-1.9/src/collective/contact/core/browser/excelexport.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/style.css` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/style.css`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/position_icon.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/position_icon.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/vcard_icon.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/person_icon.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/person_icon.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/contact_core_macros.pt` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/contact_core_macros.pt`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/directory_icon.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/directory_icon.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/create_contact.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/create_contact.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png` & `collective.contact.core-1.9/src/collective/contact/core/skins/collective_contact_core/held_position_icon.png`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/behaviors.py` & `collective.contact.core-1.9/src/collective/contact/core/behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/configure.zcml` & `collective.contact.core-1.9/src/collective/contact/core/configure.zcml`

 * *Files 15% similar despite different names*

```diff
@@ -88,14 +88,24 @@
 
   <adapter
     name="sortable_title"
     factory=".indexers.held_position_sortable_title"
     />
 
   <adapter
+    name="start"
+    factory=".indexers.start_date"
+    />
+
+  <adapter
+    name="end"
+    factory=".indexers.end_date"
+    />
+
+  <adapter
       factory=".behaviors.DefaultUseParentAddress"
       name="default" />
 
   <adapter
       factory=".behaviors.DefaultParentAddress"
       name="default" />
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/vocabulary.py` & `collective.contact.core-1.9/src/collective/contact/core/vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/interfaces.py` & `collective.contact.core-1.9/src/collective/contact/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/fti.py` & `collective.contact.core-1.9/src/collective/contact/core/fti.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/content/directory.py` & `collective.contact.core-1.9/src/collective/contact/core/content/directory.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/content/held_position.py` & `collective.contact.core-1.9/src/collective/contact/core/content/held_position.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/content/person.py` & `collective.contact.core-1.9/src/collective/contact/core/content/person.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/content/organization.py` & `collective.contact.core-1.9/src/collective/contact/core/content/organization.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/content/position.py` & `collective.contact.core-1.9/src/collective/contact/core/content/position.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/plone.pot` & `collective.contact.core-1.9/src/collective/contact/core/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.mo` & `collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.mo`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.mo` & `collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.mo`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.po` & `collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.po` & `collective.contact.core-1.9/src/collective/contact/core/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.mo` & `collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.mo`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/plone.mo` & `collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/plone.mo`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.po` & `collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/it/LC_MESSAGES/plone.po` & `collective.contact.core-1.9/src/collective/contact/core/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/locales/collective.contact.core.pot` & `collective.contact.core-1.9/src/collective/contact/core/locales/collective.contact.core.pot`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/behaviors.zcml` & `collective.contact.core-1.9/src/collective/contact/core/behaviors.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/setuphandlers.py` & `collective.contact.core-1.9/src/collective/contact/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_adapters.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_views.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_related.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_related.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_setup.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/robot/test_contacts.robot` & `collective.contact.core-1.9/src/collective/contact/core/tests/robot/test_contacts.robot`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/robot/keywords.robot` & `collective.contact.core-1.9/src/collective/contact/core/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_content_types.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_content_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,14 +149,23 @@
         self.assertEqual(self.brigadelh.get_full_title(),
                          u"Armée de terre / Corps A / Division Alpha / Régiment H / Brigade LH")
         self.assertEqual(self.brigadelh.get_full_title(separator=u' - '),
                          u"Armée de terre - Corps A - Division Alpha - Régiment H - Brigade LH")
         self.assertEqual(self.brigadelh.get_full_title(separator=u' - ', first_index=2),
                          u"Division Alpha - Régiment H - Brigade LH")
 
+    def test_reindex_suborganization(self):
+        before = self.portal.portal_catalog(UID=self.brigadelh.UID())[0].get_full_title
+        self.assertEqual(before, u'Arm\xe9e de terre / Corps A / Division Alpha / R\xe9giment H / Brigade LH')
+        self.armeedeterre.title = u"Armée de l'air"
+        from zope.lifecycleevent import modified
+        modified(self.armeedeterre)
+        after = self.portal.portal_catalog(UID=self.brigadelh.UID())[0].get_full_title
+        self.assertEqual(after, u"Arm\xe9e de l'air / Corps A / Division Alpha / R\xe9giment H / Brigade LH")
+
     def test_copy_paste(self):
         cb = self.mydirectory.manage_copyObjects(['armeedeterre'])
         self.mydirectory.manage_pasteObjects(cb)
         self.assertIn('copy_of_armeedeterre', self.mydirectory.keys())
 
 
 class TestPosition(TestContentTypes):
```

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_workflow.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_behaviors.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/src/collective/contact/core/tests/test_robot.py` & `collective.contact.core-1.9/src/collective/contact/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/versions.cfg` & `collective.contact.core-1.9/versions.cfg`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/README.rst` & `collective.contact.core-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/PKG-INFO` & `collective.contact.core-1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.contact.core
-Version: 1.8
+Version: 1.9
 Summary: Core package for collective.contact add-ons
 Home-page: http://svn.plone.org/svn/collective/
 Author: "Cedric Messiant"
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Description: .. contents::
         
@@ -61,14 +61,24 @@
         - Frédéric Peters, Entr'ouvert
         - Thomas Desvenain, Ecreall
         
         
         Changelog
         =========
         
+        1.9 (2016-07-07)
+        ----------------
+        
+        - Reindex suborganizations (and positions and held positions) when an
+          organization is modified.
+          [vincentfretin]
+        
+        - Use start and end indexes for held_position.
+          [sgeulette]
+        
         1.8 (2016-03-31)
         ----------------
         
         - Hide contact types from the navigation.
           [pcdummy]
         
         - Sort sub organizations by folder position in organization view
@@ -421,15 +431,14 @@
         0.9 (2013-03-07)
         ----------------
         
         - Initial release
           [cedricmessiant]
         
         
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.2
 Classifier: Framework :: Plone :: 4.3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `collective.contact.core-1.8/jenkins-base.cfg` & `collective.contact.core-1.9/jenkins-base.cfg`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/CHANGES.rst` & `collective.contact.core-1.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+1.9 (2016-07-07)
+----------------
+
+- Reindex suborganizations (and positions and held positions) when an
+  organization is modified.
+  [vincentfretin]
+
+- Use start and end indexes for held_position.
+  [sgeulette]
+
 1.8 (2016-03-31)
 ----------------
 
 - Hide contact types from the navigation.
   [pcdummy]
 
 - Sort sub organizations by folder position in organization view
@@ -355,8 +365,7 @@
 
 
 0.9 (2013-03-07)
 ----------------
 
 - Initial release
   [cedricmessiant]
-
```

### Comparing `collective.contact.core-1.8/.travis.yml` & `collective.contact.core-1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective.contact.core-1.8/bootstrap.py` & `collective.contact.core-1.9/bootstrap.py`

 * *Files identical despite different names*

