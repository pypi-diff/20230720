# Comparing `tmp/ckanext-check-link-0.1.1.post1.tar.gz` & `tmp/ckanext-check-link-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-check-link-0.1.1.post1.tar", last modified: Sat May 27 14:38:39 2023, max compression
+gzip compressed data, was "ckanext-check-link-0.1.2.tar", last modified: Thu Jul 20 16:52:41 2023, max compression
```

## Comparing `ckanext-check-link-0.1.1.post1.tar` & `ckanext-check-link-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3904 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3239 2023-05-27 14:37:01.000000 ckanext-check-link-0.1.1.post1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5879 2023-05-27 14:34:21.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      383 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5377 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3536 2022-08-25 20:38:04.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3615 2022-08-25 23:59:09.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.760222 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-05-05 15:32:57.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/model/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1138 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.800223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base_admin.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2218 2023-05-05 15:06:35.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/report.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/report_item.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-11-07 20:13:48.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/header.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3675 2023-05-05 15:33:16.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4019 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/test_report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4146 2023-05-09 14:30:50.000000 ckanext-check-link-0.1.1.post1/ckanext/check_link/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3904 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1886 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 14:38:39.000000 ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4447 2023-05-05 15:32:15.000000 ckanext-check-link-0.1.1.post1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1559 2023-05-27 14:38:39.810223 ckanext-check-link-0.1.1.post1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.1.post1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3898 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3239 2023-05-27 14:37:01.000000 ckanext-check-link-0.1.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.631612 ckanext-check-link-0.1.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.631612 ckanext-check-link-0.1.2/ckanext/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5879 2023-05-27 14:34:21.000000 ckanext-check-link-0.1.2/ckanext/check_link/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      383 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.2/ckanext/check_link/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5377 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/action/check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3536 2022-08-25 20:38:04.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/action/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3615 2022-08-25 23:59:09.000000 ckanext-check-link-0.1.2/ckanext/check_link/logic/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.631612 ckanext-check-link-0.1.2/ckanext/check_link/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      860 2023-07-20 16:16:33.000000 ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/versions/dad15b4f251a_add_ondelete_cascade_to_resource_id.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       79 2023-07-20 16:13:35.000000 ckanext-check-link-0.1.2/ckanext/check_link/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.2/ckanext/check_link/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-07-20 16:12:13.000000 ckanext-check-link-0.1.2/ckanext/check_link/model/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1778 2023-07-20 16:52:24.000000 ckanext-check-link-0.1.2/ckanext/check_link/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/base_admin.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2218 2023-05-05 15:06:35.000000 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/report.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/snippets/report_item.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-11-07 20:13:48.000000 ckanext-check-link-0.1.2/ckanext/check_link/templates/header.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3675 2023-05-05 15:33:16.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/test_check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4019 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/test_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext/check_link/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1239 2023-07-20 16:13:28.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/model/test_report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1254 2023-07-20 16:52:24.000000 ckanext-check-link-0.1.2/ckanext/check_link/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4146 2023-05-09 14:30:50.000000 ckanext-check-link-0.1.2/ckanext/check_link/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3898 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1987 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-20 16:52:41.000000 ckanext-check-link-0.1.2/ckanext_check_link.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4447 2023-05-05 15:32:15.000000 ckanext-check-link-0.1.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1553 2023-07-20 16:52:41.641612 ckanext-check-link-0.1.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.2/setup.py
```

### Comparing `ckanext-check-link-0.1.1.post1/LICENSE` & `ckanext-check-link-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/PKG-INFO` & `ckanext-check-link-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-check-link
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: Resource URL checker
 Home-page: https://github.com/DataShades/ckanext-check-link
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-check-link-0.1.1.post1/README.md` & `ckanext-check-link-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/cli.py` & `ckanext-check-link-0.1.2/ckanext/check_link/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/check.py` & `ckanext-check-link-0.1.2/ckanext/check_link/logic/action/check.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/action/report.py` & `ckanext-check-link-0.1.2/ckanext/check_link/logic/action/report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/auth.py` & `ckanext-check-link-0.1.2/ckanext/check_link/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/logic/schema.py` & `ckanext-check-link-0.1.2/ckanext/check_link/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/alembic.ini` & `ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/env.py` & `ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py` & `ckanext-check-link-0.1.2/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/model/report.py` & `ckanext-check-link-0.1.2/ckanext/check_link/model/report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base.html` & `ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/base_admin.html` & `ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/base_admin.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/report.html` & `ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/report.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/check_link/snippets/report_item.html` & `ckanext-check-link-0.1.2/ckanext/check_link/templates/check_link/snippets/report_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/templates/header.html` & `ckanext-check-link-0.1.2/ckanext/check_link/templates/header.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/conftest.py` & `ckanext-check-link-0.1.2/ckanext/check_link/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_check.py` & `ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/test_check.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/logic/action/test_report.py` & `ckanext-check-link-0.1.2/ckanext/check_link/tests/logic/action/test_report.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/tests/model/test_report.py` & `ckanext-check-link-0.1.2/ckanext/check_link/tests/model/test_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 
 from ckanext.check_link.model import Report
 
 
 @pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestReport:
     def test_removed_with_resource(self, resource, faker):
+        res = model.Resource.get(resource["id"])
+
         report = Report(url=faker.url(), resource_id=resource["id"], state="unknown")
         model.Session.add(report)
         model.Session.commit()
 
         assert report.id
 
-        model.Session.delete(model.Resource.get(resource["id"]))
+        res = model.Resource.get(resource["id"])
+
+        model.Session.delete(res)
         model.Session.commit()
         assert not model.Session.query(Report).filter_by(id=report.id).one_or_none()
         assert not Report.by_resource_id(resource["id"])
 
     def test_by_resource_id(self, report_factory, resource):
         with_resource = report_factory(resource_id=resource["id"])
         report_factory(resource_id=None)
```

### Comparing `ckanext-check-link-0.1.1.post1/ckanext/check_link/views.py` & `ckanext-check-link-0.1.2/ckanext/check_link/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/PKG-INFO` & `ckanext-check-link-0.1.2/ckanext_check_link.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-check-link
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: Resource URL checker
 Home-page: https://github.com/DataShades/ckanext-check-link
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-check-link-0.1.1.post1/ckanext_check_link.egg-info/SOURCES.txt` & `ckanext-check-link-0.1.2/ckanext_check_link.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ckanext/check_link/logic/action/__init__.py
 ckanext/check_link/logic/action/check.py
 ckanext/check_link/logic/action/report.py
 ckanext/check_link/migration/check_link/alembic.ini
 ckanext/check_link/migration/check_link/env.py
 ckanext/check_link/migration/check_link/script.py.mako
 ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
+ckanext/check_link/migration/check_link/versions/dad15b4f251a_add_ondelete_cascade_to_resource_id.py
 ckanext/check_link/model/__init__.py
 ckanext/check_link/model/base.py
 ckanext/check_link/model/report.py
 ckanext/check_link/templates/header.html
 ckanext/check_link/templates/check_link/base.html
 ckanext/check_link/templates/check_link/base_admin.html
 ckanext/check_link/templates/check_link/report.html
```

### Comparing `ckanext-check-link-0.1.1.post1/pyproject.toml` & `ckanext-check-link-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.1.1.post1/setup.cfg` & `ckanext-check-link-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-check-link
-version = 0.1.1.post1
+version = 0.1.2
 description = Resource URL checker
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-check-link
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-check-link-0.1.1.post1/setup.py` & `ckanext-check-link-0.1.2/setup.py`

 * *Files identical despite different names*

