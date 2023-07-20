# Comparing `tmp/ocdsextensionregistry-0.3.7.tar.gz` & `tmp/ocdsextensionregistry-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.7.tar", last modified: Thu Jul 20 03:12:46 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.8.tar", last modified: Thu Jul 20 18:06:30 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.7.tar` & `ocdsextensionregistry-0.3.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.784884 ocdsextensionregistry-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-20 03:12:46.784884 ocdsextensionregistry-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.768883 ocdsextensionregistry-0.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.768883 ocdsextensionregistry-0.3.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.772884 ocdsextensionregistry-0.3.7/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.776884 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.776884 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 03:12:46.000000 ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-20 03:12:46.784884 ocdsextensionregistry-0.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.780884 ocdsextensionregistry-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.780884 ocdsextensionregistry-0.3.7/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.784884 ocdsextensionregistry-0.3.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:12:46.784884 ocdsextensionregistry-0.3.7/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-20 03:12:37.000000 ocdsextensionregistry-0.3.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.837093 ocdsextensionregistry-0.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.837093 ocdsextensionregistry-0.3.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.841093 ocdsextensionregistry-0.3.8/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.841093 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.841093 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:06:30.000000 ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.841093 ocdsextensionregistry-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:06:30.845093 ocdsextensionregistry-0.3.8/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-20 18:06:21.000000 ocdsextensionregistry-0.3.8/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.7/LICENSE` & `ocdsextensionregistry-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/PKG-INFO` & `ocdsextensionregistry-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.7
+Version: 0.3.8
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.7/README.rst` & `ocdsextensionregistry-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/docs/Makefile` & `ocdsextensionregistry-0.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/docs/changelog.rst` & `ocdsextensionregistry-0.3.8/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.3.8 (2023-07-20)
+------------------
+
+-  feat: :class:`~ocdsextensionregistry.profile_builder.ProfileBuilder`: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.__init__`: The ``extension_versions`` argument can be a dict in which values are URLs, in addition to versions.
+
 0.3.7 (2023-07-19)
 ------------------
 
 -  feat: Change assertions to warnings, when adding or removing codes from an extension's codelist.
 
 0.3.6 (2023-07-12)
 ------------------
```

### Comparing `ocdsextensionregistry-0.3.7/docs/cli.rst` & `ocdsextensionregistry-0.3.8/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/docs/conf.py` & `ocdsextensionregistry-0.3.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.7"
+version = "0.3.8"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.7/docs/index.rst` & `ocdsextensionregistry-0.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/docs/translation.rst` & `ocdsextensionregistry-0.3.8/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/profile_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,44 +87,51 @@
     @property
     def registry(self):
         if self._registry is None:
             self._registry = ExtensionRegistry(self.registry_base_url + 'extension_versions.csv')
 
         return self._registry
 
+    @staticmethod
+    def _extension_from_url(url, parsed):
+        data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
+        kwargs = {'input_url': url}
+        if parsed.scheme == 'file':
+            data['Download URL'] = url
+        elif url.endswith('/extension.json'):
+            data['Base URL'] = url[:-14]
+        elif url.endswith('/'):
+            data['Base URL'] = url
+        # If the files are served via API, with the filename as a query string parameter.
+        elif 'extension.json' in url:
+            kwargs['url_pattern'] = url.replace('extension.json', FIELD)
+        elif 'release-schema.json' in url:
+            kwargs['url_pattern'] = url.replace('release-schema.json', FIELD)
+        elif parsed.path.endswith('.json'):
+            kwargs['file_urls'] = {'release-schema.json': url}
+        else:
+            data['Download URL'] = url
+        return ExtensionVersion(data, **kwargs)
+
     def extensions(self):
         """
         Returns the matching extension versions from the registry.
         """
         if isinstance(self.extension_versions, dict):
             for identifier, version in self.extension_versions.items():
-                yield self.registry.get(id=identifier, version=version)
+                parsed = urlsplit(version)
+                if parsed.scheme:
+                    yield self._extension_from_url(version, parsed)
+                else:
+                    yield self.registry.get(id=identifier, version=version)
         elif isinstance(self.extension_versions, Iterable):
             for url in self.extension_versions:
                 if not url or not isinstance(url, str):
                     continue
-                parsed = urlsplit(url)
-                data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
-                kwargs = {'input_url': url}
-                if parsed.scheme == 'file':
-                    data['Download URL'] = url
-                elif url.endswith('/extension.json'):
-                    data['Base URL'] = url[:-14]
-                elif url.endswith('/'):
-                    data['Base URL'] = url
-                # If the files are served via API, with the filename as a query string parameter.
-                elif 'extension.json' in url:
-                    kwargs['url_pattern'] = url.replace('extension.json', FIELD)
-                elif 'release-schema.json' in url:
-                    kwargs['url_pattern'] = url.replace('release-schema.json', FIELD)
-                elif parsed.path.endswith('.json'):
-                    kwargs['file_urls'] = {'release-schema.json': url}
-                else:
-                    data['Download URL'] = url
-                yield ExtensionVersion(data, **kwargs)
+                yield self._extension_from_url(url, urlsplit(url))
 
     def release_schema_patch(self, extension_field=None, language='en'):
         """
         Returns the consolidated release schema patch.
 
         :param str extension_field: the property with which to annotate each definition and field with the name of the
                                     extension in which the definition or field is defined
```

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.7
+Version: 0.3.8
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.7/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.8/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/setup.cfg` & `ocdsextensionregistry-0.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.7
+version = 0.3.8
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.3.7/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.8/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.8/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.8/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.8/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.8/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_api.py` & `ocdsextensionregistry-0.3.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_codelist.py` & `ocdsextensionregistry-0.3.8/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.8/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_extension.py` & `ocdsextensionregistry-0.3.8/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.8/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.8/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.8/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tests/test_util.py` & `ocdsextensionregistry-0.3.8/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.7/tox.ini` & `ocdsextensionregistry-0.3.8/tox.ini`

 * *Files identical despite different names*

